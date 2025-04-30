

# 🧠 수화 손모양 이미지 분류 AI

## 📌 1. 개요
- 🏫 **2025 프라임칼리지 AI학과 컴퓨터비전 1학기 중간고사 대체 과제**

- 🎯 **과제 목표:** 손 모양 수화 이미지를 보고 어떤 숫자인지 분류하는 AI 모델 구현
  
- 🏁 **관련 해커톤:** [DACON 공식 페이지 바로가기](https://dacon.io/competitions/official/235896/data)
  
- 💡 **기대 효과:**  
  시각적 입력(손모양 이미지)을 통해 수화를 숫자로 인식 → 청각장애인을 위한 보조 기술의 가능성 모색
  <img width="680" alt="Image" src="https://github.com/user-attachments/assets/fc8a0dc3-8ce6-443f-b8d6-037313d7ff9d" />

---

## 📊 2. AI 모델별 성능 비교

### 📌 2.1 🧱 CNN 모델 (Baseline)
- 🎯 **Train Acc:** 82.45% / **Val Acc:** 57.69% / **Test Acc:** 17.88%
  
- 📉 **Loss Curve**  
  <img src="https://github.com/user-attachments/assets/1b20ad7b-7bac-483b-b4f8-bfd89d6a4048" width="480" />

---

### 📌 2.2 🏗 DenseNet121
- 🎯 **Train Acc:** 95.49% / **Val Acc:** 96.15% / **Test Acc:** 92.12%
  
- 📉 **Loss Curve**  
  <img width="480" alt="Image" src="https://github.com/user-attachments/assets/6506f86f-9fcd-4de6-badf-1d2050433ed2" />

---

### 📌 2.3 📱 MobileNetV2
- 🎯 **Train Acc:** 95.65% / **Val Acc:** 91.67% / **Test Acc:** 86.67%
  
- 📉 **Loss Curve**  
  <img width="480" alt="Image" src="https://github.com/user-attachments/assets/bd422df5-8511-4e38-a82e-ef61164bd51e" />

---

### 📌 2.4 🏋️ ResNet18
- 🎯 **Train Acc:** 93.72% / **Val Acc:** 85.90% / **Test Acc:** 80.61%
  
- 📉 **Loss Curve**  
  <img width="480" alt="Image" src="https://github.com/user-attachments/assets/92688b9f-bf32-4c3e-8a36-2702b47df6f6" />

---

## ✅ 3. 결론 및 인사이트

- ⚠️ 단순 CNN 모델은 **과적합이 심하고**, 실제 테스트에서는 성능이 급격히 하락함
  
- ✅ Transfer Learning 기반 모델들(DenseNet121, MobileNetV2, ResNet18)이 확연한 성능 향상을 보여줌
  
- 🥇 **최종 선택 모델:** `DenseNet121`  
  → **테스트 정확도 92.12%로 가장 안정적이며 높은 일반화 성능을 보임**

---

### ✨ 향후 개선 방향
- 🔍 데이터 불균형 보정 (e.g., 클래스 가중치, 오버샘플링)
  
- 🧪 하이퍼파라미터 튜닝 및 앙상블 기법 적용 고려
  
---
