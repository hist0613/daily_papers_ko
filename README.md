# Daily Papers

## Project Description

This project aims to automatically translate and summarize [Huggingface's daily papers](https://huggingface.co/papers) into Korean using ChatGPT.

Thanks to [@AK391](https://github.com/AK391) for great work.


## Daily Papers (2023-12-05)

### [Magicoder: Source Code Is All You Need](https://arxiv.org/abs/2312.02120)

![](https://cdn-uploads.huggingface.co/production/uploads/60f1abe7544c2adfd699860c/-m7NQI--aISLeAzdzOt8h.png)

Authors: Yuxiang Wei, Zhe Wang, Jiawei Liu, Yifeng Ding, Lingming Zhang

- 'Magicoder'는 최대 7B개의 매개변수를 가진 오픈소스 코드 대규모 언어 모델(LLMs) 시리즈로, 최상위 코드 모델과의 격차를 현저히 줄인다.
- 이 모델들은 75K의 합성 교육 데이터를 사용하여, 오픈소스 코드 스니펫을 통해 고품질의 코드 교육 데이터를 생성하는 새로운 방법인 'OSS-Instruct'로 훈련되었다.
- 주된 동기는 LLM에 의해 생성되는 합성 데이터의 내재된 편향을 줄이고, 더 다양하고 현실적이며 제어 가능한 데이터 생성을 위해 그들에게 방대한 오픈소스 참고자료를 제공하는 것이다.
- 'OSS-Instruct'의 방법론이 다른 데이터 생성 방법들과 직교하므로, 우리는 'Magicoder'를 향상시킨 'MagicoderS'를 개발할 수 있다.
- Magicoder와 MagicoderS 모두 유사하거나 더 큰 크기의 최신 기술 코드 모델들을 다양한 코딩 벤치마크에서 상당히 능가한다.
- 특히, 'CodeLlama'에 기반한 'MagicoderS-CL-7B'는 ChatGPT보다도 더 높은 성능을 보여준다(HumanEval+에서 66.5 대 65.9 in pass@1).
- 종합적으로 볼 때, 'OSS-Instruct'는 풍부한 오픈소스 참고자료를 사용하여 저편향이면서 고품질의 교육 데이터를 제공하는 새로운 방향을 제시한다.

### [VMC: Video Motion Customization using Temporal Attention Adaption for Text-to-Video Diffusion Models](https://arxiv.org/abs/2312.00845)

![](https://cdn-uploads.huggingface.co/production/uploads/60f1abe7544c2adfd699860c/1KzMMuvCRLqHrRcChoDfk.png)

Authors: Hyeonho Jeong, Geon Yeong Park, Jong Chul Ye

- 텍스트-비디오 확산 모델은 비디오 생성 기술을 크게 발전시켰지만, 맞춤형 동작을 생성하는 것은 여전히 상당한 도전 과제입니다.
- 이러한 모델들은 특정한 영상의 동작을 정확하게 재현하거나, 다양한 시각적 변형을 생성하는 데 어려움을 겪습니다.
- 우리는 비디오 확산 모델 내의 시간적 주의 층을 조정하는 새로운 원샷 튜닝 방법인 비디오 모션 커스터마이제이션(VMC) 프레임워크를 소개합니다.
- VMC는 연속 프레임 사이의 잔여 벡터를 동작 참조로 사용하는 새로운 동작 증류 목표를 도입합니다.
- 확산 과정은 저주파 동작 궤적을 보존하면서 고주파 동작과 무관한 잡음을 이미지 공간에서 완화합니다.
- 우리는 다양한 실제 움직임과 맥락에서 최신 비디오 생성 모델들에 대해 우리의 방법을 검증합니다.
- 관련 코드, 데이터 및 프로젝트 데모는 https://video-motion-customization.github.io에서 확인할 수 있습니다.

### [The Unlocking Spell on Base LLMs: Rethinking Alignment via In-Context Learning](https://arxiv.org/abs/2312.01552)

![](https://cdn-uploads.huggingface.co/production/uploads/60f1abe7544c2adfd699860c/kg4oT5scURsTXbUOY3zg-.png)

Authors: Bill Yuchen Lin, Abhilasha Ravichander, Ximing Lu, Nouha Dziri, Melanie Sclar, Khyathi Chandu, Chandra Bhagavatula, Yejin Choi

- 대규모 언어 모델(LLMs)의 정렬 조정 방식이 기존의 지도 학습과 인간 피드백을 통한 강화 학습에만 의존하고 있었으나, 최근 연구인 LIMA에서 단 1,000개의 예시를 통한 지도 학습으로도 상당한 성능을 달성할 수 있음을 밝혔습니다.
- 해당 발견은 LLM의 정렬 조정이 '피상적'일 수 있다는 가설을 제시하며, 이에 대한 직접적 증거로 기본 LLM과 정렬 조정된 버전 간의 토큰 분포 변화에 대해 분석했습니다.
- 연구 결과, 대부분의 토큰 위치에서 기본 LLM과 정렬 조정된 LLM의 성과가 거의 동일하며 주로 스타일적 토큰에서만 분포 변화가 발생했다는 것을 발견했습니다.
- 이를 바탕으로, 지도 학습이나 강화 학습 없이 기본 LLM을 얼마나 효과적으로 정렬 조정할 수 있는지에 대한 연구 질문을 제기했습니다.
- 본 연구는 URIAL이라는 새로운, 조정 없는 정렬 조정 방법을 소개하며 이는 몇 개의 스타일 예시와 시스템 프롬프트만을 이용한 상황적 학습(ICL)을 통해 효과적인 정렬을 달성합니다.
- 다양한 예시를 통한 철저하고 해석 가능한 평가를 수행한 결과, URIAL을 적용한 기본 LLM은 지도 학습이나 지도 학습과 강화 학습을 결합한 정렬 조정된 모델의 성능에 필적하거나 능가함을 보여줍니다.
- 이러한 발견은 LLM의 정렬 조정이 지니는 피상적 특성과 URIAL의 결과가 전략적 프롬프팅과 상황적 학습을 통해 조정 기반 방법과의 격차를 상당히 줄일 수 있음을 시사합니다.
- 이 연구는 정렬 조정의 깊은 분석과 이론적 이해가 향후 LLM 연구에 있어 중요함을 강조하고 있습니다.

### [VideoSwap: Customized Video Subject Swapping with Interactive Semantic Point Correspondence](https://arxiv.org/abs/2312.02087)

[Watch Video]https://cdn-uploads.huggingface.co/production/uploads/60f1abe7544c2adfd699860c/PahRPBsgHAbIPAs7E8F-u.mp4
<div><video controls src="https://cdn-uploads.huggingface.co/production/uploads/60f1abe7544c2adfd699860c/PahRPBsgHAbIPAs7E8F-u.mp4" muted="false"></video></div>

Authors: Yuchao Gu, Yipin Zhou, Bichen Wu, Licheng Yu, Jia-Wei Liu, Rui Zhao, Jay Zhangjie Wu, David Junhao Zhang, Mike Zheng Shou, Kevin Tang

- 현재의 확산 기반 비디오 편집 기술은 주로 다양한 밀집 대응물을 활용하여 구조를 보존하는 편집에 초점을 맞추고 시간적 일관성과 동작 정렬을 보장했으나, 대상의 형태가 바뀌는 편집에는 비효율적임을 밝혔습니다.
- 본 연구는 원본 비디오의 주요 대상을 상이한 정체성과 형태를 가진 목표 대상으로 교체하는 맞춤형 비디오 주제 교체에 대하여 탐구합니다.
- 기존의 밀집 대응물에 의존하는 방법들과 달리, 이 연구는 대상의 동작 궤적을 맞추고 형태를 수정하기 위해서는 소수의 의미론적 점만으로 충분하다는 관찰에 영감을 받아 VideoSwap 프레임워크를 도입합니다.
- 대응하는 의미론적 점에 대해 다양한 사용자-점 상호작용(예: 점 제거 및 드래그)을 소개하여 적용 범위를 넓힙니다.
- 이 프레임워크는 다양한 실세계 비디오에서 최첨단 비디오 주제 교체 결과를 보여주는 광범위한 실험을 통해 검증되었습니다.

### [DeepCache: Accelerating Diffusion Models for Free](https://arxiv.org/abs/2312.00858)

![](https://cdn-uploads.huggingface.co/production/uploads/60f1abe7544c2adfd699860c/A3C7QqlJUqYhP0i848_QK.png)

Authors: Xinyin Ma, Gongfan Fang, Xinchao Wang

- 디퓨전 모델은 뛰어난 생성 능력으로 이미지 합성 분야에서 주목을 받고 있으나, 연속적인 노이즈 제거 과정과 큰 모델 크기로 인해 상당한 계산 비용이 발생합니다.
- 기존 디퓨전 모델 압축 방법은 대부분 재학습이 필요하며 비용과 실행 가능성 측면에서 여러 도전을 안고 있습니다.
- 본 논문에서는 모델 아키텍처 관점에서 디퓨전 모델을 가속화하는 새로운 훈련 없는 패러다임인 DeepCache를 소개합니다.
- DeepCache는 디퓨전 모델의 순차적 노이즈 제거 단계에서 관찰되는 시간적 중복성을 활용하여, 인접한 덴노이징 단계간 특징을 캐싱하고 검색함으로써 중복 계산을 줄입니다.
- U-Net의 특성을 활용하여 고수준 특징은 재사용하고 저수준 특징은 저비용으로 갱신함으로써, Stable Diffusion v1.5 모델을 2.3배 빠르게 하고 CLIP Score는 0.05만 감소시킵니다.
- LDM-4-G 모델의 경우, ImageNet에서 FID가 0.22만 감소하면서 4.1배 빠른 속도 향상을 달성했습니다.
- DeepCache는 재학습이 필요한 기존의 pruning 및 distillation 방법보다 우월하며, 현재의 샘플링 기술과도 호환됩니다.
- 동일한 처리량의 경우, DeepCache는 DDIM이나 PLMS와 비교하여 비슷하거나 약간 향상된 결과를 달성합니다.
- 해당 코드는 https://github.com/horseee/DeepCache에서 제공됩니다.

### [Segment and Caption Anything](https://arxiv.org/abs/2312.00869)

![](https://cdn-uploads.huggingface.co/production/uploads/60f1abe7544c2adfd699860c/uVoIhAqgvhaXDcF3gKB-L.png)

Authors: Xiaoke Huang, Jianfeng Wang, Yansong Tang, Zheng Zhang, Han Hu, Jiwen Lu, Lijuan Wang, Zicheng Liu

- 이 연구에서는 Segment Anything Model (SAM)을 사용하여 지역 캡션 생성 기능을 효율적으로 장착할 수 있는 방법을 제안합니다.
- SAM은 어떤 대상이든 분할하는 강력한 일반화 능력을 가지고 있으나, 의미론적 이해에는 미흡합니다.
- 경량 쿼리 기반의 특징 혼합기를 도입하여, 지역 특정 특징들을 언어 모델의 임베딩 공간과 맞추어 나중에 캡션을 생성하도록 합니다.
- 이 방법은 훈련 가능한 매개 변수 수가 적어(천만 개 정도) 계산 비용, 메모리 사용량 및 통신 대역폭이 줄어들어 빠르고 확장성 있는 훈련을 가능하게 합니다.
- 지역 캡션 데이터의 부족 문제를 해결하기 위해, 객체 감지 및 분할 작업으로 모델을 먼저 사전 훈련할 것을 제안합니다.
- 약한 감독 사전 훈련이라고 부르는 이 단계는, 전문 설명이 아닌 대신 카테고리 이름만 포함하는 사전 훈련 데이터를 활용하도록 합니다.
- 다양한 실험을 통해 우리의 방법의 우수성을 입증하고 각 설계 선택을 검증합니다.
- 이 작업은 지역 캡션 데이터를 확장하기 위한 발판을 마련하고 SAM에 지역 의미론을 효율적으로 추가하는 방법을 탐색하는 데 도움이 될 수 있습니다.
- 프로젝트 페이지와 관련 코드는 다음의 링크를 통해 접근할 수 있습니다: https://xk-huang.github.io/segment-caption-anything/.

### [GIVT: Generative Infinite-Vocabulary Transformers](https://arxiv.org/abs/2312.02116)

![](https://cdn-uploads.huggingface.co/production/uploads/60f1abe7544c2adfd699860c/G_9ZHDe9BdHde3XnD3dpn.png)

Authors: Michael Tschannen, Cian Eastwood, Fabian Mentzer

- 이 논문은 유한한 어휘 대신 실수로 구성된 벡터 시퀀스를 생성하는 새로운 방법론인 'Generative Infinite-Vocabulary Transformers (GIVT)'를 도입합니다.
- GIVT 개발을 위해 디코더 전용 트랜스포머에 두 가지 간단한 수정을 제안하는데, 입력에서 유한 어휘 룩업 테이블을 입력 벡터의 선형 투영으로 대체하고, 출력에서 로짓 예측을 다변량 가우스 혼합 모델의 매개변수로 대체합니다.
- VQ-GAN과 MaskGIT이 VQ-VAE의 이산 잠재 시퀀스를 모델링하는 이미지 생성 패러다임에서 영감을 받아, GIVT는 양자화되지 않은 실수 값 잠재 시퀀스를 모델링하는데 사용됩니다.
- GIVT는 반복적인 마스킹 모델링을 사용한 클래스 조건부 이미지 생성 분야에서 MaskGIT와 경쟁력 있는 결과를 보이며, 인과 모델링을 위해 사용될 때 VQ-GAN 및 MaskGIT를 뛰어넘는 성능을 보입니다.
- 마지막으로, 이 방법을 UViM 프레임워크의 VAE 기반 변형에 적용하여 파노프틱 세분화와 깊이 추정 분야에서도 경쟁력 있는 결과를 얻습니다.

### [Segment Any 3D Gaussians](https://arxiv.org/abs/2312.00860)

[Watch Video]https://cdn-uploads.huggingface.co/production/uploads/60f1abe7544c2adfd699860c/y-qGKx5OOM-XDqPOCLchM.mp4
<div><video controls src="https://cdn-uploads.huggingface.co/production/uploads/60f1abe7544c2adfd699860c/y-qGKx5OOM-XDqPOCLchM.mp4" muted="false"></video></div>

Authors: Jiazhong Cen, Jiemin Fang, Chen Yang, Lingxi Xie, Xiaopeng Zhang, Wei Shen, Qi Tian

- 본 논문에서는 3D 방사장에서의 인터랙티브 3D 세그먼테이션을 위한 새로운 접근 방식인 Segment Any 3D Gaussians (SAGA)를 제안한다.
- 2D 세그먼테이션 기초 모델과 최근 방사장 분야의 혁신적인 기법인 3D Gaussian Splatting (3DGS)을 결합함으로써 미세한 조정 및 다중 정밀도 세그먼테이션을 효율적으로 수행한다.
- SAGA는 세그먼테이션 기초 모델에 의해 생성된 다중 정밀도 2D 세그먼테이션 결과를 잘 설계된 대조적 학습을 통해 3D 가우시안 점 특징으로 효과적으로 내장한다.
- 평가 결과 SAGA는 기존 벤치마크에서 최신 방법와 경쟁하는 성능을 달성하며, 다양한 프롬프트와 함께 다중 정밀도 세그먼테이션을 수행하는 것으로 나타났다.
- 특히, SAGA는 이전의 최신 기술보다 약 1000배 빠른 속도로 밀리초 단위의 3D 세그먼테이션을 완료함으로써 실시간 상호 작용을 가능하게 한다.
- 프로젝트 페이지는 https://jumpat.github.io/SAGA 에서 확인할 수 있다.

### [Object Recognition as Next Token Prediction](https://arxiv.org/abs/2312.02142)

![](https://cdn-uploads.huggingface.co/production/uploads/60f1abe7544c2adfd699860c/_HhUDxs5c9K0X9WYp9CtU.png)

Authors: Kaiyu Yue, Bor-Chun Chen, Jonas Geiping, Hengduo Li, Tom Goldstein, Ser-Nam Lim

- 본 연구에서는 객체 인식을 다음 토큰 예측 문제로 제안하며, 이미지 임베딩으로부터 텍스트 토큰을 자동 회귀적으로 생성하여 라벨을 형성하는 언어 디코더를 적용합니다.
- 이 예측 과정을 자동 회귀에 기반한 것으로 바탕하고자 디코더에 대해 비인과적(non-causal) 주의 마스크를 사용자화하며, 서로 다른 라벨의 토큰들을 독립적으로 모델링하고 이미지 토큰을 접두사로 취급하는 두 가지 주요 특징을 포함합니다.
- 이러한 마스킹 메커니즘은 효율적인 방법 - 원샷 샘플링 -을 영감하여, 추론 단계에서 여러 라벨의 토큰들을 동시에 병렬로 샘플링하고 생성된 라벨들을 그들의 확률에 따라 순위를 매기는 방법을 제안합니다.
- 효율성을 더욱 향상시키기 위해, 사전 학습된 언어 모델의 중간 블록을 단순히 제거하여 컴팩트한 디코더를 구축하는 간단한 전략을 제안합니다.
- 이 방법은 완전한 모델의 성능에 부합하는 동시에 현저하게 더 효율적인 디코더를 제공하며 관련 코드는 https://github.com/kaiyuyue/nxtp 에서 확인할 수 있습니다.

### [RLHF-V: Towards Trustworthy MLLMs via Behavior Alignment from Fine-grained Correctional Human Feedback](https://arxiv.org/abs/2312.00849)

![](https://cdn-uploads.huggingface.co/production/uploads/60f1abe7544c2adfd699860c/v9NxmHM0C2OKDAYbHJRZ5.png)

Authors: Tianyu Yu, Yuan Yao, Haoye Zhang, Taiwen He, Yifeng Han, Ganqu Cui, Jinyi Hu, Zhiyuan Liu, Hai-Tao Zheng, Maosong Sun, Tat-Seng Chua

- 다중모드 대규모 언어 모델(MLLMs)은 멀티모달 이해, 추론 및 상호작용에서 인상적인 능력을 보여주었으나, 기존 MLLMs은 이미지와 맞지 않는 내용을 만들어내는 환각 문제로 신뢰성이 결여되어 있습니다.
- 연구팀은 세밀한 교정 인간 피드백을 통한 행동 조정을 통해 MLLM의 신뢰성을 높이는 RLHF-V 방법을 제시합니다.
- RLHF-V는 환각에 대한 부분 수준의 교정을 통한 인간의 선호도를 수집하여 인간 피드백에 대한 직접적인 선호도 최적화를 수행합니다.
- 자동 평가와 인간 평가를 포함한 다섯 가지 벤치마크에서의 종합적인 실험 결과, RLHF-V는 주목할만한 데이터 및 계산 효율성으로 MLLM의 신뢰성을 크게 향상시킬 수 있음을 보여주었습니다.
- 단 1.4k개의 주석이 달린 데이터 샘플을 사용하여 RLHF-V는 기본 MLLM의 환각 비율을 34.8% 크게 줄였고, 10k개의 주석이 달린 데이터를 훈련한 동시대 LLaVA-RLHF보다 뛰어난 성능을 나타냈습니다.
- 최종 모델은 공개된 MLLMs 중 신뢰도에서 최고의 성능을 달성하였으며 GPT-4V보다 일반화로 인한 환각을 방지하는 데 있어 더 나은 강인성을 보여주었습니다.
- 연구팀은 코드, 모델 및 데이터를 https://github.com/RLHF-V/RLHF-V 에서 공개하였습니다.

### [Fast View Synthesis of Casual Videos](https://arxiv.org/abs/2312.02135)

[Watch Video]https://cdn-uploads.huggingface.co/production/uploads/60f1abe7544c2adfd699860c/bOp8LHXiKmR4XSuSs6OBl.mp4
<div><video controls src="https://cdn-uploads.huggingface.co/production/uploads/60f1abe7544c2adfd699860c/bOp8LHXiKmR4XSuSs6OBl.mp4" muted="false"></video></div>

Authors: Yao-Chih Lee, Zhoutong Zhang, Kevin Blackburn-Matzen, Simon Niklaus, Jianming Zhang, Jia-Bin Huang, Feng Liu

- 자연스러운 동영상에서의 새로운 시점 합성은 장면 동적 특성과 시차 부족으로 인해 어려움이 있습니다.
- 기존의 암시적 신경 복사장 방식(implicit neural radiance fields)은 효과적이지만 훈련과 렌더링이 느립니다.
- 이 논문은 모노큘러 비디오에서 효율적으로 고품질의 새로운 시점을 합성하기 위하여 명시적 비디오 표현을 새롭게 다루고 있습니다.
- 저자는 정적 및 동적 비디오 컨텐츠를 별도로 처리하며, 확장된 평면 기반 장면 표현을 사용하여 시간적으로 일관된 새로운 시점의 비디오를 합성합니다.
- 평면 기반 장면 표현은 구면 조화와 변위 맵을 통해 시점 의존적 효과를 포착하고 비평면 복잡한 표면 기하학을 모델링하기 위해 향상시킵니다.
- 동적 콘텐츠는 효율성을 위해 프레임별 포인트 클라우드로 표현되며, 명시적인 임시 불일치는 운동으로 인해 시각적으로 마스킹 됩니다.
- 저자들은 하이브리드 비디오 표현을 빠르게 추정하고 실시간으로 새로운 시점을 렌더링하는 방법을 개발했습니다.
- 실험 결과, 이 방법은 야생 비디오에서 고품질의 새로운 시점을 최신 기술과 비교할 수 있는 품질로 렌더링하면서 훈련 속도는 100배 빠르고 실시간 렌더링을 가능하게 합니다.

### [Nash Learning from Human Feedback](https://arxiv.org/abs/2312.00886)

![](https://cdn-uploads.huggingface.co/production/uploads/60f1abe7544c2adfd699860c/EEa8IaSPKiMsWf3tNFvgz.png)

Authors: Rémi Munos, Michal Valko, Daniele Calandriello, Mohammad Gheshlaghi Azar, Mark Rowland, Daniel Guo, Yunhao Tang, Matthieu Geist, Thomas Mésnard, Andrea Michi, Marco Selvi, Sertan Girgin, Nikola Momchev, Olivier Bachem, Daniel J. Mankowitz, Doina Precup, Bilal Piot

- 인간 피드백에서 강화 학습(RLHF)은 대규모 언어 모델(LLMs)을 인간의 선호도에 맞추는 주요 패러다임으로 부상했으며, 보통 사람의 피드백으로부터 보상 모델을 학습하는 초기 단계를 포함한다.
- 이 연구에서는 인간의 피드백 쌍을 이용하여 LLMs의 파인 튜닝을 위한 새로운 파이프라인을 소개하고, 이를 인간 피드백에 기반한 나시 학습(NLHF)이라 명명한다.
- 제안하는 접근법은 주어진 프롬프트에 대해 두 입력을 조건으로 하는 선호도 모델을 학습하고, 이 선호도 모델의 나시 균형을 정의하는 정책을 추구하여 경쟁 정책에 의해 생성된 반응보다 선호되는 반응을 일관되게 생성한다.
- 태블릿 정책 표현의 맥락에서, 이 논문은 거울 하강(mirror descent)의 원칙에 기반한 새로운 알고리즘 해결책인 Nash-MD를 제시하며, 이는 정규화된 나시 균형에 수렴하는 일련의 정책들을 생성한다.
- 또한, 딥러닝 아키텍처에 대한 경사 하강 알고리즘을 도입하고 파라메트릭 정책 표현을 탐구한다.
- 저자들은 텍스트 요약 작업에서 LLM의 파인 튜닝을 포함한 실험 결과를 제시하여 접근법의 효과를 입증하고, NLHF가 선호 학습 및 정책 최적화 분야를 발전시킬 수 있는 유망한 방법임을 믿는다.

### [DiffiT: Diffusion Vision Transformers for Image Generation](https://arxiv.org/abs/2312.02139)

![](https://cdn-uploads.huggingface.co/production/uploads/60f1abe7544c2adfd699860c/DhbNL5U54i7u7x0vxoWbU.png)

Authors: Ali Hatamizadeh, Jiaming Song, Guilin Liu, Jan Kautz, Arash Vahdat

- 확산 모델이 다양한 영역에서 새로운 응용 프로그램과 사용 사례를 가능하게 하는 강력한 표현력과 높은 샘플 품질을 제공합니다.
- 본 논문에서는 확산 기반 생성 학습에서 비전 트랜스포머의 효과성을 연구하고, 이를 통해 새로운 모델인 '확산 비전 트랜스포머(DiffiT)'를 제안합니다.
- DiffiT는 U자 형태의 인코더와 디코더를 결합한 계층적인 구조를 갖춘 하이브리드 아키텍처로 구성되어 있습니다.
- 논문은 시간의존적 자기 주의(self-attention) 모듈을 도입하여 더 효율적으로 다양한 단계의 이미지 디노이징 과정에 적응하는 레이어의 행동을 가능하게 합니다.
- 더불어 고해상도 이미지 생성을 위해 제안된 자기 주의 레이어가 있는 트랜스포머 모델인 잠재 DiffiT도 소개합니다.
- 실험 결과, DiffiT는 고화질 이미지를 생성하는 데 매우 효과적이며, 다양한 분류 조건 및 비조건적 합성 작업에서 최신 기술(SOTA) 벤치마크를 달성합니다.
- 잠재 공간에서는 DiffiT가 ImageNet-256 데이터셋에서 1.73의 새로운 최신 FID 점수를 달성하였습니다.
- 해당 연구의 코드는 GitHub 저장소에서 제공됩니다.

### [Style Aligned Image Generation via Shared Attention](https://arxiv.org/abs/2312.02133)

![](https://cdn-uploads.huggingface.co/production/uploads/60f1abe7544c2adfd699860c/q5Nmf36N7XauY7PL3a9jB.png)

Authors: Amir Hertz, Andrey Voynov, Shlomi Fruchter, Daniel Cohen-Or

- 텍스트에서 이미지로 변환 (T2I) 모델이 크게 주목을 받고 있지만, 일관된 스타일을 유지하는 것은 여전히 어려운 과제입니다.
- 본 논문에서는 생성된 이미지들 사이에 스타일 일치성을 확립하기 위해 'StyleAligned'라는 새로운 기술을 소개합니다.
- 확산 과정 중 최소한의 '공유 주의(attention sharing)'를 사용하여 T2I 모델 내의 이미지 스타일 일관성을 유지합니다.
- 이 방식은 참조 스타일을 통해 스타일이 일관된 이미지 생성을 간단한 반전 연산을 통해 가능하게 합니다.
- 다양한 스타일과 텍스트 프롬프트를 통한 방법의 평가는 높은 품질의 합성과 충실도를 보여주며, 다양한 입력에 걸쳐 일관된 스타일을 달성하는 데 있어서의 효과를 강조합니다.

### [SANeRF-HQ: Segment Anything for NeRF in High Quality](https://arxiv.org/abs/2312.01531)

[Watch Video]https://cdn-uploads.huggingface.co/production/uploads/60f1abe7544c2adfd699860c/m_EQLfh0E0ctOCzvE53-Q.mp4
<div><video controls src="https://cdn-uploads.huggingface.co/production/uploads/60f1abe7544c2adfd699860c/m_EQLfh0E0ctOCzvE53-Q.mp4" muted="false"></video></div>

Authors: Yichen Liu, Benran Hu, Chi-Keung Tang, Yu-Wing Tai

- 최근 'Segment Anything Model (SAM)'이 제로샷 세그멘테이션에서 뛰어난 성능을 보이며, 'Neural Radiance Fields (NeRF)'가 새로운 시점 합성을 넘어 다양한 3D 문제에 대한 인기 있는 방법으로 자리잡았다.
- 이 두 방법을 3D 세그멘테이션에 통합하려는 초기 시도는 복잡한 시나리오에서 객체를 정확하고 일관되게 세그멘트화하는 데 어려움을 겪고 있다.
- 본 논문에서는 주어진 장면에서 어떤 객체든 고품질 3D 세그멘테이션을 달성하기 위한 'Segment Anything for NeRF in High Quality (SANeRF-HQ)'를 소개한다.
- SANeRF-HQ는 사용자가 제공한 프롬프트를 통해 오픈 월드 객체 세그멘테이션을 안내하는 SAM을 활용하고, 다양한 관점에서 정보를 집계하기 위해 NeRF를 사용한다.
- 위에서 언급한 도전 과제를 극복하기 위해, 우리는 집계 동안 세그멘테이션 경계의 정확성을 향상시키기 위해 밀도 필드와 RGB 유사도를 활용한다.
- 세그멘테이션 정확성에 중점을 두고, 본 연구는 고품질 지상 진실이 제공되거나 수작업으로 어노테이션된 여러 NeRF 데이터셋에서 정량적으로 평가되었다.
- SANeRF-HQ는 NeRF 객체 세그멘테이션의 이전 최신 방법들에 비해 상당히 향상된 품질을 보이며, 객체 위치 확인에 더 큰 유연성을 제공하고, 다양한 시점에 걸쳐 보다 일관된 객체 세그멘테이션을 가능하게 한다.
- 추가 정보는 https://lyclyc52.github.io/SANeRF-HQ/ 에서 확인할 수 있다.

### [VideoRF: Rendering Dynamic Radiance Fields as 2D Feature Video Streams](https://arxiv.org/abs/2312.01407)

[Watch Video]https://cdn-uploads.huggingface.co/production/uploads/60f1abe7544c2adfd699860c/98ZAZyaKihGgUMesFXzdh.mp4
<div><video controls src="https://cdn-uploads.huggingface.co/production/uploads/60f1abe7544c2adfd699860c/98ZAZyaKihGgUMesFXzdh.mp4" muted="false"></video></div>

Authors: Liao Wang, Kaixin Yao, Chengcheng Guo, Zhirui Zhang, Qiang Hu, Jingyi Yu, Lan Xu, Minye Wu

- NeRF(신경 복사 필드)가 정적 장면을 광사실적으로 렌더링하는 데 뛰어나지만, 데이터 저장 및 계산 제약 때문에 동적이고 긴 시간의 복사 필드를 일반적인 장치에서 렌더링하는 것은 여전히 도전적입니다.
- 이 논문에서는 VideoRF라는 첫 번째 접근 방식을 소개하며, 이를 통해 모바일 플랫폼에서 동적 복사 필드의 실시간 스트리밍 및 렌더링을 가능하게 합니다.
- VideoRF의 핵심은 4D 복사 필드 전체를 하나의 직렬화된 2D 특징 이미지 스트림으로 표현하는 것입니다.
- 본 논문은 2D 영역에 직접 적용되는 특화된 훈련 체계를 도입하여 특징 이미지 스트림의 시공간 중복성을 부과합니다.
- 중복성을 활용하여 2D 비디오 코덱으로 특징 이미지 스트림을 효율적으로 압축할 수 있으며, 이는 실시간 복호화를 위해 비디오 하드웨어 가속기를 활용할 수 있음을 보여줍니다.
- 한편, 특징 이미지 스트림을 기반으로 복사 특성을 효율적으로 질의할 수 있는 특수한 공간 매핑을 갖춘 VideoRF의 새로운 렌더링 파이프라인을 제안합니다.
- VideoRF는 효율성 덕분에 모바일 기기에서 실시간 렌더링이 가능한 지연 쉐이딩 모델과 쌍을 이룹니다.
- 연구팀은 데스크탑부터 모바일 폰에 이르기까지 다양한 장치에서 실시간으로 동적 장면의 스트리밍 및 렌더링을 가능하게 하는 실시간 인터랙티브 플레이어를 개발하여, 매끄럽고 몰입감 있는 자유 시점 경험을 제공합니다.

### [GPS-Gaussian: Generalizable Pixel-wise 3D Gaussian Splatting for Real-time Human Novel View Synthesis](https://arxiv.org/abs/2312.02155)

[Watch Video]https://cdn-uploads.huggingface.co/production/uploads/60f1abe7544c2adfd699860c/wHj8hN2pSLBJpRWXheOOM.mp4
<div><video controls src="https://cdn-uploads.huggingface.co/production/uploads/60f1abe7544c2adfd699860c/wHj8hN2pSLBJpRWXheOOM.mp4" muted="false"></video></div>

Authors: Shunyuan Zheng, Boyao Zhou, Ruizhi Shao, Boning Liu, Shengping Zhang, Liqiang Nie, Yebin Liu

- 실시간 캐릭터의 새로운 뷰를 합성하기 위한 GPS-Gaussian이라는 새로운 접근법을 제시합니다.
- 제안된 방법은 희소한 카메라 설정에서 2K 해상도 렌더링을 가능하게 합니다.
- 개별 대상 최적화가 필요한 원래 가우시안 스플래팅이나 신경 임플리시트 렌더링 방법과 달리, 본 연구는 출처 뷰에 정의된 가우스 파라미터 맵을 소개하고 즉각적인 새로운 뷰 합성을 위해 가우시안 스플래팅 특성을 직접 회귀합니다.
- 인간 스캔 데이터의 대량을 활용하여 가우스 파라미터 회귀 모듈을 깊이 추정 모듈과 함께 훈련시켜 2D 파라미터 맵을 3D 공간으로 끌어올립니다.
- 제안된 프레임워크는 전적으로 미분 가능하며, 여러 데이터셋에서의 실험은 본 방법이 최신 기술을 상회하면서도 뛰어난 렌더링 속도를 달성함을 입증합니다.

### [Generative Powers of Ten](https://arxiv.org/abs/2312.02149)

[Watch Video]https://cdn-uploads.huggingface.co/production/uploads/60f1abe7544c2adfd699860c/SahTp-Q9XHf70R3NapR6C.mp4
<div><video controls src="https://cdn-uploads.huggingface.co/production/uploads/60f1abe7544c2adfd699860c/SahTp-Q9XHf70R3NapR6C.mp4" muted="false"></video></div>

Authors: Xiaojuan Wang, Janne Kontkanen, Brian Curless, Steve Seitz, Ira Kemelmacher, Ben Mildenhall, Pratul Srinivasan, Dor Verbin, Aleksander Holynski

- 본 연구에서는 넓은 각도의 풍경부터 나무 가지에 앉은 곤충의 클로즈업 사진에 이르기까지, 다양한 이미지 스케일에 걸쳐 일관된 내용을 생성하는 텍스트-이미지 모델을 제시합니다.
- 이는 각각의 스케일이 다른 텍스트 프롬프트에 의해 안내되기 때문에, 현저히 다른 스케일에서 새로운 맥락적 구조를 생성하는데 어려움을 겪을 수 있는 전통적인 수퍼-해상도 기법들보다 더 깊은 수준의 줌을 가능하게 합니다.
- 다중 스케일 확산 샘플링 접근 방식을 공동으로 사용하여 각 스케일 간의 일관성을 유지하는 동시에 각 개별 샘플링 과정의 무결성을 보존합니다.
- 이미지 수퍼-해상도와 아웃페인팅과 같은 대안적 기술들과 비교할 때, 다양한 스케일의 내용을 일관되게 생성하는데 있어 본 방법이 가장 효과적임을 질적으로 보여줍니다.

### [Rejuvenating image-GPT as Strong Visual Representation Learners](https://arxiv.org/abs/2312.02147)

![](https://cdn-uploads.huggingface.co/production/uploads/60f1abe7544c2adfd699860c/A3jcR_RFvhJ1119SVv93n.png)

Authors: Sucheng Ren, Zeyu Wang, Hongru Zhu, Junfei Xiao, Alan Yuille, Cihang Xie

- 이 논문은 시각적 표현 학습을 위해 다음 픽셀 예측하는 오토리그레시브 전처리 방식을 소개한 초기 연구 중 하나인 image-GPT(iGPT)를 강화합니다.
- 첫 번째 변경으로, 원시 픽셀 대신 시맨틱 토큰을 예측 대상으로 삼아 시각적 내용에 대한 더 높은 수준의 이해를 가능하게 합니다.
- 두 번째로, 오토리그레시브 모델링에 보충하여 모델이 다음 토큰뿐만 아니라 보이는 토큰들도 예측하도록 합니다.
- 특히, CLIP과 같이 차별적으로 훈련된 모델로 인코딩된 시맨틱 토큰에 이 방법이 효과적입니다.
- D-iGPT라고 불리는 이 새로운 접근법은 다양한 실험을 통해 시각적 표현의 강력한 학습자로서 우수성을 입증합니다.
- D-iGPT는 공개 데이터셋에서 훈련함으로써, 기본 설정인 ViT-Large 모델로 ImageNet-1K 데이터셋에서 89.5%의 top-1 정확도를 달성하는 뛰어난 성과를 보여줍니다.
- 또한, 이 모델은 다운스트림 작업에서도 강한 일반화 능력과 분배 외 샘플에 대한 강건함을 보여줍니다.
- 코드는 https://github.com/OliverRensu/D-iGPT 에서 확인할 수 있습니다.

### [Using Large Language Models to Accelerate Communication for Users with Severe Motor Impairments](https://arxiv.org/abs/2312.01532)

![](https://cdn-uploads.huggingface.co/production/uploads/60f1abe7544c2adfd699860c/xEgNCjP26quCtrWpWqsCA.png)

Authors: Shanqing Cai, Subhashini Venugopalan, Katie Seaver, Xiang Xiao, Katrin Tomanek, Sri Jalasutram, Meredith Ringel Morris, Shaun Kane, Ajit Narayanan, Robert L. MacDonald, Emily Kornman, Daniel Vance, Blair Casey, Steve M. Gleason, Philip Q. Nelson, Michael P. Brenner

- 중증 운동 장애가 있는 개인의 텍스트 입력 속도를 높이는 연구는 오래된 연구 분야입니다.
- 대체 보완 의사소통(AAC) 디바이스의 속도 격차를 줄이는 것은 이러한 개인의 삶의 질을 개선하는 데 중요합니다.
- 자연어 처리 신경망의 최근 발전은 AAC 사용자를 위한 텍스트 입력을 향상시키기 위한 전략과 사용자 인터페이스를 재고할 새로운 기회를 제공합니다.
- 본 논문에서는 SpeakFaster를 소개하며 이것은 대규모 언어 모델(LLMs)과 고안된 사용자 인터페이스를 결합한 시스템으로, 줄여 쓰기 형식을 통한 텍스트 입력을 가능하게 하여, 오프라인 시뮬레이션에서 기존 예측 키보드보다 57% 더 많은 운동 행동을 절약할 수 있습니다.
- 19명의 비-AAC 참가자가 모바일 기기에서 수작업으로 타이핑하는 시범 연구는 오프라인 시뮬레이션과 일치하는 운동 절약에서 이익을 보였으며 전체 타이핑 속도에 상대적으로 작은 영향을 미쳤습니다.
- 근위축성 측색 경화증(ALS)이 있는 두 명의 눈동자 추적 타이핑 사용자에 대한 실험실 및 현장 테스트에서, 맥락 인식 LLM의 구문 및 단어 예측을 통해 비용이 많이 드는 키 입력의 상당한 절감으로 인해 전통적인 기준보다 29-60% 빠른 텍스트 입력 속도를 보였습니다.
- 이러한 발견은 중증 운동 장애가 있는 사용자를 위한 대폭 가속화된 텍스트 의사소통 탐색에 대한 강력한 기반을 제공하며, 텍스트 기반 사용자 인터페이스에 LLM을 적용하는 방향을 보여줍니다.

### [TextGenSHAP: Scalable Post-hoc Explanations in Text Generation with Long Documents](https://arxiv.org/abs/2312.01279)

![](https://cdn-uploads.huggingface.co/production/uploads/60f1abe7544c2adfd699860c/6TVVPQk6rBfr_lqqHbtTU.png)

Authors: James Enouen, Hootan Nakhost, Sayna Ebrahimi, Sercan O Arik, Yan Liu, Tomas Pfister

- 대규모 언어 모델(LLMs)의 블랙박스 성격 및 복잡한 추론 과정 때문에 LLM에서 생성된 콘텐츠에 대한 확장 가능하고 충실한 설명의 필요성이 증가하고 있다.
- Shapley 값과 같은 포스트호크 설명 방법은 심층 학습 모델 해석에 효과적이지만, 긴 입력 컨텍스트와 생성된 출력 시퀀스를 다룰 때 확장성에 문제가 있다.
- 본 논문에서는, 텍스트 생성에 특화된 기법을 통합하는 효율적인 포스트호크 설명 방법인 TextGenSHAP을 소개하며, 이는 기존의 Shapley 값 계산보다 빠른 속도로 설명을 생성할 수 있음을 보여준다.
- 토큰 수준 설명에서는 처리 시간을 몇 시간에서 몇 분으로, 문서 수준 설명에서는 몇 초로 단축시킨다.
- TextGenSHAP은 긴 문서 질의 응답에서 중요한 단어와 문장을 지역화하여 이해를 돕고, 선택된 단락의 정확성을 높여 최종 응답을 개선함으로써 기존 문서 검색 시스템을 향상시키는 방법에서 실시간 Shapley 값을 활용할 수 있음을 보여준다.

### [Generative Rendering: Controllable 4D-Guided Video Generation with 2D Diffusion Models](https://arxiv.org/abs/2312.01409)

[Watch Video]https://cdn-uploads.huggingface.co/production/uploads/60f1abe7544c2adfd699860c/mkfeU2AJOKh-gTWQvbrC5.mp4
<div><video controls src="https://cdn-uploads.huggingface.co/production/uploads/60f1abe7544c2adfd699860c/mkfeU2AJOKh-gTWQvbrC5.mp4" muted="false"></video></div>

Authors: Shengqu Cai, Duygu Ceylan, Matheus Gadelha, Chun-Hao Paul Huang, Tuanfeng Yang Wang, Gordon Wetzstein

- 전통적인 3D 콘텐츠 생성 도구는 사용자가 장면의 형태, 외관, 동작, 카메라 경로를 직접 조작하여 상상력을 실현할 수 있도록 하지만, 컴퓨터 생성 동영상은 수작업으로 만드는 과정이 번거롭습니다.
- 텍스트-동영상 확산 모델이 자동화 가능성을 제공하지만, 여기에서 사용자의 창의력을 적극적으로 적용하기 어려운 제어 문제가 발생합니다.
- 이러한 도전에 대응하기 위해, 동적 3D 메쉬의 조작성과 발전하는 확산 모델의 표현력 및 수정 가능성을 결합한 새로운 접근 방식을 제안합니다.
- 제안된 접근 방식은 애니메이션화된 저화질의 렌더링 메쉬를 입력으로 받아 동적 메쉬에서 얻은 실제 대응 정보를 기존 텍스트-이미지 생성 모델의 여러 단계에 주입하여 고품질이고 시간적 일관성이 있는 프레임을 출력합니다.
- 이 접근 방식은 움직임을 조작 장비에 애니메이션을 적용하거나 카메라 경로를 변경하여 여러 예제에서 시연됩니다.

### [Customize your NeRF: Adaptive Source Driven 3D Scene Editing via Local-Global Iterative Training](https://arxiv.org/abs/2312.01663)

![](https://cdn-uploads.huggingface.co/production/uploads/60f1abe7544c2adfd699860c/xOyN6ZHeXEAMBGJfs5Efr.png)

Authors: Runze He, Shaofei Huang, Xuecheng Nie, Tianrui Hui, Luoqi Liu, Jiao Dai, Jizhong Han, Guanbin Li, Si Liu

- 본 논문에서는 텍스트 설명이나 참조 이미지를 편집 유도물로 사용하는 CustomNeRF 모델을 제안하여 적응적 원천 기반 3D 장면 편집 작업에 접근합니다.
- 전경만 정확히 편집하면서 배경을 보존하는 것은 어려운 문제로, 이에 대응하기 위해 전경 영역 편집과 전체 이미지 편집을 번갈아 수행하는 Local-Global Iterative Editing (LGIE) 훈련 방식을 개발했습니다.
- 단일 시점 참조 이미지를 사용할 때 다양한 시점 간 일관성을 유지하는 것이 두 번째 도전으로, 클래스 유도 정규화를 설계하여 생성 모델 내의 클래스 사전 지식을 활용해 이미지 기반 편집의 불일치 문제를 완화합니다.
- 텍스트 및 이미지 기반 설정에서 다양한 실제 장면에 대해 정밀한 편집 결과를 제공하는 것으로 다양한 실험을 통해 우리의 CustomNeRF의 효과를 입증했습니다.



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

@misc{daily_papers_ko,
  title = {Automatically translate and summarize huggingface's daily papers into korean},
  author = {l-yohai},
  howpublished = {\url{https://github.com/l-yohai/daily_papers_ko}},
  year = {2023}
}
```

## Star History

![Star History Chart](https://api.star-history.com/svg?repos=l-yohai/daily_papers_ko&type=Date)
