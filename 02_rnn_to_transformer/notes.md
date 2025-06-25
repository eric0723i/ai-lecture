# RNN ~ Transformer 요약 (RNN to Transformer Summary)

---

## 핵심 개념 (Core Concepts)

- **RNN**(Recurrent Neural Network)은 시퀀스 데이터를 처리하는 순환 구조의 신경망입니다.  
  RNNs are neural networks designed to handle sequential data via recurrent connections.

- RNN은 시간 순서에 따라 데이터를 하나씩 처리하며, **이전의 은닉 상태**를 사용해 다음 출력을 계산합니다.  
  RNNs process input one timestep at a time, using the previous hidden state to inform the next.

- **기울기 소실/폭주 문제**로 인해 긴 시퀀스를 잘 학습하지 못합니다.  
  They suffer from **vanishing/exploding gradients**, limiting their ability to learn long-term dependencies.

---

## 개선 구조 (LSTM, GRU)

- **LSTM (Long Short-Term Memory)**:  
  게이트를 통해 어떤 정보를 기억/잊을지를 결정합니다.  
  Uses gates (input, forget, output) to control memory flow.

- **GRU (Gated Recurrent Unit)**:  
  구조가 간단하지만 유사한 성능을 냅니다.  
  Simplified architecture with update/reset gates.

---

## Transformer 도입 배경 (Motivation for Transformer)

- RNN은 **병렬 처리 불가** & 장기 의존성 학습이 어렵습니다.  
  RNNs are **sequential** and struggle with long-range dependencies.

- Transformer는 **Self-Attention** 메커니즘을 도입해  
  시퀀스를 한꺼번에 처리하고, 각 위치의 중요도를 계산합니다.  
  The Transformer uses **self-attention** to compute dependencies without recurrence.

---

## Self-Attention 핵심 수식

- Attention(Q, K, V) = softmax(QKᵀ / √dₖ) · V  
  → Query와 Key의 유사도를 기반으로 Value를 가중합함

- Query: 내가 알고 싶은 정보  
- Key: 각 입력의 의미 요약  
- Value: 최종적으로 집중할 정보

---

## 자세한 내용은 슬라이드 참고 (See PDF for Details)
