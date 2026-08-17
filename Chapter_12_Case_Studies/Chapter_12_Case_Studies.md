**Volume 44 Neuroscience for AI**


# Chapter 12. Case Studies

##  

## 12.00 Case Study Overview

![](images/image1.png){width="7.268055555555556in" height="7.268055555555556in"}

Case studies provide a practical bridge between neuroscience concepts and artificial intelligence architectures. Rather than assuming that biological mechanisms should be copied directly, they examine how selected principles from perception, learning, memory, prediction, event-driven processing, and neural hardware have influenced computational systems. The chapter therefore focuses on concrete connections between biological inspiration and engineered AI.

The purpose of these case studies is not to demonstrate that modern AI reproduces the brain. Instead, each case asks a more useful question: which biological observation inspired a computational idea, how was that idea abstracted into an engineering mechanism, and what advantages or limitations emerged after implementation? This distinction separates productive neuroscience-inspired design from superficial biological analogy.

The selected cases span several levels of abstraction. Convolutional neural networks connect hierarchical visual processing with artificial feature extraction, reinforcement learning connects reward prediction with adaptive decision making, and retrieval systems provide a computational comparison with memory organization. Predictive models, spiking networks, event cameras, and neuromorphic processors extend the comparison toward temporal and hardware-level computation.

The visual cortex and convolutional neural networks form one of the best-known historical examples. Biological vision processes information through multiple stages in which neurons respond selectively to increasingly meaningful visual structure. CNNs similarly construct hierarchical feature representations using local receptive fields, shared parameters, and layered transformations, although their actual computations and learning mechanisms differ substantially from cortical processing.

This comparison demonstrates an important principle used throughout the chapter: functional inspiration does not imply mechanistic equivalence. CNNs can reproduce useful properties associated with hierarchical vision without implementing retinal circuitry, cortical cell types, biological spikes, or synaptic learning rules. The engineering value lies in identifying abstractions that solve computational problems rather than reproducing biological anatomy in unnecessary detail.

Dopamine and deep reinforcement learning provide another influential connection. Neuroscience studies associate dopaminergic activity with reward prediction and differences between expected and obtained outcomes. Reinforcement-learning algorithms use reward prediction errors to update value estimates or policies. The correspondence is computationally informative, but artificial reward signals and biological neuromodulatory systems should not be treated as identical mechanisms.

The hippocampus and retrieval-augmented generation illustrate a more conceptual comparison between biological memory and modern AI memory architectures. The hippocampus supports rapid encoding and retrieval of experiences and interacts with broader cortical memory systems. Retrieval-augmented AI similarly separates some stored information from model parameters and retrieves relevant external representations when needed, reducing the requirement that every piece of knowledge be permanently embedded in network weights.

This case highlights the importance of separating computation from storage. A large neural model can contain extensive parametric knowledge, but external or episodic memory can preserve information that is updated independently. Retrieval mechanisms then select relevant memories according to the current context. Such architectures suggest how AI systems might combine relatively stable learned representations with more flexible and dynamically accessible knowledge.

Predictive coding and diffusion models provide a more cautious comparison. Predictive processing theories emphasize iterative relationships between expectations and sensory evidence, often interpreting error signals as important drivers of representation and learning. Diffusion models also use iterative computation to transform uncertain or noisy representations into structured outputs, but their mathematical objectives and biological interpretations are fundamentally different.

The value of this comparison therefore lies at the level of computational themes rather than direct biological correspondence. Iterative refinement, uncertainty reduction, hierarchical representation, and repeated correction can appear in both neuroscience-inspired theories and generative AI. Examining where the analogy succeeds and where it breaks down helps prevent the mistaken conclusion that similar computational patterns necessarily imply identical underlying mechanisms.

Spiking neural networks move the comparison closer to neural signaling itself. Biological neurons communicate through discrete electrical events whose timing can carry information. Artificial spiking networks represent computation through event-like activations distributed over time, potentially enabling sparse and temporally structured processing. They provide a useful experimental framework for investigating alternatives to continuously activated artificial neural networks.

However, spikes alone do not provide biological intelligence. Useful spiking systems require suitable representations, learning mechanisms, network structures, temporal dynamics, and hardware support. Their advantages are particularly relevant where event-driven computation, low power consumption, continuous sensing, or precise temporal processing matters, rather than because biological resemblance automatically makes them superior to conventional deep learning.

Event cameras demonstrate how neuroscience-inspired ideas can influence sensing as well as algorithms. Conventional cameras repeatedly capture complete image frames, whereas event cameras report local brightness changes asynchronously. This resembles some principles of biological visual processing by emphasizing change rather than transmitting every pixel continuously, allowing rapid temporal response and potentially reducing redundant sensory data.

For robotics, this sensing strategy can be valuable in high-speed motion, dynamic scenes, challenging illumination, and resource-constrained systems. Event streams can support motion estimation, tracking, navigation, and rapid reaction without requiring conventional frame acquisition at extremely high rates. The case demonstrates that brain inspiration can improve the complete perception pipeline rather than only the neural network operating after sensory acquisition.

Neuromorphic processors extend these ideas into computing hardware. Conventional accelerators generally rely on dense numerical operations and substantial movement of data between memory and compute units. Neuromorphic architectures investigate event-driven communication, local memory, sparse activity, asynchronous operation, and computation located closer to stored state, attempting to reduce some costs associated with conventional computing architectures.

The relationship between spiking networks, event sensors, and neuromorphic processors is especially important because their benefits can emerge through co-design. An event camera generates sparse asynchronous data, a spiking model can process temporally structured events, and neuromorphic hardware can execute such computation efficiently. The system-level combination may therefore be more informative than evaluating each component independently.

Across all cases, the translation process follows a common pattern. Neuroscience first provides observations or hypotheses about biological computation. Researchers then identify a computational principle, abstract it into a mathematical or algorithmic mechanism, implement it using available software or hardware, and evaluate whether the resulting system provides measurable engineering benefits. Biological plausibility and engineering effectiveness remain related but distinct evaluation criteria.

Comparison should therefore include capability, mechanism, representation, temporal behavior, learning, resource requirements, and failure modes. Two systems may achieve similar performance while relying on completely different internal processes, or they may share a computational principle while producing different behavior. Case studies are most informative when they examine both similarities and differences rather than selecting only evidence that supports a preferred analogy.

These examples also reveal a progression from isolated mechanisms toward integrated intelligent systems. Visual hierarchy concerns representation, reinforcement learning concerns adaptive behavior, retrieval concerns memory, predictive processing concerns internal modeling, and neuromorphic approaches concern efficient temporal computation. Combining such mechanisms suggests architectures in which perception, memory, prediction, learning, and action cooperate rather than operating as unrelated AI components.

For embodied AI, this integration becomes particularly relevant. A robot can combine conventional visual networks with event sensors, memory retrieval, reinforcement learning, predictive world models, and resource-aware computation according to task requirements. The objective is not to maximize biological similarity but to select mechanisms that improve latency, energy efficiency, adaptation, robustness, uncertainty handling, and autonomous operation in physical environments.

Case studies also provide a method for testing neuroscience-inspired claims. A proposed biological principle becomes scientifically and technologically more useful when it can be converted into an explicit computational model and evaluated experimentally. Conversely, failures can reveal that an abstraction was incomplete, that an analogy was misleading, or that additional mechanisms are required. AI can therefore serve as an experimental testbed for computational hypotheses.

The broader lesson is that neuroscience and AI can advance through iterative exchange. Neuroscience contributes observations, constraints, organizational principles, and hypotheses, while AI provides mathematical models, scalable implementations, controlled experiments, and alternative computational solutions. The case studies defined in this chapter---CNNs, deep reinforcement learning, retrieval systems, predictive generative models, spiking networks, event cameras, and neuromorphic processors---illustrate different points along this translation pathway.

Taken together, these cases establish a practical framework for neuroscience-inspired AI without requiring literal brain replication. The central question is not whether an artificial system looks biologically realistic, but whether a neuroscience-derived principle can be abstracted, implemented, measured, and integrated usefully. This perspective prepares the transition from individual case studies toward broader practical guidelines for brain-inspired AI architecture and system design.

사례 연구(Case Studies)는 신경과학(Neuroscience)의 개념과 인공지능 아키텍처(Artificial Intelligence Architectures)를 연결하는 실용적인 가교를 제공합니다. 생물학적 메커니즘을 직접 복제해야 한다고 가정하는 대신, 사례 연구는 지각(Perception), 학습(Learning), 기억(Memory), 예측(Prediction), 이벤트 기반 처리(Event-Driven Processing), 신경 하드웨어(Neural Hardware)에서 선택된 원리가 계산 시스템에 어떤 영향을 주었는지를 살펴봅니다. 따라서 이 장에서는 생물학적 영감(Biological Inspiration)과 공학적으로 구현된 인공지능 사이의 구체적인 연결 관계에 초점을 맞춥니다.

이러한 사례 연구의 목적은 현대 인공지능이 뇌를 재현한다는 것을 입증하는 데 있지 않습니다. 대신 각각의 사례에서는 어떤 생물학적 관찰(Biological Observation)이 계산적 아이디어(Computational Idea)에 영감을 주었는지, 그 아이디어가 어떻게 공학적 메커니즘(Engineering Mechanism)으로 추상화되었는지, 그리고 구현 이후 어떠한 장점과 한계가 나타났는지를 살펴봅니다. 이러한 구분은 생산적인 신경과학 기반 설계(Neuroscience-Inspired Design)를 피상적인 생물학적 유추(Biological Analogy)와 구별합니다.

선정된 사례들은 여러 추상화 수준(Levels of Abstraction)에 걸쳐 있습니다. 합성곱 신경망(Convolutional Neural Networks)은 계층적 시각 처리(Hierarchical Visual Processing)를 인공적인 특징 추출(Feature Extraction)과 연결하고, 강화학습(Reinforcement Learning)은 보상 예측(Reward Prediction)을 적응적 의사결정(Adaptive Decision Making)과 연결하며, 검색 시스템(Retrieval Systems)은 기억 조직(Memory Organization)과 계산적인 비교를 제공합니다. 예측 모델(Predictive Models), 스파이킹 신경망(Spiking Neural Networks), 이벤트 카메라(Event Cameras), 뉴로모픽 프로세서(Neuromorphic Processors)는 이러한 비교를 시간적 계산(Temporal Computation)과 하드웨어 수준의 계산으로 확장합니다.

시각 피질(Visual Cortex)과 합성곱 신경망은 가장 잘 알려진 역사적 사례 가운데 하나입니다. 생물학적 시각 시스템은 뉴런이 점차 의미 있는 시각 구조에 선택적으로 반응하는 여러 단계를 통해 정보를 처리합니다. 합성곱 신경망 역시 국소 수용장(Local Receptive Fields), 공유 파라미터(Shared Parameters), 계층적 변환(Layered Transformations)을 사용하여 계층적인 특징 표상(Hierarchical Feature Representations)을 구성하지만, 실제 계산 방식과 학습 메커니즘은 피질 처리(Cortical Processing)와 상당히 다릅니다.

이러한 비교는 이 장 전체에서 사용되는 중요한 원리를 보여줍니다. 기능적 영감(Functional Inspiration)이 기계적 동등성(Mechanistic Equivalence)을 의미하는 것은 아닙니다. 합성곱 신경망은 망막 회로(Retinal Circuitry), 피질 세포 유형(Cortical Cell Types), 생물학적 스파이크(Biological Spikes), 시냅스 학습 규칙(Synaptic Learning Rules)을 구현하지 않으면서도 계층적 시각 처리와 관련된 유용한 특성을 재현할 수 있습니다. 공학적 가치는 불필요한 생물학적 세부 구조를 복제하는 것이 아니라 계산 문제를 해결할 수 있는 추상화를 식별하는 데 있습니다.

도파민(Dopamine)과 심층 강화학습(Deep Reinforcement Learning)은 또 다른 중요한 연결 관계를 제공합니다. 신경과학 연구에서는 도파민성 활동(Dopaminergic Activity)을 보상 예측 및 예상된 결과와 실제로 획득한 결과 사이의 차이와 연관시킵니다. 강화학습 알고리즘은 보상 예측 오류(Reward Prediction Errors)를 이용하여 가치 추정(Value Estimates)이나 정책(Policies)을 갱신합니다. 이러한 대응 관계는 계산적으로 유용하지만 인공적인 보상 신호(Artificial Reward Signals)와 생물학적 신경조절 시스템(Biological Neuromodulatory Systems)을 동일한 메커니즘으로 간주해서는 안 됩니다.

해마(Hippocampus)와 검색 증강 생성(Retrieval-Augmented Generation)은 생물학적 기억과 현대 인공지능 기억 아키텍처(AI Memory Architectures) 사이의 보다 개념적인 비교를 보여줍니다. 해마는 경험을 빠르게 부호화(Encoding)하고 검색(Retrieval)하는 기능을 지원하며 광범위한 피질 기억 시스템(Cortical Memory Systems)과 상호작용합니다. 검색 증강 인공지능 역시 저장된 정보의 일부를 모델 파라미터와 분리하고 필요할 때 관련 외부 표상(External Representations)을 검색함으로써 모든 지식을 네트워크 가중치(Network Weights)에 영구적으로 포함해야 하는 요구를 줄입니다.

이 사례는 계산(Computation)과 저장(Storage)을 분리하는 것이 중요하다는 점을 보여줍니다. 대규모 신경 모델(Large Neural Model)은 방대한 파라미터 지식(Parametric Knowledge)을 포함할 수 있지만, 외부 기억(External Memory)이나 일화 기억(Episodic Memory)은 모델과 독립적으로 갱신되는 정보를 보존할 수 있습니다. 이후 검색 메커니즘(Retrieval Mechanisms)은 현재 맥락(Context)에 따라 관련 기억을 선택합니다. 이러한 아키텍처는 인공지능 시스템이 비교적 안정적인 학습 표상과 더욱 유연하고 동적으로 접근할 수 있는 지식을 결합할 수 있는 방법을 제시합니다.

예측 부호화(Predictive Coding)와 확산 모델(Diffusion Models)은 보다 신중하게 접근해야 하는 비교 사례를 제공합니다. 예측 처리 이론(Predictive Processing Theories)은 기대(Expectations)와 감각적 증거(Sensory Evidence) 사이의 반복적인 관계를 강조하며, 오류 신호(Error Signals)를 표상과 학습의 중요한 동인으로 해석하는 경우가 많습니다. 확산 모델 역시 반복적인 계산을 사용하여 불확실하거나 잡음이 포함된 표상을 구조화된 출력으로 변환하지만, 그 수학적 목표(Mathematical Objectives)와 생물학적 해석은 근본적으로 다릅니다.

따라서 이러한 비교의 가치는 직접적인 생물학적 대응 관계보다 계산적 주제(Computational Themes)의 수준에 있습니다. 반복적 정교화(Iterative Refinement), 불확실성 감소(Uncertainty Reduction), 계층적 표상(Hierarchical Representation), 반복적인 수정(Repeated Correction)은 신경과학 기반 이론과 생성형 인공지능(Generative AI) 모두에서 나타날 수 있습니다. 이러한 유추가 어디에서 유효하고 어디에서 한계를 가지는지를 살펴보는 것은 유사한 계산 패턴이 반드시 동일한 내부 메커니즘을 의미한다는 잘못된 결론을 방지하는 데 도움이 됩니다.

스파이킹 신경망은 신경 신호 전달(Neural Signaling) 자체에 보다 가까운 비교를 제공합니다. 생물학적 뉴런은 시간적 특성이 정보를 전달할 수 있는 이산적인 전기적 사건(Discrete Electrical Events)을 통해 통신합니다. 인공 스파이킹 신경망은 시간에 따라 분산되는 이벤트 형태의 활성화(Event-Like Activations)를 통해 계산을 표현하며, 희소하고 시간적으로 구조화된 처리(Sparse and Temporally Structured Processing)를 가능하게 할 수 있습니다. 이는 지속적으로 활성화되는 기존 인공 신경망과 다른 계산 방식을 연구할 수 있는 유용한 실험적 프레임워크를 제공합니다.

그러나 스파이크(Spikes) 자체만으로 생물학적 지능이 만들어지는 것은 아닙니다. 유용한 스파이킹 시스템을 구현하려면 적절한 표상, 학습 메커니즘, 네트워크 구조(Network Structures), 시간 동역학(Temporal Dynamics), 하드웨어 지원(Hardware Support)이 필요합니다. 이러한 시스템의 장점은 생물학적으로 유사하다는 이유 때문이 아니라 이벤트 기반 계산, 낮은 전력 소비(Low Power Consumption), 지속적인 감지(Continuous Sensing), 정밀한 시간 처리(Precise Temporal Processing)가 중요한 환경에서 특히 의미를 가집니다.

이벤트 카메라는 신경과학 기반 아이디어가 알고리즘뿐만 아니라 감지(Sensing) 기술에도 영향을 줄 수 있음을 보여줍니다. 기존 카메라는 전체 이미지 프레임(Image Frames)을 반복적으로 획득하는 반면, 이벤트 카메라는 국소적인 밝기 변화(Local Brightness Changes)를 비동기적으로 보고합니다. 이는 모든 픽셀을 지속적으로 전송하기보다 변화에 집중한다는 점에서 생물학적 시각 처리의 일부 원리와 유사하며, 빠른 시간적 응답과 중복 감각 데이터(Redundant Sensory Data)의 감소를 가능하게 할 수 있습니다.

로보틱스(Robotics)에서는 이러한 감지 전략이 고속 운동(High-Speed Motion), 동적 장면(Dynamic Scenes), 까다로운 조명 조건(Challenging Illumination), 자원이 제한된 시스템(Resource-Constrained Systems)에서 유용할 수 있습니다. 이벤트 스트림(Event Streams)은 매우 높은 프레임 속도로 기존 영상을 획득하지 않고도 운동 추정(Motion Estimation), 추적(Tracking), 내비게이션(Navigation), 빠른 반응(Rapid Reaction)을 지원할 수 있습니다. 이 사례는 뇌 기반 영감이 감각 획득 이후에 작동하는 신경망뿐만 아니라 전체 지각 파이프라인(Perception Pipeline)을 개선할 수 있음을 보여줍니다.

뉴로모픽 프로세서(Neuromorphic Processors)는 이러한 아이디어를 컴퓨팅 하드웨어(Computing Hardware)까지 확장합니다. 기존 가속기(Conventional Accelerators)는 일반적으로 밀집 수치 연산(Dense Numerical Operations)과 메모리 및 계산 장치 사이의 상당한 데이터 이동(Data Movement)에 의존합니다. 뉴로모픽 아키텍처(Neuromorphic Architectures)는 이벤트 기반 통신(Event-Driven Communication), 로컬 메모리(Local Memory), 희소 활동(Sparse Activity), 비동기 연산(Asynchronous Operation), 저장된 상태에 가까운 위치에서의 계산을 연구하여 기존 컴퓨팅 아키텍처에서 발생하는 일부 비용을 줄이고자 합니다.

스파이킹 신경망, 이벤트 센서(Event Sensors), 뉴로모픽 프로세서 사이의 관계는 이들의 장점이 공동 설계(Co-Design)를 통해 나타날 수 있다는 점에서 특히 중요합니다. 이벤트 카메라는 희소하고 비동기적인 데이터를 생성하고, 스파이킹 모델은 시간적으로 구조화된 이벤트를 처리하며, 뉴로모픽 하드웨어는 이러한 계산을 효율적으로 실행할 수 있습니다. 따라서 시스템 수준의 결합(System-Level Combination)을 평가하는 것이 각각의 구성 요소를 독립적으로 평가하는 것보다 더 의미 있을 수 있습니다.

모든 사례에서 변환 과정(Translation Process)은 공통적인 패턴을 따릅니다. 먼저 신경과학이 생물학적 계산에 대한 관찰이나 가설(Hypotheses)을 제공합니다. 이후 연구자는 계산 원리를 식별하고, 이를 수학적 또는 알고리즘적 메커니즘(Mathematical or Algorithmic Mechanism)으로 추상화하며, 사용 가능한 소프트웨어나 하드웨어를 이용하여 구현하고, 결과 시스템이 측정 가능한 공학적 이점(Measurable Engineering Benefits)을 제공하는지를 평가합니다. 생물학적 타당성(Biological Plausibility)과 공학적 효과성(Engineering Effectiveness)은 서로 관련되어 있지만 구별되는 평가 기준입니다.

따라서 비교에는 능력(Capability), 메커니즘(Mechanism), 표상(Representation), 시간적 행동(Temporal Behavior), 학습, 자원 요구사항(Resource Requirements), 실패 모드(Failure Modes)가 포함되어야 합니다. 두 시스템이 완전히 다른 내부 과정에 의존하면서도 유사한 성능을 달성할 수 있으며, 반대로 동일한 계산 원리를 공유하면서 서로 다른 행동을 생성할 수도 있습니다. 사례 연구는 선호하는 유추를 뒷받침하는 증거만 선택하는 대신 유사점과 차이점을 함께 분석할 때 가장 많은 정보를 제공합니다.

이러한 사례들은 또한 개별 메커니즘에서 통합 지능형 시스템(Integrated Intelligent Systems)으로 발전하는 과정을 보여줍니다. 시각 계층(Visual Hierarchy)은 표상과 관련되고, 강화학습은 적응적 행동(Adaptive Behavior), 검색은 기억, 예측 처리는 내부 모델링(Internal Modeling), 뉴로모픽 접근법은 효율적인 시간적 계산과 관련됩니다. 이러한 메커니즘을 결합하면 지각, 기억, 예측, 학습, 행동이 서로 분리된 인공지능 구성 요소로 작동하는 대신 협력하는 아키텍처를 구성할 수 있습니다.

체화 인공지능(Embodied AI)에서는 이러한 통합이 특히 중요합니다. 로봇은 과제 요구사항에 따라 기존 시각 신경망(Visual Networks), 이벤트 센서, 기억 검색(Memory Retrieval), 강화학습, 예측적 월드 모델(Predictive World Models), 자원 인식 계산(Resource-Aware Computation)을 결합할 수 있습니다. 목표는 생물학적 유사성을 최대화하는 것이 아니라 물리적 환경에서 지연시간, 에너지 효율성, 적응, 강건성(Robustness), 불확실성 처리(Uncertainty Handling), 자율 운영(Autonomous Operation)을 개선할 수 있는 메커니즘을 선택하는 것입니다.

사례 연구는 신경과학 기반 주장(Neuroscience-Inspired Claims)을 검증하는 방법도 제공합니다. 제안된 생물학적 원리가 명시적인 계산 모델(Computational Model)로 변환되고 실험적으로 평가될 수 있다면 과학적·기술적으로 더욱 유용해집니다. 반대로 실패한 결과는 사용된 추상화가 불완전했거나 유추가 잘못되었거나 추가적인 메커니즘이 필요하다는 사실을 보여줄 수 있습니다. 따라서 인공지능은 계산적 가설(Computational Hypotheses)을 검증하기 위한 실험 플랫폼(Experimental Testbed)으로 활용될 수 있습니다.

보다 넓은 교훈은 신경과학과 인공지능이 반복적인 상호 교환(Iterative Exchange)을 통해 함께 발전할 수 있다는 것입니다. 신경과학은 관찰, 제약 조건, 조직 원리(Organizational Principles), 가설을 제공하고, 인공지능은 수학적 모델(Mathematical Models), 확장 가능한 구현(Scalable Implementations), 통제된 실험(Controlled Experiments), 대안적인 계산 해법을 제공합니다. 이 장에서 다루는 합성곱 신경망, 심층 강화학습, 검색 시스템, 예측적 생성 모델(Predictive Generative Models), 스파이킹 신경망, 이벤트 카메라, 뉴로모픽 프로세서는 이러한 변환 경로의 서로 다른 지점을 보여줍니다.

종합하면 이러한 사례들은 뇌를 문자 그대로 복제하지 않으면서도 신경과학 기반 인공지능을 연구할 수 있는 실용적인 프레임워크를 제공합니다. 핵심 질문은 인공 시스템이 생물학적으로 얼마나 현실적으로 보이는지가 아니라, 신경과학에서 도출된 원리를 유용한 형태로 추상화하고, 구현하고, 측정하며, 통합할 수 있는가에 있습니다. 이러한 관점은 개별 사례 연구에서 더 넓은 뇌 기반 인공지능 아키텍처(Brain-Inspired AI Architecture)와 시스템 설계(System Design)를 위한 실용적인 지침으로 발전하기 위한 기반을 제공합니다.

##  

## 12.01 CNN and Visual Cortex [w/Code]

![](images/image2.png){width="7.268055555555556in" height="7.268055555555556in"}

The relationship between convolutional neural networks and the visual cortex is one of the clearest historical examples of neuroscience influencing artificial intelligence. CNNs were not designed as literal simulations of biological vision, but several of their central ideas reflect abstractions associated with cortical processing: local receptive fields, hierarchical feature extraction, spatial organization, and the progressive construction of complex representations from simpler visual patterns.

Biological vision begins before information reaches the cerebral cortex. Light captured by the retina is transformed through specialized neural circuits, and signals are routed through structures such as the lateral geniculate nucleus before reaching primary visual cortex. These stages perform substantial preprocessing rather than simply transmitting raw pixels, demonstrating that perception emerges from successive transformations of sensory information.

The primary visual cortex, commonly called V1, contains neurons that respond selectively to properties within restricted regions of visual space. Classical experiments revealed sensitivity to features such as edge orientation, spatial position, and local contrast. This organization introduced the influential idea that complex visual recognition can begin with populations of relatively specialized units responding to simple local structures.

A receptive field describes the region of sensory space capable of influencing the activity of a neuron. Nearby visual neurons may possess overlapping receptive fields, allowing many local measurements to collectively represent a scene. CNNs abstract this principle through convolutional kernels that operate over small spatial neighborhoods rather than connecting every image location independently to every feature detector.

Convolution adds an important engineering abstraction: the same learned filter can be applied across many spatial locations. This parameter sharing allows a feature detector learned in one part of an image to detect similar structure elsewhere. Biological visual processing does not implement mathematical convolution in precisely this form, but spatially repeated local processing provided an important conceptual foundation for efficient artificial visual architectures.

Early CNN layers typically learn relatively simple structures such as oriented edges, gradients, corners, and texture-like patterns. Deeper layers combine these responses into increasingly complex representations. Intermediate features can encode contours, motifs, textures, and object components, while later representations may become selective for structures strongly associated with object categories or task-relevant visual concepts.

This progression resembles the broad hierarchy of the ventral visual pathway. Information proceeds from early visual areas toward regions such as V2 and V4 and eventually into inferior temporal cortex, where neural responses can represent increasingly complex visual structures. The correspondence is approximate rather than one-to-one, but both systems illustrate how layered processing can progressively transform local sensory signals into more abstract representations.

Increasing receptive-field size is an important consequence of hierarchical processing. Although an early artificial neuron may depend on only a small image patch, deeper neurons indirectly receive information from increasingly large portions of the original image. This enables higher layers to integrate spatially separated features and represent relationships that cannot be recognized from isolated local measurements alone.

Pooling and related downsampling operations historically provided another important component of CNN architectures. By summarizing responses within neighborhoods, these operations reduce spatial resolution while preserving important feature information. The resulting representations can become less sensitive to small changes in feature position, supporting a degree of translation tolerance while simultaneously reducing computational and memory requirements.

Biological vision similarly demonstrates substantial tolerance to changes in position, scale, illumination, and viewpoint. Humans can recognize an object despite large variations in its retinal appearance. CNNs approximate portions of this capability through convolution, pooling, learned hierarchical representations, augmentation, and increasingly sophisticated architectural mechanisms, although robust invariance remains more complex than any single architectural operation.

The distinction between feature detection and feature integration is central to both perspectives. An isolated edge provides little information about object identity, but combinations of edges can form contours, contours can form shapes, and shapes can participate in object representations. Hierarchical composition therefore allows relatively simple computational operations to produce increasingly meaningful visual descriptions.

CNN feature maps also illustrate distributed representation. A visual concept is usually not stored in one artificial neuron corresponding to one human-interpretable category. Instead, information is distributed across activation patterns involving many channels and spatial positions. Biological visual representations likewise involve populations of neurons whose combined activity carries richer information than individual responses considered in isolation.

The success of CNNs also demonstrates why architectural inductive bias matters. Images possess strong spatial structure: neighboring pixels are related, visual patterns can recur across locations, and complex objects are constructed from local components. Convolution encodes assumptions compatible with this structure, allowing the model to learn visual representations more efficiently than architectures that initially treat every image location as completely unrelated.

Training nevertheless marks a major difference between conventional CNNs and biological visual systems. CNNs are commonly optimized using backpropagation and large labeled or self-supervised datasets, whereas biological learning involves interacting mechanisms including synaptic plasticity, development, recurrent activity, attention, multisensory experience, action, and neuromodulation. Similarities in architecture should therefore not be interpreted as evidence that the learning mechanisms are equivalent.

Another major difference concerns recurrence and feedback. A conventional feedforward CNN processes information sequentially from earlier layers toward later layers, but the visual cortex contains extensive lateral, recurrent, and top-down connections. Higher cortical regions can influence earlier processing, allowing expectations, attention, memory, task context, and previous interpretations to modify the processing of incoming sensory evidence.

This observation motivates recurrent and feedback-based extensions of artificial vision. Instead of producing a final interpretation in a single forward pass, a system can iteratively refine representations using contextual information or predictions from higher levels. Such architectures may be particularly useful when sensory evidence is ambiguous, partially occluded, noisy, or dependent on relationships that require repeated integration.

Attention provides another extension beyond the classical CNN analogy. Biological vision selectively allocates processing resources according to behavioral relevance rather than treating every visible location equally. Modern artificial vision similarly incorporates spatial, channel-wise, and feature-based attention mechanisms that dynamically emphasize information useful for the current task, supplementing the fixed local processing characteristic of convolution.

The visual system also separates partially distinct computational pathways. The ventral pathway is strongly associated with identifying what objects are, while dorsal processing contributes to spatial relationships, motion, visually guided action, and understanding where or how interaction should occur. This distinction is particularly relevant to robotics, where recognizing an object is insufficient without estimating its location, motion, geometry, and action possibilities.

For embodied AI, CNN-derived visual representations can therefore participate in a much larger perception-action architecture. Feature extraction may support object detection, semantic segmentation, depth estimation, tracking, localization, manipulation, and navigation. These representations can then interact with memory, world models, planning, and control, transforming visual recognition from an isolated classification problem into a component of autonomous behavior.

Modern computer vision has expanded beyond classical CNNs through vision transformers, hybrid architectures, multimodal foundation models, and self-supervised representation learning. Nevertheless, convolution remains important because locality, hierarchy, spatial reuse, and compositional feature construction continue to be useful computational principles. The historical connection to visual neuroscience therefore extends beyond any particular CNN architecture.

The case study ultimately demonstrates how neuroscience can contribute to AI without requiring direct biological replication. Observations about receptive fields and hierarchical visual processing inspired abstractions that became local connectivity, convolution, shared parameters, layered feature extraction, and increasingly complex representations. Engineering transformed these principles into scalable computational mechanisms whose usefulness could be evaluated independently of exact biological fidelity.

The broader lesson is methodological. Neuroscience can identify organizational principles, computational constraints, and recurring strategies, while AI can formalize selected principles and test them at scale. CNNs and the visual cortex show how a carefully chosen abstraction from biology can become a powerful engineering idea, while also demonstrating why functional inspiration must remain clearly separated from claims of mechanistic equivalence.

합성곱 신경망(Convolutional Neural Networks, CNNs)과 시각 피질(Visual Cortex)의 관계는 신경과학(Neuroscience)이 인공지능(Artificial Intelligence)에 영향을 미친 가장 명확한 역사적 사례 가운데 하나입니다. CNN은 생물학적 시각(Biological Vision)을 문자 그대로 시뮬레이션하도록 설계된 것은 아니지만, 핵심 아이디어 중 일부는 피질 처리(Cortical Processing)와 관련된 추상화에서 비롯되었습니다. 여기에는 국소 수용장(Local Receptive Fields), 계층적 특징 추출(Hierarchical Feature Extraction), 공간적 조직(Spatial Organization), 단순한 시각 패턴에서 복잡한 표상을 점진적으로 구성하는 방식이 포함됩니다.

생물학적 시각은 정보가 대뇌 피질(Cerebral Cortex)에 도달하기 전부터 시작됩니다. 망막(Retina)에 의해 포착된 빛은 특수화된 신경 회로(Neural Circuits)를 통해 변환되고, 신호는 일차 시각 피질(Primary Visual Cortex)에 도달하기 전에 외측슬상핵(Lateral Geniculate Nucleus, LGN)과 같은 구조를 통과합니다. 이러한 단계들은 단순히 원시 픽셀(Raw Pixels)을 전달하는 것이 아니라 상당한 전처리(Preprocessing)를 수행하며, 지각(Perception)이 감각 정보의 연속적인 변환을 통해 형성된다는 것을 보여줍니다.

일반적으로 V1이라고 불리는 일차 시각 피질(Primary Visual Cortex)은 제한된 시각 공간 영역의 특성에 선택적으로 반응하는 뉴런(Neurons)을 포함합니다. 고전적인 실험에서는 가장자리 방향(Edge Orientation), 공간적 위치(Spatial Position), 국소 대비(Local Contrast)와 같은 특징에 대한 선택성이 발견되었습니다. 이러한 조직은 복잡한 시각 인식(Visual Recognition)이 단순한 국소 구조에 반응하는 비교적 전문화된 유닛(Specialized Units)의 집단으로부터 시작될 수 있다는 중요한 아이디어를 제시했습니다.

수용장(Receptive Field)은 뉴런의 활동에 영향을 미칠 수 있는 감각 공간(Sensory Space)의 영역을 의미합니다. 서로 인접한 시각 뉴런들은 중첩되는 수용장(Overlapping Receptive Fields)을 가질 수 있으며, 이를 통해 다수의 국소적인 측정값이 함께 장면(Scene)을 표상할 수 있습니다. CNN은 모든 이미지 위치를 모든 특징 검출기(Feature Detector)에 독립적으로 연결하는 대신 작은 공간적 이웃(Spatial Neighborhoods)에 합성곱 커널(Convolutional Kernels)을 적용함으로써 이러한 원리를 추상화합니다.

합성곱(Convolution)은 중요한 공학적 추상화(Engineering Abstraction)를 추가합니다. 동일한 학습 필터(Learned Filter)를 여러 공간 위치에 적용할 수 있기 때문입니다. 이러한 파라미터 공유(Parameter Sharing)를 통해 이미지의 한 영역에서 학습된 특징 검출기가 다른 위치에서도 유사한 구조를 검출할 수 있습니다. 생물학적 시각 처리가 이러한 형태의 수학적 합성곱을 정확히 구현하는 것은 아니지만, 공간적으로 반복되는 국소 처리는 효율적인 인공 시각 아키텍처(Artificial Visual Architectures)를 위한 중요한 개념적 기반을 제공했습니다.

초기 CNN 계층(Early CNN Layers)은 일반적으로 방향성을 가진 가장자리, 기울기(Gradients), 모서리(Corners), 텍스처와 유사한 패턴과 같은 비교적 단순한 구조를 학습합니다. 더 깊은 계층은 이러한 반응을 결합하여 점점 더 복잡한 표상을 구성합니다. 중간 단계의 특징은 윤곽(Contours), 모티프(Motifs), 텍스처(Textures), 객체 구성 요소(Object Components)를 부호화할 수 있으며, 후반부의 표상은 객체 범주나 과제와 관련된 시각적 개념에 강하게 선택적으로 반응할 수 있습니다.

이러한 진행 과정은 복측 시각 경로(Ventral Visual Pathway)의 전반적인 계층 구조와 유사합니다. 정보는 초기 시각 영역에서 V2와 V4 같은 영역을 거쳐 최종적으로 하측두피질(Inferior Temporal Cortex)로 전달되며, 이 과정에서 신경 반응은 점점 더 복잡한 시각 구조를 표상할 수 있습니다. 이러한 대응은 정확한 일대일 관계가 아니라 근사적인 것이지만, 두 시스템 모두 계층적 처리(Layered Processing)를 통해 국소 감각 신호를 점진적으로 더욱 추상적인 표상으로 변환할 수 있음을 보여줍니다.

수용장 크기(Receptive-Field Size)의 증가는 계층적 처리의 중요한 결과입니다. 초기 인공 뉴런은 이미지의 작은 영역에만 의존할 수 있지만, 더 깊은 계층의 뉴런은 간접적으로 원본 이미지의 점점 더 넓은 영역에서 정보를 전달받습니다. 이를 통해 상위 계층은 공간적으로 떨어진 특징들을 통합하고, 서로 분리된 국소 측정만으로는 인식하기 어려운 관계를 표상할 수 있습니다.

풀링(Pooling)과 이와 관련된 다운샘플링(Downsampling) 연산은 역사적으로 CNN 아키텍처의 또 다른 중요한 구성 요소였습니다. 이러한 연산은 주변 영역의 반응을 요약하여 중요한 특징 정보를 보존하면서 공간 해상도(Spatial Resolution)를 감소시킵니다. 그 결과 표상은 특징 위치의 작은 변화에 덜 민감해질 수 있으며, 일정 수준의 이동 허용성(Translation Tolerance)을 제공하는 동시에 계산량과 메모리 요구량을 감소시킬 수 있습니다.

생물학적 시각 역시 위치(Position), 크기(Scale), 조명(Illumination), 시점(Viewpoint)의 변화에 대해 상당한 수준의 허용성을 보여줍니다. 인간은 망막에 나타나는 객체의 모습이 크게 변화하더라도 동일한 객체를 인식할 수 있습니다. CNN은 합성곱, 풀링, 학습된 계층적 표상, 데이터 증강(Data Augmentation), 그리고 더욱 발전된 아키텍처 메커니즘을 통해 이러한 능력의 일부를 근사하지만, 강건한 불변성(Robust Invariance)은 하나의 아키텍처 연산만으로 설명하기에는 훨씬 복잡합니다.

특징 검출(Feature Detection)과 특징 통합(Feature Integration)의 구분은 두 관점 모두에서 핵심적입니다. 하나의 독립적인 가장자리는 객체의 정체성에 관한 정보를 거의 제공하지 않지만, 여러 가장자리의 조합은 윤곽을 형성하고, 윤곽은 형태(Shapes)를 구성하며, 형태는 객체 표상(Object Representations)의 일부가 될 수 있습니다. 따라서 계층적 조합(Hierarchical Composition)은 비교적 단순한 계산 연산으로부터 점점 더 의미 있는 시각적 설명을 만들어낼 수 있도록 합니다.

CNN의 특징 맵(Feature Maps)은 분산 표상(Distributed Representation)의 개념도 보여줍니다. 하나의 시각적 개념이 일반적으로 하나의 인간 해석 가능한 범주에 대응하는 단일 인공 뉴런에 저장되는 것은 아닙니다. 대신 정보는 여러 채널(Channels)과 공간 위치에 걸친 활성화 패턴(Activation Patterns)에 분산됩니다. 생물학적 시각 표상 역시 개별 뉴런의 반응만으로는 표현하기 어려운 풍부한 정보를 다수 뉴런의 집단 활동(Population Activity)을 통해 전달합니다.

CNN의 성공은 아키텍처적 귀납 편향(Architectural Inductive Bias)이 왜 중요한지도 보여줍니다. 이미지는 강력한 공간적 구조(Spatial Structure)를 가지고 있습니다. 서로 인접한 픽셀은 연관되어 있고, 시각 패턴은 여러 위치에서 반복될 수 있으며, 복잡한 객체는 국소적인 구성 요소로 이루어집니다. 합성곱은 이러한 구조와 일치하는 가정을 아키텍처에 포함함으로써 모든 이미지 위치를 처음부터 완전히 독립적인 것으로 취급하는 아키텍처보다 더욱 효율적으로 시각 표상을 학습할 수 있도록 합니다.

그러나 학습(Training)은 기존 CNN과 생물학적 시각 시스템 사이의 중요한 차이점을 보여줍니다. CNN은 일반적으로 역전파(Backpropagation)와 대규모 레이블 데이터셋(Labeled Datasets) 또는 자기지도 데이터셋(Self-Supervised Datasets)을 이용하여 최적화됩니다. 반면 생물학적 학습에는 시냅스 가소성(Synaptic Plasticity), 발달(Development), 순환 활동(Recurrent Activity), 주의(Attention), 다중감각 경험(Multisensory Experience), 행동(Action), 신경조절(Neuromodulation)을 포함한 여러 상호작용 메커니즘이 관여합니다. 따라서 아키텍처의 유사성을 학습 메커니즘의 동등성으로 해석해서는 안 됩니다.

또 다른 중요한 차이는 순환성(Recurrence)과 피드백(Feedback)에 있습니다. 기존의 순방향 CNN(Feedforward CNN)은 초기 계층에서 후반 계층으로 정보를 순차적으로 처리하지만, 시각 피질에는 광범위한 측면 연결(Lateral Connections), 순환 연결(Recurrent Connections), 하향식 연결(Top-Down Connections)이 존재합니다. 상위 피질 영역은 초기 처리 과정에 영향을 줄 수 있으며, 이를 통해 기대(Expectations), 주의, 기억, 과제 맥락(Task Context), 이전의 해석이 새롭게 들어오는 감각 증거의 처리 방식을 변화시킬 수 있습니다.

이러한 관찰은 순환 및 피드백 기반 인공 시각(Recurrent and Feedback-Based Artificial Vision)의 확장을 촉진합니다. 한 번의 순방향 처리(Forward Pass)로 최종적인 해석을 생성하는 대신, 시스템은 맥락 정보(Contextual Information)나 상위 수준의 예측을 이용하여 표상을 반복적으로 정교화(Iterative Refinement)할 수 있습니다. 이러한 아키텍처는 감각적 증거가 모호하거나, 부분적으로 가려져 있거나, 잡음이 많거나, 반복적인 통합을 필요로 하는 관계에 의존하는 경우 특히 유용할 수 있습니다.

주의(Attention)는 고전적인 CNN과의 비교를 넘어서는 또 다른 확장 요소를 제공합니다. 생물학적 시각은 모든 보이는 위치를 동일하게 처리하는 대신 행동적 관련성(Behavioral Relevance)에 따라 처리 자원을 선택적으로 할당합니다. 현대의 인공 시각 시스템 역시 공간적 주의(Spatial Attention), 채널별 주의(Channel-Wise Attention), 특징 기반 주의(Feature-Based Attention)를 통합하여 현재 과제에 유용한 정보를 동적으로 강조함으로써 합성곱의 고정된 국소 처리를 보완합니다.

시각 시스템은 또한 부분적으로 서로 다른 계산 경로(Computational Pathways)를 구분합니다. 복측 경로(Ventral Pathway)는 객체가 무엇인지 식별하는 기능과 밀접하게 관련되어 있으며, 배측 처리(Dorsal Processing)는 공간 관계(Spatial Relationships), 움직임(Motion), 시각 유도 행동(Visually Guided Action), 그리고 어디에서 또는 어떻게 상호작용해야 하는지를 이해하는 데 기여합니다. 이러한 구분은 객체를 인식하는 것뿐만 아니라 객체의 위치, 움직임, 기하학(Geometry), 행동 가능성(Action Possibilities)을 추정해야 하는 로보틱스(Robotics)에서 특히 중요합니다.

따라서 체화 인공지능(Embodied AI)에서 CNN으로부터 얻어진 시각 표상은 훨씬 더 큰 지각-행동 아키텍처(Perception-Action Architecture)의 일부로 작동할 수 있습니다. 특징 추출(Feature Extraction)은 객체 검출(Object Detection), 의미론적 분할(Semantic Segmentation), 깊이 추정(Depth Estimation), 추적(Tracking), 위치 추정(Localization), 조작(Manipulation), 내비게이션(Navigation)을 지원할 수 있습니다. 이러한 표상은 다시 기억, 월드 모델(World Models), 계획(Planning), 제어(Control)와 상호작용하면서 시각 인식을 독립적인 분류 문제에서 자율 행동(Autonomous Behavior)의 구성 요소로 확장합니다.

현대 컴퓨터 비전(Modern Computer Vision)은 비전 트랜스포머(Vision Transformers), 하이브리드 아키텍처(Hybrid Architectures), 다중모달 파운데이션 모델(Multimodal Foundation Models), 자기지도 표상 학습(Self-Supervised Representation Learning)을 통해 고전적인 CNN을 넘어 확장되었습니다. 그럼에도 국소성(Locality), 계층성(Hierarchy), 공간적 재사용(Spatial Reuse), 조합적 특징 구성(Compositional Feature Construction)은 여전히 유용한 계산 원리이기 때문에 합성곱은 중요한 역할을 유지하고 있습니다. 따라서 시각 신경과학과의 역사적인 연결은 특정 CNN 아키텍처 하나를 넘어서는 의미를 가집니다.

이 사례 연구는 궁극적으로 신경과학이 생물학을 직접적으로 복제하지 않고도 인공지능에 기여할 수 있음을 보여줍니다. 수용장과 계층적 시각 처리에 대한 관찰은 국소 연결성(Local Connectivity), 합성곱, 파라미터 공유, 계층적 특징 추출, 점점 복잡해지는 표상과 같은 추상화에 영감을 주었습니다. 공학은 이러한 원리를 확장 가능한 계산 메커니즘(Scalable Computational Mechanisms)으로 변환했으며, 그 유용성은 정확한 생물학적 충실도(Biological Fidelity)와 독립적으로 평가될 수 있습니다.

보다 넓은 교훈은 방법론적(Methodological)입니다. 신경과학은 조직 원리(Organizational Principles), 계산적 제약(Computational Constraints), 반복적으로 나타나는 전략을 식별할 수 있으며, 인공지능은 선택된 원리를 형식화(Formalization)하고 대규모로 검증할 수 있습니다. CNN과 시각 피질의 관계는 생물학에서 신중하게 선택한 추상화가 강력한 공학적 아이디어로 발전할 수 있음을 보여주는 동시에, 기능적 영감(Functional Inspiration)과 기계적 동등성(Mechanistic Equivalence)에 대한 주장을 명확하게 구별해야 하는 이유를 보여줍니다.

##  

## 12.02 Dopamine and Deep RL [w/Code]

![](images/image3.png){width="7.268055555555556in" height="7.268055555555556in"}

Dopamine provides one of the most influential connections between neuroscience and reinforcement learning. Studies of dopaminergic systems show that neural responses can reflect differences between expected and obtained outcomes, while reinforcement learning uses related computational quantities to update predictions and behavior. This correspondence helped establish reward prediction error as a bridge between biological learning and artificial adaptive decision making.

Dopamine is a neuromodulator rather than a simple chemical representation of pleasure or reward. Dopaminergic neurons project from midbrain structures to regions including the striatum and prefrontal cortex, influencing learning, motivation, movement, attention, and action selection. Consequently, describing dopamine only as a reward signal oversimplifies a system whose effects depend on neural circuits, behavioral context, timing, and internal state.

A central finding concerns reward prediction. When an unexpected rewarding outcome occurs, some dopamine neurons show increased activity. As learning progresses and a predictive cue reliably precedes that reward, the response can shift toward the cue. If an expected reward fails to occur, activity can decrease around the expected time. This pattern suggests that learning depends strongly on deviations from expectation rather than reward magnitude alone.

This deviation is commonly described as reward prediction error. A positive error indicates that an outcome is better than expected, an error near zero indicates that the outcome approximately matches expectation, and a negative error indicates that the result is worse than expected. Prediction errors provide a directional learning signal: expectations should increase after unexpectedly favorable outcomes and decrease after unexpectedly unfavorable ones.

Reinforcement learning formalizes a related problem through interaction between an agent and an environment. At each step, the agent observes a state, selects an action according to a policy, receives a reward, and reaches a subsequent state. The objective is generally to learn behavior that maximizes expected cumulative reward rather than simply selecting whichever action produces the largest immediate reward.

This distinction introduces the problem of temporal credit assignment. An action may have little immediate benefit yet produce important consequences much later. Reinforcement-learning systems therefore use value functions to estimate expected future returns. A state-value function estimates the long-term desirability of a state, while an action-value function estimates the expected return associated with taking a particular action in a particular state.

Temporal-difference learning provides a particularly important computational connection with dopamine. Instead of waiting until an entire sequence finishes, TD methods update current predictions using the difference between successive estimates. A typical TD error compares the current value estimate with immediate reward plus the discounted estimate of the next state, allowing learning to proceed incrementally as experience unfolds.

The similarity between dopaminergic reward prediction signals and temporal-difference error became influential because both can be interpreted as signals for updating expectations. Better-than-expected outcomes support increases in predicted value, while worse-than-expected outcomes support decreases. However, this should be treated as a functional correspondence rather than evidence that the biological dopamine system literally implements one specific reinforcement-learning equation.

Deep reinforcement learning extends these ideas by replacing tables or simple function approximators with neural networks. High-dimensional observations such as images, sensor streams, proprioceptive states, or complex environment descriptions can be transformed into value estimates, policies, or both. Deep networks therefore allow reinforcement learning to operate in state spaces where explicitly storing a value for every possible situation would be impractical.

Value-based deep RL learns estimates such as Q-values that describe the expected return from state-action combinations. The agent can use these estimates to favor actions associated with higher predicted long-term value. Deep Q-learning combines this principle with neural representation learning, allowing raw or high-dimensional observations to influence decisions without requiring a manually constructed table for every state and action.

Policy-based methods take a different approach by directly parameterizing the policy that generates actions. Instead of deriving behavior only from estimated action values, policy-gradient methods adjust policy parameters in directions expected to improve cumulative reward. This approach is useful when actions are continuous, stochastic behavior is desirable, or directly representing the action distribution is more practical than maximizing over explicit action values.

Actor-critic architectures combine these perspectives. The actor represents the policy and selects actions, while the critic estimates value and evaluates the consequences of behavior. Prediction errors produced by the critic can guide updates to both components. This separation loosely resembles the broader biological distinction between evaluating outcomes and modifying action tendencies, although biological neural circuits are considerably more interconnected and complex.

Exploration creates another important connection between biological and artificial learning. An agent that always selects its currently preferred action may never discover better alternatives. Reinforcement learning therefore requires a balance between exploitation of known high-value behavior and exploration of uncertain possibilities. Biological behavior similarly reflects interactions among reward, novelty, uncertainty, motivation, and information seeking rather than reward maximization alone.

Experience replay improves deep RL by storing previous transitions and reusing them during training. Sampling past experiences can reduce correlations between consecutive observations and improve data efficiency. From a neuroscience perspective, replay has an interesting conceptual relationship with memory reactivation, but artificial replay buffers and biological memory replay should not be considered equivalent mechanisms simply because both revisit previous experience.

Model-based reinforcement learning adds predictive internal models of environmental dynamics and rewards. Instead of learning only from actions actually executed, an agent can estimate how candidate actions may change future states and use those predictions for planning. This connects reinforcement learning with world models, allowing imagined or simulated trajectories to supplement direct trial-and-error experience and potentially improve learning efficiency.

Reward design becomes especially important when reinforcement learning moves from games or simulations into real systems. A poorly specified reward can produce behavior that technically maximizes the numerical objective while violating the designer\'s actual intention. Useful rewards may need to incorporate task success, safety, energy, time, smoothness, risk, constraint satisfaction, and other factors without creating unintended optimization shortcuts.

Biological motivation demonstrates why a single scalar reward is often an incomplete description of intelligent behavior. Organisms respond to multiple interacting signals related to physiological needs, novelty, uncertainty, social context, threat, effort, and long-term goals. Dopamine itself participates in functions beyond simple reward prediction. Realistic artificial agents may therefore require richer objectives and internal regulatory mechanisms rather than one fixed reward channel.

For embodied AI and robotics, deep RL can connect perception directly with adaptive action. A robot can learn navigation, manipulation, locomotion, coordination, or control policies from interaction. Yet physical exploration is expensive and potentially dangerous, making simulation, offline datasets, demonstrations, model-based prediction, constraints, and safe fallback controllers important complements to unrestricted online trial-and-error learning.

Hierarchical reinforcement learning can improve this process by organizing behavior across different levels of abstraction. Higher levels can select goals or reusable skills, while lower levels translate those choices into detailed actions. Such organization resembles the broader hierarchical character of biological behavior, where strategic objectives, action sequences, and rapid motor control operate at different temporal and representational scales.

Human feedback can further supplement predefined reward functions. Preferences, demonstrations, evaluations, or corrections can provide information about desirable behavior when manually specifying a complete objective is difficult. This extends reinforcement learning from simple environmental rewards toward learning systems that infer or refine objectives through interaction with people, although human feedback introduces its own uncertainty and bias.

Multi-agent reinforcement learning expands the framework to environments containing multiple decision-making systems. Agents may cooperate, compete, communicate, or adapt to one another, causing the effective environment to change as other policies evolve. This creates challenges that resemble social and interactive learning, where outcomes depend not only on physical dynamics but also on predictions about the behavior of other agents.

The neuroscience-to-AI comparison must therefore remain carefully bounded. Dopamine influences many biological functions through complex neuromodulatory circuits, whereas artificial reinforcement learning typically uses simplified mathematical objects such as rewards, value functions, policies, and update rules. The scientific importance of the comparison lies in shared computational principles---prediction, error-driven updating, valuation, and adaptation---not literal equivalence.

Taken together, dopamine research and deep reinforcement learning illustrate how intelligence can improve through consequences. Experience creates expectations, actions generate outcomes, prediction errors reveal discrepancies, and learning modifies future values and policies. Deep RL transforms this principle into scalable algorithms, while neuroscience reminds AI research that adaptive behavior also depends on memory, context, motivation, uncertainty, exploration, and interacting learning systems.

도파민(Dopamine)은 신경과학(Neuroscience)과 강화학습(Reinforcement Learning)을 연결하는 가장 영향력 있는 개념 가운데 하나입니다. 도파민 시스템(Dopaminergic Systems)에 관한 연구는 신경 반응이 예상된 결과(Expected Outcomes)와 실제로 얻어진 결과(Obtained Outcomes) 사이의 차이를 반영할 수 있음을 보여주며, 강화학습 역시 이와 관련된 계산량(Computational Quantities)을 사용하여 예측과 행동을 갱신합니다. 이러한 대응 관계는 보상 예측 오류(Reward Prediction Error)를 생물학적 학습과 인공 적응형 의사결정(Artificial Adaptive Decision Making)을 연결하는 중요한 개념으로 확립하는 데 기여했습니다.

도파민은 단순히 쾌락(Pleasure)이나 보상(Reward)을 화학적으로 표현하는 물질이 아니라 신경조절물질(Neuromodulator)입니다. 도파민성 뉴런(Dopaminergic Neurons)은 중뇌 구조(Midbrain Structures)에서 선조체(Striatum)와 전전두엽 피질(Prefrontal Cortex)을 포함한 여러 영역으로 투사되며 학습, 동기(Motivation), 운동(Movement), 주의(Attention), 행동 선택(Action Selection)에 영향을 줍니다. 따라서 도파민을 단순한 보상 신호로 설명하는 것은 신경 회로, 행동 맥락, 시간적 특성(Timing), 내부 상태에 따라 효과가 달라지는 복잡한 시스템을 지나치게 단순화하는 것입니다.

핵심적인 발견 가운데 하나는 보상 예측(Reward Prediction)에 관한 것입니다. 예상하지 못한 보상 결과가 발생하면 일부 도파민 뉴런은 증가된 활동을 보입니다. 학습이 진행되어 특정 예측 단서(Predictive Cue)가 보상보다 앞서 안정적으로 나타나면 이러한 반응은 보상 자체에서 해당 단서로 이동할 수 있습니다. 반대로 예상했던 보상이 발생하지 않으면 예상된 시점 주변에서 활동이 감소할 수 있습니다. 이러한 패턴은 학습이 단순한 보상의 크기보다 기대에서 벗어난 정도(Deviation from Expectation)에 크게 의존한다는 것을 시사합니다.

이러한 기대와 결과 사이의 차이를 일반적으로 보상 예측 오류(Reward Prediction Error)라고 합니다. 양의 오류(Positive Error)는 결과가 예상보다 좋다는 것을 의미하고, 0에 가까운 오류는 결과가 대체로 예상과 일치한다는 것을 의미하며, 음의 오류(Negative Error)는 결과가 예상보다 좋지 않다는 것을 의미합니다. 예측 오류는 방향성을 가진 학습 신호(Directional Learning Signal)를 제공합니다. 예상보다 좋은 결과 이후에는 기대값을 증가시키고, 예상보다 나쁜 결과 이후에는 기대값을 감소시켜야 한다는 것입니다.

강화학습은 에이전트(Agent)와 환경(Environment)의 상호작용을 통해 이와 관련된 문제를 형식화합니다. 각 단계에서 에이전트는 상태(State)를 관찰하고, 정책(Policy)에 따라 행동(Action)을 선택하고, 보상을 받은 후 다음 상태(Subsequent State)에 도달합니다. 일반적인 목표는 단순히 가장 큰 즉각적 보상(Immediate Reward)을 제공하는 행동을 선택하는 것이 아니라 기대 누적 보상(Expected Cumulative Reward)을 최대화하는 행동을 학습하는 것입니다.

이러한 구분은 시간적 신용 할당(Temporal Credit Assignment) 문제를 발생시킵니다. 어떤 행동은 즉각적인 이익을 거의 제공하지 않더라도 훨씬 나중에 중요한 결과를 만들어낼 수 있습니다. 따라서 강화학습 시스템은 가치 함수(Value Functions)를 사용하여 기대되는 미래 수익(Expected Future Returns)을 추정합니다. 상태 가치 함수(State-Value Function)는 특정 상태의 장기적인 가치를 추정하고, 행동 가치 함수(Action-Value Function)는 특정 상태에서 특정 행동을 수행했을 때 기대되는 수익을 추정합니다.

시간차 학습(Temporal-Difference Learning, TD Learning)은 도파민과 특히 중요한 계산적 연결 관계를 제공합니다. 전체 행동 시퀀스가 끝날 때까지 기다리는 대신 TD 방법은 연속적인 가치 추정값 사이의 차이를 이용하여 현재의 예측을 갱신합니다. 일반적인 TD 오류(TD Error)는 현재 가치 추정값과 즉각적인 보상에 할인된 다음 상태의 가치 추정값을 더한 값을 비교하며, 이를 통해 경험이 진행되는 동안 점진적으로 학습할 수 있습니다.

도파민성 보상 예측 신호(Dopaminergic Reward Prediction Signals)와 시간차 오류(Temporal-Difference Error)의 유사성이 큰 영향을 미친 이유는 두 신호 모두 기대값을 갱신하기 위한 신호로 해석될 수 있기 때문입니다. 예상보다 좋은 결과는 예측 가치(Predicted Value)를 증가시키고, 예상보다 나쁜 결과는 이를 감소시키도록 합니다. 그러나 이러한 관계는 기능적 대응(Functional Correspondence)으로 이해해야 하며, 생물학적 도파민 시스템이 문자 그대로 특정 강화학습 방정식 하나를 구현한다는 증거로 해석해서는 안 됩니다.

심층 강화학습(Deep Reinforcement Learning)은 테이블(Table)이나 단순한 함수 근사기(Function Approximator)를 신경망(Neural Networks)으로 대체함으로써 이러한 아이디어를 확장합니다. 이미지, 센서 스트림(Sensor Streams), 고유수용감각 상태(Proprioceptive States), 복잡한 환경 설명과 같은 고차원 관측(High-Dimensional Observations)을 가치 추정값(Value Estimates), 정책 또는 두 가지 모두로 변환할 수 있습니다. 따라서 심층 신경망은 가능한 모든 상황의 가치를 명시적으로 저장하기 어려운 상태 공간(State Spaces)에서도 강화학습을 적용할 수 있도록 합니다.

가치 기반 심층 강화학습(Value-Based Deep RL)은 상태-행동 조합(State-Action Combinations)에서 기대되는 수익을 나타내는 Q값(Q-Values)과 같은 추정치를 학습합니다. 에이전트는 이러한 추정값을 이용하여 장기적으로 더 높은 가치가 예상되는 행동을 선호할 수 있습니다. 심층 Q학습(Deep Q-Learning)은 이러한 원리를 신경 표상 학습(Neural Representation Learning)과 결합하여 모든 상태와 행동에 대해 수작업으로 테이블을 구성하지 않고도 원시 데이터나 고차원 관측이 의사결정에 영향을 줄 수 있도록 합니다.

정책 기반 방법(Policy-Based Methods)은 행동을 생성하는 정책 자체를 직접 파라미터화(Parameterization)하는 다른 접근법을 사용합니다. 추정된 행동 가치만으로 행동을 결정하는 대신 정책 경사 방법(Policy-Gradient Methods)은 누적 보상을 향상시킬 것으로 예상되는 방향으로 정책 파라미터를 조정합니다. 이러한 접근법은 행동이 연속적(Continuous)이거나, 확률적 행동(Stochastic Behavior)이 필요하거나, 명시적인 행동 가치에서 최댓값을 선택하는 것보다 행동 분포(Action Distribution)를 직접 표현하는 것이 실용적인 경우에 유용합니다.

액터-크리틱 아키텍처(Actor-Critic Architectures)는 이러한 두 관점을 결합합니다. 액터(Actor)는 정책을 표현하고 행동을 선택하며, 크리틱(Critic)은 가치를 추정하고 행동의 결과를 평가합니다. 크리틱이 생성한 예측 오류는 두 구성 요소의 갱신을 안내할 수 있습니다. 이러한 분리는 결과를 평가하는 과정과 행동 성향(Action Tendencies)을 수정하는 과정 사이의 광범위한 생물학적 구분과 어느 정도 유사하지만, 실제 생물학적 신경 회로는 훨씬 더 상호 연결되어 있고 복잡합니다.

탐색(Exploration)은 생물학적 학습과 인공 학습 사이의 또 다른 중요한 연결점을 제공합니다. 현재 가장 선호되는 행동만 항상 선택하는 에이전트는 더 나은 대안을 발견하지 못할 수 있습니다. 따라서 강화학습에서는 이미 알려진 높은 가치의 행동을 활용하는 활용(Exploitation)과 불확실한 가능성을 조사하는 탐색 사이의 균형이 필요합니다. 생물학적 행동 역시 단순한 보상 최대화만이 아니라 보상, 새로움(Novelty), 불확실성(Uncertainty), 동기, 정보 탐색(Information Seeking)의 상호작용을 반영합니다.

경험 재생(Experience Replay)은 이전의 상태 전이(Transitions)를 저장하고 학습 과정에서 다시 사용함으로써 심층 강화학습을 개선합니다. 과거 경험을 샘플링하면 연속적인 관측 사이의 상관관계를 감소시키고 데이터 효율성(Data Efficiency)을 향상시킬 수 있습니다. 신경과학의 관점에서 재생은 기억 재활성화(Memory Reactivation)와 흥미로운 개념적 관계를 가지지만, 인공적인 재생 버퍼(Replay Buffers)와 생물학적 기억 재생을 단순히 과거 경험을 다시 사용한다는 이유만으로 동일한 메커니즘으로 간주해서는 안 됩니다.

모델 기반 강화학습(Model-Based Reinforcement Learning)은 환경 동역학(Environmental Dynamics)과 보상에 대한 예측적 내부 모델(Predictive Internal Models)을 추가합니다. 실제로 실행한 행동만으로 학습하는 대신 에이전트는 후보 행동이 미래 상태를 어떻게 변화시킬 것인지를 추정하고 이러한 예측을 계획(Planning)에 활용할 수 있습니다. 이는 강화학습을 월드 모델(World Models)과 연결하며, 상상되거나 시뮬레이션된 궤적(Simulated Trajectories)을 실제 시행착오 경험과 함께 사용하여 학습 효율성을 향상시킬 가능성을 제공합니다.

보상 설계(Reward Design)는 강화학습이 게임이나 시뮬레이션에서 실제 시스템(Real Systems)으로 이동할수록 특히 중요해집니다. 잘못 정의된 보상은 설계자의 실제 의도와 어긋나면서도 수치적 목적함수(Numerical Objective)를 기술적으로 최대화하는 행동을 만들어낼 수 있습니다. 유용한 보상은 의도하지 않은 최적화 지름길(Optimization Shortcuts)을 만들지 않으면서 과제 성공(Task Success), 안전(Safety), 에너지, 시간, 부드러운 동작(Smoothness), 위험(Risk), 제약 조건 만족(Constraint Satisfaction) 등의 요소를 포함해야 할 수 있습니다.

생물학적 동기(Biological Motivation)는 단일 스칼라 보상(Single Scalar Reward)이 지능적 행동을 설명하기에 충분하지 않은 경우가 많다는 것을 보여줍니다. 생물체는 생리적 필요(Physiological Needs), 새로움, 불확실성, 사회적 맥락(Social Context), 위협(Threat), 노력(Effort), 장기 목표(Long-Term Goals)와 관련된 여러 상호작용 신호에 반응합니다. 도파민 자체도 단순한 보상 예측을 넘어 다양한 기능에 관여합니다. 따라서 현실적인 인공 에이전트에는 하나의 고정된 보상 채널보다 더욱 풍부한 목적(Objectives)과 내부 조절 메커니즘(Internal Regulatory Mechanisms)이 필요할 수 있습니다.

체화 인공지능(Embodied AI)과 로보틱스(Robotics)에서 심층 강화학습은 지각(Perception)을 적응형 행동(Adaptive Action)과 직접 연결할 수 있습니다. 로봇은 상호작용을 통해 내비게이션(Navigation), 조작(Manipulation), 이동(Locomotion), 협응(Coordination), 제어(Control) 정책을 학습할 수 있습니다. 그러나 물리적 탐색은 비용이 높고 잠재적으로 위험하기 때문에 시뮬레이션(Simulation), 오프라인 데이터셋(Offline Datasets), 시연(Demonstrations), 모델 기반 예측(Model-Based Prediction), 제약 조건, 안전 폴백 제어기(Safe Fallback Controllers)가 제한 없는 온라인 시행착오 학습을 보완하는 중요한 수단이 됩니다.

계층적 강화학습(Hierarchical Reinforcement Learning)은 행동을 서로 다른 추상화 수준(Levels of Abstraction)으로 구성하여 이러한 과정을 개선할 수 있습니다. 상위 수준에서는 목표(Goals)나 재사용 가능한 기술(Reusable Skills)을 선택하고, 하위 수준에서는 이러한 선택을 구체적인 행동으로 변환할 수 있습니다. 이러한 구조는 전략적 목표(Strategic Objectives), 행동 시퀀스(Action Sequences), 빠른 운동 제어(Rapid Motor Control)가 서로 다른 시간적·표상적 척도에서 작동하는 생물학적 행동의 광범위한 계층적 특성과 유사합니다.

인간 피드백(Human Feedback)은 사전에 정의된 보상 함수(Reward Functions)를 추가적으로 보완할 수 있습니다. 선호(Preferences), 시연, 평가(Evaluations), 수정(Corrections)은 완전한 목적함수를 수작업으로 정의하기 어려운 경우 바람직한 행동에 관한 정보를 제공할 수 있습니다. 이는 강화학습을 단순한 환경 보상에서 사람과의 상호작용을 통해 목표를 추론하거나 개선하는 학습 시스템으로 확장하지만, 인간 피드백 자체에도 불확실성과 편향(Bias)이 존재할 수 있습니다.

다중 에이전트 강화학습(Multi-Agent Reinforcement Learning)은 이러한 프레임워크를 여러 의사결정 시스템이 존재하는 환경으로 확장합니다. 에이전트들은 협력(Cooperation), 경쟁(Competition), 통신(Communication), 상호 적응(Mutual Adaptation)을 수행할 수 있으며, 다른 에이전트의 정책이 변화함에 따라 실질적인 환경 자체도 변화하게 됩니다. 이는 결과가 물리적 동역학뿐만 아니라 다른 에이전트의 행동에 대한 예측에도 의존하는 사회적·상호작용적 학습(Social and Interactive Learning)과 유사한 문제를 발생시킵니다.

따라서 신경과학에서 인공지능으로 이어지는 비교의 범위는 신중하게 제한되어야 합니다. 도파민은 복잡한 신경조절 회로(Neuromodulatory Circuits)를 통해 다양한 생물학적 기능에 영향을 미치는 반면, 인공 강화학습은 일반적으로 보상, 가치 함수, 정책, 갱신 규칙(Update Rules)과 같이 단순화된 수학적 개체(Mathematical Objects)를 사용합니다. 이러한 비교의 과학적 중요성은 문자 그대로의 동등성이 아니라 예측, 오류 기반 갱신(Error-Driven Updating), 가치 평가(Valuation), 적응(Adaptation)이라는 공유된 계산 원리에 있습니다.

종합하면 도파민 연구와 심층 강화학습은 결과(Consequences)를 통해 지능이 어떻게 향상될 수 있는지를 보여줍니다. 경험은 기대(Expectations)를 형성하고, 행동은 결과를 생성하며, 예측 오류는 기대와 실제 결과 사이의 차이를 드러내고, 학습은 미래의 가치와 정책을 수정합니다. 심층 강화학습은 이러한 원리를 확장 가능한 알고리즘(Scalable Algorithms)으로 변환하며, 신경과학은 적응적 행동이 기억(Memory), 맥락(Context), 동기, 불확실성, 탐색, 그리고 상호작용하는 여러 학습 시스템에도 의존한다는 점을 보여줍니다.

##  

## 12.03 Hippocampus and RAG [w/Code]

![](images/image4.png){width="7.268055555555556in" height="7.268055555555556in"}

![](images/image5.png){width="7.268055555555556in" height="7.268055555555556in"}

The hippocampus and retrieval-augmented generation provide a useful case study for understanding how memory can be separated from core computation. The hippocampus supports rapid acquisition and retrieval of experiences, while RAG systems allow AI models to retrieve information from external stores when needed. The comparison is functional rather than biological: both illustrate the value of dynamically accessing relevant information instead of encoding everything within one fixed computational structure.

Human memory is distributed across interacting neural systems rather than stored in a single location. The hippocampus, located within the medial temporal lobe, plays a particularly important role in forming new episodic memories and organizing relationships among events, places, objects, and contexts. It interacts extensively with cortical regions, allowing newly acquired experiences to become connected with broader and more persistent knowledge representations.

Episodic memory allows an organism to retain information about specific experiences, including what occurred, where it happened, and the context surrounding the event. Such memories differ from generalized semantic knowledge because they preserve relationships associated with particular episodes. The hippocampus contributes to binding these distributed elements into representations that can later be reactivated when relevant cues or related situations are encountered.

This binding function is important because experiences contain multiple modalities and relationships. A single event may include visual information, sounds, spatial position, actions, goals, emotional significance, and temporal order. Rather than treating these elements independently, hippocampal mechanisms can associate them into structured representations. Retrieval can subsequently use partial cues to reactivate broader patterns associated with the original experience.

Pattern separation and pattern completion describe two useful computational ideas associated with hippocampal memory. Pattern separation helps distinguish similar experiences so that overlapping events do not become indistinguishable, while pattern completion allows a partial cue to recover a more complete stored representation. Together, these mechanisms illustrate how memory systems can balance discrimination between experiences with reconstruction from incomplete information.

Memory retrieval is therefore not simply equivalent to reading an exact record from storage. Current context, goals, cues, prior knowledge, and competing memories can influence which representation becomes accessible. Retrieval is selective and constructive, allowing information from previous experiences to participate in current reasoning and behavior. This principle provides an important conceptual connection to retrieval-based artificial intelligence systems.

Retrieval-augmented generation separates part of an AI system\'s accessible knowledge from the parameters of its generative model. Instead of requiring all information to be encoded during model training, documents, records, observations, or other knowledge can be maintained in an external repository. When a query arrives, the system retrieves relevant information and supplies it as context to the generative model before producing a response.

A typical RAG architecture therefore contains several interacting stages. Source information is divided into retrievable units, transformed into representations suitable for search, and stored in an index or database. A user query is similarly represented and compared with stored information. Relevant items are selected, inserted into the model\'s context, and used together with the model\'s parametric knowledge to generate an output.

Vector embeddings provide one common mechanism for retrieval. Text, images, or other information can be transformed into high-dimensional representations in which semantically related content tends to occupy related regions. Retrieval can then identify stored representations that are similar to the current query. This enables access based on semantic relationships rather than requiring exact keyword correspondence between the query and stored information.

The comparison with hippocampal retrieval becomes especially interesting at this point. A partial or context-dependent cue can lead biological memory toward associated experiences, while a query representation can guide an artificial retrieval system toward relevant stored information. Both cases emphasize content-sensitive access, but vector similarity search should not be interpreted as a direct computational model of hippocampal memory.

RAG also demonstrates the value of separating relatively stable parametric knowledge from dynamically updateable memory. Updating the factual contents of a neural model can require additional training, whereas an external knowledge store can often be modified without changing the model parameters. New documents can be added, obsolete information removed, and domain-specific knowledge reorganized while preserving the underlying generative model.

This separation can improve knowledge freshness. A pretrained model reflects information available during its training process, but an external retrieval system can contain more recent or application-specific material. Retrieval therefore allows the model to access information that was unavailable during pretraining. For practical AI systems, this reduces the need to repeatedly retrain a large model whenever the external knowledge environment changes.

External retrieval can also improve traceability. When generated content depends on retrieved documents, the system can preserve information about which sources contributed to the response. This does not guarantee correctness, because retrieval and generation can still fail, but it creates a stronger connection between generated claims and explicit evidence than relying exclusively on knowledge implicitly encoded in model parameters.

The hippocampal analogy also highlights the distinction between storage and reasoning. Remembering relevant experience does not by itself determine what action should be taken, just as retrieving documents does not automatically produce a correct answer. Retrieved information must be integrated with current goals, context, prior knowledge, reasoning, and decision processes. Memory becomes useful when it participates effectively in a broader cognitive architecture.

Retrieval quality is consequently a critical limitation of RAG. If relevant information is not retrieved, the generative model may respond using incomplete evidence. If irrelevant information is retrieved, it can distract the model or introduce errors. Retrieval performance depends on document segmentation, representations, indexing, query formulation, ranking, metadata, context-window constraints, and the quality of the underlying knowledge source.

Memory interference provides another useful conceptual comparison. Biological memories can compete during retrieval, particularly when experiences share similar cues. Artificial retrieval systems can likewise return multiple semantically similar but contextually different documents. Effective systems therefore require mechanisms for ranking, filtering, reranking, contextual discrimination, or combining evidence so that similarity alone does not determine what information influences the final response.

Temporal information is particularly important for dynamic memory. Two documents may describe the same entity accurately at different times but contain conflicting facts because the world has changed. A retrieval system should therefore consider timestamps, versioning, provenance, and validity when appropriate. Biological memory similarly exists within temporal context, although the mechanisms by which humans represent and reconstruct temporal relationships are much richer than database metadata.

For AI agents, retrieval can extend beyond factual documents into episodic memory. An autonomous agent may store previous interactions, observations, decisions, failures, successful plans, and environmental states. When encountering a related situation, it can retrieve relevant episodes and use them to guide planning or action. This creates a closer functional analogy with experience-based memory than conventional document retrieval alone.

Such agent memory can support continual adaptation without requiring every new experience to modify neural parameters immediately. Important events can first be stored externally and retrieved when relevant. Later processes may summarize, consolidate, generalize, or selectively incorporate repeated patterns into more persistent knowledge. This suggests a computational distinction between rapid episodic storage and slower long-term learning.

The idea resembles, at a highly abstract level, interactions between hippocampal and cortical memory systems. The hippocampus supports rapid learning of particular experiences, while longer-term cortical representations can develop through repeated interaction and consolidation. Artificial systems could similarly combine fast external memory with slower parameter updates, allowing rapid knowledge acquisition while reducing continual modification of a large foundation model.

World models can benefit from this architecture as well. A robot or embodied agent may retrieve previous observations of locations, objects, people, task outcomes, or environmental conditions when constructing predictions about the current situation. Memory retrieval can provide contextual evidence that is absent from immediate sensor data, while the world model can use that evidence to predict future states and evaluate candidate actions.

However, the hippocampus-RAG analogy has clear limits. The hippocampus participates in spatial cognition, relational representation, episodic memory, navigation, imagination, and interactions with many other neural systems. RAG is an engineered architecture that typically combines information retrieval with a generative model. Similarities in selective retrieval and externalized memory organization do not establish mechanistic equivalence between the two systems.

The broader lesson is that intelligent systems do not need to place every form of knowledge inside one monolithic parameter set. Memory can be structured according to different functions, timescales, and update requirements. Stable learned representations, external semantic knowledge, episodic experiences, working context, and procedural skills can interact while remaining partially distinct, creating a more flexible architecture for learning and reasoning.

The hippocampus and RAG therefore illustrate a general neuroscience-inspired principle: intelligence depends not only on how much information a system stores, but on how effectively it encodes, organizes, retrieves, integrates, and updates relevant experience. For future AI agents, combining foundation models with structured retrieval, episodic memory, consolidation, world models, and context-sensitive reasoning may provide a practical path toward more adaptive and memory-aware intelligence.

해마(Hippocampus)와 검색 증강 생성(Retrieval-Augmented Generation, RAG)은 기억(Memory)을 핵심 계산(Core Computation)과 어떻게 분리할 수 있는지를 이해하는 데 유용한 사례 연구를 제공합니다. 해마는 경험(Experiences)을 빠르게 획득하고 검색하는 기능을 지원하며, RAG 시스템은 인공지능 모델이 필요할 때 외부 저장소(External Stores)에서 정보를 검색할 수 있도록 합니다. 이러한 비교는 생물학적 동일성이 아니라 기능적 비교이며, 모든 정보를 하나의 고정된 계산 구조에 부호화하는 대신 관련 정보를 동적으로 접근하는 것의 가치를 보여줍니다.

인간의 기억(Human Memory)은 하나의 위치에 저장되는 것이 아니라 서로 상호작용하는 여러 신경 시스템(Neural Systems)에 분산되어 있습니다. 내측 측두엽(Medial Temporal Lobe)에 위치한 해마는 새로운 일화 기억(Episodic Memories)을 형성하고 사건, 장소, 객체, 맥락(Context) 사이의 관계를 조직하는 데 특히 중요한 역할을 합니다. 해마는 피질 영역(Cortical Regions)과 광범위하게 상호작용하며, 새롭게 획득한 경험이 더욱 광범위하고 지속적인 지식 표상(Knowledge Representations)과 연결될 수 있도록 합니다.

일화 기억(Episodic Memory)은 무엇이 발생했는지, 어디에서 발생했는지, 그리고 사건을 둘러싼 맥락이 무엇이었는지를 포함하여 특정 경험에 관한 정보를 생물체가 유지할 수 있도록 합니다. 이러한 기억은 특정 사건과 관련된 관계를 보존한다는 점에서 일반화된 의미 지식(Semantic Knowledge)과 다릅니다. 해마는 이렇게 분산된 요소들을 하나의 표상으로 결합하여 나중에 관련 단서(Related Cues)나 유사한 상황을 만났을 때 다시 활성화할 수 있도록 하는 데 기여합니다.

이러한 결합 기능(Binding Function)은 경험이 여러 감각 양식(Modalities)과 관계를 포함하기 때문에 중요합니다. 하나의 사건에는 시각 정보, 소리, 공간적 위치(Spatial Position), 행동, 목표, 정서적 중요성(Emotional Significance), 시간적 순서(Temporal Order)가 포함될 수 있습니다. 해마의 메커니즘은 이러한 요소를 독립적으로 처리하는 대신 구조화된 표상(Structured Representations)으로 연관시킬 수 있습니다. 이후 검색 과정에서는 부분적인 단서만으로도 원래 경험과 관련된 더 광범위한 패턴을 재활성화할 수 있습니다.

패턴 분리(Pattern Separation)와 패턴 완성(Pattern Completion)은 해마 기억과 관련된 두 가지 유용한 계산적 개념입니다. 패턴 분리는 서로 유사한 경험을 구별하여 중첩되는 사건들이 서로 구분되지 않는 문제를 방지하며, 패턴 완성은 부분적인 단서로부터 더욱 완전한 저장 표상을 복원할 수 있도록 합니다. 이러한 메커니즘은 기억 시스템이 경험 사이의 구별 능력과 불완전한 정보로부터의 복원 능력을 어떻게 균형 있게 유지할 수 있는지를 보여줍니다.

따라서 기억 검색(Memory Retrieval)은 단순히 저장소에서 정확한 기록 하나를 읽어오는 것과 동일하지 않습니다. 현재 맥락, 목표, 단서, 사전 지식(Prior Knowledge), 서로 경쟁하는 기억들이 어떤 표상에 접근할 수 있는지에 영향을 줄 수 있습니다. 검색은 선택적이고 구성적(Constructive)이며, 이전 경험의 정보가 현재의 추론과 행동에 참여할 수 있도록 합니다. 이러한 원리는 검색 기반 인공지능 시스템(Retrieval-Based Artificial Intelligence Systems)과 중요한 개념적 연결을 제공합니다.

검색 증강 생성(Retrieval-Augmented Generation)은 인공지능 시스템이 접근할 수 있는 지식의 일부를 생성 모델(Generative Model)의 파라미터와 분리합니다. 모든 정보를 모델 학습 과정에서 부호화하도록 요구하는 대신 문서, 기록, 관측, 기타 지식을 외부 저장소(External Repository)에 유지할 수 있습니다. 질의(Query)가 입력되면 시스템은 관련 정보를 검색하고, 응답을 생성하기 전에 해당 정보를 생성 모델의 맥락(Context)으로 제공합니다.

일반적인 RAG 아키텍처(RAG Architecture)는 따라서 여러 상호작용 단계로 구성됩니다. 원본 정보(Source Information)는 검색 가능한 단위(Retrievable Units)로 분할되고, 검색에 적합한 표상으로 변환되어 인덱스(Index)나 데이터베이스(Database)에 저장됩니다. 사용자 질의 역시 표상으로 변환되어 저장된 정보와 비교됩니다. 관련 항목을 선택한 후 모델의 맥락에 삽입하고, 모델의 파라미터 지식(Parametric Knowledge)과 함께 사용하여 출력을 생성합니다.

벡터 임베딩(Vector Embeddings)은 일반적으로 사용되는 검색 메커니즘 가운데 하나입니다. 텍스트, 이미지 또는 기타 정보를 고차원 표상(High-Dimensional Representations)으로 변환하여 의미적으로 관련된 콘텐츠가 서로 가까운 영역에 위치하도록 할 수 있습니다. 이후 검색 시스템은 현재 질의와 유사한 저장 표상을 식별할 수 있습니다. 이를 통해 질의와 저장된 정보 사이에 정확한 키워드 일치가 없어도 의미적 관계(Semantic Relationships)를 기반으로 정보에 접근할 수 있습니다.

이 지점에서 해마 검색과의 비교가 특히 흥미로워집니다. 부분적이거나 맥락 의존적인 단서(Context-Dependent Cue)는 생물학적 기억을 관련 경험으로 유도할 수 있으며, 질의 표상(Query Representation)은 인공 검색 시스템을 관련 저장 정보로 안내할 수 있습니다. 두 경우 모두 콘텐츠에 민감한 접근(Content-Sensitive Access)을 강조하지만, 벡터 유사도 검색(Vector Similarity Search)을 해마 기억의 직접적인 계산 모델로 해석해서는 안 됩니다.

RAG는 비교적 안정적인 파라미터 지식과 동적으로 갱신 가능한 기억(Dynamically Updateable Memory)을 분리하는 것의 가치도 보여줍니다. 신경망 모델의 사실적 내용을 갱신하려면 추가적인 학습이 필요할 수 있지만, 외부 지식 저장소(External Knowledge Store)는 모델 파라미터를 변경하지 않고도 수정할 수 있는 경우가 많습니다. 새로운 문서를 추가하고, 오래된 정보를 제거하며, 도메인 특화 지식(Domain-Specific Knowledge)을 재구성하면서도 기반 생성 모델을 그대로 유지할 수 있습니다.

이러한 분리는 지식 최신성(Knowledge Freshness)을 향상시킬 수 있습니다. 사전학습된 모델(Pretrained Model)은 학습 과정에서 이용할 수 있었던 정보를 반영하지만, 외부 검색 시스템은 더욱 최신이거나 특정 응용 분야에 특화된 자료를 포함할 수 있습니다. 따라서 검색을 이용하면 모델이 사전학습 당시에는 사용할 수 없었던 정보에 접근할 수 있습니다. 실용적인 인공지능 시스템에서는 외부 지식 환경이 변경될 때마다 대규모 모델을 반복적으로 재학습해야 하는 필요성을 줄일 수 있습니다.

외부 검색(External Retrieval)은 추적 가능성(Traceability)도 향상시킬 수 있습니다. 생성된 콘텐츠가 검색된 문서에 의존할 경우 시스템은 어떤 출처가 응답에 기여했는지에 관한 정보를 보존할 수 있습니다. 검색과 생성 과정 모두 여전히 실패할 수 있기 때문에 이것이 정확성을 보장하는 것은 아니지만, 모델 파라미터에 암묵적으로 부호화된 지식에만 의존하는 것보다 생성된 주장과 명시적인 증거(Explicit Evidence)를 더욱 강하게 연결할 수 있습니다.

해마와의 유추는 저장(Storage)과 추론(Reasoning)의 차이도 강조합니다. 관련 경험을 기억한다고 해서 어떤 행동을 취해야 하는지가 자동으로 결정되는 것은 아니며, 문서를 검색했다고 해서 자동으로 정확한 답이 생성되는 것도 아닙니다. 검색된 정보는 현재 목표, 맥락, 사전 지식, 추론, 의사결정(Decision Processes)과 통합되어야 합니다. 기억은 더 넓은 인지 아키텍처(Cognitive Architecture)에 효과적으로 참여할 때 유용해집니다.

따라서 검색 품질(Retrieval Quality)은 RAG의 중요한 한계 요소입니다. 관련 정보가 검색되지 않으면 생성 모델은 불완전한 증거를 기반으로 응답할 수 있습니다. 반대로 관련 없는 정보가 검색되면 모델의 판단을 방해하거나 오류를 유발할 수 있습니다. 검색 성능은 문서 분할(Document Segmentation), 표상, 인덱싱(Indexing), 질의 구성(Query Formulation), 순위 결정(Ranking), 메타데이터(Metadata), 컨텍스트 윈도(Context-Window) 제약, 기반 지식 출처의 품질에 따라 달라집니다.

기억 간섭(Memory Interference)은 또 다른 유용한 개념적 비교를 제공합니다. 생물학적 기억은 특히 여러 경험이 유사한 단서를 공유할 때 검색 과정에서 서로 경쟁할 수 있습니다. 인공 검색 시스템 역시 의미적으로 유사하지만 맥락적으로는 서로 다른 여러 문서를 반환할 수 있습니다. 따라서 효과적인 시스템에는 단순한 유사도만으로 최종 응답에 영향을 줄 정보를 결정하지 않도록 순위 결정, 필터링(Filtering), 재순위화(Reranking), 맥락적 구별(Contextual Discrimination), 증거 결합(Evidence Combination) 등의 메커니즘이 필요합니다.

시간 정보(Temporal Information)는 동적 기억(Dynamic Memory)에서 특히 중요합니다. 두 문서가 서로 다른 시점에서 동일한 대상에 대해 정확하게 설명하더라도 현실 세계가 변화했기 때문에 서로 상충하는 사실을 포함할 수 있습니다. 따라서 검색 시스템은 필요한 경우 타임스탬프(Timestamps), 버전 관리(Versioning), 출처 정보(Provenance), 유효성(Validity)을 고려해야 합니다. 생물학적 기억 역시 시간적 맥락 안에 존재하지만 인간이 시간 관계를 표상하고 재구성하는 메커니즘은 데이터베이스의 메타데이터보다 훨씬 복잡합니다.

인공지능 에이전트(AI Agents)의 경우 검색은 사실 문서를 넘어 일화 기억으로 확장될 수 있습니다. 자율 에이전트(Autonomous Agent)는 이전의 상호작용, 관측, 의사결정, 실패, 성공적인 계획, 환경 상태(Environmental States)를 저장할 수 있습니다. 이후 유사한 상황에 직면하면 관련된 과거 사건을 검색하여 계획이나 행동에 활용할 수 있습니다. 이는 일반적인 문서 검색만을 사용하는 것보다 경험 기반 기억(Experience-Based Memory)에 더욱 가까운 기능적 유사성을 형성합니다.

이러한 에이전트 기억(Agent Memory)은 모든 새로운 경험이 즉시 신경망 파라미터를 변경하지 않아도 지속적인 적응(Continual Adaptation)을 지원할 수 있습니다. 중요한 사건은 먼저 외부에 저장하고 필요한 경우 검색할 수 있습니다. 이후의 처리 과정에서는 반복되는 패턴을 요약(Summarization), 공고화(Consolidation), 일반화(Generalization)하거나 선택적으로 더욱 지속적인 지식에 통합할 수 있습니다. 이는 빠른 일화 저장(Rapid Episodic Storage)과 느린 장기 학습(Slower Long-Term Learning)을 계산적으로 구분할 수 있음을 시사합니다.

이러한 아이디어는 매우 추상적인 수준에서 해마와 피질 기억 시스템(Cortical Memory Systems)의 상호작용과 유사합니다. 해마는 특정 경험을 빠르게 학습하는 기능을 지원하는 반면, 장기적인 피질 표상(Cortical Representations)은 반복적인 상호작용과 기억 공고화를 통해 발달할 수 있습니다. 인공 시스템 역시 빠른 외부 기억(Fast External Memory)과 느린 파라미터 갱신(Slower Parameter Updates)을 결합하여 대규모 파운데이션 모델(Foundation Model)의 지속적인 변경을 줄이면서 새로운 지식을 빠르게 획득할 수 있습니다.

월드 모델(World Models) 역시 이러한 아키텍처의 이점을 활용할 수 있습니다. 로봇이나 체화 에이전트(Embodied Agent)는 현재 상황을 예측할 때 장소, 객체, 사람, 과제 결과, 환경 조건에 관한 이전의 관측을 검색할 수 있습니다. 기억 검색은 즉각적인 센서 데이터(Immediate Sensor Data)에 존재하지 않는 맥락적 증거(Contextual Evidence)를 제공하고, 월드 모델은 이러한 증거를 이용하여 미래 상태를 예측하고 후보 행동(Candidate Actions)을 평가할 수 있습니다.

그러나 해마와 RAG의 유추에는 명확한 한계가 있습니다. 해마는 공간 인지(Spatial Cognition), 관계적 표상(Relational Representation), 일화 기억, 내비게이션(Navigation), 상상(Imagination), 그리고 다양한 다른 신경 시스템과의 상호작용에 관여합니다. 반면 RAG는 일반적으로 정보 검색(Information Retrieval)과 생성 모델을 결합하는 공학적 아키텍처입니다. 선택적 검색(Selective Retrieval)과 외부화된 기억 조직(Externalized Memory Organization)의 유사성이 두 시스템 사이의 기계적 동등성(Mechanistic Equivalence)을 의미하지는 않습니다.

보다 넓은 관점에서 얻을 수 있는 교훈은 지능형 시스템(Intelligent Systems)이 모든 형태의 지식을 하나의 거대한 파라미터 집합(Monolithic Parameter Set) 안에 저장할 필요가 없다는 것입니다. 기억은 서로 다른 기능, 시간 척도(Timescales), 갱신 요구사항에 따라 구조화될 수 있습니다. 안정적인 학습 표상(Stable Learned Representations), 외부 의미 지식(External Semantic Knowledge), 일화적 경험(Episodic Experiences), 작업 맥락(Working Context), 절차적 기술(Procedural Skills)은 부분적으로 구별된 상태를 유지하면서 상호작용하여 더욱 유연한 학습 및 추론 아키텍처를 구성할 수 있습니다.

따라서 해마와 RAG는 일반적인 신경과학 기반 원리(Neuroscience-Inspired Principle)를 보여줍니다. 지능은 시스템이 얼마나 많은 정보를 저장하는지에만 의존하는 것이 아니라 관련 경험을 얼마나 효과적으로 부호화(Encoding), 조직화(Organization), 검색(Retrieval), 통합(Integration), 갱신(Update)할 수 있는지에도 의존합니다. 미래의 인공지능 에이전트에서는 파운데이션 모델과 구조화된 검색(Structured Retrieval), 일화 기억, 기억 공고화, 월드 모델, 맥락 의존적 추론(Context-Sensitive Reasoning)을 결합하는 것이 더욱 적응적이고 기억 인식적인 지능(Memory-Aware Intelligence)으로 발전하기 위한 실용적인 경로가 될 수 있습니다.

##  

## 12.04 Predictive Coding and Diffusion [w/Code]

![](images/image6.png){width="7.268055555555556in" height="7.268055555555556in"}

Predictive coding and diffusion models provide an instructive case study in how a broad computational principle can appear in both neuroscience and modern generative AI without implying direct mechanistic equivalence. Predictive coding describes perception in terms of predictions, sensory evidence, and prediction errors, while diffusion models generate structured data through repeated denoising. Their connection is best understood through iterative refinement and error reduction.

Predictive coding proposes that perception is not simply a bottom-up process in which sensory information travels through successive neural stages until an interpretation appears. Instead, higher levels of a processing hierarchy generate expectations about lower-level activity. Incoming sensory evidence is compared with these predictions, and discrepancies provide information that can be used to revise internal representations.

This creates a recurrent interaction between top-down prediction and bottom-up evidence. Higher levels communicate what should be observed according to the current internal model, while lower levels communicate information about mismatches between predictions and observations. Perception can therefore be interpreted as an iterative process in which internal hypotheses are repeatedly tested and refined against sensory input.

Prediction error is central to this framework. If an internal model accurately predicts incoming information, relatively little discrepancy remains to drive further revision. Unexpected observations create larger errors and indicate that the current representation does not adequately explain the sensory evidence. Error signals can consequently guide inference and learning toward representations that better capture regularities in the environment.

Hierarchical organization makes this process particularly powerful. Lower levels may represent relatively local or rapidly changing sensory properties, while higher levels can encode increasingly abstract causes, objects, contexts, or expectations. Predictions propagate downward through the hierarchy, while information related to prediction errors propagates upward, allowing representations at multiple levels to constrain one another through repeated interaction.

The concept of latent causes provides another important element. Sensory observations often result from hidden factors that cannot be directly observed, such as object identity, illumination, physical structure, intention, or environmental dynamics. A predictive system can infer internal latent representations that explain observed data and then use those representations to generate expectations about what should be perceived under particular conditions.

Generative models address a related computational problem by learning statistical structure that allows them to reconstruct, predict, transform, or generate data. Rather than learning only a boundary between predefined categories, a generative model attempts to capture aspects of how observations are distributed or produced. This capability makes generation and inference closely related: a model that captures structure can use it both to explain existing observations and to create plausible new ones.

Different generative architectures implement this principle differently. Autoencoders reconstruct inputs through compressed representations, variational autoencoders introduce probabilistic latent variables, and autoregressive models generate sequences through repeated conditional prediction. Diffusion models provide another approach by learning how to transform progressively corrupted data back toward structured samples through a sequence of denoising operations.

A diffusion model begins conceptually with a forward process in which noise is gradually added to data over multiple steps. As corruption increases, recognizable structure is progressively destroyed until the representation approaches a simple noise distribution. This forward process provides a controlled sequence connecting structured data with increasingly uncertain or noisy states.

Learning focuses on the reverse direction. The model is trained to estimate information required to remove corruption at different noise levels. During generation, it begins from noise and repeatedly applies learned denoising transformations. Each step produces a somewhat more structured representation, and after many iterations the process can produce a coherent sample consistent with the learned data distribution.

The repeated refinement characteristic of diffusion provides the strongest conceptual connection with predictive coding. Neither framework requires a complete solution to emerge in a single computational step. Instead, an imperfect state is progressively modified using information about what is inconsistent with the learned structure. The shared theme is iterative correction, although the mathematical quantities and biological interpretations involved are substantially different.

Prediction error and diffusion error should therefore not be treated as identical. Predictive coding theories describe discrepancies between internally generated expectations and sensory activity within a proposed model of neural processing. Diffusion objectives typically train artificial networks to estimate noise, denoised samples, scores, or related mathematical quantities. Similarity at the level of error-guided refinement does not establish equality between the underlying algorithms.

The direction of computation also differs. Predictive coding is commonly discussed as continuous interaction between sensory evidence and internal expectations during perception and learning. Diffusion generation can begin without an external sensory observation and progressively construct a sample from noise. Conditional diffusion can nevertheless incorporate text, images, states, or other contextual information that constrains the iterative generation process.

Conditioning demonstrates how prior information can influence generation. A text description, image, class label, sensor state, or other representation can guide the denoising trajectory toward outputs compatible with that context. At an abstract level, this resembles the role of higher-level expectations in constraining lower-level interpretations, although the implementation in artificial diffusion networks is an engineered probabilistic computation rather than cortical feedback.

Uncertainty provides another important connection. Ambiguous sensory evidence may support multiple possible interpretations, and generative models can represent distributions containing multiple plausible outcomes. Diffusion models can generate different samples from different initial noise states while respecting the same conditioning information. This property is valuable when the future or hidden state cannot be represented adequately by a single deterministic prediction.

For world models, such uncertainty is especially important. An intelligent agent may need to predict several possible future states rather than one supposedly certain future. Generative predictive models can represent alternative trajectories conditioned on current observations and candidate actions. These imagined futures can then support planning, risk estimation, exploration, and decision making before actions are executed in the physical environment.

Diffusion can also support reconstruction and completion. When sensory data are incomplete, corrupted, or noisy, learned generative structure can constrain plausible restorations. This capability connects naturally with the broader predictive idea that internal models help interpret uncertain observations. The system does not merely copy available input; it uses learned regularities to infer structures that are compatible with both observed evidence and prior knowledge.

For robotics, this principle can operate across multiple modalities. A predictive model may estimate future camera observations, depth, trajectories, object motion, robot states, or action consequences. Generative models can represent several plausible futures when environmental dynamics are uncertain. The resulting predictions can support planning by allowing the robot to evaluate possible consequences before committing to physical actions.

This creates an important connection with active perception. An agent does not have to remain a passive recipient of uncertain sensory evidence. If several interpretations remain plausible, it can move a camera, change viewpoint, manipulate an object, or navigate toward a location that provides more informative observations. Prediction and action can therefore form a closed loop in which uncertainty influences behavior and new observations refine internal models.

Predictive coding also emphasizes that context and prior knowledge influence perception. Identical sensory evidence may be interpreted differently depending on expectations, goals, or surrounding information. Modern conditional generative systems similarly combine observed information with contextual representations. However, these functional similarities should be used to identify useful design principles rather than to claim that artificial generative models reproduce biological perception.

Training mechanisms provide another major distinction. Modern diffusion models are generally optimized through large-scale gradient-based learning using artificial neural networks and extensive datasets. Biological predictive processing, if predictive-coding accounts are correct, would operate through neural circuits, recurrent signaling, synaptic plasticity, and biological dynamics. The two systems therefore differ substantially in substrate, learning rules, representations, and temporal organization.

Computational cost is also an important engineering consideration. Iterative denoising can require many neural-network evaluations, making diffusion generation slower than methods that produce outputs in one or a few passes. Research therefore explores faster samplers, reduced-step methods, latent diffusion, distillation, and alternative generative processes. Iterative refinement provides expressive power, but the number and cost of iterations matter greatly for real-time systems.

For embodied AI, latency constraints make this tradeoff particularly important. High-quality generative prediction may be useful for strategic planning over longer horizons, while rapid control loops require much faster responses. A practical architecture may therefore combine slower generative world-model reasoning with fast perception and control mechanisms operating at higher frequencies, creating a hierarchy of computational timescales.

The comparison ultimately reveals a broader principle shared by predictive and generative intelligence. Internal models capture regularities behind observations; predictions expose where those models succeed or fail; discrepancies provide information for refinement; and improved models support reconstruction, generation, forecasting, planning, and action. This progression connects predictive processing with a wider family of modern generative approaches.

Predictive coding and diffusion should therefore be viewed as conceptually related but mechanistically distinct frameworks. Their most useful correspondence lies in repeated inference, model-based expectation, uncertainty reduction, and iterative correction rather than literal algorithmic similarity. For future AI agents, these principles suggest systems that continuously predict, compare, refine, imagine alternatives, and use internal generative models to guide intelligent action in uncertain environments.

예측 부호화(Predictive Coding)와 확산 모델(Diffusion Models)은 하나의 광범위한 계산 원리(Computational Principle)가 신경과학(Neuroscience)과 현대 생성형 인공지능(Generative AI) 모두에서 어떻게 나타날 수 있는지를 보여주는 유용한 사례 연구입니다. 그렇다고 해서 두 시스템이 직접적으로 동일한 메커니즘을 가진다는 의미는 아닙니다. 예측 부호화는 예측(Predictions), 감각 증거(Sensory Evidence), 예측 오류(Prediction Errors)를 중심으로 지각을 설명하는 반면, 확산 모델은 반복적인 잡음 제거(Denoising)를 통해 구조화된 데이터를 생성합니다. 두 접근법의 연결은 반복적 정교화(Iterative Refinement)와 오류 감소(Error Reduction)를 중심으로 이해하는 것이 가장 적절합니다.

예측 부호화는 지각(Perception)이 단순한 상향식 처리(Bottom-Up Processing), 즉 감각 정보가 연속적인 신경 단계를 통과한 뒤 최종적인 해석이 나타나는 과정만은 아니라고 설명합니다. 대신 처리 계층(Processing Hierarchy)의 상위 수준은 하위 수준의 활동에 대한 기대(Expectations)를 생성합니다. 입력되는 감각 증거는 이러한 예측과 비교되며, 그 차이는 내부 표상(Internal Representations)을 수정하는 데 사용될 수 있는 정보를 제공합니다.

이 과정은 하향식 예측(Top-Down Prediction)과 상향식 증거(Bottom-Up Evidence) 사이의 순환적 상호작용(Recurrent Interaction)을 형성합니다. 상위 수준은 현재 내부 모델(Internal Model)에 따라 무엇이 관찰되어야 하는지를 전달하고, 하위 수준은 예측과 실제 관측 사이의 불일치(Mismatch)에 관한 정보를 전달합니다. 따라서 지각은 내부 가설(Internal Hypotheses)이 감각 입력에 대해 반복적으로 검증되고 정교화되는 반복적 과정(Iterative Process)으로 해석할 수 있습니다.

예측 오류(Prediction Error)는 이러한 프레임워크의 핵심입니다. 내부 모델이 입력 정보를 정확하게 예측한다면 추가적인 수정을 유도할 불일치가 상대적으로 적게 남습니다. 예상하지 못한 관측은 더 큰 오류를 생성하며 현재 표상이 감각 증거를 충분히 설명하지 못하고 있음을 나타냅니다. 따라서 오류 신호(Error Signals)는 환경의 규칙성(Regularities)을 더 잘 포착하는 표상을 향해 추론(Inference)과 학습(Learning)을 유도할 수 있습니다.

계층적 조직(Hierarchical Organization)은 이러한 과정을 특히 강력하게 만듭니다. 하위 수준은 비교적 국소적이거나 빠르게 변화하는 감각적 속성을 표상할 수 있는 반면, 상위 수준은 점점 더 추상적인 원인(Causes), 객체(Objects), 맥락(Context), 기대를 부호화할 수 있습니다. 예측은 계층을 따라 아래쪽으로 전달되고, 예측 오류와 관련된 정보는 위쪽으로 전달되면서 여러 수준의 표상이 반복적인 상호작용을 통해 서로를 제약할 수 있습니다.

잠재 원인(Latent Causes)의 개념은 또 다른 중요한 요소를 제공합니다. 감각 관측(Sensory Observations)은 객체의 정체성(Object Identity), 조명(Illumination), 물리적 구조(Physical Structure), 의도(Intention), 환경 동역학(Environmental Dynamics)과 같이 직접 관찰할 수 없는 숨겨진 요인에 의해 발생하는 경우가 많습니다. 예측 시스템은 관측 데이터를 설명하는 내부 잠재 표상(Latent Representations)을 추론하고, 이러한 표상을 이용하여 특정 조건에서 무엇이 지각되어야 하는지에 대한 기대를 생성할 수 있습니다.

생성 모델(Generative Models)은 데이터를 재구성(Reconstruction), 예측, 변환 또는 생성할 수 있도록 통계적 구조(Statistical Structure)를 학습함으로써 이와 관련된 계산 문제를 다룹니다. 미리 정의된 범주 사이의 경계만 학습하는 대신, 생성 모델은 관측이 어떻게 분포하거나 생성되는지에 관한 구조를 포착하려고 합니다. 이러한 능력은 생성(Generation)과 추론을 밀접하게 연결합니다. 구조를 포착한 모델은 기존 관측을 설명하는 데 사용할 수도 있고 새로운 데이터를 생성하는 데 사용할 수도 있습니다.

서로 다른 생성형 아키텍처(Generative Architectures)는 이러한 원리를 서로 다른 방법으로 구현합니다. 오토인코더(Autoencoders)는 압축된 표상(Compressed Representations)을 통해 입력을 재구성하고, 변분 오토인코더(Variational Autoencoders)는 확률적 잠재 변수(Probabilistic Latent Variables)를 도입하며, 자기회귀 모델(Autoregressive Models)은 반복적인 조건부 예측(Conditional Prediction)을 통해 시퀀스를 생성합니다. 확산 모델은 점진적으로 손상된 데이터를 일련의 잡음 제거 연산을 통해 다시 구조화된 샘플로 변환하는 방법을 학습하는 또 다른 접근법을 제공합니다.

확산 모델은 개념적으로 여러 단계에 걸쳐 데이터에 점진적으로 잡음(Noise)을 추가하는 순방향 과정(Forward Process)에서 시작합니다. 손상이 증가할수록 인식 가능한 구조는 점진적으로 파괴되고, 최종적으로 표상은 단순한 잡음 분포(Noise Distribution)에 가까워집니다. 이러한 순방향 과정은 구조화된 데이터와 점점 더 불확실하고 잡음이 많은 상태 사이를 연결하는 제어된 시퀀스를 제공합니다.

학습은 반대 방향인 역방향 과정(Reverse Process)에 초점을 맞춥니다. 모델은 서로 다른 잡음 수준에서 손상을 제거하는 데 필요한 정보를 추정하도록 학습됩니다. 생성 과정에서는 잡음에서 시작하여 학습된 잡음 제거 변환(Denoising Transformations)을 반복적으로 적용합니다. 각각의 단계에서 조금씩 더 구조화된 표상이 만들어지고, 여러 번의 반복을 거친 후 학습된 데이터 분포와 일치하는 일관성 있는 샘플(Coherent Sample)을 생성할 수 있습니다.

확산 모델의 이러한 반복적 정교화는 예측 부호화와의 가장 강력한 개념적 연결점을 제공합니다. 두 프레임워크 모두 하나의 계산 단계에서 완전한 해답이 만들어질 필요가 없습니다. 대신 불완전한 상태를 학습된 구조와 일치하지 않는 부분에 관한 정보를 이용하여 점진적으로 수정합니다. 공통된 주제는 반복적인 수정(Iterative Correction)이지만, 여기에 사용되는 수학적 양(Mathematical Quantities)과 생물학적 해석(Biological Interpretations)은 상당히 다릅니다.

따라서 예측 오류와 확산 오류(Diffusion Error)를 동일한 것으로 취급해서는 안 됩니다. 예측 부호화 이론은 제안된 신경 처리 모델에서 내부적으로 생성된 기대와 감각 활동 사이의 불일치를 설명합니다. 반면 확산 모델의 목적함수(Diffusion Objectives)는 일반적으로 인공 신경망이 잡음, 잡음이 제거된 샘플, 스코어(Score) 또는 관련된 수학적 양을 추정하도록 학습시킵니다. 오류 기반 정교화(Error-Guided Refinement)라는 수준에서의 유사성이 기반 알고리즘 자체의 동일성을 의미하지는 않습니다.

계산의 방향(Direction of Computation) 역시 다릅니다. 예측 부호화는 일반적으로 지각과 학습 과정에서 감각 증거와 내부 기대가 지속적으로 상호작용하는 과정으로 논의됩니다. 반면 확산 생성(Diffusion Generation)은 외부 감각 관측 없이도 잡음에서 시작하여 점진적으로 샘플을 구성할 수 있습니다. 그러나 조건부 확산(Conditional Diffusion)은 텍스트, 이미지, 상태 또는 기타 맥락 정보를 통합하여 반복적인 생성 과정을 제약할 수 있습니다.

조건화(Conditioning)는 사전 정보(Prior Information)가 생성 과정에 어떻게 영향을 줄 수 있는지를 보여줍니다. 텍스트 설명, 이미지, 클래스 레이블(Class Label), 센서 상태(Sensor State), 기타 표상을 이용하여 잡음 제거 궤적(Denoising Trajectory)이 해당 맥락과 일치하는 출력으로 진행되도록 유도할 수 있습니다. 추상적인 수준에서는 이것이 하위 수준의 해석을 제약하는 상위 수준의 기대와 유사하지만, 인공 확산 네트워크의 구현은 피질 피드백(Cortical Feedback)이 아니라 공학적으로 설계된 확률적 계산(Probabilistic Computation)입니다.

불확실성(Uncertainty)은 또 다른 중요한 연결점을 제공합니다. 모호한 감각 증거는 여러 가능한 해석을 지원할 수 있으며, 생성 모델은 여러 가능한 결과를 포함하는 분포를 표현할 수 있습니다. 확산 모델은 동일한 조건 정보(Conditioning Information)를 유지하면서 서로 다른 초기 잡음 상태에서 서로 다른 샘플을 생성할 수 있습니다. 이러한 특성은 미래나 숨겨진 상태를 하나의 결정론적 예측(Deterministic Prediction)만으로 충분히 표현할 수 없는 상황에서 특히 유용합니다.

월드 모델(World Models)에서는 이러한 불확실성이 특히 중요합니다. 지능형 에이전트(Intelligent Agent)는 하나의 확정된 미래만 예측하기보다 여러 가능한 미래 상태(Future States)를 예측해야 할 수 있습니다. 생성형 예측 모델(Generative Predictive Models)은 현재 관측과 후보 행동(Candidate Actions)을 조건으로 여러 대안적 궤적(Alternative Trajectories)을 표현할 수 있습니다. 이러한 상상된 미래(Imagined Futures)는 물리적 환경에서 실제 행동을 수행하기 전에 계획(Planning), 위험 추정(Risk Estimation), 탐색(Exploration), 의사결정(Decision Making)을 지원할 수 있습니다.

확산 모델은 재구성과 완성(Completion)에도 활용될 수 있습니다. 감각 데이터가 불완전하거나 손상되었거나 잡음이 포함된 경우 학습된 생성 구조(Learned Generative Structure)를 이용하여 가능한 복원 결과를 제약할 수 있습니다. 이러한 능력은 내부 모델이 불확실한 관측을 해석하는 데 도움을 준다는 광범위한 예측적 개념과 자연스럽게 연결됩니다. 시스템은 이용 가능한 입력을 단순히 복사하는 것이 아니라 학습된 규칙성을 이용하여 관측 증거와 사전 지식 모두에 부합하는 구조를 추론합니다.

로보틱스(Robotics)에서는 이러한 원리를 여러 감각 양식에 걸쳐 적용할 수 있습니다. 예측 모델은 미래 카메라 관측(Future Camera Observations), 깊이(Depth), 궤적(Trajectories), 객체 움직임(Object Motion), 로봇 상태(Robot States), 행동 결과(Action Consequences)를 추정할 수 있습니다. 생성 모델은 환경 동역학이 불확실한 경우 여러 가능한 미래를 표현할 수 있으며, 이러한 예측을 통해 로봇은 실제 행동을 실행하기 전에 가능한 결과를 평가할 수 있습니다.

이는 능동 지각(Active Perception)과 중요한 연결 관계를 형성합니다. 에이전트는 불확실한 감각 증거를 수동적으로 받아들이기만 할 필요가 없습니다. 여러 해석이 여전히 가능하다면 카메라를 움직이고, 시점을 변경하고, 객체를 조작하거나, 더 많은 정보를 제공하는 위치로 이동할 수 있습니다. 따라서 예측과 행동은 불확실성이 행동에 영향을 주고 새로운 관측이 내부 모델을 다시 정교화하는 폐쇄 루프(Closed Loop)를 형성할 수 있습니다.

예측 부호화는 맥락과 사전 지식이 지각에 영향을 준다는 점도 강조합니다. 동일한 감각 증거라도 기대, 목표(Goals), 주변 정보에 따라 다르게 해석될 수 있습니다. 현대의 조건부 생성 시스템(Conditional Generative Systems)도 관측 정보와 맥락 표상을 결합합니다. 그러나 이러한 기능적 유사성은 인공 생성 모델이 생물학적 지각을 재현한다고 주장하기보다 유용한 설계 원리(Design Principles)를 식별하는 데 활용해야 합니다.

학습 메커니즘(Training Mechanisms)은 두 시스템 사이의 또 다른 중요한 차이입니다. 현대 확산 모델은 일반적으로 대규모 데이터셋과 인공 신경망을 이용한 경사 기반 학습(Gradient-Based Learning)을 통해 최적화됩니다. 예측 부호화 이론이 생물학적으로 정확하다면 생물학적 예측 처리는 신경 회로(Neural Circuits), 순환 신호(Recurrent Signaling), 시냅스 가소성(Synaptic Plasticity), 생물학적 동역학(Biological Dynamics)을 통해 작동할 것입니다. 따라서 두 시스템은 물리적 기반(Substrate), 학습 규칙, 표상, 시간적 조직(Temporal Organization)에서 상당한 차이를 가집니다.

계산 비용(Computational Cost) 역시 중요한 공학적 고려사항입니다. 반복적인 잡음 제거는 많은 신경망 평가(Neural-Network Evaluations)를 요구할 수 있기 때문에 확산 생성은 한 번 또는 소수의 순방향 처리만으로 출력을 생성하는 방식보다 느릴 수 있습니다. 따라서 연구에서는 빠른 샘플러(Faster Samplers), 단계 감소 방법(Reduced-Step Methods), 잠재 확산(Latent Diffusion), 증류(Distillation), 대안적인 생성 과정 등을 통해 계산량을 줄이는 방법을 탐구합니다. 반복적 정교화는 강력한 표현 능력을 제공하지만 반복 횟수와 각 반복의 계산 비용은 실시간 시스템에서 매우 중요합니다.

체화 인공지능(Embodied AI)에서는 지연시간(Latency) 제약으로 인해 이러한 절충 관계가 특히 중요합니다. 높은 품질의 생성형 예측은 더 긴 시간 범위의 전략적 계획(Strategic Planning)에 유용할 수 있지만, 빠른 제어 루프(Control Loops)는 훨씬 더 신속한 응답을 요구합니다. 따라서 실용적인 아키텍처는 느린 생성형 월드 모델 추론(Generative World-Model Reasoning)과 더 높은 주파수에서 작동하는 빠른 지각 및 제어 메커니즘을 결합하여 서로 다른 계산 시간 척도(Computational Timescales)의 계층 구조를 구성할 수 있습니다.

이러한 비교는 궁극적으로 예측 지능(Predictive Intelligence)과 생성 지능(Generative Intelligence)이 공유하는 보다 광범위한 원리를 보여줍니다. 내부 모델은 관측의 배후에 존재하는 규칙성을 포착하고, 예측은 이러한 모델이 어디에서 성공하거나 실패하는지를 드러내며, 불일치는 모델을 정교화하기 위한 정보를 제공합니다. 개선된 모델은 재구성, 생성, 미래 예측(Forecasting), 계획, 행동을 지원할 수 있습니다. 이러한 과정은 예측 처리(Predictive Processing)를 현대 생성형 접근법의 더 광범위한 계열과 연결합니다.

따라서 예측 부호화와 확산 모델은 개념적으로 관련되어 있지만 메커니즘적으로는 구별되는(Mechanistically Distinct) 프레임워크로 이해해야 합니다. 두 접근법의 가장 유용한 대응 관계는 문자 그대로의 알고리즘적 유사성이 아니라 반복적 추론(Repeated Inference), 모델 기반 기대(Model-Based Expectation), 불확실성 감소(Uncertainty Reduction), 반복적 수정에 있습니다. 미래의 인공지능 에이전트에서는 이러한 원리를 활용하여 지속적으로 예측하고, 비교하고, 정교화하고, 여러 대안을 상상하며, 내부 생성 모델(Internal Generative Models)을 이용해 불확실한 환경에서 지능적인 행동을 유도하는 시스템을 구축할 수 있습니다.

##  

## 12.05 Spiking Neural Networks [w/Code]

![](images/image7.png){width="7.268055555555556in" height="7.268055555555556in"}

Spiking neural networks represent an approach to artificial intelligence that models computation through discrete events called spikes rather than continuously valued activations. They are inspired by the event-driven signaling of biological neurons, where information is transmitted through electrical impulses occurring over time. This makes temporal dynamics an explicit part of computation and distinguishes SNNs from conventional artificial neural networks.

In a conventional neural network, neurons usually receive numerical inputs, calculate weighted sums, apply activation functions, and transmit continuous-valued outputs to subsequent layers. A spiking neuron instead maintains an internal state that evolves over time. Incoming spikes modify this state, and when its membrane-like potential reaches a threshold, the neuron emits a spike and subsequently resets or modifies its internal dynamics.

This temporal behavior means that an SNN cannot generally be understood only from instantaneous activation values. The timing, frequency, and sequence of spikes may all carry information. Two neurons producing the same number of spikes can represent different temporal patterns if those spikes occur at different moments. Computation therefore depends simultaneously on network connectivity, neural state, and the temporal organization of events.

The integrate-and-fire neuron provides one of the simplest abstractions for spiking computation. Incoming signals accumulate within an internal membrane potential until a threshold is reached, after which a spike is emitted. The leaky integrate-and-fire model extends this principle by allowing accumulated potential to decay over time, representing the idea that earlier inputs gradually lose influence unless reinforced by subsequent activity.

These dynamics provide SNNs with an intrinsic form of temporal memory. A neuron\'s current response depends not only on the present input but also on signals received during preceding moments. This property makes spiking computation naturally relevant to temporally structured problems such as sensory streams, motion, auditory signals, robotic interaction, and other tasks in which the order and timing of events contain useful information.

Information can be represented in SNNs using several coding strategies. Rate coding represents information through the number or frequency of spikes within a time interval, while temporal coding uses precise spike timing. Other approaches rely on latency, population activity, relative timing, or combinations of these mechanisms. The appropriate representation depends strongly on the task, sensor characteristics, learning algorithm, and computing hardware.

Sparse activity is another important characteristic of many spiking systems. A neuron does not necessarily perform an output-producing operation at every computational step; instead, significant communication can occur only when a spike is generated. If activity remains sufficiently sparse, event-driven processing can avoid some unnecessary computation and data movement associated with repeatedly updating every unit in a dense artificial neural network.

This property creates an important connection between SNNs and energy-efficient computing. Conventional accelerators frequently perform large numbers of multiply-accumulate operations even when much of the represented information changes slowly. Event-driven architectures can instead concentrate computational resources on changes and significant events. The potential efficiency advantage, however, depends on the complete algorithm-hardware system rather than on spikes alone.

Learning in spiking networks presents substantial challenges because spike generation is typically discontinuous. Standard backpropagation assumes differentiable operations, whereas a threshold-triggered spike does not provide an ordinary smooth derivative. Researchers therefore use approaches such as surrogate gradients, local plasticity rules, conversion from trained conventional networks, evolutionary optimization, and other methods designed specifically for temporal and event-driven computation.

Spike-timing-dependent plasticity provides a biologically inspired example of a local learning rule. In simplified STDP models, changes in synaptic strength depend on the relative timing between presynaptic and postsynaptic spikes. Connections can be strengthened or weakened according to temporal relationships between events. This illustrates how learning can potentially emerge from locally available timing information rather than from a globally calculated error signal.

Nevertheless, STDP should not be interpreted as a complete replacement for modern deep-learning optimization. Complex tasks require mechanisms capable of assigning credit across large networks, long temporal intervals, and multiple processing stages. Practical SNN research therefore explores combinations of local plasticity, global objectives, surrogate-gradient learning, reinforcement signals, and architectural constraints rather than assuming that one biological learning rule solves every optimization problem.

Artificial neural network to SNN conversion offers another practical strategy. A conventional network can first be trained using mature deep-learning methods and then transformed into a spiking representation. Activation magnitudes may be approximated through spike rates or temporal patterns. This approach can preserve useful learned representations while enabling deployment on event-driven hardware, although conversion can introduce latency, accuracy, and calibration tradeoffs.

Direct training provides greater opportunity to exploit temporal spike structure. Instead of treating spikes primarily as an alternative representation of conventional activations, directly trained SNNs can learn from event sequences and internal dynamics. This becomes particularly attractive when input sensors already generate asynchronous events, because temporal information can flow through the system without first being converted into conventional fixed-rate image frames.

Event cameras therefore form a natural sensory interface for spiking computation. Rather than repeatedly capturing complete frames, these sensors report local brightness changes asynchronously. The resulting event stream is sparse and temporally precise. An SNN can process such events using similar event-driven principles, potentially creating a perception pipeline in which sensing, communication, and neural computation all respond primarily to environmental changes.

This combination is particularly relevant to robotics. Rapid motion, changing illumination, collision avoidance, optical flow, tracking, localization, gesture recognition, and reactive control can benefit from low-latency temporal information. A robot equipped with event-driven sensing and spiking processing may react to important changes without waiting for the next conventional frame, although practical performance depends heavily on algorithms, sensors, processors, and integration quality.

Neuromorphic processors provide hardware designed to exploit characteristics associated with spiking and event-driven computation. Instead of organizing all processing around dense synchronous matrix operations, neuromorphic architectures may place computation near local state, communicate through events, and activate resources selectively. This can reduce memory traffic and unnecessary activity for suitable workloads, which is especially important for power-constrained edge systems.

The relationship between SNNs and neuromorphic hardware demonstrates the importance of co-design. Running a spiking model inefficiently on hardware optimized for dense conventional neural networks may provide little benefit. Likewise, specialized neuromorphic hardware cannot automatically create efficient intelligence without appropriate algorithms. Advantages emerge when neural representation, learning, communication, sensor interfaces, software, and hardware are designed to complement one another.

SNNs are particularly interesting for edge AI because power and latency constraints often limit continuous high-performance computation. Mobile robots, drones, wearable devices, autonomous sensors, and embedded systems may need to operate for long periods from limited energy sources. Event-driven processing could allow selected perception and monitoring functions to remain continuously active while more computationally expensive systems are activated only when necessary.

This suggests a hybrid architecture rather than complete replacement of conventional deep learning. Spiking networks can handle continuous low-power monitoring, temporal event detection, or rapid reflex-like processing, while CNNs, transformers, generative models, or foundation models perform richer semantic interpretation and planning. Different computational mechanisms can therefore operate at different timescales according to task complexity and available resources.

Such a hierarchy resembles an important principle of biological intelligence: not every sensory event requires expensive global processing. Many signals can be filtered or handled locally, while unusual, uncertain, or behaviorally important events recruit broader processing resources. Artificial agents could similarly use lightweight event-driven modules to detect changes and selectively invoke larger models when deeper reasoning becomes necessary.

Temporal credit assignment remains a major challenge when SNNs are used for adaptive behavior. An action may depend on spike patterns occurring across extended periods, while useful feedback may arrive much later. Reinforcement learning, eligibility traces, local temporal states, and neuromodulatory learning mechanisms provide possible approaches for connecting delayed outcomes with earlier neural activity, but scalable solutions remain an active research area.

SNNs also reveal why biological similarity should not itself be treated as an engineering objective. A model does not become more intelligent merely because it emits spikes. Biological brains combine spikes with complex dendritic computation, diverse cell types, recurrent connectivity, chemical modulation, structural plasticity, development, embodiment, and continual interaction. Artificial spiking networks capture only selected abstractions from this much richer biological system.

Evaluation must therefore focus on measurable system-level benefits. Relevant metrics include accuracy, response latency, energy consumption, memory traffic, event sparsity, robustness, learning efficiency, hardware utilization, and performance under temporal uncertainty. A spiking solution is valuable when these properties improve for a particular application, not simply because its internal signals appear more biologically realistic than conventional activations.

For Physical AI, SNNs are especially promising as components of multi-timescale intelligence. Fast event-driven circuits can process immediate sensory changes, conventional perception networks can construct semantic representations, world models can predict future states, and higher-level agents can perform planning and reasoning. These layers can cooperate instead of forcing every problem through a single neural architecture operating at one computational frequency.

The broader significance of spiking neural networks therefore lies in reconsidering when computation should occur. Conventional AI commonly performs synchronized computation continuously, whereas event-driven systems can allocate computation according to changes in information. This shift from continuous processing toward activity-dependent processing may become increasingly important as intelligent systems move from data centers into robots and autonomous machines constrained by energy and real-time operation.

Spiking neural networks ultimately demonstrate how neuroscience can inspire alternative computational architectures without requiring literal replication of the brain. Spikes introduce explicit time, sparse communication, internal dynamics, and event-driven processing into artificial neural computation. Combined with event sensors and neuromorphic processors, these principles provide a potential foundation for low-power, responsive, temporally aware intelligence operating directly within the physical world.

스파이킹 신경망(Spiking Neural Networks, SNNs)은 연속적인 값을 가지는 활성화(Continuously Valued Activations) 대신 스파이크(Spikes)라고 불리는 이산적인 이벤트(Discrete Events)를 통해 계산을 모델링하는 인공지능 접근법입니다. 이는 생물학적 뉴런(Biological Neurons)이 시간에 따라 발생하는 전기적 임펄스(Electrical Impulses)를 통해 정보를 전달하는 이벤트 기반 신호 전달(Event-Driven Signaling)에서 영감을 받았습니다. 이러한 특성은 시간적 동역학(Temporal Dynamics)을 계산의 명시적인 일부로 만들며 SNN을 기존 인공 신경망(Artificial Neural Networks)과 구별합니다.

기존 신경망(Conventional Neural Network)에서 뉴런은 일반적으로 수치 입력을 받아 가중합(Weighted Sum)을 계산하고 활성화 함수(Activation Function)를 적용한 후 연속값 출력을 다음 계층으로 전달합니다. 반면 스파이킹 뉴런(Spiking Neuron)은 시간에 따라 변화하는 내부 상태(Internal State)를 유지합니다. 입력 스파이크는 이러한 상태를 변화시키며, 막전위(Membrane-Like Potential)가 임계값(Threshold)에 도달하면 뉴런이 스파이크를 발생시키고 이후 내부 상태를 초기화하거나 동역학을 변화시킵니다.

이러한 시간적 행동(Temporal Behavior)은 일반적으로 SNN을 특정 순간의 활성화 값만으로 이해할 수 없다는 것을 의미합니다. 스파이크의 타이밍(Timing), 빈도(Frequency), 순서(Sequence)가 모두 정보를 전달할 수 있습니다. 두 뉴런이 동일한 수의 스파이크를 생성하더라도 서로 다른 시점에 스파이크가 발생하면 서로 다른 시간 패턴(Temporal Patterns)을 표현할 수 있습니다. 따라서 계산은 네트워크 연결성(Network Connectivity), 신경 상태(Neural State), 이벤트의 시간적 조직(Temporal Organization)에 동시에 의존합니다.

적분-발화 뉴런(Integrate-and-Fire Neuron)은 스파이킹 계산(Spiking Computation)을 설명하는 가장 단순한 추상화 가운데 하나입니다. 입력 신호는 내부 막전위에 누적되며 임계값에 도달하면 스파이크가 발생합니다. 누설 적분-발화 모델(Leaky Integrate-and-Fire Model)은 누적된 전위가 시간에 따라 감소하도록 이 원리를 확장하며, 이전 입력이 후속 활동에 의해 강화되지 않는 경우 점차 영향력을 잃는다는 개념을 표현합니다.

이러한 동역학은 SNN에 본질적인 형태의 시간적 기억(Temporal Memory)을 제공합니다. 뉴런의 현재 반응은 현재 입력뿐만 아니라 이전 순간에 수신한 신호에도 의존합니다. 이러한 특성으로 인해 스파이킹 계산은 감각 스트림(Sensory Streams), 움직임(Motion), 청각 신호(Auditory Signals), 로봇 상호작용(Robotic Interaction)과 같이 이벤트의 순서와 타이밍이 유용한 정보를 포함하는 시간적으로 구조화된 문제에 자연스럽게 적용될 수 있습니다.

SNN에서는 여러 부호화 전략(Coding Strategies)을 사용하여 정보를 표현할 수 있습니다. 발화율 부호화(Rate Coding)는 일정 시간 구간 동안 발생하는 스파이크의 수 또는 빈도를 이용해 정보를 표현하며, 시간 부호화(Temporal Coding)는 정확한 스파이크 발생 시점을 활용합니다. 이외에도 지연시간(Latency), 집단 활동(Population Activity), 상대적 타이밍(Relative Timing), 또는 이들을 결합한 방법을 사용할 수 있습니다. 적절한 표상 방식은 과제, 센서 특성, 학습 알고리즘, 컴퓨팅 하드웨어에 크게 의존합니다.

희소 활동(Sparse Activity)은 많은 스파이킹 시스템에서 나타나는 또 다른 중요한 특성입니다. 뉴런이 모든 계산 단계에서 반드시 출력을 생성하는 연산을 수행할 필요는 없으며, 의미 있는 통신은 스파이크가 발생할 때만 일어날 수 있습니다. 활동이 충분히 희소하다면 이벤트 기반 처리(Event-Driven Processing)는 밀집 인공 신경망(Dense Artificial Neural Network)에서 모든 유닛을 반복적으로 갱신할 때 발생하는 일부 불필요한 계산과 데이터 이동(Data Movement)을 줄일 수 있습니다.

이러한 특성은 SNN과 에너지 효율적 컴퓨팅(Energy-Efficient Computing) 사이의 중요한 연결을 형성합니다. 기존 가속기(Conventional Accelerators)는 표현되는 정보가 느리게 변화하는 경우에도 많은 수의 곱셈-누산 연산(Multiply-Accumulate Operations)을 수행하는 경우가 많습니다. 반면 이벤트 기반 아키텍처(Event-Driven Architectures)는 변화와 중요한 이벤트에 계산 자원을 집중할 수 있습니다. 그러나 잠재적인 효율성 이점은 스파이크 자체가 아니라 전체 알고리즘-하드웨어 시스템(Algorithm-Hardware System)의 구성에 따라 달라집니다.

스파이킹 네트워크의 학습은 스파이크 생성이 일반적으로 불연속적(Discontinuous)이기 때문에 상당한 어려움을 가집니다. 표준 역전파(Backpropagation)는 미분 가능한 연산(Differentiable Operations)을 가정하지만 임계값에 의해 발생하는 스파이크는 일반적인 형태의 부드러운 미분값을 제공하지 않습니다. 따라서 연구자들은 대리 경사(Surrogate Gradients), 국소 가소성 규칙(Local Plasticity Rules), 학습된 기존 신경망으로부터의 변환(Conversion), 진화적 최적화(Evolutionary Optimization), 시간 및 이벤트 기반 계산을 위해 특별히 설계된 다양한 방법을 사용합니다.

스파이크 타이밍 의존 가소성(Spike-Timing-Dependent Plasticity, STDP)은 생물학적으로 영감을 받은 국소 학습 규칙(Local Learning Rule)의 대표적인 예입니다. 단순화된 STDP 모델에서는 시냅스 전 스파이크(Presynaptic Spike)와 시냅스 후 스파이크(Postsynaptic Spike)의 상대적 발생 시점에 따라 시냅스 강도(Synaptic Strength)가 변화합니다. 이벤트 사이의 시간적 관계에 따라 연결이 강화되거나 약화될 수 있습니다. 이는 전역적으로 계산된 오류 신호(Global Error Signal) 대신 국소적으로 이용 가능한 타이밍 정보를 기반으로 학습이 이루어질 가능성을 보여줍니다.

그러나 STDP를 현대 심층학습 최적화(Deep-Learning Optimization)를 완전히 대체할 수 있는 방법으로 해석해서는 안 됩니다. 복잡한 과제에서는 대규모 네트워크, 긴 시간 구간, 여러 처리 단계에 걸쳐 신용 할당(Credit Assignment)을 수행할 수 있는 메커니즘이 필요합니다. 따라서 실용적인 SNN 연구에서는 하나의 생물학적 학습 규칙이 모든 최적화 문제를 해결한다고 가정하기보다 국소 가소성, 전역 목적함수(Global Objectives), 대리 경사 학습(Surrogate-Gradient Learning), 강화 신호(Reinforcement Signals), 아키텍처적 제약(Architectural Constraints)을 결합하는 방법을 탐구합니다.

인공 신경망에서 SNN으로의 변환(ANN-to-SNN Conversion)은 또 다른 실용적인 전략입니다. 먼저 기존 신경망을 성숙한 심층학습 방법으로 학습한 후 이를 스파이킹 표상(Spiking Representation)으로 변환할 수 있습니다. 활성화 크기(Activation Magnitudes)는 스파이크 발화율이나 시간 패턴을 통해 근사할 수 있습니다. 이러한 접근법은 유용하게 학습된 표상을 보존하면서 이벤트 기반 하드웨어에 배포할 수 있게 하지만, 변환 과정에서 지연시간(Latency), 정확도(Accuracy), 보정(Calibration) 사이의 절충이 발생할 수 있습니다.

직접 학습(Direct Training)은 시간적인 스파이크 구조를 활용할 수 있는 더 많은 가능성을 제공합니다. 스파이크를 단순히 기존 활성화의 대체 표현으로 취급하는 대신 직접 학습된 SNN은 이벤트 시퀀스(Event Sequences)와 내부 동역학으로부터 학습할 수 있습니다. 이는 입력 센서가 이미 비동기 이벤트(Asynchronous Events)를 생성하는 경우 특히 매력적이며, 시간 정보를 기존의 고정 프레임률 이미지(Fixed-Rate Image Frames)로 먼저 변환하지 않고 시스템 전체로 전달할 수 있습니다.

따라서 이벤트 카메라(Event Cameras)는 스파이킹 계산을 위한 자연스러운 감각 인터페이스(Sensory Interface)를 형성합니다. 이러한 센서는 완전한 프레임을 반복적으로 촬영하는 대신 국소적인 밝기 변화(Local Brightness Changes)를 비동기적으로 보고합니다. 그 결과 생성되는 이벤트 스트림(Event Stream)은 희소하면서 시간적으로 정밀합니다. SNN은 유사한 이벤트 기반 원리를 이용해 이러한 이벤트를 처리할 수 있으며, 감지(Sensing), 통신(Communication), 신경 계산(Neural Computation)이 모두 주로 환경 변화에 반응하는 지각 파이프라인을 구성할 가능성이 있습니다.

이러한 조합은 특히 로보틱스(Robotics)와 관련성이 높습니다. 빠른 움직임, 변화하는 조명, 충돌 회피(Collision Avoidance), 광학 흐름(Optical Flow), 추적(Tracking), 위치 추정(Localization), 제스처 인식(Gesture Recognition), 반응형 제어(Reactive Control)는 낮은 지연시간의 시간 정보로부터 이점을 얻을 수 있습니다. 이벤트 기반 센싱과 스파이킹 처리를 갖춘 로봇은 다음 기존 이미지 프레임을 기다리지 않고 중요한 변화에 반응할 수 있지만, 실제 성능은 알고리즘, 센서, 프로세서, 시스템 통합 품질에 크게 의존합니다.

뉴로모픽 프로세서(Neuromorphic Processors)는 스파이킹 및 이벤트 기반 계산의 특성을 활용하도록 설계된 하드웨어를 제공합니다. 모든 처리를 밀집된 동기식 행렬 연산(Dense Synchronous Matrix Operations)을 중심으로 구성하는 대신, 뉴로모픽 아키텍처(Neuromorphic Architectures)는 계산을 국소 상태(Local State) 가까이에 배치하고 이벤트를 통해 통신하며 필요한 경우에만 자원을 선택적으로 활성화할 수 있습니다. 이는 적절한 워크로드에서 메모리 트래픽(Memory Traffic)과 불필요한 활동을 줄일 수 있으며, 전력 제약이 있는 엣지 시스템(Edge Systems)에서 특히 중요합니다.

SNN과 뉴로모픽 하드웨어의 관계는 공동 설계(Co-Design)의 중요성을 보여줍니다. 밀집형 기존 신경망을 위해 최적화된 하드웨어에서 스파이킹 모델을 비효율적으로 실행하면 큰 이점을 얻지 못할 수 있습니다. 마찬가지로 특수화된 뉴로모픽 하드웨어만으로 효율적인 지능이 자동으로 만들어지는 것도 아닙니다. 신경 표상, 학습, 통신, 센서 인터페이스, 소프트웨어, 하드웨어가 서로 보완하도록 설계될 때 실질적인 장점이 나타납니다.

SNN은 전력과 지연시간 제약으로 인해 지속적인 고성능 계산이 제한되는 엣지 인공지능(Edge AI)에서 특히 흥미로운 가능성을 제공합니다. 모바일 로봇(Mobile Robots), 드론(Drones), 웨어러블 장치(Wearable Devices), 자율 센서(Autonomous Sensors), 임베디드 시스템(Embedded Systems)은 제한된 에너지 자원으로 장시간 작동해야 할 수 있습니다. 이벤트 기반 처리를 사용하면 일부 지각 및 모니터링 기능을 저전력으로 지속적으로 활성화하면서 계산 비용이 높은 시스템은 필요한 경우에만 작동시킬 수 있습니다.

이는 기존 심층학습을 완전히 대체하기보다 하이브리드 아키텍처(Hybrid Architecture)를 구성하는 방향을 제시합니다. 스파이킹 네트워크는 지속적인 저전력 모니터링(Continuous Low-Power Monitoring), 시간적 이벤트 검출(Temporal Event Detection), 빠른 반사적 처리(Reflex-Like Processing)를 담당하고, CNN, 트랜스포머(Transformers), 생성 모델(Generative Models), 파운데이션 모델(Foundation Models)은 더욱 풍부한 의미적 해석(Semantic Interpretation)과 계획(Planning)을 수행할 수 있습니다. 서로 다른 계산 메커니즘이 과제 복잡성과 사용 가능한 자원에 따라 서로 다른 시간 척도에서 작동할 수 있습니다.

이러한 계층 구조는 생물학적 지능(Biological Intelligence)의 중요한 원리와 유사합니다. 모든 감각 이벤트가 비용이 높은 전역 처리(Global Processing)를 요구하는 것은 아닙니다. 많은 신호는 국소적으로 필터링되거나 처리될 수 있으며, 비정상적이거나 불확실하거나 행동적으로 중요한 이벤트만 더 광범위한 처리 자원을 활성화합니다. 인공 에이전트(Artificial Agents) 역시 경량 이벤트 기반 모듈을 이용하여 변화를 감지하고 더 깊은 추론(Reasoning)이 필요한 경우에만 더 큰 모델을 선택적으로 호출할 수 있습니다.

SNN이 적응형 행동(Adaptive Behavior)에 사용될 때 시간적 신용 할당(Temporal Credit Assignment)은 여전히 중요한 과제로 남습니다. 행동은 긴 시간 동안 발생한 스파이크 패턴에 의존할 수 있지만 유용한 피드백은 훨씬 나중에 도착할 수 있습니다. 강화학습(Reinforcement Learning), 적격성 흔적(Eligibility Traces), 국소 시간 상태(Local Temporal States), 신경조절 학습 메커니즘(Neuromodulatory Learning Mechanisms)은 지연된 결과와 이전의 신경 활동을 연결하기 위한 가능한 접근법을 제공하지만, 확장 가능한 해결 방법은 여전히 활발한 연구 영역입니다.

SNN은 생물학적 유사성(Biological Similarity) 자체를 공학적 목표로 간주해서는 안 되는 이유도 보여줍니다. 모델이 스파이크를 발생시킨다는 이유만으로 더 지능적이 되는 것은 아닙니다. 생물학적 뇌는 스파이크뿐만 아니라 복잡한 수상돌기 계산(Dendritic Computation), 다양한 세포 유형(Cell Types), 순환 연결성(Recurrent Connectivity), 화학적 조절(Chemical Modulation), 구조적 가소성(Structural Plasticity), 발달(Development), 체화(Embodiment), 지속적인 환경 상호작용을 결합합니다. 인공 스파이킹 네트워크는 이러한 훨씬 풍부한 생물학적 시스템의 일부 추상화만을 포착합니다.

따라서 평가는 측정 가능한 시스템 수준의 이점(System-Level Benefits)에 초점을 맞추어야 합니다. 관련 지표에는 정확도, 응답 지연시간(Response Latency), 에너지 소비(Energy Consumption), 메모리 트래픽, 이벤트 희소성(Event Sparsity), 강건성(Robustness), 학습 효율성(Learning Efficiency), 하드웨어 활용률(Hardware Utilization), 시간적 불확실성(Temporal Uncertainty)에서의 성능이 포함됩니다. 스파이킹 솔루션은 내부 신호가 기존 활성화보다 생물학적으로 더 현실적으로 보이기 때문이 아니라 특정 응용 분야에서 이러한 특성을 실질적으로 개선할 때 가치가 있습니다.

피지컬 인공지능(Physical AI)에서 SNN은 특히 다중 시간 척도 지능(Multi-Timescale Intelligence)의 구성 요소로서 유망합니다. 빠른 이벤트 기반 회로(Event-Driven Circuits)는 즉각적인 감각 변화를 처리하고, 기존 지각 네트워크(Perception Networks)는 의미적 표상을 구성하며, 월드 모델(World Models)은 미래 상태를 예측하고, 상위 수준 에이전트는 계획과 추론을 수행할 수 있습니다. 모든 문제를 하나의 계산 주파수에서 동작하는 단일 신경 아키텍처로 처리하는 대신 이러한 계층들이 서로 협력할 수 있습니다.

따라서 스파이킹 신경망의 보다 광범위한 중요성은 계산이 언제 수행되어야 하는가를 다시 생각하게 한다는 데 있습니다. 기존 인공지능은 일반적으로 동기화된 계산(Synchronized Computation)을 지속적으로 수행하지만, 이벤트 기반 시스템은 정보의 변화에 따라 계산 자원을 할당할 수 있습니다. 지속적 처리(Continuous Processing)에서 활동 의존적 처리(Activity-Dependent Processing)로의 이러한 전환은 지능형 시스템이 데이터센터(Data Centers)를 벗어나 에너지와 실시간 동작의 제약을 받는 로봇 및 자율 기계(Autonomous Machines)로 확장됨에 따라 점점 더 중요해질 수 있습니다.

궁극적으로 스파이킹 신경망은 뇌를 문자 그대로 복제하지 않으면서 신경과학이 대안적인 계산 아키텍처(Alternative Computational Architectures)에 어떻게 영감을 줄 수 있는지를 보여줍니다. 스파이크는 인공 신경 계산에 명시적인 시간(Explicit Time), 희소 통신(Sparse Communication), 내부 동역학(Internal Dynamics), 이벤트 기반 처리를 도입합니다. 이러한 원리를 이벤트 센서(Event Sensors) 및 뉴로모픽 프로세서와 결합하면 물리적 세계에서 직접 동작하는 저전력(Low-Power), 고반응성(Responsive), 시간 인식 지능(Temporally Aware Intelligence)을 구축하기 위한 잠재적인 기반을 제공할 수 있습니다.

##  

## 12.06 Event Cameras and Robotics [w/Code]

![](images/image8.png){width="7.268055555555556in" height="7.268055555555556in"}

Event cameras provide a fundamentally different approach to visual sensing from conventional frame-based cameras. Instead of repeatedly capturing complete images at fixed intervals, they report local changes in brightness asynchronously as individual events. Each event typically indicates a pixel location, time, and polarity of intensity change, producing a sparse temporal stream that emphasizes what is changing rather than continuously recording what remains static.

This sensing principle is strongly inspired by biological vision, where retinal and neural circuits respond selectively to changes, contrasts, motion, and temporally significant signals. Biological visual systems do not transmit every element of a visual scene with equal priority at every moment. Event cameras apply a related engineering principle by reducing redundant information and allocating sensing bandwidth primarily to changes occurring within the environment.

A conventional camera samples the entire image plane according to a predefined frame rate such as 30, 60, or 120 frames per second. Events occurring between frames are not directly represented, and very rapid motion can produce blur or temporal ambiguity. Event cameras instead allow individual pixels to respond independently, creating measurements with very fine temporal resolution when local visual intensity changes significantly.

An event can conceptually be represented by spatial coordinates, a timestamp, and a polarity indicating whether brightness increased or decreased. The resulting data are therefore not naturally organized as conventional rectangular images. Algorithms must process asynchronous spatiotemporal events directly or accumulate them into representations such as event frames, voxel grids, time surfaces, point-like structures, or learned feature representations.

This asynchronous structure creates an important connection with spiking neural networks and neuromorphic computing. Event cameras generate sparse signals only when visual changes occur, while spiking networks communicate through discrete events over time. Neuromorphic processors can similarly execute computation in an event-driven manner. Combining these components can create sensing-to-computation pipelines that avoid repeatedly converting sparse temporal information into dense synchronous representations.

Low latency is one of the most important advantages for robotics. A frame-based system may need to wait until the next image is captured and processed before reacting to an environmental change. An event sensor can report relevant changes as they occur. For rapidly moving robots, drones, manipulators, vehicles, or collision-avoidance systems, reducing sensing latency can significantly improve the speed of perception and control responses.

High temporal resolution is also valuable for motion estimation. Because event streams describe changes with precise timestamps, they can preserve information about fast motion that may be difficult to recover from conventional images. Optical flow, object tracking, visual odometry, rotational motion estimation, and high-speed navigation can potentially benefit from this temporal structure when suitable event-processing algorithms are available.

Motion blur represents another area where event cameras offer advantages. Conventional cameras integrate incoming light during an exposure interval, causing rapidly moving objects or cameras to produce blurred images. Event cameras respond to brightness changes rather than integrating complete frames over comparable exposure periods. They can therefore preserve useful motion-related information under conditions where frame-based imagery becomes severely degraded.

Dynamic range is particularly important for robots operating outside controlled indoor environments. A robot may simultaneously encounter bright sunlight, deep shadows, reflective surfaces, tunnels, windows, headlights, or rapidly changing illumination. Event cameras can provide high dynamic range and respond effectively across challenging lighting transitions, making them attractive for autonomous systems that must operate across diverse visual conditions.

However, event cameras do not simply replace conventional cameras. Static regions may generate few or no events even when their appearance contains important semantic information. Color, texture, object identity, written text, and slowly changing visual structures are often more naturally captured by frame-based cameras. Consequently, many robotic systems benefit from combining event sensing with conventional RGB or other complementary sensors.

Sensor fusion can exploit the strengths of each modality. RGB cameras provide dense appearance and semantic information, event cameras provide rapid temporal changes, depth sensors provide geometric structure, LiDAR measures spatial range, and IMUs provide high-frequency inertial motion. A robotic perception system can combine these signals to obtain a richer estimate of environmental state than any individual sensor can provide alone.

Visual-inertial estimation is a particularly natural application. An IMU measures angular velocity and acceleration at high frequency, while event cameras provide temporally precise visual changes associated with motion through the environment. Combining these measurements can improve estimates of camera motion, orientation, and trajectory, especially during rapid rotations or other conditions in which conventional visual features become difficult to track.

Event-based visual odometry and SLAM extend this principle toward spatial intelligence. A robot can use event streams to estimate its movement relative to surrounding structures while constructing or maintaining representations of the environment. Because events are generated according to visual change, these methods require algorithms specifically designed to exploit temporal geometry rather than simply applying conventional frame-based SLAM unchanged.

Event-based optical flow provides another important capability. The movement of edges and brightness structures generates characteristic patterns across space and time. Algorithms can infer local motion from these patterns and use it for obstacle avoidance, tracking, navigation, or control. The fine temporal structure of events can be especially valuable when the robot itself or objects in its environment move quickly.

For drones and other agile robots, this capability can directly support high-speed control. A rapidly moving platform has very little time between sensing a potential obstacle and executing an avoidance maneuver. Event-based perception can provide low-latency motion information that feeds reactive control loops, allowing fast local responses while slower perception and planning systems maintain higher-level understanding of the environment.

This suggests a multi-timescale architecture for Physical AI. Event cameras and lightweight event-processing networks can operate at very high frequency to detect motion and sudden environmental changes. Conventional neural perception can construct semantic scene representations, while world models predict future states and higher-level agents perform planning. Each computational layer can therefore operate at a timescale appropriate to its function.

Sparse event streams may also reduce data movement. Conventional high-resolution cameras continuously generate complete images even when most of the scene remains unchanged. Event cameras primarily transmit pixels that experience significant intensity changes. In suitable environments this can substantially reduce redundant visual information, although event rates can become very high when the camera or scene undergoes extensive motion or illumination changes.

Energy efficiency therefore depends strongly on operating conditions. Event-driven sensing does not guarantee low total power consumption if downstream algorithms convert every event stream into large dense tensors and process them using computationally expensive networks. The greatest efficiency gains are more likely when sensing, representation, algorithms, communication, and hardware preserve sparsity throughout the complete processing pipeline.

Neuromorphic processors offer one possible architecture for maintaining this sparsity. Events can trigger local computation only where and when activity occurs, reducing unnecessary operations and memory transfers. Spiking neural networks can further preserve explicit temporal information across processing stages. Event camera, SNN, and neuromorphic processor co-design therefore represents a promising path toward low-power perception for continuously operating autonomous machines.

Deep learning has also expanded event-based vision beyond purely handcrafted algorithms. Neural networks can learn representations from raw events, accumulated event tensors, voxel grids, time surfaces, or combinations of events and frames. Depending on the architecture, these representations can support recognition, detection, depth estimation, motion prediction, segmentation, localization, or control while exploiting varying amounts of the original temporal structure.

Transformers and other sequence-oriented models provide another possible approach because event data naturally form temporally ordered sequences. However, directly processing every event with a large model can become computationally expensive when event rates are high. Practical architectures may therefore require temporal aggregation, sparse attention, hierarchical representations, token selection, or hybrid processing to preserve useful temporal detail without excessive computation.

World models can extend event-based perception from detecting current changes toward predicting future changes. An embodied agent can use event history together with actions, inertial information, images, and geometric observations to estimate how the visual scene may evolve. Unexpected events can then indicate differences between predicted and observed dynamics, providing information for updating the internal representation of the environment.

This creates a conceptual connection with predictive processing. If a robot predicts that its own movement should generate a particular pattern of visual change, observed events can be compared with those expectations. Large discrepancies may indicate an unexpected obstacle, moving object, surface change, external disturbance, or incorrect state estimate. Event streams can therefore become efficient carriers of prediction-relevant information in continuously changing environments.

Active perception can further exploit this relationship. A robot may deliberately change its viewpoint or motion to generate informative events when uncertainty is high. Instead of passively receiving sensory input, the robot can act to reveal object boundaries, depth relationships, motion patterns, or navigational structure. Perception and action then become coupled through a closed loop in which movement actively improves the information available for inference.

Event cameras nevertheless introduce important challenges. Their output is less intuitive to inspect than ordinary images, specialized algorithms and datasets remain less mature than the conventional vision ecosystem, and sensor noise can generate unwanted events. Performance can also depend strongly on motion, contrast, illumination changes, threshold settings, calibration, and the methods used to synchronize event data with other sensors.

Evaluation must therefore consider the complete robotic system rather than isolated sensor specifications. Relevant measures include end-to-end latency, trajectory accuracy, detection performance, robustness to rapid motion and illumination, bandwidth, power consumption, computational cost, synchronization accuracy, and failure behavior. An event camera is useful when its temporal characteristics produce measurable improvements in the task performed by the robot.

For practical robotics, hybrid perception is likely to remain particularly important. Event cameras can serve as fast temporal sensors, while RGB cameras provide dense semantic appearance, LiDAR or depth cameras provide geometry, and IMUs capture rapid body motion. The perception system can selectively combine these modalities according to uncertainty, environmental conditions, task requirements, and available computational resources.

Event cameras ultimately illustrate a broader principle for intelligent machines: sensing does not always need to sample the entire world uniformly. By emphasizing change, timing, sparsity, and asynchronous operation, event-based vision shifts perception from continuous frame collection toward information-driven sensing. Combined with neuromorphic computation, predictive world models, and multi-timescale control, this approach can contribute to faster, more energy-efficient, and more responsive robotic intelligence.

이벤트 카메라(Event Cameras)는 기존의 프레임 기반 카메라(Frame-Based Cameras)와 근본적으로 다른 시각 감지(Visual Sensing) 방식을 제공합니다. 고정된 시간 간격으로 전체 이미지를 반복해서 촬영하는 대신, 개별 이벤트(Events)의 형태로 국소적인 밝기 변화를 비동기적으로 보고합니다. 각 이벤트는 일반적으로 픽셀 위치(Pixel Location), 시간(Time), 밝기 변화의 극성(Polarity)을 나타내며, 정적으로 유지되는 정보를 지속적으로 기록하기보다 변화하는 정보에 집중하는 희소 시간 스트림(Sparse Temporal Stream)을 생성합니다.

이러한 감지 원리는 망막 및 신경 회로가 변화, 대비(Contrast), 움직임(Motion), 시간적으로 중요한 신호에 선택적으로 반응하는 생물학적 시각(Biological Vision)에서 많은 영감을 받았습니다. 생물학적 시각 시스템은 모든 순간마다 시각 장면의 모든 요소를 동일한 우선순위로 전달하지 않습니다. 이벤트 카메라는 이와 관련된 공학적 원리를 적용하여 중복 정보(Redundant Information)를 줄이고 주로 환경에서 발생하는 변화에 감지 대역폭(Sensing Bandwidth)을 할당합니다.

기존 카메라(Conventional Camera)는 초당 30, 60, 120 프레임과 같이 미리 정의된 프레임률(Frame Rate)에 따라 전체 이미지 평면(Image Plane)을 샘플링합니다. 프레임 사이에서 발생한 이벤트는 직접적으로 표현되지 않으며 매우 빠른 움직임은 모션 블러(Motion Blur) 또는 시간적 모호성(Temporal Ambiguity)을 발생시킬 수 있습니다. 반면 이벤트 카메라는 개별 픽셀이 독립적으로 반응하도록 하여 국소적인 시각 강도(Local Visual Intensity)가 크게 변화할 때 매우 높은 시간 해상도(Temporal Resolution)의 측정값을 생성합니다.

하나의 이벤트는 개념적으로 공간 좌표(Spatial Coordinates), 타임스탬프(Timestamp), 밝기가 증가했는지 감소했는지를 나타내는 극성으로 표현할 수 있습니다. 따라서 생성되는 데이터는 기존의 직사각형 이미지 형태로 자연스럽게 구성되지 않습니다. 알고리즘은 비동기 시공간 이벤트(Asynchronous Spatiotemporal Events)를 직접 처리하거나 이벤트 프레임(Event Frames), 복셀 그리드(Voxel Grids), 시간 표면(Time Surfaces), 점 형태 구조(Point-Like Structures), 학습된 특징 표상(Learned Feature Representations)과 같은 형태로 누적하여 처리해야 합니다.

이러한 비동기 구조(Asynchronous Structure)는 스파이킹 신경망(Spiking Neural Networks) 및 뉴로모픽 컴퓨팅(Neuromorphic Computing)과 중요한 연결 관계를 형성합니다. 이벤트 카메라는 시각적 변화가 발생할 때만 희소 신호(Sparse Signals)를 생성하며, 스파이킹 네트워크는 시간에 따라 발생하는 이산 이벤트를 통해 통신합니다. 뉴로모픽 프로세서(Neuromorphic Processors) 역시 이벤트 기반 방식으로 계산을 수행할 수 있습니다. 이러한 구성 요소를 결합하면 희소한 시간 정보를 밀집된 동기식 표상(Dense Synchronous Representations)으로 반복적으로 변환할 필요가 없는 감지-계산 파이프라인(Sensing-to-Computation Pipeline)을 구성할 수 있습니다.

낮은 지연시간(Low Latency)은 로보틱스(Robotics)에서 가장 중요한 장점 가운데 하나입니다. 프레임 기반 시스템은 환경 변화에 반응하기 전에 다음 이미지가 촬영되고 처리될 때까지 기다려야 할 수 있습니다. 이벤트 센서(Event Sensor)는 관련 변화가 발생하는 즉시 이를 보고할 수 있습니다. 빠르게 움직이는 로봇, 드론(Drones), 매니퓰레이터(Manipulators), 차량(Vehicles), 충돌 회피 시스템(Collision-Avoidance Systems)에서는 감지 지연시간을 줄이는 것이 지각과 제어 응답 속도를 크게 향상시킬 수 있습니다.

높은 시간 해상도는 움직임 추정(Motion Estimation)에서도 유용합니다. 이벤트 스트림은 정밀한 타임스탬프를 통해 변화를 설명하므로 기존 이미지에서는 복원하기 어려운 빠른 움직임 정보를 보존할 수 있습니다. 적절한 이벤트 처리 알고리즘이 사용될 경우 광학 흐름(Optical Flow), 객체 추적(Object Tracking), 시각 주행 거리 추정(Visual Odometry), 회전 운동 추정(Rotational Motion Estimation), 고속 내비게이션(High-Speed Navigation)이 이러한 시간적 구조의 이점을 활용할 수 있습니다.

모션 블러는 이벤트 카메라가 장점을 제공하는 또 다른 영역입니다. 기존 카메라는 노출 시간(Exposure Interval) 동안 들어오는 빛을 통합하기 때문에 빠르게 움직이는 객체나 카메라에서는 흐릿한 이미지가 발생할 수 있습니다. 이벤트 카메라는 비슷한 노출 시간 동안 전체 프레임을 통합하는 대신 밝기 변화에 반응합니다. 따라서 프레임 기반 영상이 심각하게 저하되는 조건에서도 움직임과 관련된 유용한 정보를 보존할 수 있습니다.

동적 범위(Dynamic Range)는 통제된 실내 환경을 벗어나 작동하는 로봇에서 특히 중요합니다. 로봇은 밝은 햇빛, 짙은 그림자, 반사 표면(Reflective Surfaces), 터널, 창문, 전조등, 급격한 조명 변화 등을 동시에 경험할 수 있습니다. 이벤트 카메라는 높은 동적 범위(High Dynamic Range)를 제공하고 까다로운 조명 전환에서도 효과적으로 반응할 수 있기 때문에 다양한 시각 조건에서 작동해야 하는 자율 시스템(Autonomous Systems)에 매력적인 센서가 될 수 있습니다.

그러나 이벤트 카메라가 단순히 기존 카메라를 대체하는 것은 아닙니다. 정적인 영역은 외형적으로 중요한 의미 정보(Semantic Information)를 포함하더라도 이벤트를 거의 생성하지 않거나 전혀 생성하지 않을 수 있습니다. 색상(Color), 텍스처(Texture), 객체 정체성(Object Identity), 문자(Written Text), 느리게 변화하는 시각 구조는 프레임 기반 카메라로 더욱 자연스럽게 포착되는 경우가 많습니다. 따라서 많은 로봇 시스템은 이벤트 감지와 기존 RGB 또는 기타 보완 센서(Complementary Sensors)를 결합함으로써 이점을 얻을 수 있습니다.

센서 융합(Sensor Fusion)은 각 모달리티(Modality)의 장점을 활용할 수 있습니다. RGB 카메라는 밀집된 외형 및 의미 정보를 제공하고, 이벤트 카메라는 빠른 시간적 변화를 제공하며, 깊이 센서(Depth Sensors)는 기하학적 구조(Geometric Structure)를 제공하고, 라이다(LiDAR)는 공간 거리를 측정하며, 관성 측정 장치(Inertial Measurement Unit, IMU)는 고주파 관성 운동(High-Frequency Inertial Motion)을 제공합니다. 로봇 지각 시스템은 이러한 신호를 결합하여 단일 센서만으로 얻을 수 있는 것보다 더욱 풍부한 환경 상태(Environmental State)를 추정할 수 있습니다.

시각-관성 추정(Visual-Inertial Estimation)은 특히 자연스러운 응용 분야입니다. IMU는 높은 주파수로 각속도(Angular Velocity)와 가속도(Acceleration)를 측정하고, 이벤트 카메라는 환경을 이동하면서 발생하는 움직임과 관련된 시간적으로 정밀한 시각 변화를 제공합니다. 이러한 측정값을 결합하면 특히 빠른 회전이나 기존 시각 특징(Visual Features)을 추적하기 어려운 조건에서 카메라 움직임, 방향(Orientation), 궤적(Trajectory)의 추정 성능을 향상시킬 수 있습니다.

이벤트 기반 시각 주행 거리 추정(Event-Based Visual Odometry)과 동시적 위치추정 및 지도작성(Simultaneous Localization and Mapping, SLAM)은 이러한 원리를 공간 지능(Spatial Intelligence)으로 확장합니다. 로봇은 이벤트 스트림을 이용하여 주변 구조에 대한 자신의 움직임을 추정하면서 환경 표상을 구축하거나 유지할 수 있습니다. 이벤트는 시각적 변화에 따라 생성되기 때문에 이러한 방법에는 기존의 프레임 기반 SLAM을 그대로 적용하는 것이 아니라 시간적 기하학(Temporal Geometry)을 활용하도록 특별히 설계된 알고리즘이 필요합니다.

이벤트 기반 광학 흐름(Event-Based Optical Flow)은 또 다른 중요한 기능을 제공합니다. 가장자리와 밝기 구조의 움직임은 공간과 시간에 걸쳐 특징적인 패턴을 생성합니다. 알고리즘은 이러한 패턴으로부터 국소 움직임(Local Motion)을 추론하여 장애물 회피(Obstacle Avoidance), 추적, 내비게이션, 제어에 활용할 수 있습니다. 이벤트의 정밀한 시간 구조는 로봇 자체나 환경의 객체가 빠르게 움직일 때 특히 유용할 수 있습니다.

드론과 기타 민첩한 로봇(Agile Robots)의 경우 이러한 기능은 고속 제어(High-Speed Control)를 직접 지원할 수 있습니다. 빠르게 움직이는 플랫폼은 잠재적인 장애물을 감지한 순간부터 회피 동작을 수행할 때까지 사용할 수 있는 시간이 매우 짧습니다. 이벤트 기반 지각(Event-Based Perception)은 반응형 제어 루프(Reactive Control Loops)에 낮은 지연시간의 움직임 정보를 제공하여 빠른 국소 반응을 가능하게 하고, 상대적으로 느린 지각 및 계획 시스템은 환경에 대한 상위 수준의 이해를 유지할 수 있습니다.

이는 피지컬 인공지능(Physical AI)을 위한 다중 시간 척도 아키텍처(Multi-Timescale Architecture)를 제안합니다. 이벤트 카메라와 경량 이벤트 처리 네트워크(Lightweight Event-Processing Networks)는 매우 높은 주파수로 동작하면서 움직임과 갑작스러운 환경 변화를 감지할 수 있습니다. 기존 신경망 기반 지각은 의미론적 장면 표상(Semantic Scene Representations)을 구성하고, 월드 모델(World Models)은 미래 상태를 예측하며, 상위 수준 에이전트(Higher-Level Agents)는 계획을 수행할 수 있습니다. 따라서 각각의 계산 계층은 자신의 기능에 적합한 시간 척도로 작동할 수 있습니다.

희소 이벤트 스트림은 데이터 이동(Data Movement)도 줄일 수 있습니다. 기존 고해상도 카메라는 장면의 대부분이 변하지 않더라도 지속적으로 전체 이미지를 생성합니다. 이벤트 카메라는 주로 유의미한 밝기 변화를 경험한 픽셀만 전송합니다. 적절한 환경에서는 이러한 방식으로 중복 시각 정보를 크게 줄일 수 있지만, 카메라 또는 장면에서 광범위한 움직임이나 조명 변화가 발생하면 이벤트 발생률(Event Rate)이 매우 높아질 수도 있습니다.

따라서 에너지 효율성(Energy Efficiency)은 작동 조건에 크게 의존합니다. 다운스트림 알고리즘(Downstream Algorithms)이 모든 이벤트 스트림을 대규모 밀집 텐서(Dense Tensors)로 변환한 후 계산 비용이 높은 네트워크로 처리한다면 이벤트 기반 감지가 전체 전력 소비를 낮춘다고 보장할 수 없습니다. 가장 큰 효율성 향상은 감지, 표상, 알고리즘, 통신, 하드웨어가 전체 처리 파이프라인에서 희소성(Sparsity)을 유지할 때 나타날 가능성이 높습니다.

뉴로모픽 프로세서는 이러한 희소성을 유지하기 위한 하나의 가능한 아키텍처를 제공합니다. 이벤트는 활동이 발생하는 위치와 시점에서만 국소 계산(Local Computation)을 활성화하여 불필요한 연산과 메모리 전송(Memory Transfers)을 줄일 수 있습니다. 스파이킹 신경망은 처리 단계 전체에서 명시적인 시간 정보를 더욱 효과적으로 유지할 수 있습니다. 따라서 이벤트 카메라, SNN, 뉴로모픽 프로세서의 공동 설계(Co-Design)는 지속적으로 작동하는 자율 기계(Autonomous Machines)를 위한 저전력 지각(Low-Power Perception)의 유망한 경로를 제공합니다.

심층학습(Deep Learning)은 이벤트 기반 비전(Event-Based Vision)을 순수하게 수작업으로 설계된 알고리즘(Handcrafted Algorithms)의 범위를 넘어 확장시켰습니다. 신경망은 원시 이벤트(Raw Events), 누적 이벤트 텐서(Accumulated Event Tensors), 복셀 그리드, 시간 표면 또는 이벤트와 프레임의 조합으로부터 표상을 학습할 수 있습니다. 아키텍처에 따라 이러한 표상은 원래 시간 구조의 다양한 수준을 활용하면서 인식(Recognition), 검출(Detection), 깊이 추정(Depth Estimation), 움직임 예측(Motion Prediction), 분할(Segmentation), 위치 추정(Localization), 제어를 지원할 수 있습니다.

트랜스포머(Transformers)와 기타 시퀀스 지향 모델(Sequence-Oriented Models)은 이벤트 데이터가 본질적으로 시간 순서가 있는 시퀀스를 형성하기 때문에 또 다른 가능한 접근법을 제공합니다. 그러나 이벤트 발생률이 높을 때 대규모 모델로 모든 이벤트를 직접 처리하면 계산 비용이 지나치게 증가할 수 있습니다. 따라서 실용적인 아키텍처에서는 과도한 계산 없이 유용한 시간적 세부 정보를 유지하기 위해 시간적 집계(Temporal Aggregation), 희소 어텐션(Sparse Attention), 계층적 표상(Hierarchical Representations), 토큰 선택(Token Selection), 하이브리드 처리(Hybrid Processing)가 필요할 수 있습니다.

월드 모델은 이벤트 기반 지각을 현재의 변화를 감지하는 수준에서 미래 변화를 예측하는 수준으로 확장할 수 있습니다. 체화 에이전트(Embodied Agent)는 이벤트 이력(Event History)을 행동, 관성 정보(Inertial Information), 이미지, 기하학적 관측과 함께 사용하여 시각 장면이 어떻게 변화할지를 추정할 수 있습니다. 예상하지 못한 이벤트는 예측된 동역학(Predicted Dynamics)과 관측된 동역학 사이의 차이를 나타낼 수 있으며, 이를 통해 환경에 대한 내부 표상을 갱신하기 위한 정보를 제공할 수 있습니다.

이는 예측 처리(Predictive Processing)와 개념적인 연결 관계를 형성합니다. 로봇이 자신의 움직임으로 인해 특정한 시각 변화 패턴이 발생할 것이라고 예측한다면 관측된 이벤트를 이러한 기대와 비교할 수 있습니다. 큰 차이는 예상하지 못한 장애물, 움직이는 객체, 표면 변화(Surface Change), 외부 교란(External Disturbance), 잘못된 상태 추정(Incorrect State Estimate)을 나타낼 수 있습니다. 따라서 이벤트 스트림은 지속적으로 변화하는 환경에서 예측과 관련된 정보를 효율적으로 전달하는 수단이 될 수 있습니다.

능동 지각(Active Perception)은 이러한 관계를 더욱 적극적으로 활용할 수 있습니다. 로봇은 불확실성이 높은 경우 유용한 이벤트를 생성하기 위해 의도적으로 시점이나 움직임을 변화시킬 수 있습니다. 감각 입력을 수동적으로 받아들이는 대신 로봇은 객체 경계(Object Boundaries), 깊이 관계(Depth Relationships), 움직임 패턴(Motion Patterns), 내비게이션 구조(Navigational Structure)를 더욱 명확하게 드러내도록 행동할 수 있습니다. 이때 지각과 행동은 움직임이 추론에 사용할 수 있는 정보를 능동적으로 개선하는 폐쇄 루프(Closed Loop)를 형성합니다.

그러나 이벤트 카메라는 중요한 과제도 가지고 있습니다. 출력은 일반 이미지보다 직관적으로 확인하기 어렵고, 전문화된 알고리즘과 데이터셋 생태계는 기존 컴퓨터 비전(Conventional Vision)보다 아직 성숙도가 낮으며, 센서 잡음(Sensor Noise)은 불필요한 이벤트를 생성할 수 있습니다. 성능 역시 움직임, 대비, 조명 변화, 임계값 설정(Threshold Settings), 보정(Calibration), 다른 센서와의 이벤트 데이터 동기화(Synchronization) 방법에 크게 영향을 받을 수 있습니다.

따라서 평가는 개별 센서 사양(Isolated Sensor Specifications)이 아니라 전체 로봇 시스템(Complete Robotic System)을 고려해야 합니다. 관련 평가 지표에는 종단간 지연시간(End-to-End Latency), 궤적 정확도(Trajectory Accuracy), 검출 성능(Detection Performance), 빠른 움직임과 조명 변화에 대한 강건성(Robustness), 대역폭(Bandwidth), 전력 소비(Power Consumption), 계산 비용(Computational Cost), 동기화 정확도(Synchronization Accuracy), 실패 동작(Failure Behavior)이 포함됩니다. 이벤트 카메라는 시간적 특성이 로봇이 수행하는 과제에서 측정 가능한 성능 향상을 제공할 때 실질적인 가치를 가집니다.

실제 로보틱스에서는 하이브리드 지각(Hybrid Perception)이 특히 중요할 가능성이 높습니다. 이벤트 카메라는 빠른 시간 센서(Fast Temporal Sensors)의 역할을 수행하고, RGB 카메라는 밀집된 의미론적 외형 정보를 제공하며, 라이다 또는 깊이 카메라는 기하학 정보를 제공하고, IMU는 빠른 로봇 본체의 움직임을 포착할 수 있습니다. 지각 시스템은 불확실성, 환경 조건, 과제 요구사항, 사용 가능한 계산 자원에 따라 이러한 모달리티를 선택적으로 결합할 수 있습니다.

궁극적으로 이벤트 카메라는 지능형 기계(Intelligent Machines)를 위한 보다 광범위한 원리를 보여줍니다. 감지 시스템이 항상 전체 세계를 균일하게 샘플링해야 하는 것은 아닙니다. 이벤트 기반 비전은 변화(Change), 타이밍(Timing), 희소성(Sparsity), 비동기 동작(Asynchronous Operation)을 강조함으로써 지각을 지속적인 프레임 수집(Continuous Frame Collection)에서 정보 중심 감지(Information-Driven Sensing)로 전환합니다. 이를 뉴로모픽 컴퓨팅, 예측형 월드 모델(Predictive World Models), 다중 시간 척도 제어(Multi-Timescale Control)와 결합하면 더욱 빠르고, 에너지 효율적이며, 높은 반응성을 가진 로봇 지능(Robotic Intelligence)을 구현하는 데 기여할 수 있습니다.

##  

## 12.07 Neuromorphic Processors [w/Code]

![](images/image9.png){width="7.268055555555556in" height="7.268055555555556in"}

Neuromorphic processors are computing architectures designed around principles inspired by biological nervous systems rather than the conventional organization of general-purpose CPUs and GPUs. Their central goal is not to reproduce the brain literally, but to exploit properties such as event-driven computation, distributed local state, sparse communication, temporal processing, and computation close to memory. These characteristics make neuromorphic hardware particularly relevant to energy-constrained intelligent systems.

Conventional computing systems are largely based on the von Neumann architecture, in which processing and memory are functionally separated. Instructions and data must repeatedly move between memory and computational units. Modern accelerators reduce this bottleneck through caches, parallelism, high-bandwidth memory, and specialized matrix engines, but large neural networks can still require substantial energy and bandwidth simply to move parameters and intermediate representations.

Neuromorphic architectures approach this problem differently by distributing computation and state across many relatively small processing elements. Instead of continuously transferring large arrays between centralized memory and arithmetic units, local computational elements can maintain their own states and update them when relevant information arrives. This organization attempts to reduce expensive data movement while supporting highly parallel neural dynamics.

Event-driven computation is one of the defining principles of many neuromorphic processors. Conventional processors frequently execute operations according to synchronized clock cycles regardless of whether the represented information has changed significantly. In an event-driven architecture, computation can instead be triggered by activity. When no meaningful event occurs, parts of the system may remain inactive, potentially reducing unnecessary computation and energy consumption.

This principle naturally complements spiking neural networks. SNNs represent communication using discrete spikes occurring over time, and neuromorphic processors can route these events among artificial neurons or computational cores. A spike may identify its source and trigger updates only in connected destinations. Computation therefore becomes closely related to communication events rather than requiring every neuron to be evaluated continuously at every global timestep.

Local state is equally important. A spiking neuron may maintain variables representing membrane potential, thresholds, adaptation, synaptic traces, or other temporal properties. Neuromorphic hardware can store such state near the processing elements responsible for updating it. This reduces repeated movement of state information and allows large populations of artificial neurons to evolve concurrently according to local dynamics.

Sparse communication provides another potential efficiency advantage. Biological neural systems contain enormous numbers of possible connections, yet only a fraction of neurons may produce relevant events during a short interval. Neuromorphic systems can exploit similar activity sparsity by communicating primarily when events occur. The resulting efficiency depends strongly on network activity, connectivity, routing architecture, and the workload being executed.

Asynchronous operation can extend this principle further. Some neuromorphic architectures do not require every component to advance according to a single globally synchronized computation step. Different regions can respond when events arrive and operate according to local timing. This can make computation naturally compatible with irregular sensory streams and physical environments in which significant changes occur unpredictably rather than at fixed sampling intervals.

Event cameras illustrate an especially suitable input modality. These sensors report local brightness changes asynchronously instead of continuously transmitting complete image frames. Their sparse event streams can be passed to neuromorphic processors without necessarily converting them into dense images first. This creates the possibility of an end-to-end event-driven pipeline spanning sensing, communication, neural processing, and robotic response.

The combination of event cameras, spiking networks, and neuromorphic processors is therefore attractive for low-latency perception. A visual event can be detected by the sensor, transmitted through an event stream, processed by neural circuits, and converted into a control-relevant signal without waiting for an entire image frame. Such architectures may be useful for high-speed tracking, collision avoidance, motion estimation, and other rapidly changing robotic tasks.

Energy efficiency is another major motivation. Mobile robots, drones, autonomous sensors, wearable systems, and embedded intelligent devices operate under strict power budgets. Running large GPU workloads continuously can reduce operating time and increase thermal requirements. Neuromorphic processors may provide efficient always-on computation for selected workloads by activating computational resources primarily when informative events occur.

However, energy efficiency is not guaranteed simply because hardware is described as neuromorphic. If a workload produces dense activity, requires extensive communication, or repeatedly converts between event-based and conventional representations, much of the theoretical advantage can disappear. Evaluation must therefore measure complete system energy, latency, throughput, communication cost, and accuracy rather than relying only on architectural labels.

Memory organization is particularly important because data movement is often a major contributor to energy consumption in AI hardware. Neuromorphic designs may place synaptic parameters and neural states physically or logically close to computational elements. This near-memory or distributed-memory organization reduces the distance that frequently accessed information must travel and can support highly parallel updates across neural populations.

Some architectures also support learning directly on the processor. Local learning rules can modify synaptic parameters according to neural activity, timing relationships, reinforcement signals, or programmable update mechanisms. On-chip learning is potentially important for autonomous systems that must adapt after deployment because it can reduce dependence on external servers and allow learning to occur close to the sensory and behavioral context.

Spike-timing-dependent plasticity provides one example of a learning mechanism that maps naturally onto neuromorphic hardware. Synaptic updates can depend on temporal relationships between presynaptic and postsynaptic activity. More programmable architectures can implement additional learning rules, eligibility traces, reward-modulated adaptation, or approximations to gradient-based optimization, enabling researchers to explore different forms of local and continual learning.

Training remains one of the major challenges. Modern deep learning benefits from highly optimized GPU ecosystems built around differentiable tensor operations and backpropagation. Neuromorphic computation often involves discrete events, temporal states, and hardware-specific constraints that do not map as directly onto these methods. Surrogate-gradient training, ANN-to-SNN conversion, local learning, and hardware-aware optimization provide possible approaches, but the ecosystem remains less standardized.

Software maturity is consequently as important as hardware capability. Effective deployment requires programming models, compilers, simulators, debugging tools, profiling systems, neural-network libraries, and interfaces with conventional robotics software. Specialized hardware can remain difficult to use if developers cannot efficiently map models onto it or analyze performance. A mature neuromorphic ecosystem must therefore address the complete development workflow.

Hardware-software co-design becomes essential under these conditions. Neural models should exploit the processor\'s event routing, memory hierarchy, neuron dynamics, and sparsity mechanisms rather than merely reproduce conventional dense networks inefficiently. At the same time, hardware must provide sufficient programmability to support useful real-world algorithms. Performance emerges from alignment between models, representations, software, sensors, and physical hardware.

Neuromorphic processors should therefore not be viewed simply as replacements for GPUs. GPUs remain exceptionally effective for large-scale training, dense matrix computation, transformers, generative models, and foundation-model inference. Neuromorphic processors address a different region of the design space, particularly workloads involving sparse events, temporal dynamics, low-power continuous operation, and rapid local responses.

A hybrid architecture can exploit both approaches. A neuromorphic processor may continuously monitor event sensors and execute fast temporal perception using very little power, while a GPU or other AI accelerator performs semantic recognition, multimodal fusion, world-model prediction, and complex planning when required. The neuromorphic subsystem can effectively act as an always-on intelligent front end that determines when expensive computation should be activated.

This architecture is particularly relevant to Physical AI because robotic intelligence operates across multiple timescales. Reflex-like reactions may require millisecond-scale responses, perception and state estimation operate continuously, planning may occur at slower frequencies, and strategic reasoning may span seconds or longer. Using one computational architecture for every layer can be inefficient. Specialized processors can instead serve the timescale and computational pattern for which they are best suited.

For example, event-driven hardware could detect rapid approaching motion and initiate an immediate avoidance response while simultaneously informing a higher-level system. A conventional perception network could then identify the object, a world model could estimate future trajectories, and an agent could revise its plan. Fast local reaction and slower global reasoning can therefore cooperate instead of competing for the same computational pathway.

Robust autonomous operation also benefits from this separation. If communication with cloud or on-premise computing becomes unavailable, low-level perception and safety functions must continue operating locally. Neuromorphic processors can potentially support energy-efficient edge autonomy for continuous monitoring, anomaly detection, motion processing, and safety responses, while computationally intensive services remain optional higher-level resources.

Continual learning provides another long-term opportunity. A robot operating for months or years encounters changing environments, sensor characteristics, objects, users, and tasks. Local adaptive mechanisms could allow selected neural circuits to adjust without repeatedly retraining an entire foundation model. Neuromorphic hardware with programmable plasticity may therefore become useful for fast adaptation while more stable knowledge remains encoded in larger models.

Several limitations remain significant. Neuromorphic processors differ considerably in neuron models, precision, connectivity, learning capabilities, memory capacity, communication architecture, and programming interfaces. Algorithms optimized for one platform may not transfer directly to another. Benchmarking is also difficult because comparisons must account for accuracy, latency, energy, workload sparsity, hardware utilization, and differences in model representation.

The relationship with neuroscience must also be interpreted carefully. Biological brains achieve remarkable efficiency, but their capabilities arise from far more than spikes and distributed computation. Dendritic processing, diverse cell populations, recurrent circuits, neuromodulation, plasticity, development, embodiment, and continuous interaction all contribute. Neuromorphic processors abstract selected principles from biology rather than reproducing the complete computational organization of the brain.

The broader engineering lesson is that intelligence does not require every operation to occur continuously or centrally. Computation can be distributed across specialized components, activated according to events, and performed near the information that changes. This approach shifts AI hardware design from maximizing raw arithmetic throughput alone toward optimizing the relationship among information flow, temporal dynamics, memory movement, energy, and behavioral requirements.

For future robots, neuromorphic processors may therefore occupy an important layer between sensors and large AI models. Event cameras and other asynchronous sensors can provide sparse observations, neuromorphic circuits can perform rapid temporal processing, conventional accelerators can construct semantic and predictive representations, and foundation models can support higher-level reasoning. Together they form a heterogeneous architecture optimized across multiple computational scales.

Neuromorphic processing ultimately represents a transition from continuously calculating everything toward selectively computing what matters when it matters. Its strongest potential lies not in replacing conventional AI hardware, but in complementing it with sparse, event-driven, temporally aware computation. For Physical AI, this combination could enable autonomous machines that remain continuously perceptive and responsive while consuming far less energy than architectures that rely exclusively on dense computation.

뉴로모픽 프로세서(Neuromorphic Processors)는 범용 중앙처리장치(CPU)와 그래픽처리장치(GPU)의 기존 구성 방식보다는 생물학적 신경계(Biological Nervous Systems)에서 영감을 받은 원리를 중심으로 설계된 컴퓨팅 아키텍처(Computing Architectures)입니다. 핵심 목표는 뇌를 문자 그대로 재현하는 것이 아니라 이벤트 기반 계산(Event-Driven Computation), 분산된 국소 상태(Distributed Local State), 희소 통신(Sparse Communication), 시간적 처리(Temporal Processing), 메모리 인접 계산(Computation Close to Memory)과 같은 특성을 활용하는 것입니다. 이러한 특성으로 인해 뉴로모픽 하드웨어(Neuromorphic Hardware)는 에너지 제약이 있는 지능형 시스템에 특히 적합합니다.

기존 컴퓨팅 시스템(Conventional Computing Systems)은 주로 처리 장치와 메모리가 기능적으로 분리된 폰 노이만 아키텍처(Von Neumann Architecture)를 기반으로 합니다. 명령어와 데이터는 메모리와 계산 장치 사이를 반복적으로 이동해야 합니다. 현대 가속기(Modern Accelerators)는 캐시(Cache), 병렬 처리(Parallelism), 고대역폭 메모리(High-Bandwidth Memory), 특수 행렬 연산 엔진(Specialized Matrix Engines)을 통해 이러한 병목 현상을 완화하지만, 대규모 신경망은 파라미터와 중간 표상(Intermediate Representations)을 이동시키는 것만으로도 상당한 에너지와 대역폭을 요구할 수 있습니다.

뉴로모픽 아키텍처(Neuromorphic Architectures)는 계산과 상태를 상대적으로 작은 다수의 처리 요소(Processing Elements)에 분산시킴으로써 이 문제에 다르게 접근합니다. 중앙집중식 메모리와 산술 연산 장치 사이에서 대규모 배열을 지속적으로 전송하는 대신, 국소 계산 요소(Local Computational Elements)가 자체 상태를 유지하고 관련 정보가 도착할 때 이를 갱신할 수 있습니다. 이러한 구성은 비용이 높은 데이터 이동(Data Movement)을 줄이면서 고도의 병렬 신경 동역학(Parallel Neural Dynamics)을 지원하는 것을 목표로 합니다.

이벤트 기반 계산(Event-Driven Computation)은 많은 뉴로모픽 프로세서를 정의하는 핵심 원리 가운데 하나입니다. 기존 프로세서는 표현되는 정보가 크게 변화하지 않았더라도 동기화된 클록 주기(Synchronized Clock Cycles)에 따라 연산을 수행하는 경우가 많습니다. 이벤트 기반 아키텍처에서는 활동(Activity)이 발생할 때 계산을 활성화할 수 있습니다. 의미 있는 이벤트가 발생하지 않을 경우 시스템의 일부는 비활성 상태를 유지하여 불필요한 계산과 에너지 소비를 줄일 수 있습니다.

이러한 원리는 스파이킹 신경망(Spiking Neural Networks, SNNs)과 자연스럽게 결합됩니다. SNN은 시간에 따라 발생하는 이산적인 스파이크(Discrete Spikes)를 이용하여 정보를 전달하며, 뉴로모픽 프로세서는 이러한 이벤트를 인공 뉴런(Artificial Neurons)이나 계산 코어(Computational Cores) 사이에서 전달할 수 있습니다. 하나의 스파이크는 발생원을 식별하고 연결된 목적지에서만 갱신을 유발할 수 있습니다. 따라서 모든 뉴런을 모든 전역 시간 단계(Global Timestep)마다 지속적으로 평가하는 대신 계산이 통신 이벤트(Communication Events)와 밀접하게 연계됩니다.

국소 상태(Local State) 역시 중요합니다. 스파이킹 뉴런은 막전위(Membrane Potential), 임계값(Thresholds), 적응(Adaptation), 시냅스 흔적(Synaptic Traces), 기타 시간적 특성을 나타내는 변수를 유지할 수 있습니다. 뉴로모픽 하드웨어는 이러한 상태를 갱신하는 처리 요소 가까이에 해당 상태를 저장할 수 있습니다. 이를 통해 상태 정보의 반복적인 이동을 줄이고 대규모 인공 뉴런 집단이 국소적인 동역학에 따라 동시에 변화하도록 할 수 있습니다.

희소 통신(Sparse Communication)은 또 다른 잠재적인 효율성 이점을 제공합니다. 생물학적 신경계에는 매우 많은 잠재적 연결이 존재하지만 짧은 시간 동안 실제로 관련 이벤트를 생성하는 뉴런은 일부에 불과할 수 있습니다. 뉴로모픽 시스템은 이벤트가 발생할 때 주로 통신함으로써 이러한 활동 희소성(Activity Sparsity)을 활용할 수 있습니다. 결과적인 효율성은 네트워크 활동, 연결성(Connectivity), 라우팅 아키텍처(Routing Architecture), 실행되는 워크로드(Workload)에 크게 의존합니다.

비동기 동작(Asynchronous Operation)은 이러한 원리를 더욱 확장할 수 있습니다. 일부 뉴로모픽 아키텍처에서는 모든 구성 요소가 하나의 전역적으로 동기화된 계산 단계에 따라 진행될 필요가 없습니다. 서로 다른 영역은 이벤트가 도착할 때 반응하고 국소적인 타이밍(Local Timing)에 따라 동작할 수 있습니다. 이러한 방식은 중요한 변화가 고정된 샘플링 간격이 아니라 예측하기 어려운 시점에 발생하는 물리적 환경 및 불규칙한 감각 스트림(Irregular Sensory Streams)과 자연스럽게 호환됩니다.

이벤트 카메라(Event Cameras)는 특히 적합한 입력 모달리티(Input Modality)를 보여줍니다. 이러한 센서는 전체 이미지 프레임을 지속적으로 전송하는 대신 국소적인 밝기 변화를 비동기적으로 보고합니다. 희소한 이벤트 스트림(Sparse Event Streams)은 반드시 밀집 이미지(Dense Images)로 먼저 변환하지 않고 뉴로모픽 프로세서에 전달할 수 있습니다. 이를 통해 감지(Sensing), 통신, 신경 처리(Neural Processing), 로봇 반응(Robotic Response)에 이르는 종단간 이벤트 기반 파이프라인(End-to-End Event-Driven Pipeline)을 구성할 수 있습니다.

따라서 이벤트 카메라, 스파이킹 네트워크, 뉴로모픽 프로세서의 결합은 저지연 지각(Low-Latency Perception)에 매력적입니다. 시각 이벤트는 센서에서 감지되고 이벤트 스트림을 통해 전달된 뒤 신경 회로(Neural Circuits)에서 처리되어 전체 이미지 프레임을 기다리지 않고 제어에 필요한 신호로 변환될 수 있습니다. 이러한 아키텍처는 고속 추적(High-Speed Tracking), 충돌 회피(Collision Avoidance), 움직임 추정(Motion Estimation), 기타 빠르게 변화하는 로봇 과제에 유용할 수 있습니다.

에너지 효율성(Energy Efficiency)은 또 다른 주요 동기입니다. 모바일 로봇(Mobile Robots), 드론(Drones), 자율 센서(Autonomous Sensors), 웨어러블 시스템(Wearable Systems), 임베디드 지능형 장치(Embedded Intelligent Devices)는 엄격한 전력 예산(Power Budgets) 아래에서 작동합니다. 대규모 GPU 워크로드를 지속적으로 실행하면 작동 시간이 감소하고 열 관리 요구사항이 증가할 수 있습니다. 뉴로모픽 프로세서는 정보 가치가 있는 이벤트가 발생할 때 주로 계산 자원을 활성화함으로써 일부 워크로드에서 효율적인 상시 동작 계산(Always-On Computation)을 제공할 수 있습니다.

그러나 하드웨어가 뉴로모픽이라고 불린다는 이유만으로 에너지 효율성이 보장되는 것은 아닙니다. 워크로드가 밀집된 활동(Dense Activity)을 생성하거나 광범위한 통신을 요구하거나 이벤트 기반 표상과 기존 표상 사이를 반복적으로 변환한다면 이론적인 장점의 상당 부분이 사라질 수 있습니다. 따라서 평가는 아키텍처 명칭에만 의존하기보다 전체 시스템 에너지(System Energy), 지연시간(Latency), 처리량(Throughput), 통신 비용(Communication Cost), 정확도(Accuracy)를 측정해야 합니다.

메모리 구성(Memory Organization)은 데이터 이동이 인공지능 하드웨어의 에너지 소비에서 중요한 부분을 차지하기 때문에 특히 중요합니다. 뉴로모픽 설계는 시냅스 파라미터(Synaptic Parameters)와 신경 상태(Neural States)를 계산 요소와 물리적 또는 논리적으로 가까운 위치에 배치할 수 있습니다. 이러한 메모리 인접(Near-Memory) 또는 분산 메모리(Distributed-Memory) 구성은 자주 사용되는 정보의 이동 거리를 줄이고 신경 집단 전체에서 고도로 병렬화된 갱신을 지원할 수 있습니다.

일부 아키텍처는 프로세서 자체에서 직접 학습(On-Chip Learning)을 수행하는 기능도 지원합니다. 국소 학습 규칙(Local Learning Rules)은 신경 활동, 시간적 관계(Timing Relationships), 강화 신호(Reinforcement Signals), 프로그래밍 가능한 갱신 메커니즘(Programmable Update Mechanisms)에 따라 시냅스 파라미터를 변경할 수 있습니다. 온칩 학습은 배포 이후에도 적응해야 하는 자율 시스템에서 특히 중요할 수 있으며, 외부 서버에 대한 의존도를 줄이고 감각 및 행동 맥락 가까이에서 학습할 수 있도록 합니다.

스파이크 타이밍 의존 가소성(Spike-Timing-Dependent Plasticity, STDP)은 뉴로모픽 하드웨어에 자연스럽게 대응되는 학습 메커니즘의 한 예입니다. 시냅스 갱신은 시냅스 전(Presynaptic) 활동과 시냅스 후(Postsynaptic) 활동 사이의 시간적 관계에 따라 이루어질 수 있습니다. 더욱 프로그래밍 가능한 아키텍처에서는 추가적인 학습 규칙, 적격성 흔적(Eligibility Traces), 보상 조절 적응(Reward-Modulated Adaptation), 경사 기반 최적화(Gradient-Based Optimization)의 근사 방법 등을 구현하여 다양한 형태의 국소 및 지속 학습(Continual Learning)을 연구할 수 있습니다.

학습(Training)은 여전히 주요 과제 가운데 하나입니다. 현대 심층학습(Deep Learning)은 미분 가능한 텐서 연산(Differentiable Tensor Operations)과 역전파(Backpropagation)를 중심으로 구축된 고도로 최적화된 GPU 생태계의 이점을 활용합니다. 뉴로모픽 계산은 이산 이벤트(Discrete Events), 시간적 상태(Temporal States), 하드웨어 특화 제약(Hardware-Specific Constraints)을 포함하는 경우가 많기 때문에 이러한 방법에 직접 대응하기 어렵습니다. 대리 경사 학습(Surrogate-Gradient Training), 인공 신경망에서 SNN으로의 변환(ANN-to-SNN Conversion), 국소 학습, 하드웨어 인식 최적화(Hardware-Aware Optimization)가 가능한 접근법을 제공하지만 생태계는 아직 상대적으로 표준화 수준이 낮습니다.

따라서 소프트웨어 성숙도(Software Maturity)는 하드웨어 성능만큼 중요합니다. 효과적인 배포에는 프로그래밍 모델(Programming Models), 컴파일러(Compilers), 시뮬레이터(Simulators), 디버깅 도구(Debugging Tools), 프로파일링 시스템(Profiling Systems), 신경망 라이브러리(Neural-Network Libraries), 기존 로보틱스 소프트웨어와의 인터페이스가 필요합니다. 개발자가 모델을 하드웨어에 효율적으로 매핑하거나 성능을 분석하기 어렵다면 특수 하드웨어의 활용도 역시 제한될 수 있습니다. 따라서 성숙한 뉴로모픽 생태계는 전체 개발 워크플로(Development Workflow)를 지원해야 합니다.

이러한 조건에서는 하드웨어-소프트웨어 공동 설계(Hardware-Software Co-Design)가 필수적입니다. 신경 모델은 기존의 밀집 신경망(Dense Networks)을 비효율적으로 재현하는 데 그치지 않고 프로세서의 이벤트 라우팅(Event Routing), 메모리 계층 구조(Memory Hierarchy), 뉴런 동역학(Neuron Dynamics), 희소성 메커니즘(Sparsity Mechanisms)을 활용해야 합니다. 동시에 하드웨어는 실제 환경에서 유용한 알고리즘을 지원할 수 있을 정도의 프로그래밍 가능성(Programmability)을 제공해야 합니다. 성능은 모델, 표상, 소프트웨어, 센서, 물리적 하드웨어 사이의 정렬(Alignment)을 통해 만들어집니다.

따라서 뉴로모픽 프로세서를 단순히 GPU를 대체하는 기술로 보아서는 안 됩니다. GPU는 대규모 학습(Large-Scale Training), 밀집 행렬 계산(Dense Matrix Computation), 트랜스포머(Transformers), 생성 모델(Generative Models), 파운데이션 모델 추론(Foundation-Model Inference)에 매우 효과적입니다. 뉴로모픽 프로세서는 희소 이벤트, 시간적 동역학, 저전력 연속 동작(Low-Power Continuous Operation), 빠른 국소 반응(Rapid Local Responses)을 포함하는 워크로드와 같이 설계 공간(Design Space)의 다른 영역을 대상으로 합니다.

하이브리드 아키텍처(Hybrid Architecture)는 두 접근법의 장점을 모두 활용할 수 있습니다. 뉴로모픽 프로세서는 매우 낮은 전력으로 이벤트 센서를 지속적으로 모니터링하고 빠른 시간적 지각(Temporal Perception)을 수행하는 반면, GPU 또는 다른 인공지능 가속기(AI Accelerator)는 필요한 경우 의미론적 인식(Semantic Recognition), 멀티모달 융합(Multimodal Fusion), 월드 모델 예측(World-Model Prediction), 복잡한 계획(Complex Planning)을 수행할 수 있습니다. 뉴로모픽 서브시스템은 비용이 높은 계산을 언제 활성화해야 하는지를 결정하는 상시 동작 지능형 프런트엔드(Always-On Intelligent Front End)의 역할을 수행할 수 있습니다.

이러한 아키텍처는 로봇 지능이 여러 시간 척도(Multiple Timescales)에서 작동한다는 점에서 피지컬 인공지능(Physical AI)과 특히 관련성이 높습니다. 반사적 반응(Reflex-Like Reactions)은 밀리초 단위의 응답을 요구할 수 있고, 지각과 상태 추정(State Estimation)은 지속적으로 동작하며, 계획은 더 낮은 주파수에서 수행될 수 있고, 전략적 추론(Strategic Reasoning)은 수초 이상의 시간을 다룰 수 있습니다. 모든 계층에 하나의 계산 아키텍처를 사용하는 것은 비효율적일 수 있으므로 특수 프로세서가 각 시간 척도와 계산 패턴에 가장 적합한 역할을 담당할 수 있습니다.

예를 들어 이벤트 기반 하드웨어(Event-Driven Hardware)는 빠르게 접근하는 물체의 움직임을 감지하여 즉각적인 회피 반응(Avoidance Response)을 시작하면서 동시에 상위 수준 시스템에 정보를 전달할 수 있습니다. 이후 기존 지각 네트워크(Conventional Perception Network)가 객체를 식별하고, 월드 모델이 미래 궤적(Future Trajectories)을 추정하며, 에이전트(Agent)가 계획을 수정할 수 있습니다. 따라서 빠른 국소 반응(Fast Local Reaction)과 느린 전역 추론(Slower Global Reasoning)은 동일한 계산 경로를 두고 경쟁하는 대신 서로 협력할 수 있습니다.

강건한 자율 동작(Robust Autonomous Operation) 역시 이러한 분리 구조의 이점을 얻을 수 있습니다. 클라우드(Cloud) 또는 온프레미스 컴퓨팅(On-Premise Computing)과의 통신이 불가능해지더라도 저수준 지각 및 안전 기능(Low-Level Perception and Safety Functions)은 로컬에서 계속 작동해야 합니다. 뉴로모픽 프로세서는 지속적인 모니터링, 이상 감지(Anomaly Detection), 움직임 처리(Motion Processing), 안전 대응(Safety Responses)을 위한 에너지 효율적인 엣지 자율성(Edge Autonomy)을 지원할 수 있으며, 계산 집약적인 서비스는 선택적인 상위 수준 자원으로 활용할 수 있습니다.

지속 학습(Continual Learning)은 또 다른 장기적인 가능성을 제공합니다. 수개월 또는 수년 동안 작동하는 로봇은 변화하는 환경, 센서 특성, 객체, 사용자, 과제를 지속적으로 경험합니다. 국소 적응 메커니즘(Local Adaptive Mechanisms)은 전체 파운데이션 모델을 반복적으로 재학습하지 않고도 일부 신경 회로를 조정할 수 있도록 합니다. 따라서 프로그래밍 가능한 가소성(Programmable Plasticity)을 지원하는 뉴로모픽 하드웨어는 빠른 적응에 활용되고, 보다 안정적인 지식은 대규모 모델에 유지되는 구조가 가능할 수 있습니다.

여러 중요한 한계도 여전히 존재합니다. 뉴로모픽 프로세서는 뉴런 모델(Neuron Models), 정밀도(Precision), 연결성, 학습 기능, 메모리 용량(Memory Capacity), 통신 아키텍처, 프로그래밍 인터페이스에서 상당한 차이를 보입니다. 한 플랫폼에 최적화된 알고리즘이 다른 플랫폼으로 직접 이전되지 않을 수도 있습니다. 벤치마킹(Benchmarking) 역시 정확도, 지연시간, 에너지, 워크로드 희소성(Workload Sparsity), 하드웨어 활용률(Hardware Utilization), 모델 표상의 차이를 함께 고려해야 하므로 어렵습니다.

신경과학(Neuroscience)과의 관계 역시 신중하게 해석해야 합니다. 생물학적 뇌는 놀라운 효율성을 달성하지만 그 능력이 단순히 스파이크와 분산 계산에서만 발생하는 것은 아닙니다. 수상돌기 처리(Dendritic Processing), 다양한 세포 집단(Cell Populations), 순환 신경 회로(Recurrent Circuits), 신경조절(Neuromodulation), 가소성(Plasticity), 발달(Development), 체화(Embodiment), 지속적인 환경 상호작용이 모두 기여합니다. 뉴로모픽 프로세서는 뇌의 전체 계산 구조를 재현하는 것이 아니라 생물학에서 선택된 일부 원리를 추상화합니다.

보다 광범위한 공학적 교훈은 지능(Intelligence)을 구현하기 위해 모든 연산이 지속적으로 또는 중앙집중적으로 수행될 필요가 없다는 것입니다. 계산은 특수화된 구성 요소에 분산되고, 이벤트에 따라 활성화되며, 변화하는 정보와 가까운 위치에서 수행될 수 있습니다. 이러한 접근법은 인공지능 하드웨어 설계의 초점을 단순히 최대 산술 처리량(Raw Arithmetic Throughput)을 높이는 것에서 정보 흐름(Information Flow), 시간적 동역학, 메모리 이동(Memory Movement), 에너지, 행동 요구사항(Behavioral Requirements) 사이의 관계를 최적화하는 방향으로 전환합니다.

미래의 로봇에서 뉴로모픽 프로세서는 센서와 대규모 인공지능 모델(Large AI Models) 사이의 중요한 계층을 담당할 수 있습니다. 이벤트 카메라와 기타 비동기 센서(Asynchronous Sensors)는 희소한 관측을 제공하고, 뉴로모픽 회로(Neuromorphic Circuits)는 빠른 시간적 처리를 수행하며, 기존 가속기(Conventional Accelerators)는 의미론적 및 예측적 표상(Semantic and Predictive Representations)을 구성하고, 파운데이션 모델(Foundation Models)은 상위 수준 추론을 지원할 수 있습니다. 이들을 결합하면 여러 계산 규모(Computational Scales)에 걸쳐 최적화된 이기종 아키텍처(Heterogeneous Architecture)를 구성할 수 있습니다.

궁극적으로 뉴로모픽 처리(Neuromorphic Processing)는 모든 것을 지속적으로 계산하는 방식에서 중요한 것을 필요한 순간에 선택적으로 계산하는 방식으로의 전환을 나타냅니다. 가장 큰 잠재력은 기존 인공지능 하드웨어를 대체하는 데 있는 것이 아니라 희소하고 이벤트 기반이며 시간 인식적인 계산(Sparse, Event-Driven, Temporally Aware Computation)을 통해 기존 하드웨어를 보완하는 데 있습니다. 피지컬 인공지능에서는 이러한 결합을 통해 밀집 계산(Dense Computation)에만 의존하는 아키텍처보다 훨씬 적은 에너지를 사용하면서도 지속적으로 주변을 인지하고 빠르게 반응할 수 있는 자율 기계(Autonomous Machines)를 구현할 가능성이 있습니다.
