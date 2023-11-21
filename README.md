# Daily Papers

## Project Description

This project aims to automatically translate and summarize [Huggingface's daily papers](https://huggingface.co/papers) into Korean using ChatGPT.

Thanks to [@AK391](https://github.com/AK391) for great work.

## Daily Papers (2023-11-21)

### [Video-LLaVA: Learning United Visual Representation by Alignment Before Projection](https://arxiv.org/abs/2311.10122)

- 대규모 비전-언어 모델 (LVLM)은 시각-언어 이해 작업의 성능을 향상시켰으나, 기존 접근 방식들은 이미지와 비디오를 별도의 특징 공간으로 인코딩하여 대규모 언어 모델에 입력으로 사용한다는 한계가 있습니다.
- 이는 이미지와 비디오에 대한 통합적인 토큰화가 부족하여, 여러 빈약한 투영층에서 다중 모달 상호작용을 학습하는데 어려움을 초래합니다.
- 본 연구에서는 기초 LLM을 통합된 LVLM으로 발전시키기 위해 시각적 표현을 언어 특징 공간으로 통합하는 방법을 제안합니다.
- 이로 인해 간단하지만 강력한 LVLM 베이스라인인 Video-LLaVA가 제시되었고, 이미지와 비디오의 혼합 데이터셋으로부터 학습하여 서로의 성능을 상호 향상시키는 결과를 도출했습니다.
- Video-LLaVA는 5개의 이미지 질의응답 데이터셋과 4개의 이미지 벤치마크 툴킷을 포함한 9개의 이미지 벤치마크에서 우수한 성능을 달성했습니다.
- 또한, Video-LLaVA는 MSRVTT, MSVD, TGIF, ActivityNet에서 각각 5.8%, 9.9%, 18.6%, 10.1% 향상된 성능으로 Video-ChatGPT를 능가했습니다.
- 광범위한 실험을 통해 Video-LLaVA가 이미지와 비디오에 특화된 모델들을 능가하는 통합된 시각적 표현을 통해 이미지와 비디오의 상호 이점을 강조하는 것으로 나타났습니다.
### [Emu Video: Factorizing Text-to-Video Generation by Explicit Image Conditioning](https://arxiv.org/abs/2311.10709)

- Emu Video는 텍스트 기반 이미지 생성 후 그 이미지와 텍스트를 기반으로 동영상을 생성하는 두 단계로 구성된 텍스트-비디오 생성 모델을 제시한다.
- 본 연구는 확산에 대한 조정된 노이즈 스케줄 및 다단계 훈련과 같은 중요한 설계 결정을 통해 고해상도의 고품질 비디오를 직접 생성할 수 있게 한다.
- 인간 평가에서 Emu Video는 기존 연구에 비해 더 높은 품질의 비디오 생성을 선호하며, Google의 Imagen Video, Nvidia의 PYOCO, Meta의 Make-A-Video와 비교하였을 때 각각 81%, 90%, 96%의 선호도를 나타냈다.
- Emu Video는 RunwayML의 Gen2나 Pika Labs와 같은 상업용 솔루션보다도 성능이 뛰어나다.
- 이러한 요소화 접근 방식은 사용자의 텍스트 프롬프트에 기반하여 이미지를 애니메이션화하는 데 자연스럽게 적용되며, 이 방식에서 생성된 비디오는 기존 연구 대비 96% 높은 선호도를 얻었다.
### [Rethinking Attention: Exploring Shallow Feed-Forward Neural Networks as an Alternative to Attention Layers in Transformers](https://arxiv.org/abs/2311.10642)

- 이 연구는 기존 Transformer 모델의 주의 기제를 흉내내기 위해 표준 얕은 전방향 신경망을 사용하는 효과에 대한 분석을 제시합니다.
- Transformer의 주요 주목 메커니즘 요소를 간단한 전방향 네트워크로 대체하고, 지식 증류를 사용하여 원래 구성 요소를 훈련시켰습니다.
- IWSLT2017 데이터셋에서 수행된 실험을 통해 이러한 "주목 없는 Transformers"가 원래 아키텍처의 성능과 경쟁할 수 있는 능력을 드러냈습니다.
- 다양한 네트워크 유형 및 크기를 대체하며 실시한 철저한 소거 연구를 통해 접근 방식의 실현가능성에 대한 통찰력을 제공합니다.
- 이 연구는 얕은 전방향 네트워크가 주의 메커니즘을 모방하는 데 적응할 수 있는 능력뿐만 아니라, 시퀀스 대 시퀀스 작업을 위한 복잡한 아키텍처를 간소화할 수 있는 잠재력을 강조합니다.
### [MetaDreamer: Efficient Text-to-3D Creation With Disentangling Geometry and Texture](https://arxiv.org/abs/2311.10123)

- 3D 객체 합성을 위한 생성 모델은 2D 확산 모델에서 추출된 사전 지식을 통합하면서 상당한 발전을 이루었지만, 기존 3D 합성 프레임워크 내에서 여전히 다중 시점 기하학적 불일치와 느린 생성 속도라는 문제가 남아 있다.
- 이러한 문제들은 주로 기하학적 사전 지식의 부족과 전통적인 3D 생성 방법에서의 기하학과 질감의 얽힘이라는 두 가지 요인에 기인한다.
- 이에 따라, MetaDreamer는 풍부한 2D 및 3D 사전 지식을 활용하는 두 단계 최적화 접근법을 도입한다.
- 첫 단계에서는 3D 객체의 다중 시점 일관성과 정확도를 보장하기 위해 기하학적 표현을 최적화하는 데 중점을 둔다.
- 두 번째 단계에서는 기하학을 미세 조정하고 질감을 최적화하여 더 세련된 3D 객체를 달성한다.
- 두 단계에서 각각 2D 및 3D 사전 지식을 활용함으로써 기하학과 질감 사이의 상호 의존성을 효과적으로 해결한다.
- MetaDreamer는 각 단계에 대해 명확한 최적화 목표를 설정함으로써 3D 생성 과정에서 중요한 시간 절약을 실현한다.
- 결과적으로, MetaDreamer는 텍스트 프롬프트에 기반한 고품질의 3D 객체를 20분 내에 생성할 수 있으며, 현재로서는 가장 효율적인 text-to-3D 생성 방법이다.
- 또한, 프로세스에 이미지 제어를 도입하여 3D 생성의 조종성을 향상시킨다.
- 광범위한 경험적 증거는 우리의 방법이 높은 효율성뿐만 아니라 현재 최신의 3D 생성 기술과 맞먹는 품질 수준을 달성한다는 것을 확인한다.
### [Camels in a Changing Climate: Enhancing LM Adaptation with Tulu 2](https://arxiv.org/abs/2311.10702)

- TÜLU의 릴리즈 이후, 오픈 리소스 지침 튜닝이 빠르게 발전해왔으며, 기본 모델 향상과 새로운 파인 튜닝 기술들이 등장하였습니다.
- 저자들은 이러한 발전들을 TÜLU에 통합하여 TÜLU 2를 개발하였는데, 이는 사전 훈련된 언어 모델을 다운스트림 작업과 사용자 선호에 맞추는 것에 대한 이해와 최선의 관행을 향상시키기 위한 개선된 TÜLU 모델 시리즈입니다.
- 구체적으로, (1) 향상된 고품질 지침 데이터셋 컬렉션인 TÜLU-V2-mix, (2) V2 혼합물에 파인 튜닝된 LLAMA-2 모델인 TÜLU 2, (3) 직접 선호 최적화(DPO)를 이용한 훈련을 받은 TÜLU 2+DPO 모델들을 포함하여 현재까지 가장 큰 DPO 훈련 모델인 TÜLU 2+DPO 70B, (4) V2 혼합물에서 파인 튜닝된 CODE LLAMA 모델들을 능가하는 CODE TÜLU 2를 출시하였습니다.
- 여러 관점에서의 평가를 통해 TÜLU 2 시리즈가 오픈 모델 중 최상의 성능을 달성하며, 일부 벤치마크에서는 GPT-3.5-turbo-0301과 동등하거나 그 이상의 성능을 보임을 확인하였습니다.
- 연구진은 이러한 체크포인트, 데이터, 훈련 및 평가 코드를 모두 공개하여 대규모 언어 모델의 적응에 대한 미래의 오픈 노력을 촉진하고자 합니다.
### [I&S-ViT: An Inclusive & Stable Method for Pushing the Limit of Post-Training ViTs Quantization](https://arxiv.org/abs/2311.10126)

- 본 논문에서는 새로운 방법인 I&S-ViT를 도입하여 비전 변환기(ViTs)의 사후 학습 양자화(PTQ)를 포괄적이고 안정적으로 조절하는 방법을 제시합니다.
- I&S-ViT는 ViTs의 PTQ에 있어서 두 가지 문제를 식별합니다: (1) 사후-Softmax 활성화를 위한 풍부한 로그2 양자화기의 양자화 비효율성; (2) 사후-LayerNorm 활성화를 위한 미세한 양자화 입자도에서 울퉁불퉁하고 확대된 손실 풍경.
- 이러한 문제들을 해결하기 위해, I&S-ViT는 (1) 이동 메커니즘이 포함된 새로운 이동-일관성-로그2 양자화기(SULQ)를 도입하여 포괄적인 도메인 표현과 정확한 분포 근사를 달성; (2) 채널별 및 계층별 양자화의 장점을 결합하는 3단계 순조로운 최적화 전략(SOS)을 제시합니다.
- 다양한 비전 작업에서의 포괄적인 평가를 통해 특히 저비트 상황에서 기존 ViTs의 PTQ 방법들에 비해 I&S-ViT의 우수성을 검증합니다.
- 예를 들어, I&S-ViT는 3비트 ViT-B의 성능을 50.68% 향상시키는 인상적인 결과를 달성합니다.
### [SelfEval: Leveraging the discriminative nature of generative models for evaluation](https://arxiv.org/abs/2311.10708)

- 본 연구에서는 텍스트-이미지 생성 모델을 이용하여 모델이 스스로 텍스트-이미지 이해능력을 완전히 자동화된 방식으로 평가하는 방법을 제시하였다.
- 'SelfEval'이라고 불리는 우리의 방법은 생성 모델을 사용하여 실제 이미지들이 텍스트 프롬프트를 통해 얼마나 가능성이 있는지를 계산함으로써 생성 모델을 판별적인 과제에 직접 적용할 수 있게 한다.
- SelfEval을 사용하여, 다양한 모달의 텍스트-이미지 판별 모델을 평가하기 위해 만들어진 표준 데이터셋을 재활용하여, 속성 결합, 색상 인식, 수량 세기, 모양 인식, 공간 이해와 같은 분야에서 생성 모델의 성능을 세밀하게 평가한다.
- SelfEval은 다양한 모델과 벤치마크에 걸쳐 텍스트 충실도를 측정하는 골드 스탠다드인 인간 평가와 높은 일치도를 보여주는 최초의 자동화된 척도라고 할 수 있다.
- 뿐만 아니라, SelfEval은 Winoground 이미지 점수와 같은 도전적인 과제에서 생성 모델이 판별 모델과 경쟁력 있는 성능을 보이게 할 수 있다.
- 표준 자동화 척도들이 DrawBench와 같은 벤치마크에서 텍스트 충실성을 측정하는데 있어 가지는 심각한 단점을 보여주고, SelfEval이 이런 문제들을 어떻게 회피하는지도 보여준다.
- 연구팀은 SelfEval이 확산 모델에 대한 쉽고 신뢰할 수 있는 자동 평가를 가능하게 해줄 것을 기대한다.
### [VideoCon: Robust Video-Language Alignment via Contrast Captions](https://arxiv.org/abs/2311.10111)

- 최신 비디오-언어 정렬 모델은 대규모 데이터에 (사전)훈련되어 있음에도 불구하고 언어 캡션의 의미상 타당한 대조적 변경에 대해 견고하지 못합니다.
- 본 연구는 엔티티 교체, 행동 변화, 이벤트 순서 반전 등 모델이 견고해야 할 다양한 대조적 미스얼라인먼트를 확인했습니다.
- 이에 따라, 대규모 언어 모델을 사용하여 생성된 대조적인 비디오 캡션과 원본 및 대조 캡션 간의 차이에 대한 설명문을 포함하는 비디오-언어 정렬 데이터셋인 VideoCon을 소개합니다.
- 비디오-언어 추론 평가 및 설명 생성을 위해 VideoCon으로 파인튜닝된 비디오-언어 생성 모델이 제안됩니다.
- VideoCon 기반 정렬 모델은 기존 모델들에 비해 뛰어난 성능을 보이며, 인간이 생성한 대조 캡션에서 비디오-언어 정렬 작업의 AUC가 12점 증가했습니다.
- 또한, 이 모델은 텍스트-비디오 검색(SSv2-Temporal) 및 비디오 질문 답변(ATP-Hard)과 같은 시간적으로 광범위한 비디오-언어 작업에서새로운 최첨단 제로샷 성능을 달성했습니다.
- 새로운 비디오와 인간이 만든 설명에 대해서도 뛰어난 성능을 보여줍니다.
- 연구에 사용된 코드와 데이터는 https://github.com/Hritikbansal/videocon 에서 사용할 수 있습니다.
### [Testing Language Model Agents Safely in the Wild](https://arxiv.org/abs/2311.10538)

- 실세계에서 안전한 자율 행동을 위해서는 야외 테스트에서 안전성이 확보되어야 한다는 전제 하에, 실제 환경에서 자율 테스트 시 독특한 안전 문제들이 대두되며, 이는 테스트 중 해를 끼칠 가능성뿐만 아니라 새롭고 위험할 수 있는 에이전트 행동을 실세계에서 잠재적으로 악의적인 행위자들과 접할 위험 때문이다.
- 이 연구는 인터넷 상에서 자율 에이전트 테스트를 안전하게 수행할 수 있는 프레임워크를 제시하며, 에이전트의 행동을 맥락에 따라 감시하는 모니터가 안전 경계를 강력하게 적용해 위험한 테스트를 중단시키고 의심스러운 행동을 분류하여 사람이 검토할 수 있도록 한다.
- 기본적인 안전 모니터 설계 가능성을 확인하고, 적대적인 시뮬레이션 에이전트를 사용하여 이 모니터가 불안한 상황을 식별하고 중단하는 능력을 측정했다.
- 실제 AutoGPT를 사용한 일련의 실제 테스트를 적용하여, 성장하고 있는 자율 에이전트들이 야외 테스트 환경에서 마주하게 될 여러 한계점과 도전 과제를 확인했다.
### [Distilling and Retrieving Generalizable Knowledge for Robot Manipulation via Language Corrections](https://arxiv.org/abs/2311.10678)

- 오늘날의 로봇 정책은 새로운 환경에 일반화하는 데에 있어서 미흡한 성능을 보이고 있으며, 인간의 수정 피드백은 이러한 일반화를 가능하게 하는 중요한 지도 방식이다.
- 온라인 인간 수정에서 적응하고 학습하는 것은 쉽지 않은 작업이며, 로봇은 새로운 상황에서 올바른 정보를 검색하고 개입율을 줄이기 위해 시간이 지남에 따라 인간 피드백을 기억해야 할 뿐만 아니라, 고차원적인 인간의 선호 사항에 관한 임의의 수정부터 저차원적인 기술 매개변수의 조정에 이르는 피드백에 대응할 수 있어야 한다.
- 본 연구에서는, 임의의 언어 피드백에 응답하고, 수정에서 일반화 가능한 지식을 추출하며, 텍스트와 시각적 유사성에 근거하여 새로운 설정에서 성능을 향상시키기 위해 관련된 과거 경험을 검색할 수 있는 대형 언어 모델(LLM) 기반 시스템인 'Distillation and Retrieval of Online Corrections (DROC)'을 제시한다.
- DROC는 고차원적인 태스크 계획부터 저차원적인 스킬 원시데이터의 실패에 이르는 온라인 언어 수정의 연속에 반응할 수 있다.
- DROC가 온라인 수정의 연속에서 관련 정보를 지식 베이스에 효과적으로 추출하며 새로운 태스크 또는 객체 인스턴스 설정에서 그 지식을 검색하는 것을 입증하였다.
- DROC는 다른 기술들과 비교했을 때, LLM에 의해 직접 생성된 로봇 코드를 사용함으로써 첫 라운드에서 필요한 수정의 총 수의 절반만을 사용하여 성능을 뛰어넘고, 두 번의 반복 후 거의 또는 전혀 수정이 필요 없었다.
- 추가적인 결과, 비디오, 프롬프트, 코드 등은 https://sites.google.com/stanford.edu/droc 에서 확인할 수 있다.
### [UnifiedVisionGPT: Streamlining Vision-Oriented AI through Generalized Multimodal Framework](https://arxiv.org/abs/2311.10125)

- 현재 인공지능 분야에서 기초 모델은 언어와 시각 도메인에서 발전의 토대를 마련하고 있으며, OpenAI의 GPT-4는 대형 언어 모델로써, Meta의 SAM과 DINO, YOLOS 같은 컴퓨터 비전(CV)도메인 최첨단 모델들과 경쟁하고 있다.
- 그러나 새로운 모델을 처음부터 훈련하는데 필요한 재정적, 계산적 부담이 진전에 상당한 장벽으로 남아 있다.
- 이러한 도전에 대응하여, 우리는 'UnifiedVisionGPT'라는 새로운 프레임워크를 도입하여 최첨단 비전 모델을 통합하고 자동화함으로써 시각 지향 AI의 발전을 용이하게 할 수 있는 방안을 제시한다.
- UnifiedVisionGPT는 네 가지 주요 특징을 통해 자신을 차별화한다:
  - (1) 다양한 어플리케이션에 적용 가능한 범용 멀티모달 프레임워크를 제공하며, 멀티모달 기반 모델의 강점을 활용한다.
  - (2) 다양한 최첨단 비전 모델을 매끄럽게 통합하여 각 모델의 최상의 구성요소를 활용한 종합 멀티모달 플랫폼을 생성한다.
  - (3) 시각 지향 AI에 우선 순위를 두어, 현재 대형 언어 모델(LMMs)의 발전 경로와 비교하여 CV 도메인에서의 더 빠른 진전을 보장한다.
  - (4) 텍스트 프롬프트와 이미지와 같은 다양한 멀티모달 입력을 기반으로 최적의 결과를 생성하는 최첨단 비전 모델 선택을 자동화한다.
- 이 논문은 UnifiedVisionGPT의 구조와 능력을 설명하며, 향상된 효율성, 범용성, 일반화 및 성능을 통해 컴퓨터 비전 분야를 혁신할 잠재력을 보여준다.
- 구현체, 통합 멀티모달 프레임워크 및 포괄적 데이터셋은 https://github.com/LHBuilder/SA-Segment-Anything에서 공개적으로 이용 가능하다.


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
  howpublished = {\url{https://github.com/l-yohai/daily_papers}},
  year = {2023}
}
```

## Star History

![Star History Chart](https://api.star-history.com/svg?repos=l-yohai/daily_papers&type=Date)
