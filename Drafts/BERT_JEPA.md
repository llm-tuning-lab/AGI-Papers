# BERT-JEPA: 언어 불변 의미론적 공간 구축

논문: **"BERT-JEPA: Reorganizing CLS Embeddings for Language-Invariant Semantics"**

이 연구는 기존 BERT 아키텍처의 고질병인 [CLS] 토큰 임베딩의 '공간 붕괴' 현상을 해결하기 위해, 얀 르쿤(Yann LeCun) 교수의 JEPA(Joint Embedding Predictive Architectures) 사상을 도입한 BEPA 프레임워크를 제안합니다.

### 1. 배경: [CLS] 공간의 붕괴
기존 언어 모델들은 의미가 전혀 다른 두 문장이나 언어가 아예 다른 문장 사이에서도 코사인 유사도가 비정상적으로 높게(0.99 등) 나타나는 정보 중첩 및 붕괴 현상이 있습니다. 이를 통해 차원의 풍부성을 잃는 저랭크(Low-rank) 임베딩 환경이 형성됩니다.

### 2. BEPA 프레임워크 합체 방식
- **입력 패키징**: 단일 언어 또는 이중 언어 문장을 트랜스포머 입력에 나란히 패킹합니다.
- **MLM (Masked Language Modeling)**: 기존 BERT의 언어 파악 능력을 보존하기 위해 병렬로 문법과 구문을 학습시킵니다.
- **JEPA 정렬(Alignment)**: 입력 데이터 자체를 복원하는 것이 아니라, 문장을 각각 독립적으로 마스킹 처리하여 [CLS] 잠재 표현(Latent representation)을 일치시키도록 학습(InfoNCE 손실 함수 활용)합니다.

### 3. 결론과 성과
이 훈련 목표를 통해 모델은 문법이라는 껍데기를 버리고, t-SNE로 시각화 시 언어 간 클러스터 경계가 완전히 허물어지는 '진보적인 생각의 공간(Thought Space)'을 구축합니다. GLUE 성능 저하 없이 XNLI 및 이기종 간 번역-추론 등에서 더 우수한 성능과 Fuller-rank 공간을 입증했습니다.
