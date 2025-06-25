# CNN 요약 (Convolutional Neural Network Summary)

---

## 핵심 개념 (Core Concepts)

- **CNN**은 이미지와 같은 **공간 구조를 가진 데이터**를 처리하기 위한 딥러닝 모델입니다.  
  CNNs are deep learning models optimized for spatially structured data like images.

- 입력 이미지 = 픽셀로 구성된 2D 또는 3D 행렬  
  Input image is represented as a 2D/3D tensor of pixel values (with RGB channels).

---

## 주요 구성 요소 (Key Components)

### 1. **합성곱 (Convolution)**

- 필터(커널)가 이미지 위를 이동하며 **부분 특징(엣지 등)을 감지**  
  A small filter slides across the input to detect local features (e.g., edges).

- 각 필터는 고정된 크기의 패치마다 내적을 수행 → **특징맵 생성**  
  Applies dot product over patches → produces a feature map

- 여러 필터 → 여러 특징맵 (채널 확장)  
  Multiple filters yield multiple feature maps.

### 2. **활성화 함수 (Activation)**

- 일반적으로 **ReLU** 사용: 0 이하면 0, 양수는 그대로 출력  
  ReLU is commonly used: `f(x) = max(0, x)`

- 비선형성 도입 → 복잡한 패턴 학습 가능  
  Introduces non-linearity, enabling the network to learn complex patterns.

### 3. **풀링 (Pooling)**

- **MaxPooling / AveragePooling**을 통해 차원 축소 + 과적합 방지  
  Reduces spatial size and overfitting via downsampling.

- 중요한 특징만 남기고 정보 압축  
  Retains essential information while compressing input.

---

## 분류 단계 (Classification Layer)

- Fully Connected Layer (FC) + Softmax를 통해  
  입력 이미지가 어떤 **클래스에 속하는지 확률로 출력**  
  FC + softmax produces probability distribution over class labels.

---

##  기타 개념 (Other Concepts)

- **Stride**: 필터 이동 간격  
- **Padding**: 경계 정보 보존용  
- **Dropout**: 과적합 방지 기법 (FC Layer 이후 적용)

---

## 자세한 내용은 슬라이드 참고 (See PDF for Details)
