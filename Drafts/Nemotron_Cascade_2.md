# Nemotron-Cascade 2 논문 리뷰

엔비디아가 공개한 30B 크기의(실제 활성화 파라미터 3B) MoE 오픈 가중치 모델입니다. 놀라운 **지능 밀도(Intelligence density)**로 2025 IMO, IOI, ICPC 대회 수준을 정복한 것이 특징입니다.

### 1. 한계 없는 Cascade RL 훈련
파괴적 망각(Catastrophic Forgetting)을 막는 파이프라인. 여러 도메인을 섞지 않고, IF-RL부터 Multi-domain RL → Code RL → SWE RL 등 능력을 수직(Sequential)으로 쌓았습니다. (최대 256K 토큰 길이 허용).

### 2. MOPD (초정밀 지식 증류)
순차 강화학습 중 이전 도메인 능력이 떨어지는 현상을, 강력한 중간 교사(Teacher) 모델을 통한 On-Policy 증류로 차단합니다. Mamba-Transformer 하이브리드 아키텍처의 강점 위에서 각 도메인간 밸런스를 복구하고 극대화하여 30B 모델임에도 불구하고 최상위 거대 모델(DeepSeekV3.2) 성능에 도달한 비결입니다.
