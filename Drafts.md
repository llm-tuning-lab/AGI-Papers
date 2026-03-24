# 📝 Drafts & New Summaries

This file contains drafts and summaries of new papers that have not yet been fully integrated into the main [README.md](README.md).

---

## 🤖 Agents

*   [**코딩 에이전트의 역설: 친절한 설명서 (AGENTS.md)가 망치는 효율성**](Drafts/Evaluating_AGENTS_md.md)
    *   **Topic**: Agent / Evaluation
    *   **Summary**: 코딩 에이전트에게 리포지토리 컨텍스트 파일(AGENTS.md)을 제공하는 것이 오히려 정보 과부하를 유발해 성공률을 떨어뜨리고 비용을 높인다는 흥미로운 반직관적 연구 결과.

*   [**Zero-Swap Tiny-MoA: 16GB 로컬 에이전트 아키텍처**](Drafts/Zero_Swap_Tiny_MoA.md)
    *   **Topic**: Local Agent Architecture
    *   **Summary**: 16GB RAM 제약 속에서 ModernBERT 라우터와 350M 다이내믹 LoRA 스와핑, 1.2B 모델을 버무려 지연 시간(I/O 스와핑)을 0에 수렴시킨 현존 최고 효율의 다중 에이전트 마스터플랜.

*   [**AI Can Learn Scientific Taste**](Drafts/Scientific_Taste.md)
    *   **Topic**: Agent / Scientific Discovery
    *   **Summary**: AI 과학자가 지시된 연구를 넘어 가치 있는 연구 방향을 판별하고 고안하는 능력을 RLCF로 학습. 인용 수와 전문가 평가를 통한 '과학적 안목' 구축 프레임워크 제안.

*   [**AI Era Cognitive Surrender**](Drafts/Cognitive_Surrender.md)
    *   **Topic**: Human-AI Interaction
    *   **Summary**: System 1 (Intuition)과 System 2 (Deliberation)를 넘어, 외부 인지 시스템인 **System 3 (AI)**에 의존하는 인간의 '인지적 항복(Cognitive Surrender)' 현상과 그 위험성을 경고한 행동과학 연구.
    *   **Key Insight**: AI가 틀린 답을 줘도 맹목적으로 따르는 현상을 실험적으로 증명.

*   [**ASA: Training-Free Tool Calling**](Drafts/ASA_Tool_Calling.md)
    *   **Topic**: Tool Use / Efficiency
    *   **Summary**: LLM이 도구 사용 시점은 알지만 행동으로 옮기지 못하는 'Representation-Behavior Gap'을 해결. 학습 없이(Training-Free) 추론 시점에 모델 내부 활성화(Activation)를 조작하여 도구 호출 성능을 극대화하는 **ASA(Activation Steering Adapter)** 제안.
    *   **Performance**: 단 20KB 용량으로 F1 Score 2배 향상.

*   [**HUMANLM: State Alignment for User Simulation**](Drafts/HUMANLM.md)
    *   **Topic**: User Simulation
    *   **Summary**: 사용자의 말투만 흉내 내는 기존 방식을 비판하며, 사용자의 **신념, 감정, 목표 등 심리적 상태(State)**를 먼저 추론하고 이를 정렬(Alignment in Latent Space)하여 완벽한 페르소나를 구현하는 프레임워크.
    *   **Benchmark**: HUMANUAL 벤치마크 공개.

*   [**SKILLRL: Skill-Augmented Reinforcement Learning**](Drafts/SKILLRL.md)
    *   **Topic**: Reinforcement Learning
    *   **Summary**: 에이전트가 겪은 성공과 실패의 경험을 **'스킬(Skill)'** 형태로 증류(Distill)하여 라이브러리에 저장하고, 이를 재사용하여 점점 더 똑똑해지는 평생 학습(Lifelong Learning) 프레임워크.

*   [**PicoClaw: Low-Cost On-Device AI**](Drafts/PicoClaw.md)
    *   **Topic**: On-Device / Edge AI
    *   **Summary**: 10MB RAM의 라즈베리 파이 Pico에서도 구동 가능한 Go 언어 기반의 초경량 AI 에이전트. Agent.cpp와 유사한 철학을 공유하며 극단적인 효율성을 추구.

*   [**Training Agents to Self-Report Misbehavior**](Drafts/Self_Report_Misbehavior.md)
    *   **Topic**: Safety / Self-Control
    *   **Summary**: 외부 감시 모델 없이, AI가 자신의 오작동이나 기만적 행동을 내부에서 스스로 감지하고 고발하는 '자가 통제 시스템' 훈련.

*   [**Everything is Context: Agentic File System**](Drafts/Agentic_File_System.md)
    *   **Topic**: Agent Architecture
    *   **Summary**: 유닉스의 "Everything is a file" 철학을 에이전트에 이식. 지식, 도구, 기억을 파일 시스템처럼 마운트/언마운트하는 운영체제 아키텍처.

*   [**OpenSandbox: Isolated Execution for Agents**](Drafts/OpenSandbox.md)
    *   **Topic**: Agent Infrastructure
    *   **Summary**: 에이전트가 OS를 제어하고 코드를 실행해도 실제 시스템에 피해가 없도록, 컨테이너 기반으로 완벽히 격리된 범용 실행 인프라.

*   [**CUDA Agent: Agentic RL for CUDA Kernel Generation**](Drafts/CUDA_Agent.md)
    *   **Topic**: Hardware Optimization / RL
    *   **Summary**: 에이전트가 CUDA 커널을 직접 작성하고, 실행 결과를 피드백으로 받아 다중 턴 강화학습으로 고성능 커널을 자동 생성.

*   [**AgentCgroup: OS Resource Control for AI Agents**](Drafts/AgentCgroup.md)
    *   **Topic**: OS Resource Management
    *   **Summary**: 다중 테넌트 환경에서 에이전트의 메모리 피크(15.4배 폭발)를 커널 내부(eBPF)에서 마이크로초 단위로 제어. 생존율 66% → 100%.

*   [**Sniper-Router-Surgeon: ELECTRA + dLLM Coding Agent**](Drafts/ELECTRA_dLLM_Pipeline.md)
    *   **Topic**: Coding Agent Architecture
    *   **Summary**: ELECTRA가 버그 토큰을 저격(Sniper), dLLM이 양방향 문맥으로 수술(Surgeon), RLVR이 검증하는 자가 치유형 코딩 에이전트. GLM-4.7-Flash(SWE-bench 73.8%) 기반.

*   [**Nemotron-Terminal: Scaling LLM Terminal Capabilities**](Drafts/Nemotron_Terminal.md)
    *   **Topic**: Terminal Agent / Data Engineering
    *   **Summary**: 32B SFT 모델이 480B Qwen3-Coder를 능가(27.4%). 모델 크기보다 고품질 터미널 궤적 데이터가 핵심.

*   [**LFM2-24B Terminal Agent: FP8 LoRA SFT + RL**](Drafts/LFM2_Terminal_Agent.md)
    *   **Topic**: Terminal Agent / Training Strategy
    *   **Summary**: H100 1대에서 FP8 LoRA로 4,500개 SFT(1에폭) → 실환경 RL로 자가 치유형 터미널 에이전트 구축. 활성 2.3B의 미친 속도, 총비용 ~$150.

*   [**FORMAL JUDGE: Neuro-Symbolic Agentic Oversight**](Drafts/FormalJudge.md)
    *   **Topic**: Safety / Verification
    *   **Summary**: LLM+SMT Solver 결합. 7B 심판이 72B 에이전트 기만을 90%+ 탐지. 안전성 70.7% → 99.8% 달성. GitHub 코드 공개.

---

## 🧠 Architecture

*   [**글로벌 확장의 새로운 룰 'Tiny Aya': 3B 체급으로 70개 국어를 정복하다**](Drafts/Tiny_Aya_Multilingual.md)
    *   **Topic**: Tiny Model / Multilingual
    *   **Summary**: 토크나이저 최적화, 합성 데이터 융합(Fusion-of-N), 지역 특화 병합(SIMMERGE) 기술로 거대 모델의 다국어 번역 성능을 3B 크기로 압축해낸 Cohere Labs의 오프라인 모바일 엣지 아키텍처.

*   [**디퓨전 LLM: 속도와 보안의 룰을 바꾸다 (Mercury 2)**](Drafts/Diffusion_LLM_Mercury2.md)
    *   **Topic**: Diffusion Language Model / Inference
    *   **Summary**: 뮌헨 공대의 인페인팅 보안 공격과 초당 1,009 토큰을 생성하는 Mercury 2 상용 모델을 통해 본 디퓨전 LLM의 파괴적 혁신(속도, 보안, 부분 수정)과 구조적 한계.

*   [**ModernBERT: 2026년 시맨틱 라우터의 글로벌 표준**](Drafts/ModernBERT_Router.md)
    *   **Topic**: Encoder / LLM Routing
    *   **Summary**: Unpadding 및 Alternating Attention 설계로 인텔 CPU 8비트 환경의 연산 한계를 돌파한 2조 개 토큰 인코더의 효율성 벤치마킹 분석.

*   [**Omni-Diffusion: 이산 확산(Discrete Diffusion) 기반 멀티모달**](Drafts/Omni_Diffusion.md)
    *   **Topic**: Multimodal / Diffusion
    *   **Summary**: AR(자가회귀)의 순차적 토큰 제한을 뛰어넘어, 이미지·오디오·텍스트의 단일 정렬 의미 공간을 구축해 병렬 디코딩을 구현한 Any-to-Any 모델 리뷰.

*   [**MDM-Prime-v2: 확산 언어 모델 연산 효율성 최적화**](Drafts/MDM_Prime_v2.md)
    *   **Topic**: Diffusion Language Model
    *   **Summary**: 이진 인코딩(Binary Encoding)과 인덱스 셔플링을 적용해 마스크 확산 언어 모델(MDM)의 연산 효율성을 ARM 대비 21.8배 향상시킨 혁신.

*   [**Nemotron-Cascade 2 아키텍처 및 학습 방법론**](Drafts/Nemotron_Cascade_2.md)
    *   **Topic**: Architecture / Post-Training
    *   **Summary**: 활성 3B의 MoE 모델로 놀라운 지능 밀도(IMO 금메달)를 달성한 비법. 순차적 강화학습(Cascade RL)과 다중 도메인 지식 증류(MOPD) 구조 분석.

*   [**선형 RNN 병렬화 처리 속도와 표현력 분석**](Drafts/Linear_RNN_Parallelizable.md)
    *   **Topic**: Linear RNN / Expressivity
    *   **Summary**: 선형, 비선형 RNN, 트랜스포머 간 회로 깊이(Circuit Depth)의 수학적 증명을 통해 지능과 처리 속도의 양자택일 트레이드오프 파헤치기.

*   [**BERT-JEPA: 언어 불변 의미론적 공간 구축**](Drafts/BERT_JEPA.md)
    *   **Topic**: Latent Space / Embeddings
    *   **Summary**: BERT의 [CLS] 붕괴 한계를 Yann LeCun의 JEPA(Predictive Architecture) 구조로 해결. 언어에 얽매이지 않는 진보적인 생각/의미역(Thought space) 융합.

*   [**TEON vs Muon: Pre-training Optimizer**](Drafts/TEON_vs_Muon.md)
    *   **Topic**: Optimization
    *   **Summary**: 
        *   **Muon**: 각 레이어를 독립적으로 직교화하여 학습 효율을 높임.
        *   **TEON**: 여러 레이어의 그라디언트를 **3차원 텐서(Tensor)**로 묶어 한꺼번에 직교화함으로써 레이어 간 상관관계를 반영, Muon보다 더 빠른 수렴 속도 달성.
    *   **Strategy**: TEON의 강력한 최적화와 Muon 논문의 효율적 튜닝 기법(Telescoping)을 결합하는 것이 최상의 전략.

*   [**Nested Learning: The Illusion of Deep Learning**](Drafts/Nested_Learning.md)
    *   **Topic**: Architecture Philosophy
    *   **Summary**: 구글 딥마인드 논문. "딥러닝의 핵심은 깊이(Deep)가 아니라, 서로 다른 시간척도(Timescale)로 도는 **중첩된 루프(Nested Loop)**다." 인간의 기억 메커니즘을 모방한 새로운 학습 패러다임 제안.

*   [**EinFields: Neural Tensor Fields for Relativity**](Drafts/EinFields.md)
    *   **Topic**: AI for Science
    *   **Summary**: ICLR 2026 채택. 일반 상대성 이론의 시뮬레이션을 위한 신경망 아키텍처. 복잡한 4차원 시공간 데이터를 효율적으로 압축하고 연산하는 **Neural Tensor Field** 기술.

*   [**Micro GPT Code Analysis**](Drafts/Micro_GPT.md)
    *   **Topic**: Education / Implementation
    *   **Summary**: Andrej Karpathy의 `microgpt.py` (200줄) 분석. LLM의 바닥부터 이해하기 위한 최고의 교육 자료.

*   [**RadixMLP: Intra-batch Deduplication**](Drafts/RadixMLP.md)
    *   **Topic**: Inference Optimization
    *   **Summary**: 동일한 시스템 프롬프트의 중복 연산을 트리 구조로 압축하여 원천 제거. 대규모 서빙의 추론 병목을 알고리즘 단에서 파괴.

*   [**T-GRAPHORMER: Spatiotemporal Forecasting**](Drafts/T_GRAPHORMER.md)
    *   **Topic**: AI for Physical World
    *   **Summary**: 트랜스포머에 시간 부호화를 결합하여 교통 흐름 등 복잡한 시공간의 비선형적 역학을 분석·예측.

*   [**Graphormer: Transformers for Graph Representation**](Drafts/Graphormer.md)
    *   **Topic**: Graph Neural Networks
    *   **Summary**: 중심성·공간 부호화를 도입해 소셜 네트워크·분자 구조 등 복잡한 그래프 데이터에 트랜스포머를 이식. OGB-LSC 1위.

*   [**xgboost2ww: Spectral Weight Diagnostics**](Drafts/xgboost2ww.md)
    *   **Topic**: Model Diagnostics
    *   **Summary**: 딥러닝의 WeightWatcher 스펙트럼 진단 기법을 XGBoost 등 전통 트리 모델에 이식. 실서비스 배치 전 과적합 탐지.

*   [**Qwen3.5: Native Multimodal Agents**](Drafts/Qwen3_5.md)
    *   **Topic**: Hybrid Architecture
    *   **Summary**: 델타넷 기반 선형 주의집중 + 희소 전문가 혼합 하이브리드 구조. 화면 픽셀을 직접 제어하는 행동 지능과 추론 속도를 동시에 확보.

*   [**Molmo2: Open Vision-Language Models with Grounding**](Drafts/Molmo2.md)
    *   **Topic**: Vision-Language / Grounding
    *   **Summary**: 화면 내 특정 객체를 픽셀 단위로 지목·추적하는 행동 기반 시각 지능을 완전한 개방형 가중치로 공개.

*   [**dLLM: Simple Diffusion Language Modeling**](Drafts/dLLM.md)
    *   **Topic**: Diffusion Language Model
    *   **Summary**: 확산 기반 언어 모델의 훈련·배포를 단일 개방형 프레임워크로 표준화. AR 모델에서 Diffusion으로의 세대교체 인프라.

*   [**mHC: Manifold-Constrained Hyper-Connections**](Drafts/mHC.md)
    *   **Topic**: Signal Propagation / ResNet
    *   **Summary**: DeepSeek이 1967년 Sinkhorn-Knopp 알고리즘으로 ResNet의 신호 폭발 문제를 해결. 3,000배 → 1.6배로 억제.

*   [**FlashOptim: Memory-Efficient Deep Learning Optimizer**](Drafts/FlashOptim.md)
    *   **Topic**: Optimizer / Memory Efficiency
    *   **Summary**: AdamW의 파라미터당 메모리를 16B → 7B(5B)로 절반 이하로 축소. 성능 손실 제로(Zero Degradation). Llama-3.1-8B 학습 메모리 36% 절감.

*   [**GAT + LLM: Graph Attention Networks Integration**](Drafts/GAT_LLM.md)
    *   **Topic**: Graph Neural Networks / LLM
    *   **Summary**: ICLR 2018 근간 논문. Transformer Attention을 그래프에 이식. GraphRAG, Multi-Agent Router, Node Feature Encoder 등 LLM 결합 방안 분석.

*   [**Multi-GPU: Tensor Parallelism vs Device Map**](Drafts/TP_vs_DeviceMap.md)
    *   **Topic**: Infrastructure / Parallelism
    *   **Summary**: HuggingFace 멀티 GPU 가이드. device_map(메모리 분산, 순차 실행) vs tp_plan(진정한 병렬, torchrun 필요)의 선택 기준.

---

## 📚 Pre-Training & Post-Training

*   [**생각의 궤적에 보상을 주다: RLTT 알고리즘 구현의 핵심**](Drafts/RLTT_Algorithm_Implementation.md)
    *   **Topic**: Reinforcement Learning / Looped Model
    *   **Summary**: 최종 출력값뿐만 아니라 다중 추론 루프의 모든 중간 궤적에 가중합 보상을 할당하여 학습 병목을 해결하고 모델 통제력을 극대화하는 RLTT 알고리즘 메커니즘과 구현 가이드.

*   [**환각의 뿌리를 뽑는 'PretrainRL': 사후 교정의 한계를 넘다**](Drafts/PretrainRL_Hallucination.md)
    *   **Topic**: Pre-training / Hallucination
    *   **Summary**: 포스트 트레이닝의 한계(망각 현상)를 극복하기 위해, 사전 학습 단계에서 빔 서치와 DPO를 결합해 근본적인 팩트 체계를 재정렬하는 강화학습 방법론.

*   [**희소 메모리 파인튜닝: 파괴적 망각 방지법**](Drafts/Sparse_Memory_Finetuning.md)
    *   **Topic**: Continual Learning / Finetuning
    *   **Summary**: FFN 레이어를 '메모리 슬롯'으로 교체하고 TF-IDF로 새로운 지식 슬롯만 타겟팅해 업데이트함으로써, 기존 지식 망각률을 89%에서 11%로 방어한 지속 학습 혁신.

*   [**LLM 학습의 본질: 잠재/희소성 구조, Pre-training vs SFT**](Drafts/Latent_Sparse_Training.md)
    *   **Topic**: Philosophy / AI Training
    *   **Summary**: 모델의 공간 효율성(PCA, SVD, Lasso 정규화 철학)과 목적별 학습 파이프라인(Pre-training, SFT, RL)의 본질적 의미, Instruction 사전 훈련의 이점 고찰.

*   [**신경망 덤불과 RandOpt 리뷰**](Drafts/RandOpt_Review.md)
    *   **Topic**: Optimization / Evaluation / Post-Training
    *   **Summary**: 기울기(Gradient) 계산 없이 무작위로 가중치를 섞는 RandOpt 알고리즘의 실체를 파헤친 리뷰. 막대한 추론 비용(K배 폭발), 포맷팅에 치우친 가짜 지능, H100 1대 기준 비현실적인 학습 시간을 지적하며 극단적 학술 연구가 지닌 실무적 한계와 의의를 정리.

*   [**LIE: Length-Incentivized Exploration**](Drafts/LIE_Reasoning.md)
    *   **Topic**: Reasoning / RL
    *   **Summary**: LLM이 추론 시 "더 길게 생각하도록(Think Longer)" 유도하는 강화학습 기법. 정답을 못 맞춰도 논리적인 탐색 과정을 길게 가져가면 보상을 주어, **Self-Correction** 능력을 이끌어냄.

*   [**iGRPO: Iterative GRPO**](Drafts/iGRPO.md)
    *   **Topic**: Post-training / Reasoning
    *   **Summary**: **Self-Feedback-Driven Reasoning**. 모델이 스스로 생성한 초안(Draft)을 입력으로 받아 비평하고 수정하는 과정을 반복하며 학습하는, GRPO의 진화형.

*   [**QED-Nano: Tiny Model, Big Proofs**](Drafts/QED_Nano.md)
    *   **Topic**: Math / Reasoning
    *   **Summary**: 4B 파라미터의 작은 모델로 수학 올림피아드 증명(IMO)에서 거대 모델을 압도. **Agent Scaffold**(검색, 도구 사용 등 외부 지원)와 도메인 특화 RL의 승리.

*   [**DuPO: Dual Preference Optimization**](Drafts/DuPO.md)
    *   **Topic**: Translation / Self-Verification RL
    *   **Summary**: 정답이 없는 번역 영역에서 역번역(Back-Translation)을 보상으로 활용. 외부 데이터 없이 7B 모델이 GPT-4o급 번역 품질 달성.

*   [**Search-R1++: How to Train Your Deep Research Agent**](Drafts/Search_R1_Plus_Plus.md)
    *   **Topic**: Deep Research / RL Training
    *   **Summary**: Fast Thinking + F1+ 보상 + REINFORCE 삼위일체. "생각을 많이 할수록 성능 향상"이라는 통념을 뒤집고, Qwen2.5-7B에서 기존 대비 +3.9% 정확도 향상.

*   [**OPCD: On-Policy Context Distillation**](Drafts/OPCD.md)
    *   **Topic**: Knowledge Distillation / RL
    *   **Summary**: ICL로 얻은 경험적 지식을 영구 파라미터로 내재화. 역 KL 발산 기반 On-Policy 증류. Qwen3-8B 수학 80.9%, 시스템 프롬프트 증류로 Llama-3.2-3B 59.4%→76.3%.

---

## 🗂️ RAG & Knowledge

*   [**PathRAG: 노이즈를 쳐내는 핵심 관계 경로 추출**](Drafts/PathRAG.md)
    *   **Topic**: Graph RAG
    *   **Summary**: 그래프 기반 RAG에서 무분별한 이웃 노드(노이즈) 검색을 탈피, 가지치기 탐색을 통해 가장 영양가 높은(핵심 깊이) 연결선 흐름으로만 정보를 조합하는 LLM 최적화 서칭.

*   [**LimRank: Less is More**](Drafts/LimRank.md)
    *   **Topic**: RAG / Reranking
    *   **Summary**: 검색된 문서의 순위를 재조정(Reranking)하는 모델을 만들 때, 많은 데이터보다 **양질의 합성 데이터** 소량이 더 효과적임을 증명. 2만 개 데이터로 SOTA 달성.

*   [**ZELO: ELO-inspired Training for Search Models**](Drafts/ZELO.md)
    *   **Topic**: Search / Unsupervised Learning
    *   **Summary**: 체스의 ELO 랭킹 원리를 차용해, 정답 라벨 없는 비지도 데이터만으로 상용 검색 모델을 뛰어넘는 Reranker/Embedding 모델 훈련.

---

## 💻 On-Device & Audio

*   [**xLSTM 증류, 로컬 환경 커널 최적화 및 투기적 해독**](Drafts/xLSTM_Local_Engine.md)
    *   **Topic**: Inference Optimization / xLSTM
    *   **Summary**: 트랜스포머 KV 캐시 파괴(가변적 램 병목 억제)를 위한 xLSTM 증류 설계 방향성과 Speculative Decoding(투기적 해독) 등을 통한 제약 환경 내 최고 속도 가속화 기법.

*   [**Moonshine: Speech Recognition**](Drafts/Moonshine.md)
    *   **Topic**: Audio / On-Device
    *   **Summary**: Whisper Large v3보다 5배 빠르고 가벼운 실시간 음성 인식 모델. **한국어 공식 지원** 및 스트리밍 처리에 최적화되어 에이전트의 '귀' 역할로 적합.

*   [**Whisper Fine-tuning for Proper Noun ASR**](Drafts/Whisper_Street_ASR.md)
    *   **Topic**: ASR / Fine-tuning
    *   **Summary**: 상용 ASR 모델의 고유명사(길 이름) 인식 실패율 44%를 합성 TTS 데이터 1,000개로 파인튜닝하여 60% 개선. 비영어 화자 편향 문제도 해결.

*   [**Dynamic 2-bit Quantization for Edge LLM**](Drafts/Dynamic_2bit_Quantization.md)
    *   **Topic**: Quantization / Edge Deployment
    *   **Summary**: Unsloth Dynamic 2.0의 혼합 정밀도로 MoE 모델을 12GB GGUF로 압축. Imatrix 캘리브레이션 데이터의 도메인 혼합(영어+한국어+터미널)이 핵심.

---

## 🔥 Trends & Industry

*   [**친노동자적 AI: AI는 왜 당신을 대체하려고만 할까?**](Drafts/Pro_Worker_AI.md)
    *   **Topic**: Future of Work / AI Policy
    *   **Summary**: NBER 논문 분석. 기술 알고리즘의 문제가 아닌 AGI 지상주의와 경영진의 자동화 선호(세제 혜택 등) 구조가 혁신적 '인간-AI 협업'을 막고 있음을 지적한 정책 제언.

*   [**데이터가 90%다: AI 시대의 가장 중요한 습관**](Drafts/Data_Is_Everything.md)
    *   **Topic**: AI Era Philosophy
    *   **Summary**: 모델 스펙이나 거대 에이전트에 매몰되지 말고 실패/해결사례 기록만 남긴다면, AGI 체제의 가장 차별성 높은 데이터 무기를 얻는다는 실전 철학.

*   [**AI 시대, 완전히 뒤집힌 직업의 안전성 (앤트로픽 차트)**](Drafts/AI_Job_Safety.md)
    *   **Topic**: Future of Work
    *   **Summary**: 앤트로픽의 이론적 커버리지 분석에 따른, 코딩·법률·사무직 지식 노동의 완전한 위험성과 대면·육체 현장 노동의 절대적 안전성으로 붕괴된 시대의 역설 분석.

*   [**NCCL 오류(Silent Failure) 원인과 대안 라이브러리**](Drafts/NCCL_Alternative.md)
    *   **Topic**: AI Infrastructure
    *   **Summary**: 분산 학습 시 악명 높은 NCCL의 침묵 종료 문제와 대처법(Fail Fast, 타임아웃 감소), 그리고 MSCCL++ 및 RCCL 등의 차세대 대체 기술 분석.

*   [**Open Claw & The Philosophy of Engineering**](Drafts/Open_Claw_Philosophy.md)
    *   **Topic**: Insight
    *   **Summary**: Matplotlib 관리자를 비난한 AI 에이전트 사건(Open Claw)을 통해 본 **'자율성과 통제'**의 딜레마. 엔지니어링 성공 후 필연적으로 마주하게 될 철학적 질문들.

*   [**Vibe Coding (바이브 코딩)**](Drafts/Vibe_Coding.md)
    *   **Topic**: Trend
    *   **Summary**: Andrej Karpathy가 제안한 개념. 코드를 한 줄씩 짜는 것이 아니라, AI에게 자연어로 지시하고 그 결과물의 **'분위기(Vibe)'**와 작동 여부를 관리하는 새로운 프로그래밍 패러다임. "영원한 주니어"가 되지 않기 위한 기본기의 중요성 역설.

*   [**How Well Does Agent Development Reflect Real-World Work?**](Drafts/Agent_Dev_Real_World.md)
    *   **Topic**: Agent / Industry Gap
    *   **Summary**: 실제 노동 수요와 자본이 어디에 있는지 실증 데이터를 분석해, 현재 에이전트 개발 방향이 현실 비즈니스와 얼마나 동떨어져 있는지 뼈아픈 일침.

*   [**9 Years to AGI? Post-Training Paradigm**](Drafts/Nine_Years_to_AGI.md)
    *   **Topic**: Paradigm Shift
    *   **Summary**: 사전 학습은 뼈대일 뿐. 모델이 스스로 생각하는 시간과 강화학습에 연산을 집중시키는 Post-Training Scaling 패러다임 전환.

*   [**데이터가 90%다: AI 시대의 가장 중요한 습관**](Drafts/Data_Is_Everything.md)
    *   **Topic**: Data / Insight
    *   **Summary**: AI 중요도: 데이터 90%, 에이전트 9%, 모델 1%. 최신 도구보다 고객 데이터를 저장·정리하는 습관이 핵심. 데이터 없는 AI는 헛소리 생성기.

*   [**Reward Hacking in Real-World AI Systems**](Drafts/Reward_Hacking.md)
    *   **Topic**: AI Safety / Alignment
    *   **Summary**: Anthropic 연구. 추천 시스템·LLM·로보틱스에서 보상 해킹 실사례 분석. 굿하트의 법칙 — AI 성능↑ = 해킹 위험↑. RLHF·적대적 훈련·해석 가능성으로 대응.

*   [**AI 사회화와 확률적 앵무새 (Stochastic Parrots)**](Drafts/AI_Socialization.md)
    *   **Topic**: Philosophy / AI Ethics
    *   **Summary**: AI 합성 텍스트가 인간 언어 신뢰성 체계를 교란하는 메커니즘 분석. "포템킨 문장" 개념 제안 — 문법·맥락은 완벽하지만 지칭 대상이 부재.

