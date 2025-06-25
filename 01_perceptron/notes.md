# 퍼셉트론 요약 (Perceptron Summary)

---

## 핵심 개념 (Core Concepts)

- 퍼셉트론은 인공신경망의 가장 기본 단위입니다.  
  A perceptron is the most fundamental unit of an artificial neural network.

- 입력값과 가중치의 내적, 바이어스를 더한 뒤 활성화 함수를 통해 출력을 결정합니다.  
  The output is computed by applying an activation function to the weighted sum of inputs plus a bias.

- 단일 퍼셉트론은 선형 분류만 가능합니다 (XOR 문제 해결 불가).  
  A single-layer perceptron can only perform linear classification (cannot solve XOR).

---

## 학습 과정 (Learning Steps)

- **순전파 (Forward Propagation)**  
  입력을 통해 출력을 계산합니다.  
  Calculates output based on current weights.

- **역전파 (Backpropagation)**  
  오차를 기반으로 가중치를 수정합니다.  
  Adjusts weights based on the output error.

- **경사 하강법 (Gradient Descent)**  
  손실 함수를 최소화하도록 파라미터를 업데이트합니다.  
  Updates weights to minimize the loss function.

---

## 기타 요소 (Other Concepts)

- **정규화 (Normalization)**: 학습 안정성을 위해 입력/가중치 범위 조정  
- **드롭아웃 (Dropout)**: 과적합 방지를 위한 무작위 뉴런 제거 (MLP에 적용됨)

---

## 자세한 내용은 슬라이드 참고 (See PDF for Details)
