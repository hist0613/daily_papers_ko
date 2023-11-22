# Daily Papers

## Project Description

This project aims to automatically translate and summarize [Huggingface's daily papers](https://huggingface.co/papers) into Korean using ChatGPT.

Thanks to [@AK391](https://github.com/AK391) for great work.

## Daily Papers (2023-11-21)

### [Orca 2: Teaching Small Language Models How to Reason](https://arxiv.org/abs/2311.11045)

- 'Orca 1'은 설명 흔적과 같은 풍부한 신호로부터 학습하여, 'BigBench Hard' 및 'AGIEval' 벤치마크에서 전통적인 지시-튠 모델들을 능가하는 성과를 보여주었습니다.
- 'Orca 2'에서는 개선된 훈련 신호가 작은 언어 모델(LM)의 추론 능력을 강화하는 방법에 대해 계속 탐구합니다.
- 작은 LMs의 훈련에 관한 연구는 종종 보다 능력 있는 모델의 출력을 모방하는 모방 학습에 의존했습니다.
- 저자들은 지나치게 모방에 중점을 두면 작은 모델의 잠재력이 제한될 수 있다고 주장합니다.
- 'Orca 2'에서는 작은 모델이 단계별 추리, 회상 후 생성, 회상-추리-생성, 직접 답변 등 다양한 추리 기술을 사용하도록 가르칩니다.
- 더 중요한 것은, 모델이 각 작업에 가장 효과적인 해결 전략을 결정하도록 학습하는 것을 목표로 합니다.
- 'Orca 2'는 약 100개의 작업과 36,000개의 고유 프롬프트에 해당하는 15가지 다양한 벤치마크 세트를 사용하여 평가됩니다.
- 비슷한 크기의 모델을 크게 능가하고, 특히 제로샷 설정에서 고급 추론 능력을 테스트하는 복잡한 작업에 대해 5-10배 큰 모델의 성능 수준과 유사하거나 더 나은 성과를 달성합니다.
- 작은 LMs의 개발, 평가, 그리고 정렬에 대한 추가 연구를 장려하기 위해 'Orca 2'를 오픈소스로 제공합니다.

### [Exponentially Faster Language Modelling](https://arxiv.org/abs/2311.10770)

- 언어 모델은 추론 시 사용하는 뉴런의 지수적 비율만큼만 필요하다는 것을 입증하기 위해, 기존 BERT 모델과 유사한 성능을 보이면서 추론 중에 단지 0.3%의 뉴런을 사용하는 FastBERT를 제안합니다.
- FastBERT는 각 층의 추론을 위해 4095개 중 단 12개 뉴런만을 활성화하며 이는 피드포워드 네트워크를 빠른 피드포워드 네트워크(FFFs)로 대체함으로써 달성됩니다.
- 조건부 신경 실행의 전체 가속 잠재력을 활용할 수 있는 진정으로 효율적인 구현은 현재 존재하지 않으나, 제공된 고수준 CPU 코드는 최적화된 기준 피드포워드 구현 대비 78배 빠른 속도를 달성합니다.
- 또한, PyTorch 구현은 베치 피드포워드 추론보다 40배 더 빠른 속도를 제공합니다.
- 연구팀은 본 논문을 통해 훈련 코드, 벤치마킹 셋업 및 모델 가중치를 공개합니다.

### [System 2 Attention (is something you might need too)](https://arxiv.org/abs/2311.11829)

- 트랜스포머 기반 대규모 언어 모델(Large Language Models, LLMs)의 소프트 어텐션은 맥락에서 관련 없는 정보를 잠재적 표현에 통합하여 다음 토큰 생성에 부정적인 영향을 미칠 수 있습니다.
- 이러한 문제를 해결하기 위해, 연구팀은 LLM이 자연어 추론과 지시사항을 따르는 능력을 활용하여 무엇에 집중해야 할지 결정하는 System 2 Attention (S2A)을 제안합니다.
- S2A는 입력 맥락을 재생성하여 관련 있는 부분만 포함하도록 하고, 재생성된 맥락에 집중하여 최종 응답을 이끌어냅니다.
- 실험 결과, S2A는 의견이나 무관한 정보가 포함된 세 가지 과제에서 표준 어텐션 기반 LLMs보다 우수한 성능을 보였습니다: 질의응답(QA), 수학 단어 문제 해결, 장문 생성입니다.
- S2A는 사실성과 객관성을 증가시키고 아첨을 감소시킴으로써, 이러한 과제들에서의 결과를 개선했습니다.

### [AutoStory: Generating Diverse Storytelling Images with Minimal Human Effort](https://arxiv.org/abs/2311.11243)

- 기존의 스토리 시각화 방법들이 특정 인물이나 시나리오에만 초점을 맞추거나 사용자가 스케치 같은 이미지 제어 조건을 제공해야 하는 등 문제를 과도하게 단순화했다는 점에서 출발합니다.
- 본 논문에서는 최소한의 인간 상호작용으로 다양하고 고품질, 일관된 스토리 이미지를 효과적으로 생성할 수 있는 자동화된 스토리 시각화 시스템을 제안합니다.
- 이 시스템은 대규모 언어 모델을 활용하여 레이아웃 계획을 수립하고, 대규모 텍스트-이미지 변환 모델을 사용하여 레이아웃에 기반한 복잡한 스토리 이미지를 생성합니다.
- 또한, 본 논문은 박스 레이아웃 같은 희소 조건이 레이아웃 계획에 적합하며 스케치와 키포인트 같은 밀집 조건이 고품질 이미지 콘텐츠 생성에 유리하다는 것을 경험적으로 밝혀냈습니다.
- 이를 바탕으로, 박스 레이아웃을 스케치나 키포인트 제어 조건으로 변환하는 밀집 조건 생성 모듈을 개발하여 이미지 품질을 향상시키고 사용자 상호작용을 쉽고 직관적으로 만듭니다.
- 더불어, 인간 노동에 의존하지 않고 다양한 시점에서 일관된 캐릭터 이미지를 생성하는 간단하면서도 효과적인 방법을 제안합니다.

### [Memory Augmented Language Models through Mixture of Word Experts](https://arxiv.org/abs/2311.10768)

- 모델의 사이즈를 늘림으로써 언어 모델의 성능을 향상시키는 것이 효과적이지만, 밀집 모델(dense models)에서는 모델의 사이즈와 계산량이 비례해서 증가한다.
- 본 연구에서는 Mixture-of-Experts(MoE) 스타일 모델들을 통해 학습 용량과 FLOPs(부동소수점 연산) 간의 상관관계를 크게 줄이려고 시도하였다.
- 제안된 접근 방법은 'Mixture of Word Experts (MoWE)'로, 다수의 단어별 전문가가 희소 메모리 역할을 하는 메모리 확장 모델로 볼 수 있다.
- MoWE는 유사한 FLOPs를 가진 T5 모델 계열에 비해 다양한 자연어 처리(NLP) 과제에서 상당히 더 나은 성능을 보여줬다.
- 또한, MoWE는 지식 집약적인 과제에서 일반 MoE 모델을 능가하며, 희소 메모리를 검색하는 복잡한 메커니즘을 요구하는 기타 복잡한 메모리 확장 방식과 유사한 성능을 보인다.

### [ProAgent: From Robotic Process Automation to Agentic Process Automation](https://arxiv.org/abs/2311.10751)

- 고대 수차에서 로봇 프로세스 자동화(RPA)에 이르기까지, 자동화 기술은 지난 역사를 통해 힘든 작업으로부터 인간을 해방시켜 왔습니다.
- 현재 RPA는 워크플로우 구성의 정교한 설계와 워크플로우 실행 중의 동적 의사 결정과 같이 인간과 유사한 지능을 요구하는 작업에서 어려움을 겪고 있습니다.
- 이 논문은 대규모 언어 모델(LLMs)을 기반으로 한 에이전트를 사용하여 작업 구성과 실행에 따른 인간 노동을 에이전트에 맡기는 새로운 자동화 패러다임인 '에이전틱 프로세스 자동화(APA)'를 소개합니다.
- 또한, 인간 지시에 따라 워크플로우를 만들고 전문화된 에이전트를 조정하여 복잡한 결정을 내리는 LLM 기반 에이전트인 ProAgent를 구현합니다.
- 실증 실험을 통해 APA의 실행 가능성을 보여주고 에이전트에 의해 주도되는 새로운 자동화 패러다임의 가능성을 드러냅니다.
- 이 논문의 코드는 https://github.com/OpenBMB/ProAgent 에 공개되어 있습니다.

### [MultiLoRA: Democratizing LoRA for Better Multi-Task Learning](https://arxiv.org/abs/2311.11501)

- LoRA는 특정 작업에 대해 LLM(Large Language Models)을 적용할 때 눈에 띄는 자원 효율성을 가지며, 비교적 우수한 성능을 달성하고 있습니다.
- 다양한 작업에서 뛰어난 성능을 보여준 ChatGPT 이후로 하나의 모델을 모든 작업에 적용하려는 시도가 증가하고 있습니다.
- 그러나 LoRA의 명시적인 낮은 랭크는 복잡한 다중 작업 환경에서 적응 성능의 한계를 드러내고 있습니다.
- 본 논문에서는 LoRA에서 관찰되는 상위 단일 벡터의 지배성을 줄임으로써 다중 작업 적응을 보다 나아지게 할 수 있는 MultiLoRA를 제안합니다.
- MultiLoRA는 LoRA 모듈을 수평적으로 확장하고 적응 행렬의 매개변수 초기화를 변경하여 매개변수 의존성을 줄입니다.
- 이러한 방식은 더 균형 잡힌 고유 부공간을 제공합니다.
- 저자들은 지시문 따르기, 자연어 이해, 세계 지식 등 서로 다른 의미와 구문 샘플을 포함하기 위해 특화된 훈련 데이터를 구축합니다.
- 추가 매개변수의 단 2.5%만을 사용하여, MultiLoRA는 다양한 벤치마크와 모델 크기에서 단일 LoRA 방식과 미세 조정(fine-tuning)을 능가하는 성과를 보여줍니다.
- MultiLoRA의 가중치 업데이트 행렬에 대한 추가 조사는 상위 단일 벡터에 대한 의존성이 감소되고 더 민주적인 단위 변환 기여를 보여줍니다.

### [GPT-4V(ision) for Robotics: Multimodal Task Planning from Human Demonstration](https://arxiv.org/abs/2311.12015)

- 본 논문에서는 인간의 행동 관찰을 통합함으로써 로봇 조작을 용이하게 하는 일반 목적의 비전 언어 모델인 GPT-4V를 강화하는 파이프라인을 소개합니다.
- 이 시스템은 인간이 수행하는 작업을 담은 비디오를 분석하여 작업환경과 행동의 세부사항을 텍스트로 변환하는 GPT-4V를 활용하여 실행 가능한 로봇 프로그램을 생성합니다.
- 이어서 GPT-4 기반의 작업 계획자를 사용하여 작업 계획과 관련된 비디오를 재분석합니다.
- 개방형 어휘 객체 감지기를 사용하여 객체 이름을 확인하고, 손과 객체의 상호작용에 초점을 맞추어 집거나 놓는 순간을 탐지합니다.
- 이 공간적-시간적 맥락의 탐지는 특정한 접촉 방식, 경유지, 신체 자세 등과 같은 affordance 데이터를 추가로 수집하는 것을 허용합니다.
- 다양한 시나리오에 걸친 실험을 통해 이 방법이 인간의 시범을 토대로 제로샷 방식으로 실제 로봇 작업을 달성하는 데 효과적인 것으로 나타났습니다.
- GPT-4V/GPT-4의 프롬프트는 이 프로젝트 페이지에서 확인할 수 있습니다: https://microsoft.github.io/GPT4Vision-Robot-Manipulation-Prompts/.

### [Text-to-Sticker: Style Tailoring Latent Diffusion Models for Human Expression](https://arxiv.org/abs/2311.10794)

- '스타일 맞춤'이라는 새로운 방식을 소개하여 잠재 확산 모델(LDMs)을 높은 시각적 품질, 프롬프트 정렬 및 장면 다양성을 가진 특정 도메인에서 미세 조정할 수 있다.
- 스티커 이미지 생성을 대상 도메인으로 선택하였는데, 이는 대규모 LDM에서 일반적으로 생성되는 사실적 샘플과 상당히 다르다.
- 텍스트-투-이미지 모델인 Emu로 시작하여, 사실적 모델을 이용한 프롬프트 공학이 스티커를 생성할 때 프롬프트 정렬과 장면 다양성이 낮다는 것을 보여준다.
- 이러한 단점을 극복하기 위해 수백만 개의 스티커 같은 이미지를 약한 감독을 사용하여 수집하고, 다양성을 이끌어내기 위해 Emu를 처음에 미세 조정한다.
- 그 다음, 모델 생성물에서 사람 중심의 루프(HITL) 정렬 및 스타일 데이터 세트를 큐레이션하고 각각 프롬프트 정렬과 스타일 정렬을 개선하기 위해 미세 조정한다.
- 이러한 데이터 세트에 순차적으로 미세 조정을 하면 스타일 정렬과 프롬프트 정렬 개선 사이에 트레이드 오프가 발생한다.
- 이러한 트레이드 오프를 해결하기 위해, 내용과 스타일 분포에 동시에 적합한 새로운 미세 조정 방법인 '스타일 맞춤'을 제안한다.
- 평가 결과는 기본 Emu 모델을 스티커 생성을 위해 프롬프트 공학을 사용하는 것과 비교하여, 시각적 품질은 14%, 프롬프트 정렬은 16.2%, 장면 다양성은 15.3% 향상되었다는 것을 보여준다.

### [TPTU-v2: Boosting Task Planning and Tool Usage of Large Language Model-based Agents in Real-world Systems](https://arxiv.org/abs/2311.11315)

- 대규모 언어 모델(Large Language Models, LLM)은 자연어 처리 작업뿐만 아니라 API와 같은 외부 도구를 사용하는 것을 포함한 작업 계획(task planning)에 능숙함을 보여왔습니다.
- 그러나 실세계 복잡한 시스템은 작업 계획과 도구 사용에 있어 세 가지 일반적인 문제가 있습니다: (1) 많은 API를 LLM의 프롬프트에 모두 적용할 수 없는 토큰 길이 제한, (2) 복잡한 작업에 대한 올바른 하위 작업 및 API 호출 순서를 LLM이 계획하기 어렵고, (3) 비슷한 의미와 기능을 가진 API 간에 구분하는 어려움이 있습니다.
- 이 논문은 실제 시스템 내에서 LLM 기반 에이전트의 작업 계획과 도구 사용(Task Planning and Tool Usage, TPTU) 능력을 향상시키기 위한 종합적인 프레임워크를 소개합니다.
- 이 프레임워크는 세 가지 핵심 구성요소를 포함합니다: (1) 사용자 작업과 관련된 가장 적절한 API를 선택하는 API Retriever, (2) 작업 계획과 API 호출에 더 유능한 LLM로 기본 LLM을 미세 조정하는 LLM Finetuner, (3) 구분하기 어려운 API와 관련된 다양한 데모를 적응적으로 검색하는 Demo Selector로, 이는 최종 성능을 향상시키기 위한 맥락 내 학습에 사용됩니다.
- 상업적 시스템과 오픈 소스 학술 데이터셋에서 방법론을 검증했으며, 개별 구성요소 및 통합된 프레임워크의 효율성을 명확히 나타내는 결과를 제시합니다.

### [M$^{2}$UGen: Multi-modal Music Understanding and Generation with the Power of Large Language Models](https://arxiv.org/abs/2311.11255)

- 대규모 언어 모델(Large Language Models, LLMs)을 활용한 연구가 급증하는 가운데, 텍스트, 음성, 이미지, 비디오 등 다양한 모달리티를 이해하고 이미지, 비디오, 음악과 같은 결과물을 생성하는 강력한 이유 능력을 활용하는 연구가 많다.
- 그러나 LLMs을 이용하여 이해와 생성을 결합하는 연구는 여전히 제한적이며 초기 단계에 있다.
- 이러한 격차를 해소하기 위해, 저자들은 다양한 모달리티에 대한 음악 이해와 생성을 통합하는 멀티모달 음악 이해 및 생성(M$^{2}$UGen) 프레임워크를 소개한다.
- M$^{2}$UGen 프레임워크는 음악, 이미지, 비디오에서 영감을 받아 창의성을 발휘할 수 있도록 설계되었으며, 미리 훈련된 MERT, ViT, ViViT 모델을 사용한다.
- 음악 생성을 위해 저자들은 AudioLDM 2와 MusicGen의 사용을 탐구한다.
- 멀티모달 이해와 음악 생성 사이의 연결은 LLaMA 2 모델의 통합을 통해 이루어진다.
- 또한, 텍스트/이미지/비디오-투-뮤직 생성을 지원하는 광범위한 데이터셋을 생성하기 위해 MU-LLaMA 모델을 사용한다.
- 저자들은 제안된 M$^{2}$UGen 프레임워크에 대해 철저한 평가를 실시한다.
- 실험 결과는 저자들의 모델이 현재 최고 수준의 모델들의 성능을 달성하거나 능가함을 보여준다.

### [Adapters: A Unified Library for Parameter-Efficient and Modular Transfer Learning](https://arxiv.org/abs/2311.11077)

- 'Adapters'라는 오픈 소스 라이브러리를 제공하여 대규모 언어 모델에서의 파라미터 효율적이고 모듈러한 전이 학습을 통일합니다.
- 다양한 어댑터 방법 10가지를 통합한 단일 인터페이스로 사용자의 편의성과 유연한 구성을 제공합니다.
- 연구자와 실무자들이 복잡한 어댑터 설정을 설계할 수 있도록 구성 블록을 통해 어댑터의 모듈성을 활용할 수 있습니다.
- Adapters 라이브러리는 기존의 전체 파인 튜닝에 비해 다양한 자연어 처리(NLP) 작업에서의 성능을 평가함으로써 효과를 입증합니다.
- 전통적인 파인 튜닝 패러다임의 도전 과제에 대응하고 더욱 효과적이고 모듈러한 전이 학습을 촉진하기 위한 강력한 도구를 제공합니다.
- 이 라이브러리는 [https://adapterhub.ml/adapters](https://adapterhub.ml/adapters)를 통해 사용할 수 있습니다.

### [GPQA: A Graduate-Level Google-Proof Q&A Benchmark](https://arxiv.org/abs/2311.12022)

- GPQA 데이터셋은 생물학, 물리학, 화학 분야 전문가들에 의해 작성된 448개의 다지선다형 문제를 포함하고 있으며, 높은 수준의 질문들로 구성되어 있다.
- 해당 분야 박사학위 소지자나 박사과정에 있는 전문가들조차 평균 65%의 정확도를 보였고(명백한 실수를 인정한 후에는 74%), 비전문가 검증자들은 웹을 무제한으로 활용하여 30분 이상 투자한 뒤에도 34%의 정확도에 그쳤다.
- 이러한 결과는 문제들이 구글 검색으로 쉽게 답을 찾을 수 없는 'Google-proof' 수준임을 나타낸다.
- 최첨단 인공지능 시스템도 이러한 질문들에 어려움을 겪으며, GPT-4 기반의 가장 강력한 기준 모델이 39%의 정확도를 달성했을 뿐이다.
- 향후 AI 시스템이 새로운 과학적 지식 개발 등 매우 어려운 문제를 해결하는 데 도움을 주기 위해서는, 전문가들조차 어려워하는 이러한 문제를 처리할 수 있는 확장 가능한 감독 방법을 개발해야 한다.
- GPQA의 난이도는 인간의 감독자로서 전문 지식과 기술을 가진 사람들에게도 도전이 될 뿐만 아니라, 최첨단 AI 시스템에도 도전적이어서 현실적인 확장 가능한 감독 실험을 할 수 있는 기회를 제공한다.
- 이 연구는 인간 전문가가 인간 능력을 뛰어넘는 AI 시스템으로부터 신뢰할 수 있는 정보를 얻는 방법을 고안하는 데 도움이 될 수 있을 것으로 기대된다.

### [ToolTalk: Evaluating Tool-Usage in a Conversational Setting](https://arxiv.org/abs/2311.10775)

- 대형 언어 모델(대규모 언어 모델, LLMs)은 추론 및 의사 결정 기술에서 상당한 개선을 보여주며 사용자와 자연스러운 대화를 할 수 있음.
- 최근 연구들은 비공개 또는 최신 정보에 접근하고 사용자를 대신하여 행동을 취할 수 있도록 외부 도구로 LLM 기반 어시스턴트를 확장하려고 함.
- 이 논문은 대화를 통해서 명시된 다단계 도구 사용이 필요한 복잡한 사용자 의도를 포함하는 벤치마크인 ToolTalk을 도입함.
- ToolTalk는 7개 플러그인으로 그룹화된 28개 도구를 포함하며 각 도구의 완전한 시뮬레이션 구현을 포함하여 실행 피드백에 의존하는 어시스턴트의 완전 자동화된 평가를 가능하게 함.
- ToolTalk는 정보 검색이나 참조를 위한 도구보다는 세계에 외부적으로 영향을 미치는 도구에 중점을 둠.
- GPT-3.5와 GPT-4는 ToolTalk에서 각각 26% 및 50%의 성공률을 보임.
- 오류 분석을 통해 세 가지 주요 오류 범주가 드러나며 향후 개선 방향을 제시함.
- ToolTalk는 https://github.com/microsoft/ToolTalk에서 공개됨.


## License

This project is licensed under the [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/deed.ko) license.

## Citation

If this work is helpful, please kindly cite as:

```bibtex
@misc{daily_papers,
  title = {Huggingface Daily Papers},
  author = {AK391},
  howpublished = {\url{https://huggingface.co/papers}},
  year = {2023}
}

@misc{daily_papers,
  title = {Automatically translate and summarize huggingface's daily papers into korean},
  author = {l-yohai},
  howpublished = {\url{https://github.com/l-yohai/daily_papers_ko}},
  year = {2023}
}
```

## Star History

![Star History Chart](https://api.star-history.com/svg?repos=l-yohai/daily_papers_ko&type=Date)
