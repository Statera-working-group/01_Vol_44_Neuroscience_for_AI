**Volume 44 Neuroscience for AI**

# Chapter 04. Predictive Coding

## 04.00 Predictive Coding Overview

![](images/image1.png){width="7.268055555555556in" height="7.268055555555556in"}

예측 부호화(Predictive Coding)는 뇌가 들어오는 감각 정보(Sensory Information)에 대한 예측을 지속적으로 생성하고, 실제 입력이 기대와 다를 때 그 예측을 갱신한다고 제안하는 이론적 프레임워크(Theoretical Framework)입니다. 지각(Perception)을 외부 신호의 순수한 순방향 변환(Feedforward Transformation)으로 처리하는 대신, 뇌는 내부 모델(Internal Models)이 감각적 원인(Sensory Causes)을 예상하고 예측 오차(Prediction Errors)가 학습, 지각, 적응(Adaptation)을 이끄는 능동적 추론 시스템(Active Inference System)으로 이해됩니다.

핵심적인 개념은 신경 계층(Neural Hierarchy)의 상위 수준이 하위 수준의 활동에 대한 기대(Expectations)를 생성한다는 것입니다. 이러한 하향식 예측(Top-Down Predictions)은 들어오는 상향식 신호(Bottom-Up Signals)와 비교되며, 두 신호 사이의 차이가 예측 오차(Prediction Error)를 형성합니다. 예측이 정확하면 수정이 거의 필요하지 않습니다. 반대로 불일치(Mismatch)가 크면 미래의 예측이 관찰된 감각 증거(Sensory Evidence)와 더욱 일치하도록 신경 활동이 조정됩니다.

이러한 아키텍처는 예측(Prediction)과 수정(Correction) 사이에 지속적인 루프를 형성합니다. 상위 피질 영역(Higher Cortical Regions)은 환경에 무엇이 존재할 가능성이 높은지에 대한 해석을 제안하고, 하위 영역은 실제로 감지되고 있는 것에 관한 정보를 제공합니다. 예측 오차는 계층 구조를 통해 전달되면서 내부 표현(Internal Representations)을 수정합니다. 따라서 지각은 감각 데이터를 수동적으로 받아들이는 과정이 아니라 기대와 들어오는 증거 사이의 반복적인 상호작용으로부터 형성됩니다.

예측 부호화(Predictive Coding)는 감각 정보가 여러 추상화 수준(Levels of Abstraction)의 구조를 포함하기 때문에 계층적으로 이해할 수 있습니다. 하위 수준은 가장자리(Edges), 주파수(Frequencies), 움직임(Motion)과 같은 국소적 특징을 표현할 수 있는 반면, 상위 수준은 객체(Objects), 장면(Scenes), 맥락(Contexts), 의도(Intentions), 더욱 추상적인 관계를 표현할 수 있습니다. 상위 수준에서 생성된 예측은 하위 수준의 해석을 제약하며, 해결되지 않은 오차는 상위 수준이 내부 모델을 수정해야 한다는 정보를 제공합니다.

이러한 계층적 조직(Hierarchical Organization)의 유용한 결과 가운데 하나는 뇌가 모든 세부 정보를 동일한 수준으로 전달할 필요가 없다는 것입니다. 이미 잘 예측되는 정보는 효율적으로 표현될 수 있는 반면, 예상하지 못한 구성 요소는 더욱 강조됩니다. 이러한 의미에서 예측 오차는 정보성이 높은 잔차 신호(Informative Residual Signal)의 형태로 기능합니다. 신경 처리는 변화하지 않거나 예상 가능한 모든 정보를 반복적으로 부호화하기보다 기대에서 벗어나는 정보에 자원을 집중할 수 있습니다.

예측 부호화는 내부 모델(Internal Models)의 개념과 밀접하게 연결됩니다. 내부 모델은 세계의 원인(Causes)이 어떻게 감각적 결과(Sensory Consequences)를 만들어내는지에 관한 규칙성을 표현합니다. 반복적인 경험을 통해 뇌는 특정 객체가 특징적인 시각 패턴을 생성하고, 특정 행동이 예상되는 움직임을 만들어내며, 특정 사건이 다른 사건에 이어 발생하는 경향이 있다는 것을 학습할 수 있습니다. 이러한 모델을 통해 완전한 감각 증거가 제공되기 전에도 기대를 기반으로 지각과 행동을 안내할 수 있습니다.

학습(Learning)은 예측 오차가 지속될 때 발생합니다. 뇌가 특정 사건을 반복적으로 잘못 예측한다면 해당 예측을 생성하는 내부 모델을 수정해야 합니다. 시냅스 가소성(Synaptic Plasticity)은 기대를 생성하는 표현과 연결을 점진적으로 변화시켜 시간이 지남에 따라 예측 정확도를 향상시킬 수 있습니다. 따라서 예측 부호화는 지각과 학습을 하나의 프레임워크 안에서 연결합니다. 예측은 해석을 지원하고, 오차는 적응을 지원합니다.

이러한 관점은 자기지도 학습(Self-Supervised Learning)과도 자연스럽게 연결됩니다. 환경은 모든 감각 사건에 대해 명시적인 레이블(Explicit Labels)을 제공할 필요가 없습니다. 미래의 입력(Future Input), 누락된 정보(Missing Information), 또는 감각 양식 사이의 관계(Relationships Between Modalities)가 학습 목표로 사용될 수 있기 때문입니다. 뇌는 자신이 예상했던 것과 실제로 관찰한 것을 비교할 수 있습니다. 따라서 예측 자체가 지도 신호(Supervisory Signal)를 생성하며, 지속적인 경험으로부터 구조화된 지식(Structured Knowledge)이 형성될 수 있도록 합니다.

시간적 예측(Temporal Prediction)은 생물학적 개체가 변화하는 환경에서 작동하기 때문에 특히 중요합니다. 감각 사건은 시퀀스(Sequences)로 전개되며 행동의 결과는 일정 시간이 지난 후에 나타날 수 있습니다. 예측 시스템은 이전 관찰과 현재 맥락을 기반으로 다음에 발생할 가능성이 높은 사건을 추정할 수 있습니다. 미래가 기대와 다르게 전개되면 예측 오차는 내부 모델이 불완전하거나 오래되었거나 부정확한 부분을 보여줍니다.

예측 부호화는 감각 적응(Sensory Adaptation)의 일부 측면도 설명할 수 있습니다. 반복되거나 예측 가능성이 높은 자극은 기존 기대에 의해 점점 더 잘 설명되기 때문에 점진적으로 작은 반응을 생성할 수 있습니다. 반대로 새롭거나 예상하지 못한 사건은 더 큰 예측 오차를 생성하므로 강한 신경 반응을 유발할 수 있습니다. 이러한 관계는 예측 처리(Predictive Processing)를 새로움 탐지(Novelty Detection), 주의(Attention), 학습 우선순위(Learning Priority), 신경 자원의 적응적 할당(Adaptive Allocation)과 연결합니다.

주의(Attention)는 서로 다른 신호에 부여되는 상대적 중요성을 변화시킴으로써 예측 부호화에 영향을 줄 수 있습니다. 감각 정보는 신뢰성과 행동적 관련성(Behavioral Relevance)이 서로 다르기 때문에 모든 예측 오차를 동일하게 처리해서는 안 됩니다. 뇌는 주의를 기울이고 있거나 정밀하며 중요한 정보와 관련된 오차를 증폭시키는 동시에 잡음이 많거나 관련성이 낮은 신호의 영향은 감소시킬 수 있습니다. 이는 예측 처리에 정밀도 가중(Precision Weighting)이라는 개념을 도입합니다.

정밀도(Precision)는 신호의 추정된 신뢰성(Reliability) 또는 확신도(Confidence)를 의미합니다. 매우 신뢰할 수 있는 감각 정보에서 발생한 예측 오차는 불확실하거나 잡음이 많은 입력에서 발생한 오차보다 믿음 갱신(Belief Updating)에 더 강한 영향을 미쳐야 합니다. 마찬가지로 감각 정보가 모호한 경우에는 강한 사전 기대(Prior Expectations)가 더 큰 영향을 미칠 수 있습니다. 따라서 지각은 사전 예측(Prior Predictions)과 감각 증거 사이의 균형으로 이해할 수 있으며, 각각은 추정된 신뢰도에 따라 가중됩니다.

이러한 균형은 지각이 맥락 의존적(Context Dependent)인 이유를 설명하는 데 도움을 줍니다. 동일한 감각 입력이라도 사전 지식(Prior Knowledge), 주변 정보(Surrounding Information), 현재 목표(Current Goals), 기대에 따라 다르게 해석될 수 있습니다. 하향식 예측은 모호한 데이터에 대해 가능한 해석을 제약하는 반면, 상향식 오차(Bottom-Up Errors)는 기대가 현실과 완전히 분리되는 것을 방지합니다. 정확한 지각을 위해서는 유용한 사전 구조와 모순되는 증거에 대한 충분한 민감성이 모두 필요합니다.

예측 부호화는 운동 제어(Motor Control)와도 관련됩니다. 뇌가 운동 명령(Motor Command)을 생성하면 내부 모델은 해당 행동의 감각적 결과를 예측할 수 있습니다. 예상되는 시각(Visual), 고유수용감각(Proprioceptive), 촉각(Tactile) 피드백은 실제 피드백과 비교될 수 있습니다. 예측된 결과와 관찰된 결과 사이의 차이는 움직임을 수정하고 행동과 그 결과를 연결하는 내부 모델을 갱신하기 위한 정보를 제공합니다.

이는 예측 부호화와 능동적 지각(Active Perception) 사이에 강한 관계를 형성합니다. 생물은 감각 증거가 들어오기를 단순히 기다리지 않고 눈, 머리, 신체, 팔다리를 움직여 불확실성을 줄일 수 있는 정보를 능동적으로 획득할 수 있습니다. 행동은 뇌가 이용할 수 있는 감각 입력을 변화시키며, 새로운 관찰은 기존 예측을 검증합니다. 따라서 지각과 행동은 행동이 환경을 능동적으로 탐색하고 내부 모델을 개선하는 폐쇄 루프(Closed Loop)를 형성할 수 있습니다.

예측 부호화는 강화학습(Reinforcement Learning)과도 중요한 연관성을 가지지만, 두 개념을 동일한 것으로 간주해서는 안 됩니다. 감각 처리에서의 예측 오차는 예상한 입력과 관찰된 입력 사이의 불일치를 나타내는 반면, 보상 예측 오차(Reward Prediction Error)는 기대한 가치와 실제로 획득한 가치 사이의 차이를 나타냅니다. 두 방식 모두 오차 신호를 이용해 기대를 갱신하지만 서로 다른 대상을 다루며, 감각 예측이 행동 선택(Action Selection)과 결과에 영향을 줄 때 서로 상호작용할 수 있습니다.

해마(Hippocampus)와 피질(Cortex)은 예측 처리에 상호보완적인 정보를 제공할 수 있습니다. 피질 시스템(Cortical Systems)은 안정적인 기대를 지원하는 규칙성을 점진적으로 학습하는 반면, 해마 시스템(Hippocampal Systems)은 특정한 일화(Episodes)와 맥락적 관계(Contextual Relationships)를 빠르게 부호화할 수 있습니다. 따라서 저장된 경험은 익숙하거나 부분적으로 익숙한 상황에서 뇌가 무엇을 예측할지에 영향을 줄 수 있으며, 예상하지 못한 관찰은 일화적 지식과 일반화된 지식 모두의 갱신을 유도할 수 있습니다.

인공지능(Artificial Intelligence)의 관점에서 예측 부호화는 레이블이 없는 경험(Unlabeled Experience)으로부터 표현(Representations)을 학습하기 위한 생물학적 영감을 받은 프레임워크를 제공합니다. 인공 시스템은 미래의 관찰을 예측하고, 누락된 입력을 복원하며, 잠재적 원인(Latent Causes)을 추정하거나 생성된 예측과 실제 데이터 사이의 차이를 최소화하도록 학습될 수 있습니다. 이러한 원리는 자기지도 학습(Self-Supervised Learning), 월드 모델(World Models), 생성 모델링(Generative Modeling), 표현 학습(Representation Learning)과 관련됩니다.

예측 부호화는 일반적인 역전파(Backpropagation)와도 중요한 차이를 가집니다. 역전파는 일반적으로 미리 정의된 계산 그래프(Computational Graph)를 통해 명시적인 전역 손실(Global Loss)의 그래디언트(Gradients)를 계산하는 반면, 예측 부호화는 상호작용하는 계층적 표현 사이에서 교환되는 국소 예측 오차(Local Prediction Errors)를 강조합니다. 일부 이론적 모델은 이러한 국소 오차 역학(Local Error Dynamics)이 그래디언트 기반 학습의 일부 형태를 근사할 수 있는지 연구하지만, 생물학적 예측 부호화를 표준 역전파와 동일한 것으로 간주해서는 안 됩니다.

체화 인공지능(Embodied AI)과 피지컬 AI(Physical AI)에서 예측 부호화는 지능형 에이전트(Intelligent Agents)가 지각과 행동의 결과를 지속적으로 예상해야 하기 때문에 특히 중요합니다. 로봇(Robot)은 움직임 이후 환경이 어떻게 변화할지를 예측하고, 예측된 감각 상태(Predicted Sensory States)를 실제 관찰과 비교하며, 예상하지 못한 사건을 탐지하고, 내부 월드 모델을 갱신할 수 있습니다. 이러한 능력은 이상 탐지(Anomaly Detection), 적응형 제어(Adaptive Control), 계획(Planning), 동적 환경에서의 지속 학습(Continual Learning)을 지원합니다.

따라서 예측 부호화(Predictive Coding)는 지각(Perception), 학습(Learning), 기억(Memory), 주의(Attention), 행동(Action), 내부 모델(Internal Models)을 연결하는 통합된 관점을 제공합니다. 뇌는 사전 지식(Prior Knowledge)을 기반으로 기대를 생성하고, 이를 들어오는 증거와 비교하며, 발생한 오차에 신뢰도에 따른 가중치를 부여하고, 예측이 실패할 때 표현을 갱신합니다. 이러한 반복적인 순환을 통해 경험은 효율적인 지각, 미래 예측(Future Prediction), 적응적 행동(Adaptive Behavior)을 지원하는 더욱 구조화된 모델로 점진적으로 변환됩니다.

## 04.01 Brain as Prediction Machine [w/Code]

![](images/image2.png){width="7.268055555555556in" height="7.268055555555556in"}

뇌를 예측 기계(Brain as a Prediction Machine)로 보는 관점은 신경 시스템(Neural Systems)이 단순히 감각 정보(Sensory Information)가 들어오기를 기다렸다가 도착한 이후에 반응하는 것이 아니라고 제안합니다. 대신 뇌는 이전 경험(Prior Experience), 맥락(Context), 기억(Memory), 현재 목표(Current Goals)를 활용하여 다음에 발생할 가능성이 높은 것을 지속적으로 예상합니다. 들어오는 감각 신호는 이러한 기대(Expectations)를 기준으로 해석되며, 이를 통해 지각(Perception)과 행동(Action)은 단순히 반응적인 과정이 아니라 미래를 고려하는 선행적 과정(Prospective Processes)으로 작동할 수 있습니다.

예측(Prediction)이 유용한 이유는 물리적 세계(Physical World)에 규칙성(Regularities)이 존재하기 때문입니다. 객체(Objects)는 지속되는 경향이 있고, 움직임(Movements)은 일정한 궤적(Trajectories)을 따르며, 행동은 특징적인 결과를 만들어내고, 사건은 익숙한 순서로 전개되는 경우가 많습니다. 뇌는 이러한 패턴을 학습함으로써 완전한 증거가 제공되기 전에 미래 상태(Future States)를 추정할 수 있습니다. 이는 감각 정보가 지연되거나, 잡음이 많거나, 불완전하거나, 모호한 상황에서 생물학적 시스템에 중요한 이점을 제공합니다.

예측적 관점(Predictive View)은 전통적인 지각 해석을 변화시킵니다. 순수한 상향식 모델(Bottom-Up Model)에서는 감각 수용기(Sensory Receptors)가 신호를 제공하고, 이러한 신호가 점진적으로 더욱 복잡한 표현으로 변환됩니다. 예측 시스템에서는 상위 수준 표현(Higher-Level Representations)도 하위 영역이 어떤 정보를 받아야 하는지에 관한 가설(Hypotheses)을 생성합니다. 따라서 지각은 일방향적인 정보 흐름이 아니라 들어오는 감각 증거와 내부적으로 생성된 기대 사이의 상호작용으로부터 형성됩니다.

내부 모델(Internal Models)은 이러한 과정의 핵심입니다. 내부 모델은 환경에 존재하는 숨겨진 원인(Hidden Causes)과 그 원인이 만들어낼 것으로 예상되는 감각적 결과(Sensory Consequences) 사이의 관계를 포착합니다. 예를 들어 뇌는 객체가 서로 다른 시점(Viewpoints)에서 어떻게 보일지 또는 특정 움직임 이후 어떤 감각 피드백(Sensory Feedback)이 발생할지를 학습할 수 있습니다. 이렇게 학습된 관계를 통해 시스템은 불완전한 입력에도 원인을 추론하고, 결과를 예상하며, 안정적인 해석을 유지할 수 있습니다.

예측은 여러 추상화 수준(Levels of Abstraction)에서 발생합니다. 낮은 신경 수준(Lower Neural Levels)은 가장자리(Edges), 움직임(Motion), 주파수(Frequencies), 짧은 시간적 변화와 같은 국소 패턴(Local Patterns)을 예측할 수 있는 반면, 높은 수준에서는 객체, 장면(Scenes), 맥락, 의도(Intentions), 과제 상태(Task States)를 예측할 수 있습니다. 이러한 수준들은 계층적으로 상호작용하므로 추상적인 기대가 하위 수준의 해석을 제약하는 동시에 예상하지 못한 감각 증거가 상위 수준 표현을 변화시키도록 만들 수 있습니다.

예측의 중요한 장점 가운데 하나는 효율적인 정보 처리(Efficient Information Processing)입니다. 감각 사건이 뇌가 이미 예상한 것과 일치한다면 전체 신호를 새로운 정보로 처리할 필요성이 감소합니다. 대신 예측된 입력과 관찰된 입력 사이의 차이를 강조하여 처리할 수 있습니다. 이러한 관점에서 예상하지 못했거나 설명되지 않은 정보는 현재 내부 모델이 불완전하거나 부정확한 부분을 보여주기 때문에 특히 중요해집니다.

따라서 예측 오차(Prediction Errors)는 유용한 내부 모델을 유지하는 데 핵심적인 역할을 합니다. 기대와 관찰이 서로 다르면 그 불일치는 일부 표현을 수정해야 한다는 증거를 제공합니다. 작은 오차는 현재 모델이 입력을 적절하게 설명하고 있음을 나타낼 수 있는 반면, 지속적이거나 큰 오차는 학습(Learning)과 적응(Adaptation)을 유도할 수 있습니다. 따라서 뇌는 예측 실패(Prediction Failure)를 아직 무엇을 학습해야 하는지를 알려주는 지속적인 정보원으로 활용할 수 있습니다.

예측하는 뇌(Predictive Brain)는 외부 감각 입력만을 예상하는 것이 아닙니다. 내부 신체 상태(Internal Bodily States), 행동의 결과(Action Consequences), 환경의 전이(Environmental Transitions), 가능한 미래 결과(Future Outcomes)도 예측합니다. 운동 시스템(Motor Systems)은 신체가 어떻게 움직여야 하는지를 추정할 수 있고, 지각 시스템(Perceptual Systems)은 앞으로 발생할 감각 변화를 예상할 수 있으며, 인지 시스템(Cognitive Systems)은 의사결정의 가능한 결과를 추정할 수 있습니다. 따라서 예측은 지각, 행동, 고차 인지(Higher Cognition)를 연결하는 공통적인 계산 원리를 제공합니다.

운동 제어(Motor Control)는 이를 명확하게 보여주는 사례입니다. 행동이 생성되면 뇌는 실제 피드백이 완전히 도착하기 전에 예상되는 감각적 결과를 예측할 수 있습니다. 예측된 고유수용감각(Proprioceptive), 시각(Visual), 촉각(Tactile) 신호는 이후 실제 관찰과 비교될 수 있습니다. 움직임이 기대와 다르면 수정 과정(Corrective Processes)이 진행 중인 제어를 조정하고 미래 행동에 사용되는 모델을 갱신할 수 있습니다.

이러한 능력은 자기 생성 사건(Self-Generated Events)과 외부에서 생성된 사건(Externally Generated Events)을 구분하는 것도 지원합니다. 자신의 움직임으로 발생한 감각 변화는 운동 명령(Motor Commands)으로부터 예측할 수 있는 경우가 많지만, 예상하지 못한 변화는 외부 원인(External Cause)을 나타낼 수 있습니다. 따라서 예측 메커니즘은 감각 입력이 왜 변화했는지를 뇌가 해석하도록 도우며, 예상된 결과에 대한 반응은 줄이면서 현재 행동으로 설명할 수 없는 사건에 대한 민감성은 유지할 수 있습니다.

예측은 시간적 처리(Temporal Processing)와 깊이 연결되어 있습니다. 지능적 행동(Intelligent Behavior)은 다음에 무엇이 발생할지를 추정해야 하기 때문입니다. 신경 시스템은 여러 시간 척도(Timescales)에 걸쳐 상태(States), 사건(Events), 행동(Actions) 사이의 전이를 학습할 수 있습니다. 단기 예측(Short Predictions)은 즉각적인 움직임을 안내할 수 있고, 장기 예측(Longer Predictions)은 내비게이션(Navigation), 계획(Planning), 목표 지향적 행동(Goal-Directed Behavior)을 지원할 수 있습니다. 시간적 구조는 지각을 서로 분리된 관찰의 연속에서 지속적으로 변화하는 세계 모델(World Model)로 전환합니다.

기억(Memory)은 이러한 예측 능력에 필수적입니다. 예측은 이전 경험을 통해 학습한 규칙성을 기반으로 생성되므로, 기억은 미래 사건의 가능성을 추정하는 데 필요한 정보를 제공합니다. 피질 시스템(Cortical Systems)은 안정적인 통계적 규칙성(Statistical Regularities)을 부호화할 수 있으며, 해마 시스템(Hippocampal Systems)은 특정한 일화(Episodes)와 맥락적 관계(Contextual Relationships)를 제공할 수 있습니다. 이러한 기억 시스템들이 함께 작동함으로써 일반화된 지식과 특정한 과거 경험 모두가 현재의 기대를 형성할 수 있습니다.

맥락(Context)은 동일한 감각 신호가 서로 다른 상황에서 다른 의미를 가질 수 있기 때문에 예측에 강한 영향을 미칩니다. 소리(Sound), 움직임, 시각 패턴(Visual Pattern)은 익숙한 환경에서는 하나의 의미를 가질 수 있지만 낯선 환경에서는 다른 의미를 가질 수 있습니다. 맥락에 대한 상위 수준 표현(Higher-Level Representations)은 어떤 예측이 가능한지를 제약하여 가능한 해석의 범위를 좁히고, 들어오는 증거가 불완전한 경우에도 뇌가 빠르게 반응하도록 돕습니다.

주의(Attention)는 어떤 예측과 오차에 처리 우선순위(Processing Priority)를 부여할지를 조절하는 메커니즘으로 부분적으로 해석할 수 있습니다. 뇌는 모든 신호에 동일한 계산 자원을 할당할 수 없습니다. 불확실하거나(Uncertain), 행동적으로 중요하거나, 새롭거나(Novel), 현재 목표와 관련된 정보에는 더 높은 가중치가 부여될 수 있습니다. 따라서 예측 처리(Predictive Processing)는 어떤 불일치가 지각, 학습 또는 행동에 가장 강하게 영향을 주어야 하는지를 결정하는 과정에서 주의와 상호작용합니다.

불확실성(Uncertainty) 역시 중요합니다. 예측마다 확신도(Confidence)가 다르기 때문입니다. 일부 기대는 매우 신뢰할 수 있는 경험에 기반하는 반면, 다른 기대는 약하거나 모호할 수 있습니다. 따라서 뇌는 무엇이 발생할 가능성이 높은지만 추정하는 것이 아니라 그 예측이 얼마나 확실한지도 추정해야 합니다. 신뢰할 수 있는 예측은 해석에 강하게 영향을 줄 수 있지만, 불확실한 예측은 모순되는 감각 증거가 나타날 때 더 쉽게 수정되어야 합니다.

이러한 특성은 자연스럽게 능동적 지각(Active Perception)으로 이어집니다. 예측 기계는 불확실성이 지속되는 동안 수동적인 상태로 머물 필요가 없습니다. 눈(Eyes), 머리(Head), 신체(Body), 센서(Sensors)를 움직여 서로 경쟁하는 가설을 구별할 수 있는 관찰을 획득할 수 있습니다. 따라서 행동은 부분적으로 유용한 정보를 얻기 위해 선택될 수 있습니다. 생물은 예측을 검증하기 위해 자신의 감각 입력을 변화시키며, 환경과의 상호작용을 통해 불확실성을 감소시킵니다.

학습과 예측은 지속적인 순환(Continuous Cycle)을 형성합니다. 경험은 내부 모델을 만들고, 내부 모델은 예측을 생성하며, 감각 입력은 이러한 예측을 검증하고, 그 결과 발생하는 오차는 다시 모델을 수정합니다. 개선된 모델은 이후 더욱 정확한 미래 기대를 생성합니다. 따라서 학습은 지각과 분리된 과정이 아니며, 새로운 상호작용 하나하나가 세계가 어떻게 작동하는지에 관한 시스템의 이해를 검증하고 개선할 기회를 제공합니다.

예측적 관점은 인공지능(Artificial Intelligence)의 자기지도 학습(Self-Supervised Learning)과도 자연스럽게 연결됩니다. 시스템은 사람이 제공하는 레이블(Human-Provided Labels) 없이 미래, 누락된 관찰(Missing Observations), 인접한 감각 양식(Neighboring Modalities), 행동의 결과를 학습 목표로 사용할 수 있습니다. 다음에 무엇이 발생할지를 예측하려면 모델이 데이터 내부의 잠재적 규칙성(Latent Regularities)을 추출해야 합니다. 이러한 의미에서 예측은 유용한 표현(Useful Representations)을 학습하기 위한 내부적으로 생성된 학습 신호(Internally Generated Training Signal)로 기능할 수 있습니다.

인공지능의 월드 모델(World Models)도 이와 밀접하게 관련된 원리를 따릅니다. 에이전트(Agent)는 상태와 전이에 대한 내부 표현을 유지하고, 이를 이용해 환경이 어떻게 변화할지를 추정하며, 예측된 결과와 실제 관찰을 비교할 수 있습니다. 오차는 모델에서 개선이 필요한 부분을 보여줍니다. 이러한 시스템은 특히 직접적인 시행착오(Trial-and-Error) 상호작용의 비용이 높은 경우 시뮬레이션(Simulation), 계획, 이상 탐지(Anomaly Detection), 적응형 제어(Adaptive Control), 의사결정(Decision Making)을 지원할 수 있습니다.

그러나 뇌를 예측 기계(Brain as a Prediction Machine)라고 설명한다고 해서 모든 신경 과정(Neural Processes)을 하나의 단순한 예측 알고리즘으로 환원할 수 있다는 의미는 아닙니다. 뇌에는 지각, 기억, 강화(Reinforcement), 주의, 행동, 항상성 조절(Homeostatic Regulation)을 담당하는 여러 시스템이 상호작용하고 있습니다. 예측은 강력한 통합적 관점(Unifying Perspective)을 제공하지만, 서로 다른 신경 회로는 서로 다른 메커니즘과 공간적·시간적 척도(Spatial and Temporal Scales)를 통해 예측과 오차 처리를 구현할 수 있습니다.

따라서 뇌를 예측 기계로 보는 관점(Brain-as-Prediction-Machine Perspective)은 지능(Intelligence)을 단순히 반응적인 것이 아니라 선행적으로 미래를 예상하는 특성(Anticipatory Property)으로 강조합니다. 내부 모델은 경험에서 얻은 규칙성을 부호화하고, 계층적 시스템(Hierarchical Systems)은 기대를 생성하며, 예측 오차는 불일치를 드러냅니다. 기억은 사전 구조(Prior Structure)를 제공하고, 행동은 증거를 능동적으로 수집합니다. 이러한 지속적인 순환을 통해 뇌는 불확실성을 줄이고 변화에 적응하며, 과거 경험을 활용하여 미래 상태가 완전히 전개되기 전에 미리 준비할 수 있습니다.

## 04.02 Prediction Error [w/Code]

![](images/image3.png){width="7.268055555555556in" height="7.268055555555556in"}

예측 오차(Prediction Error)는 시스템이 관찰할 것으로 기대한 것과 실제로 받아들인 것 사이의 차이를 의미합니다. 예측 부호화(Predictive Coding)에서 이러한 불일치(Mismatch)는 단순한 실패로 간주되지 않고 내부 모델(Internal Model)의 적절성을 평가하는 유용한 증거로 처리됩니다. 예측이 감각 입력(Sensory Input)과 밀접하게 일치하면 수정이 거의 필요하지 않습니다. 반대로 서로 크게 다르면 발생한 오차는 지각(Perception), 믿음(Belief), 또는 학습된 구조(Learned Structure)를 수정해야 할 가능성을 나타냅니다.

예측 오차의 가장 단순한 계산적 형태는 관찰된 신호(Observed Signal)에서 예측된 신호(Predicted Signal)를 빼는 것으로 표현할 수 있습니다. 차이의 부호(Sign)와 크기(Magnitude)는 기대가 현실과 어떻게 다른지에 관한 정보를 제공합니다. 작은 오차는 현재 모델이 관찰을 비교적 잘 설명하고 있음을 나타내는 반면, 크거나 지속적인 오차는 모델에 부호화된 일부 가정(Assumption), 표현(Representation), 또는 관계(Relationship)가 부정확하다는 것을 의미합니다.

예측 오차는 뇌가 감각 처리가 완료되기 전에 기대(Expectations)를 생성한다고 가정하기 때문에 예측 처리(Predictive Processing)의 핵심적인 요소입니다. 상위 수준 표현(Higher-Level Representations)은 하위 수준에서 예상되는 패턴을 예측하고, 감각 시스템(Sensory Systems)은 실제로 들어오는 증거를 제공합니다. 이 두 신호를 비교하면 잔차 정보(Residual Information)가 생성되며, 이는 신경 계층(Neural Hierarchy)을 통해 전달되어 이후의 해석, 주의(Attention), 학습(Learning)에 영향을 줄 수 있습니다.

이러한 메커니즘은 이미 잘 예측된 정보가 신경 처리(Neural Processing)를 지배할 필요가 없기 때문에 효율성을 향상시킬 수 있습니다. 들어오는 신호의 대부분이 현재 내부 모델에 의해 이미 설명된다면, 처리는 설명되지 않은 부분만을 강조할 수 있습니다. 따라서 예측 오차는 예측 가능한 모든 것을 반복적으로 표현하는 대신 새로움(Novelty), 변화(Change), 불일치(Inconsistency), 또는 부족한 지식(Missing Knowledge)을 강조하는 잔차 신호(Residual Signal)처럼 개념적으로 작동합니다.

예측 오차는 여러 표현 수준(Levels of Representation)에서 발생할 수 있습니다. 낮은 감각 수준에서는 예상하지 못한 가장자리(Edge), 소리 주파수(Sound Frequency), 움직임(Motion), 밝기 변화(Brightness Change) 등이 오차를 발생시킬 수 있습니다. 높은 수준에서는 객체(Object), 사건(Event), 맥락(Context), 인과 관계(Causal Relationship), 의도(Intention)와 관련된 불일치가 발생할 수 있습니다. 따라서 예측 부호화는 오차 처리를 지각의 마지막 단계에서 한 번만 수행되는 비교가 아니라 계층적인 과정으로 간주합니다.

하위 수준에서 생성된 오차는 들어오는 증거를 기존 예측으로 설명할 수 없을 때 상위 수준의 해석에 영향을 줄 수 있습니다. 동시에 상위 수준의 기대는 하위 수준에서 발생한 어떤 불일치가 의미 있는지를 변화시킬 수 있습니다. 이러한 상호적인 상호작용(Reciprocal Interaction)은 감각 증거를 설명하면서도 사전 지식(Prior Knowledge), 맥락, 환경 구조에 대한 기대와 일관성을 유지하는 해석으로 지각이 수렴하도록 합니다.

모든 예측 오차가 동일한 영향력을 가져야 하는 것은 아닙니다. 일부 감각 신호는 신뢰할 수 있고 정밀한 반면, 다른 신호는 잡음이 많거나(Noisy), 모호하거나(Ambiguous), 불확실할 수 있습니다. 따라서 예측 처리는 정밀도 가중(Precision Weighting)을 포함하며, 신뢰할 수 있는 정보에서 발생한 것으로 추정되는 오차가 믿음 갱신(Belief Updating)에 더 큰 영향을 미치도록 합니다. 신뢰도가 낮은 신호와 관련된 오차는 불안정하거나 잡음이 많은 관찰이 유용한 내부 모델을 지속적으로 방해하지 않도록 영향력이 감소될 수 있습니다.

주의(Attention)는 선택된 오차 신호(Error Signals)의 처리 우선순위를 높임으로써 이러한 가중 과정과 상호작용할 수 있습니다. 중요한 목표(Goal), 예상하지 못한 사건, 또는 주의를 기울이는 감각 특징과 관련된 불일치는 관련성이 낮은 배경 정보에서 발생한 동일한 크기의 불일치보다 더 큰 영향을 받을 수 있습니다. 따라서 예측 오차는 단순한 수치적 불일치뿐만 아니라 추정된 신뢰성(Reliability), 행동적 중요성(Behavioral Importance), 불확실성(Uncertainty), 현재의 과제 요구(Task Demands)에 의해서도 영향을 받습니다.

지속적인 예측 오차(Persistent Prediction Error)는 학습에서 특히 중요합니다. 한 번의 불일치는 일시적인 잡음 때문에 발생할 수 있지만, 반복적인 불일치는 모델이 경험을 체계적으로 설명하지 못한다는 것을 의미합니다. 이 경우 시냅스 가소성(Synaptic Plasticity)과 표현 학습(Representation Learning)이 예측을 생성하는 연결을 수정할 수 있습니다. 반복적인 갱신을 통해 시스템은 환경의 규칙성(Regularities)을 더욱 정확하게 포착하는 내부 표현을 구성함으로써 미래의 오차를 줄일 수 있습니다.

예측 오차는 새로움(Novelty)과 익숙함(Familiarity)을 구분하는 데에도 도움을 줍니다. 익숙한 상황은 기존 모델에 의해 잘 표현되는 경우가 많기 때문에 상대적으로 작은 설명되지 않은 잔차를 생성합니다. 반대로 새로운 사건은 기존 기대를 위반하기 때문에 더 강한 오차를 생성할 수 있습니다. 이러한 관계는 예측 부호화, 새로움 탐지(Novelty Detection), 주의 할당(Attention Allocation), 기억 형성(Memory Formation), 학습이 필요한 경험의 우선순위 설정을 개념적으로 연결합니다.

시간적 예측 오차(Temporal Prediction Error)는 동일한 원리를 시간 차원으로 확장합니다. 신경 시스템은 현재의 감각 입력뿐만 아니라 다음에 무엇이 발생할지도 예측할 수 있습니다. 예상했던 사건이 발생하지 않거나 예상하지 못한 사건이 대신 발생하면, 이러한 불일치는 학습된 상태 전이(State Transitions)에 관한 정보를 제공합니다. 따라서 반복적인 시간적 오차는 시퀀스(Sequences), 궤적(Trajectories), 행동 결과(Action Consequences), 환경 동역학(Environmental Dynamics)에 관한 기대를 수정할 수 있습니다.

운동 제어(Motor Control) 역시 예측 오차에 의존합니다. 움직임 전이나 움직임 중에 내부 모델은 행동으로부터 예상되는 감각적 결과(Sensory Consequences)를 예측할 수 있습니다. 실제 고유수용감각(Proprioceptive), 시각(Visual), 촉각(Tactile) 피드백을 이러한 예측과 비교할 수 있습니다. 그 차이는 움직임을 수정하고 운동 명령(Motor Commands)과 예상 결과를 연결하는 순방향 모델(Forward Model)을 갱신하는 신호를 제공하여 미래의 행동을 더욱 정확하게 만들 수 있습니다.

예측 오차는 능동적 지각(Active Perception)의 핵심적인 요소이기도 합니다. 현재의 감각 증거만으로 서로 경쟁하는 여러 설명을 구분할 수 없다면, 생물은 더욱 유용한 관찰을 생성하는 행동을 수행할 수 있습니다. 눈(Eyes), 머리(Head), 신체(Body), 센서(Sensors)를 움직이면 비교에 사용할 수 있는 감각 증거가 변화합니다. 따라서 행동은 예측을 직접 검증하기 위한 수단으로 사용될 수 있으며, 수동적인 관찰에만 의존하지 않고 환경과의 상호작용을 통해 불확실성을 줄일 수 있습니다.

감각 예측 오차(Sensory Prediction Error)는 보상 예측 오차(Reward Prediction Error)와 구분해야 합니다. 감각 오차는 예상된 상태 또는 신호와 실제로 관찰된 상태 또는 신호 사이의 차이를 의미하는 반면, 보상 예측 오차는 기대한 가치(Expected Value)와 실제로 획득한 가치(Obtained Value) 사이의 차이를 의미합니다. 두 방식 모두 불일치를 이용해 기대를 갱신하지만 서로 다른 대상을 다룹니다. 그러나 이들의 상호작용은 지각 학습(Perceptual Learning)을 강화학습(Reinforcement Learning) 및 행동적 의사결정(Behavioral Decision Making)과 연결할 수 있습니다.

기억(Memory)은 기대가 이전에 학습된 규칙성에 의존하기 때문에 예측 오차에 강한 영향을 미칩니다. 피질 지식(Cortical Knowledge)은 반복적인 경험을 기반으로 일반화된 예측을 제공할 수 있는 반면, 해마 기억(Hippocampal Memory)은 맥락적이거나 특정 일화에 기반한 기대를 제공할 수 있습니다. 따라서 불일치는 일반적인 모델이 부적절하다는 것을 나타낼 수도 있고, 현재 상황이 기억된 특정 경험과 다르다는 것을 나타낼 수도 있으며, 각각 서로 다른 형태의 학습과 갱신을 유도할 수 있습니다.

예측 오차는 자기지도(Self-Supervision)를 위한 자연스러운 신호도 제공합니다. 지능형 시스템(Intelligent System)은 자신의 예측이 부정확했음을 판단하기 위해 사람이 제공하는 레이블(Human Label)을 반드시 필요로 하지 않습니다. 관찰 자체가 학습 목표(Target)를 제공하기 때문입니다. 미래의 감각 상태(Future Sensory States), 입력의 숨겨진 부분(Hidden Parts), 감각 양식(Modality) 사이의 관계를 예측하고 현실과 비교할 수 있습니다. 따라서 오차 최소화(Error Minimization)는 레이블이 없는 연속적인 경험으로부터 표현을 학습하도록 지원할 수 있습니다.

이러한 원리는 인공지능(Artificial Intelligence)에 직접적으로 적용될 수 있습니다. 예측 모델(Predictive Models)은 예상되는 관찰을 생성하고 실제 데이터와 비교한 다음 발생한 잔차를 이용하여 표현을 갱신할 수 있습니다. 이와 관련된 메커니즘은 자기지도 학습(Self-Supervised Learning), 생성 모델링(Generative Modeling), 이상 탐지(Anomaly Detection), 상태 추정(State Estimation), 월드 모델(World Models)에서 나타납니다. 예측 오차는 인공 모델이 환경의 구조 또는 동역학을 제대로 포착하지 못하는 부분을 알려주는 공통적인 신호를 제공합니다.

월드 모델(World Models)에서 예측 오차는 학습된 상태 전이(State Transitions)의 약점을 드러낼 수 있습니다. 에이전트(Agent)는 다음 시각 장면(Visual Scene), 객체 위치(Object Position), 물리적 상태(Physical State), 행동의 결과를 예측한 뒤 이를 실제 관찰과 비교할 수 있습니다. 반복적인 불일치는 누락된 동역학(Missing Dynamics), 잘못된 가정(Incorrect Assumptions), 익숙하지 않은 상황(Unfamiliar Situations)을 식별하는 데 도움을 줄 수 있습니다. 따라서 예측 오차는 체화 인공지능(Embodied AI)과 피지컬 AI(Physical AI)의 지속적인 적응(Continual Adaptation)에 특히 유용합니다.

예측 오차는 지능형 시스템이 항상 0으로 줄여야 하는 대상으로 해석해서는 안 됩니다. 환경은 확률적(Stochastic)일 수 있고, 관찰에는 잡음이 존재하며, 여러 미래가 동시에 가능할 수 있기 때문에 일부 불확실성은 피할 수 없습니다. 따라서 효과적인 학습은 감소시킬 수 있는 모델 오차(Reducible Model Error)와 제거할 수 없는 불확실성(Irreducible Uncertainty)을 구분해야 합니다. 강건한 예측 시스템(Robust Predictive System)은 언제 모델을 갱신해야 하는지와 언제 남아 있는 변동성을 단순히 불확실성으로 표현해야 하는지를 판단할 수 있어야 합니다.

따라서 예측 오차(Prediction Error)는 예측 부호화(Predictive Coding)에서 핵심적인 학습 및 수정 신호(Teaching and Correction Signal)로 작동합니다. 기대는 감각 입력에 관한 가설을 생성하고, 관찰은 이러한 가설을 검증하며, 정밀도(Precision)는 불일치가 얼마나 강하게 영향을 미쳐야 하는지를 결정하고, 지속적인 오차는 내부 모델의 변화를 유도합니다. 이러한 예측과 현실 사이의 지속적인 비교를 통해 신경 시스템은 지각을 향상시키고, 새로움을 탐지하며, 행동을 정교화하고, 환경의 구조를 학습하며, 변화하는 조건에 적응할 수 있습니다.

## 04.03 Hierarchical Predictive Processing [w/Code]

![](images/image4.png){width="7.268055555555556in" height="7.268055555555556in"}

계층적 예측 처리(Hierarchical Predictive Processing)는 뇌를 서로 다른 수준이 각기 다른 추상화 정도(Degrees of Abstraction)의 정보를 표현하는 다층 예측 시스템(Multilayer Prediction System)으로 설명합니다. 낮은 수준은 비교적 즉각적인 감각 특징(Sensory Features)을 처리하는 반면, 높은 수준은 객체(Objects), 장면(Scenes), 맥락(Contexts), 목표(Goals), 더 광범위한 인과 구조(Causal Structure)를 표현합니다. 이러한 수준 사이의 정보 교환을 통해 지각(Perception)은 세부적인 감각 증거와 세계에 대한 점점 더 추상적인 기대(Expectations)를 결합할 수 있습니다.

이러한 계층 구조(Hierarchy)는 원시 감각 신호(Raw Sensory Signals)를 점진적으로 복잡한 표현으로 변환하는 단순한 순방향 처리 사슬(Feedforward Chain)이 아닙니다. 높은 수준은 낮은 수준에서 예상되는 활동에 대한 예측(Predictions)을 지속적으로 생성합니다. 이러한 예측은 피드백 경로(Feedback Pathways)를 통해 하향식(Top-Down)으로 전달되는 반면, 예측된 활동과 실제 관찰된 활동 사이의 불일치 정보는 상향식(Bottom-Up)으로 전달됩니다. 따라서 지각은 여러 수준에 걸친 예측과 예측 오차(Prediction Error)의 반복적인 교환으로부터 형성됩니다.

계층 구조의 낮은 수준에서 예측은 가장자리(Edges), 방향성(Orientation), 밝기(Brightness), 주파수(Frequency), 질감(Texture), 국소적 움직임(Local Motion)과 같은 비교적 단순한 특성과 관련될 수 있습니다. 이러한 특징은 빠르게 변화하며 감각 입력과 밀접하게 연결되어 있습니다. 높은 수준에서는 더 넓은 공간적·시간적 범위에 걸쳐 패턴을 결합하여 객체, 행동(Actions), 환경적 맥락(Environmental Contexts), 사건 시퀀스(Event Sequences), 그리고 이들 사이의 더욱 추상적인 관계를 표현할 수 있습니다.

이러한 조직은 한 수준의 예측이 그 아래 수준의 처리를 위한 맥락(Context)을 제공하도록 합니다. 높은 수준의 표현이 특정 객체가 존재한다고 예측한다면, 낮은 수준의 감각 표현에서 나타날 가능성이 높은 형태(Shapes), 질감, 경계(Boundaries), 움직임에 관한 기대를 생성할 수 있습니다. 이후 들어오는 증거는 이러한 기대를 기준으로 평가되며, 지각은 감각 데이터뿐만 아니라 기존의 사전 구조(Prior Structure)에도 의존하게 됩니다.

예측 오차(Prediction Errors)는 이를 보완하는 상향식 신호를 제공합니다. 낮은 수준의 관찰이 하향식 기대와 다르면, 이러한 불일치는 현재의 높은 수준 설명이 불완전하거나 부정확하다는 것을 나타냅니다. 이러한 잔차 신호(Residual Signals)는 상위 방향으로 전파되어 점점 더 추상적인 표현에 영향을 줄 수 있습니다. 불일치가 지속되면 결국 시스템이 객체, 장면, 맥락 또는 더 광범위한 환경 상태(Environmental State)에 대한 해석을 수정하도록 만들 수 있습니다.

계층적 처리는 서로 다른 표현 수준에서 불확실성(Uncertainty)을 해결할 수 있기 때문에 유용합니다. 국소적인 시각 특징은 단독으로 고려하면 모호할 수 있지만 익숙한 객체의 일부로 해석하면 이해할 수 있습니다. 마찬가지로 객체도 주변 장면이나 과제 맥락(Task Context)을 고려하기 전까지는 모호할 수 있습니다. 높은 수준의 예측은 낮은 수준에서 가능한 해석을 제한하여 맥락적 지식(Contextual Knowledge)이 불완전하거나 잡음이 많은 신호를 효율적으로 해석하도록 지원합니다.

그러나 하향식 기대(Top-Down Expectations)가 아무런 제약 없이 지각을 지배해서는 안 됩니다. 높은 수준의 예측이 감각 증거를 완전히 압도한다면 시스템은 모순되는 관찰에도 불구하고 잘못된 해석을 유지할 수 있습니다. 상향식 예측 오차(Bottom-Up Prediction Errors)는 기대가 실패할 때 이를 알림으로써 수정 압력(Corrective Pressure)을 제공합니다. 따라서 효과적인 지각은 사전 예측(Prior Predictions)과 계층의 낮은 수준에서 들어오는 증거 사이의 역동적인 균형에 의존합니다.

정밀도 가중(Precision Weighting)은 이러한 균형을 조절하는 데 도움을 줍니다. 감각 신호는 잡음(Noise), 모호성(Ambiguity), 관련성(Relevance)이 서로 다르기 때문에 예측 오차의 신뢰성도 달라집니다. 정밀하고 신뢰할 수 있는 증거와 관련된 오차는 높은 수준의 갱신에 더 큰 영향을 주어야 하는 반면, 불확실한 오차에는 더 낮은 가중치가 부여될 수 있습니다. 따라서 계층 구조는 예측과 오차뿐만 아니라 교환되는 정보에 대한 신뢰도(Confidence)의 추정값도 함께 처리합니다.

주의(Attention)는 이러한 실질적인 정밀도(Effective Precision)를 변화시킴으로써 계층적 예측 처리에 영향을 줄 수 있습니다. 현재 목표와 관련되거나 행동적으로 중요한 사건(Behaviorally Important Events)과 관련된 신호는 더 높은 처리 우선순위를 부여받아 그 예측 오차가 더 강한 영향력을 갖도록 할 수 있습니다. 반대로 관련성이 낮거나 신뢰할 수 없는 신호는 억제될 수 있습니다. 따라서 주의는 특정 순간에 계층적 예측 시스템의 어떤 부분이 지각과 학습을 지배해야 하는지를 결정하는 데 도움을 줄 수 있습니다.

계층적 예측 처리는 여러 시간 척도(Temporal Scales)에 걸쳐서도 작동합니다. 낮은 수준은 밀리초(Milliseconds) 또는 1초보다 짧은 시간 동안 빠르게 변화하는 감각 특징을 예측할 수 있는 반면, 높은 수준은 행동, 사건 또는 행동적 에피소드(Behavioral Episodes)에 걸쳐 지속되는 더 느린 패턴을 표현할 수 있습니다. 이러한 시간적 계층(Temporal Hierarchy)은 즉각적인 감각 변화를 장기적인 맥락 안에서 해석할 수 있도록 하며, 순간적인 지각을 시퀀스(Sequences), 목표, 계획(Plans)과 연결합니다.

이러한 시간적 조직(Temporal Organization)은 동적 환경(Dynamic Environments)을 이해하는 데 특히 중요합니다. 하나의 관찰만으로는 현재 무엇이 일어나고 있는지를 충분히 이해할 수 없는 경우가 많습니다. 뇌는 이전 상태를 이용해 앞으로의 상태를 예측하고 관찰된 전이가 예상된 것인지를 평가할 수 있습니다. 높은 수준의 표현은 더 긴 사건 구조(Event Structures)를 부호화할 수 있는 반면, 낮은 수준은 더 빠른 물리적 변화를 추적하여 여러 시간 척도의 예측이 동시에 작동하도록 합니다.

기억(Memory)은 예측 계층의 높은 수준에 강하게 기여합니다. 반복적인 경험을 통해 피질 시스템(Cortical Systems)은 안정적인 통계적 규칙성(Statistical Regularities)을 학습할 수 있는 반면, 일화 기억(Episodic Memory)은 특정한 과거 상황에 관한 정보를 제공할 수 있습니다. 이렇게 저장된 표현은 현재 맥락에서 어떤 객체, 사건 또는 결과가 발생할 가능성이 높은지에 관한 사전 기대(Priors)를 생성합니다. 이후 예측 오차는 기존 지식이 여전히 충분한지 또는 수정되어야 하는지를 결정하는 데 기여합니다.

예측 오차가 반복적으로 체계적인 불일치를 나타내면 계층 구조 전체에서 학습(Learning)이 발생할 수 있습니다. 낮은 수준에서는 감각 특징의 표현을 정교화할 수 있는 반면, 높은 수준에서는 범주(Categories), 맥락적 관계(Contextual Relationships), 인과 모델(Causal Models)을 수정할 수 있습니다. 오차는 여러 표현 척도에서 발생하기 때문에 학습이 시스템의 모든 부분을 동일하게 변화시킬 필요는 없습니다. 각 수준은 자신이 경험하는 불일치의 유형과 지속성에 따라 서로 다르게 적응할 수 있습니다.

이러한 계층적 구조는 높은 수준이 낮은 수준의 감각 표현에 포함된 모든 세부 정보를 보존할 필요가 없기 때문에 추상화(Abstraction)를 지원합니다. 대신 여러 관찰에 걸쳐 계속 유용하게 유지되는 규칙성을 부호화할 수 있습니다. 예를 들어 수많은 시각적 형태가 동일한 객체 정체성(Object Identity)에 대응할 수 있고, 다양한 구체적 상황이 하나의 공통 개념(Common Concept)을 나타낼 수 있습니다. 예측은 이렇게 점점 더 불변적인 표현(Invariant Representations)을 경험과 비교하여 검증할 수 있는 메커니즘을 제공합니다.

다중모달 처리(Multimodal Processing)도 이러한 계층 구조에 포함될 수 있습니다. 높은 수준의 표현은 시각(Visual), 청각(Auditory), 촉각(Tactile), 고유수용감각(Proprioceptive), 기타 감각 흐름을 동시에 제약하는 예측을 생성할 수 있습니다. 따라서 하나의 감각 양식(Modality)에서 얻은 정보가 다른 감각 양식의 불확실성을 해결하는 데 도움을 줄 수 있습니다. 일관된 높은 수준 모델은 여러 감각 증거를 함께 설명하며, 서로 일치하지 않는 관찰은 통합된 해석에서 수정이 필요한 부분을 나타내는 오차를 생성합니다.

계층적 예측 처리는 자연스럽게 행동(Action)으로 확장됩니다. 높은 수준은 목표 또는 원하는 미래 상태(Desired Future States)를 표현할 수 있는 반면, 낮은 수준은 이러한 기대를 점점 더 구체적인 운동 및 감각 예측(Motor and Sensory Predictions)으로 변환할 수 있습니다. 실제 움직임은 고유수용감각, 시각, 촉각 피드백을 생성하며, 이를 예상된 결과와 비교할 수 있습니다. 서로 다른 수준에서 발생하는 오차는 즉각적인 운동 수정(Motor Correction) 또는 더 광범위한 행동 전략(Action Strategy)의 변화를 지원할 수 있습니다.

능동적 지각(Active Perception) 역시 동일한 아키텍처에서 도출됩니다. 서로 경쟁하는 여러 높은 수준의 해석이 여전히 가능하다면, 시스템은 이들을 구별할 수 있는 감각 증거를 생성하는 행동을 선택할 수 있습니다. 눈의 움직임(Eye Movements), 신체 움직임(Body Movements), 탐색 행동(Exploratory Actions)은 낮은 수준의 입력을 변화시키고 높은 수준의 예측을 검증합니다. 따라서 계층 구조는 감각 정보를 해석하는 것뿐만 아니라 다음에 어떤 정보를 획득해야 하는지를 결정하는 데에도 참여합니다.

인공지능(Artificial Intelligence)의 관점에서 계층적 예측 처리는 딥 표현 학습(Deep Representation Learning) 및 월드 모델링(World Modeling)과 유사한 측면을 가집니다. 인공 시스템은 낮은 수준의 관찰(Low-Level Observations), 중간 수준 특징(Intermediate Features), 객체, 의미적 상태(Semantic States), 높은 수준의 과제 구조(Task Structure)를 서로 다른 계층에서 표현할 수 있습니다. 이러한 수준 사이의 예측은 학습 신호를 제공할 수 있으며, 불일치는 표현이 환경의 중요한 구조를 포착하지 못하는 부분을 식별할 수 있습니다.

이러한 접근법은 로봇이 공간적(Spatial), 의미적(Semantic), 시간적(Temporal) 척도에 분산된 정보를 처리해야 하기 때문에 체화 인공지능(Embodied AI)과 피지컬 AI(Physical AI)에 특히 중요합니다. 로봇은 낮은 수준에서 픽셀(Pixels)이나 센서 특징(Sensor Features)을 예측하고, 중간 수준에서는 객체 움직임(Object Motion)을 예측하며, 높은 수준에서는 과제 또는 환경의 변화(Task or Environmental Evolution)를 예측해야 할 수 있습니다. 예측을 계층적으로 구성하면 빠른 센서 처리와 상대적으로 느린 추론(Reasoning), 계획(Planning), 의사결정(Decision Making)을 연결하는 데 도움이 될 수 있습니다.

그럼에도 계층적 예측 처리(Hierarchical Predictive Processing)는 모든 신경 계산(Neural Computation)을 완전히 설명하는 이론이라기보다 하나의 이론적 프레임워크(Theoretical Framework)로 이해해야 합니다. 서로 다른 뇌 영역은 복잡한 순환 연결(Recurrent Connectivity), 측방 연결(Lateral Connectivity), 피드백 연결(Feedback Connectivity)을 포함하며, 예측과 관련된 신호도 여러 메커니즘을 통해 구현될 수 있습니다. 이 프레임워크의 가치는 상향식 증거와 하향식 지식이 여러 수준에 걸쳐 어떻게 상호작용할 수 있는지를 연구하기 위한 공통적인 계산적 언어(Computational Language)를 제공한다는 데 있습니다.

따라서 계층적 예측 처리(Hierarchical Predictive Processing)는 지능적 지각(Intelligent Perception)을 추상화(Abstraction)와 증거(Evidence) 사이의 지속적인 조정 과정으로 설명합니다. 높은 수준은 아래에서 예상되는 구조를 예측하고, 낮은 수준은 불일치를 보고하며, 정밀도(Precision)는 어떤 오차가 중요한지를 결정하고, 지속적인 불일치는 표현의 학습과 수정을 유도합니다. 공간적, 의미적, 시간적 척도에 걸친 이러한 반복적인 정보 교환을 통해 뇌는 불확실한 감각 흐름을 지각, 예측, 학습, 적응적 행동(Adaptive Action)을 지원하는 일관된 내부 모델(Coherent Internal Models)로 변환할 수 있습니다.

## 04.04 Perception as Inference

![](images/image5.png){width="7.268055555555556in" height="7.268055555555556in"}

추론으로서의 지각(Perception as Inference)은 뇌가 감각 신호(Sensory Signals)로부터 외부 세계를 직접적으로 복원하는 것이 아니라는 관점을 설명합니다. 감각 수용기(Sensory Receptors)는 불완전하고 잡음이 많으며 종종 모호한 정보를 받아들이고, 이러한 정보는 여러 가능한 원인에 의해 생성될 수 있습니다. 따라서 지각 시스템(Perceptual System)은 이용 가능한 증거를 가장 그럴듯하게 생성했을 숨겨진 객체, 사건, 환경 상태를 추론해야 하며, 지각은 단순한 측정이 아니라 해석(Interpretation)의 문제가 됩니다.

이러한 문제는 흔히 역문제(Inverse Problem)라고 설명됩니다. 물리적 세계(Physical World)는 빛의 반사(Light Reflection), 소리의 전파(Sound Propagation), 기계적 접촉(Mechanical Contact), 신체 움직임(Body Movement)과 같은 과정을 통해 감각적 결과(Sensory Consequences)를 생성합니다. 지각은 이와 반대 방향으로 작동하여 이러한 감각적 결과에서 시작해 그 기저에 존재하는 원인을 추정해야 합니다. 서로 다른 원인이 유사한 관찰을 생성할 수 있기 때문에 감각 증거만으로는 하나의 고유한 해석을 결정하기 어려운 경우가 많습니다.

사전 지식(Prior Knowledge)은 이러한 모호성(Ambiguity)을 해결하는 데 도움을 줍니다. 경험을 통해 뇌는 객체, 환경, 행동, 사건에 관한 통계적 규칙성(Statistical Regularities)을 학습합니다. 이렇게 학습된 규칙성은 특정 맥락(Context)에서 무엇이 발생할 가능성이 높은지에 관한 기대(Expectations)를 형성합니다. 감각 증거가 불완전할 때 사전 지식은 가능한 해석의 범위를 제한하여 지각 시스템이 현재 입력과 과거 경험 모두에 일치하는 설명을 선택하도록 할 수 있습니다.

이러한 관계는 흔히 베이지안 추론(Bayesian Inference)을 통해 표현됩니다. 베이지안 관점에서 사전 믿음(Prior Beliefs)은 새로운 증거가 관찰되기 이전의 기대를 나타내며, 가능도(Likelihood)는 감각 증거가 가능한 원인과 얼마나 일치하는지를 설명합니다. 사전 정보와 가능도를 결합하면 무엇이 존재할 가능성이 가장 높은지에 관한 사후 믿음(Posterior Belief)이 형성됩니다. 이 프레임워크는 경험과 증거가 어떻게 함께 지각에 영향을 줄 수 있는지를 이해하기 위한 계산적 언어(Computational Language)를 제공합니다.

베이지안 설명(Bayesian Descriptions)이 반드시 뉴런(Neurons)이 수학적인 확률 공식을 명시적으로 계산한다는 것을 의미하는 것은 아닙니다. 베이지안 추론은 불확실한 정보를 어떻게 효율적으로 결합할 수 있는지를 설명하는 규범적 프레임워크(Normative Framework)를 제공합니다. 신경 집단(Neural Populations)은 분산된 활동(Distributed Activity), 순환적 상호작용(Recurrent Interactions), 시냅스 강도(Synaptic Strengths), 또는 다른 메커니즘을 통해 불확실성과 기대를 표현할 수 있습니다. 중요한 원리는 지각이 어느 한쪽에만 의존하지 않고 사전 구조(Prior Structure)와 들어오는 증거를 통합한다는 것입니다.

예측 부호화(Predictive Coding)는 지각적 추론(Perceptual Inference)의 일부 측면을 구현할 수 있는 하나의 가능한 메커니즘을 제공합니다. 신경 계층(Neural Hierarchy)의 높은 수준은 낮은 수준에서 예상되는 감각 패턴에 대한 예측(Predictions)을 생성합니다. 들어오는 관찰은 이러한 예측과 비교되고, 기대와 증거가 다르면 예측 오차(Prediction Errors)가 발생합니다. 예측과 오차 사이의 반복적인 교환은 신경 표현(Neural Representations)을 감각 입력을 더 잘 설명하는 해석으로 점진적으로 조정할 수 있습니다.

따라서 지각은 하향식(Top-Down) 정보와 상향식(Bottom-Up) 정보를 모두 포함합니다. 상향식 신호는 감각 수용기에서 시작된 증거를 제공하는 반면, 하향식 신호는 맥락, 기억(Memory), 상위 수준 표현(Higher-Level Representations)으로부터 생성된 기대를 전달합니다. 어느 한 방향만으로는 충분하지 않습니다. 사전 구조가 없는 상향식 처리는 모호한 신호를 해결하지 못할 수 있으며, 지나치게 강한 하향식 영향은 감각 증거가 기대와 모순되더라도 기존의 기대를 유지하게 만들 수 있습니다.

불확실성(Uncertainty)은 서로 다른 정보원이 추론에 얼마나 강한 영향을 주어야 하는지를 결정합니다. 감각 증거가 명확하고 신뢰할 수 있을 때 지각은 들어오는 관찰에 강하게 의존해야 합니다. 감각 신호가 잡음이 많거나 모호할 때는 사전 지식이 더 큰 역할을 할 수 있습니다. 반대로 사전 기대 자체가 매우 불확실하다면 신뢰할 수 있는 증거가 나타났을 때 쉽게 수정되어야 합니다. 따라서 지각적 추론은 가능한 원인뿐만 아니라 그러한 추정에 대한 확신도(Confidence)를 함께 평가해야 합니다.

정밀도 가중(Precision Weighting)은 이러한 조절을 설명하는 방법을 제공합니다. 정밀도(Precision)는 예측 또는 감각 신호의 추정된 신뢰성(Reliability)을 의미합니다. 높은 정밀도의 증거와 관련된 예측 오차는 신뢰할 수 없는 입력에서 발생한 오차보다 지각적 갱신(Perceptual Updating)에 더 강한 영향을 주어야 합니다. 정보를 추정된 정밀도에 따라 가중함으로써 시스템은 잡음에 과도하게 반응하지 않으면서도 현재의 기대에 반하는 신뢰할 수 있는 관찰에는 민감하게 반응할 수 있습니다.

주의(Attention)는 어떤 감각 신호가 더 높은 실질적 가중치를 받을지를 변화시킬 수 있기 때문에 이러한 과정과 밀접하게 관련됩니다. 현재의 목표(Current Goals), 위협(Threats), 과제(Tasks), 불확실성과 관련된 정보는 우선적으로 처리되어 추론에 더 큰 영향을 줄 수 있습니다. 따라서 주의는 단순히 감각 입력을 증폭하는 것에 그치지 않고, 어떤 증거를 환경에 대한 현재의 해석을 수정할 만큼 중요하거나 신뢰할 수 있는 것으로 취급할지를 조절할 수 있습니다.

맥락(Context)은 지각적 추론에 또 하나의 강력한 제약을 제공합니다. 동일한 감각 특징(Sensory Feature)이라도 주변 장면(Surrounding Scene), 앞서 발생한 사건, 현재의 과제에 따라 서로 다른 해석을 지원할 수 있습니다. 높은 수준의 맥락적 표현(Contextual Representations)은 가능한 원인의 공간을 좁혀 모호한 국소 증거(Local Evidence)를 효율적으로 해석하도록 합니다. 이는 지각이 독립적으로 고려된 개별 감각 특징보다 여러 신호 사이의 관계에 의존하는 경우가 많은 이유를 설명합니다.

지각 착시(Perceptual Illusions)는 추론의 강점과 한계를 모두 보여줍니다. 감각 증거가 모호할 때 지각 시스템은 학습된 규칙성에 비추어 일반적으로 합리적이지만 인위적으로 구성된 상황에서는 잘못된 해석을 선택할 수 있습니다. 이러한 착시는 단순히 지각이 결함을 가지고 있다는 것을 보여주는 것이 아닙니다. 오히려 불완전한 감각 정보로부터 세계의 안정적인 속성을 추론하기 위해 뇌가 평상시에 성공적으로 사용하는 가정(Assumptions)을 드러냅니다.

추론은 지각적 항상성(Perceptual Constancy)에도 필수적입니다. 객체의 감각적 모습은 조명(Illumination), 시점(Viewpoint), 거리(Distance), 방향(Orientation), 주변 조건에 따라 변화하지만, 객체 자체는 여전히 안정적으로 지각될 수 있습니다. 뇌는 변화하는 감각 측정값 뒤에 존재하는 지속적인 속성을 추론해야 합니다. 따라서 즉각적인 감각 표현이 크게 달라지더라도 객체 정체성(Object Identity), 크기(Size), 형태(Shape), 표면 특성(Surface Characteristics)은 비교적 일정하게 유지될 수 있습니다.

시간적 정보(Temporal Information)는 추론을 더욱 제약합니다. 현재의 관찰은 직전에 발생한 사건과 완전히 독립적으로 해석되는 경우가 거의 없습니다. 이전 상태(Previous States)는 가능한 전이(Transitions), 움직임, 사건 시퀀스(Event Sequences)에 관한 기대를 제공합니다. 뇌는 시간에 걸쳐 정보를 통합함으로써 지속적인 객체와 일시적인 잡음을 구분하고, 궤적(Trajectories)을 추정하며, 일시적인 가림(Occlusion)을 해결하고, 하나의 감각적 순간만으로는 이해할 수 없는 진행 중인 과정을 추론할 수 있습니다.

기억(Memory)은 이러한 추론에 필요한 지식의 상당 부분을 제공합니다. 의미 기억(Semantic Memory)은 범주(Categories)와 관계에 관한 일반화된 지식을 제공할 수 있으며, 일화 기억(Episodic Memory)은 특정한 과거 경험의 정보를 제공할 수 있습니다. 작업 기억(Working Memory)은 현재 관련된 가설(Hypotheses)이나 맥락 정보를 유지할 수 있습니다. 따라서 지각은 완성된 표현을 인지(Cognition)에 단순히 전달하는 독립적인 단계가 아니라 기억 시스템과 지속적으로 상호작용하는 과정입니다.

추론으로서의 지각은 여러 감각 양식(Sensory Modalities)에 걸쳐서도 확장됩니다. 시각(Visual), 청각(Auditory), 촉각(Tactile), 고유수용감각(Proprioceptive), 전정감각(Vestibular) 신호는 동일한 기저 사건에 관한 상호보완적인 증거를 제공할 수 있습니다. 하나의 감각 양식이 불확실할 때 다른 감각 양식이 모호성을 해결하는 데 도움을 줄 수 있습니다. 뇌는 이러한 신호를 신뢰성에 따라 통합하여 단일 감각 채널만으로 가능한 것보다 더 일관된 환경 또는 신체 상태의 추정치를 구성할 수 있습니다.

행동(Action)은 생물이 능동적으로 더 나은 증거를 획득할 수 있기 때문에 추론 문제 자체를 변화시킵니다. 감각 정보가 충분하지 않을 때 눈(Eyes), 머리(Head), 손(Hands), 신체의 움직임을 통해 서로 경쟁하는 해석을 구별할 수 있는 새로운 관찰을 얻을 수 있습니다. 따라서 지각은 순수하게 수동적인 과정이 아니라 능동적 과정입니다. 시스템은 행동의 정보적 가치(Informational Value)를 고려하여 행동을 선택할 수 있으며, 불확실성 감소(Uncertainty Reduction)를 지속적인 지각-행동 루프(Perception--Action Loop)로 전환합니다.

이러한 원리는 체화 지능(Embodied Intelligence)에 특히 중요합니다. 물리적 세계에서 작동하는 에이전트(Agent)는 객체 상태(Object State), 주행 가능성(Traversability), 숨겨진 기하 구조(Hidden Geometry), 다른 에이전트의 의도(Intentions), 가능한 행동의 결과처럼 직접 관찰할 수 없는 속성을 추론해야 합니다. 신뢰할 수 있는 행동을 위해서는 이러한 잠재 상태(Latent States)에 관한 믿음을 유지하고, 상호작용을 통해 새로운 감각 증거가 들어올 때마다 이를 지속적으로 수정해야 합니다.

인공지능(Artificial Intelligence)에서 추론으로서의 지각은 확률적 상태 추정(Probabilistic State Estimation), 베이지안 필터링(Bayesian Filtering), 잠재 변수 모델(Latent-Variable Models), 생성 모델(Generative Models), 월드 모델(World Models)에서 나타납니다. 인공 시스템은 숨겨진 상태에 대한 가설을 유지하고, 해당 상태와 연관된 관찰을 예측하며, 새로운 측정값이 들어오면 추정치를 갱신할 수 있습니다. 이러한 메커니즘은 센서에 잡음이 많고, 관찰이 부분적이며, 환경이 시간에 따라 변화하는 경우 특히 유용합니다.

피지컬 AI(Physical AI)와 로보틱스(Robotics)에서 이러한 관점은 지각을 단순한 객체 인식(Object Recognition)으로 취급하는 것에서 벗어나 변화하는 세계 상태(Evolving State of the World)를 추정하는 방향으로 전환하도록 합니다. 카메라(Cameras), 라이다(LiDAR), 레이더(Radar), 고유수용감각 및 기타 센서는 완전한 현실이 아니라 부분적인 관찰을 제공합니다. 로봇(Robot)은 이러한 측정값을 이전 상태, 학습된 동역학(Learned Dynamics), 맥락, 불확실성과 통합하여 계획(Planning)과 제어(Control)를 지원할 수 있는 일관된 표현을 추론해야 합니다.

따라서 추론으로서의 지각(Perception as Inference)은 지각을 설명을 구성하고 검증하는 능동적 과정(Active Process)으로 설명합니다. 감각 증거는 가능한 해석을 제약하고, 사전 지식은 기대를 제공하며, 정밀도는 이들의 상대적 영향력을 조절하고, 예측 오차는 불일치를 드러냅니다. 기억은 학습된 구조를 제공하고 행동은 추가적인 증거를 수집합니다. 이러한 지속적인 추론 과정을 통해 지능형 시스템(Intelligent Systems)은 불확실한 감각 신호를 세계의 숨겨진 원인과 변화하는 상태에 관한 유용한 믿음(Useful Beliefs)으로 변환할 수 있습니다.

## 04.05 Active Inference [w/Code]

![](images/image6.png){width="7.268055555555556in" height="7.268055555555556in"}

![](images/image7.png){width="7.268055555555556in" height="7.268055555555556in"}

능동 추론(Active Inference)은 지능을 가진 생물체가 감각 입력(Sensory Input)을 지속적으로 예측하고, 관찰 결과가 예상되거나 선호되는 상태(Expected or Preferred States)와 일치하도록 행동함으로써 생존 가능한 상태(Viable States)를 유지하는 방식을 이해하기 위한 프레임워크입니다. 이는 예측 처리(Predictive Processing)를 지각을 넘어 행동까지 확장합니다. 생물체는 내부 믿음(Internal Beliefs)을 변화시키는 것뿐만 아니라 행동을 통해 세계를 변화시킴으로써도 예측 오차(Prediction Error)를 줄일 수 있습니다. 이를 통해 통합된 지각-행동 순환(Perception--Action Cycle)이 형성됩니다.

핵심적인 구분은 지각적 추론(Perceptual Inference)과 능동 추론(Active Inference) 사이에 있습니다. 지각적 추론은 감각 증거(Sensory Evidence)가 기대와 다를 때 내부 믿음을 갱신하는 반면, 능동 추론은 미래의 감각 관찰(Future Sensory Observations)을 변화시키는 행동을 선택합니다. 세계가 중요한 예측과 일치하지 않는다면 시스템은 자신의 모델을 수정하거나, 예상된 상태가 실제로 발생할 가능성이 높아지도록 행동할 수 있습니다.

내부 생성 모델(Internal Generative Models)은 이러한 과정에 필요한 구조를 제공합니다. 생성 모델은 숨겨진 환경 상태(Hidden Environmental States), 감각 관찰(Sensory Observations), 행동(Actions), 시간에 따른 예상 전이(Expected Transitions) 사이의 관계를 표현합니다. 뇌는 이러한 모델을 이용하여 서로 다른 조건에서 무엇을 관찰하게 될지를 예측하고, 특정 행동 이후 어떤 감각적 결과(Sensory Consequences)가 발생할 가능성이 높은지를 예상함으로써 행동을 선행적으로 안내할 수 있습니다.

예측 오차(Prediction Error)는 여전히 중요하지만, 능동 추론은 오차를 해결할 수 있는 방법을 확장합니다. 수동적 지각(Passive Perception)에서는 불일치가 주로 믿음 갱신(Belief Updating)을 유도합니다. 능동 추론에서는 일부 불일치가 감각 입력 자체를 변화시키는 행동을 유도할 수 있습니다. 불확실한 객체를 바라보거나, 자세히 살펴보기 위해 가까이 이동하거나, 원하는 물체에 손을 뻗거나, 신체 자세를 수정하는 행동은 모두 관찰 결과가 예측을 더 잘 충족하거나 불확실성을 감소시키도록 변화시킬 수 있습니다.

따라서 선호 상태(Preferred States)는 모든 예측된 미래가 동일하게 바람직한 것은 아니기 때문에 중요합니다. 생물학적 시스템(Biological Systems)은 신체적 온전성(Bodily Integrity), 체온(Temperature), 에너지(Energy), 안전(Safety), 사회적 조건(Social Conditions), 목표 달성(Goal Achievement)과 관련된 기대를 유지합니다. 이러한 기대는 생물체가 어떤 미래 상태를 추구하는지에 영향을 줍니다. 따라서 행동은 감각 및 생리적 상태를 생물체가 존재할 것으로 기대하는 범위로 이동시키는 과정으로 해석할 수 있습니다.

능동 추론은 항상성(Homeostasis)과 알로스타시스(Allostasis)에 대한 관점도 제공합니다. 항상성은 중요한 생리적 변수(Physiological Variables)를 생존 가능한 범위 내에서 유지하는 반면, 알로스타시스는 미래의 요구를 예상하여 심각한 편차가 발생하기 전에 행동이나 내부 조절을 변화시킵니다. 예측하는 생물체는 심각한 불균형이 발생할 때까지 기다릴 필요가 없으며, 발생할 가능성이 높은 변화를 예상하고 안정적인 기능을 유지하기 위해 사전에 행동할 수 있습니다.

불확실성(Uncertainty)은 에이전트(Agent)가 현재의 관찰을 발생시킨 숨겨진 상태(Hidden State)가 정확히 무엇인지 알지 못하는 경우가 많기 때문에 중요한 역할을 합니다. 따라서 행동은 부분적으로 정보적 가치(Informational Value)를 기준으로 선택될 수 있습니다. 머리를 돌리거나, 센서를 움직이거나, 객체에 접근하거나, 익숙하지 않은 영역을 탐색하면 서로 경쟁하는 가설(Competing Hypotheses)을 구분할 수 있는 관찰을 생성할 수 있습니다. 이러한 행동은 불확실성을 감소시키고 이후의 추론을 개선합니다.

이러한 정보 탐색 행동(Information-Seeking Behavior)은 능동 추론과 능동적 지각(Active Perception)을 연결합니다. 지각은 우연히 들어오는 정보만을 해석하는 과정으로 제한되지 않습니다. 생물체는 어디를 바라볼지, 무엇을 만질지, 어떻게 움직일지, 환경의 어떤 부분을 관찰할지를 제어할 수 있습니다. 따라서 행동은 내부 예측을 검증하는 실험(Experiments)이 되며, 지각과 행동이 협력하여 세계에 대한 내부 모델(Internal Model)을 개선할 수 있도록 합니다.

정밀도 가중(Precision Weighting)은 어떤 예측 오차가 추론과 행동에 영향을 주어야 하는지를 결정하는 데 도움을 줍니다. 신뢰할 수 있는 감각 증거는 부정확한 예측에 강하게 영향을 주어야 하지만, 불확실하거나 잡음이 많은 관찰에는 상대적으로 낮은 영향력이 부여될 수 있습니다. 주의(Attention)는 이러한 실질적인 정밀도 추정(Effective Precision Estimates)을 변화시켜 목표, 잠재적 위협, 새로움(Novelty), 해결되지 않은 불확실성과 관련된 신호를 우선적으로 처리하고 덜 유용한 불일치에 사용되는 처리를 감소시킬 수 있습니다.

능동 추론은 계층적(Hierarchical)으로도 작동합니다. 높은 수준에서는 목표(Goals), 맥락(Contexts), 의도(Intentions), 예상되는 미래 상황(Expected Future Situations)을 표현할 수 있는 반면, 낮은 수준에서는 즉각적인 감각 및 운동 상태(Sensory and Motor States)를 표현합니다. 따라서 높은 수준의 기대는 낮은 수준의 행동을 안내할 수 있고, 낮은 수준의 예측 오차는 해당 행동이 성공하고 있는지를 알려줄 수 있습니다. 이러한 조직은 추상적인 목표(Abstract Goals)를 구체적인 움직임과 순간적인 감각 피드백에 연결합니다.

시간(Time)은 행동이 즉각적인 효과만이 아니라 예상되는 미래 결과(Expected Future Consequences)를 기준으로 선택되기 때문에 필수적입니다. 에이전트는 여러 가능한 행동 시퀀스(Action Sequences)를 고려하고 각각의 행동과 관련된 관찰 결과를 예측할 수 있습니다. 이후 행동은 유용한 정보를 생성하는 동시에 선호 상태로 이어질 것으로 예상되는 정책(Policies)을 우선할 수 있습니다. 따라서 계획(Planning)은 미래 궤적(Future Trajectories)에 대한 예측과 밀접하게 연결됩니다.

기억(Memory)은 예측을 생성할 수 있는 학습된 규칙성(Learned Regularities)과 이전 경험을 제공함으로써 능동 추론에 기여합니다. 피질 지식(Cortical Knowledge)은 일반화된 기대를 제공할 수 있고, 해마 기억(Hippocampal Memories)은 특정 맥락에 해당하는 경험을 제공할 수 있습니다. 따라서 과거의 성공과 실패는 가능한 행동의 결과에 대한 믿음에 영향을 주며, 능동 추론이 모든 상황을 처음부터 완전히 새롭게 평가하지 않고 이전 경험을 재사용하도록 합니다.

능동 추론은 강화학습(Reinforcement Learning)과 중요한 유사성을 가지지만 두 프레임워크가 동일한 것은 아닙니다. 강화학습은 일반적으로 보상(Rewards), 가치 함수(Value Functions), 기대 수익(Expected Return)을 최대화하는 정책을 통해 행동을 설명합니다. 반면 능동 추론은 확률적 믿음(Probabilistic Beliefs), 선호되는 관찰(Preferred Observations), 불확실성, 예측을 강조합니다. 두 접근법 모두 적응적 행동 선택(Adaptive Action Selection)을 다루며, 실제 지능형 시스템에서는 두 관점의 아이디어를 결합할 수 있습니다.

이 프레임워크는 로보틱스(Robotics)와 체화 인공지능(Embodied AI)에 특히 중요합니다. 로봇(Robot)은 카메라(Cameras), 라이다(LiDAR), 고유수용감각(Proprioception), 기타 센서에서 불완전한 관찰을 받아들이면서 동시에 자신의 움직임을 통해 이러한 관찰을 지속적으로 변화시킵니다. 로봇은 숨겨진 세계 상태에 관한 믿음을 유지하고, 후보 행동(Candidate Actions)의 결과를 예측하며, 더 유용한 측정값을 획득하기 위해 움직이고, 관찰이 기대와 모순될 때 내부 모델을 수정할 수 있습니다.

예를 들어 자율 로봇(Autonomous Robot)이 특정 경로의 주행 가능 여부(Traversability)를 확신하지 못한다면, 불확실한 지각 결과를 수동적으로 받아들이는 대신 더 좋은 시점(Viewpoint)을 확보하기 위해 능동적으로 이동할 수 있습니다. 새로운 관찰은 경로를 결정하기 전에 지형(Terrain), 장애물(Obstacles), 기하 구조(Geometry)에 대한 불확실성을 줄일 수 있습니다. 따라서 능동 추론은 지능형 센싱(Intelligent Sensing), 탐색(Exploration), 상태 추정(State Estimation), 계획, 제어(Control)를 서로 분리된 모듈이 아니라 상호작용하는 과정으로 다루어야 한다는 관점을 제공합니다.

인공지능(Artificial Intelligence)의 관점에서 이와 관련된 원리는 월드 모델(World Models), 모델 기반 제어(Model-Based Control), 확률적 계획(Probabilistic Planning), 정보 탐색형 탐험(Information-Seeking Exploration), 불확실성 인식 의사결정(Uncertainty-Aware Decision Making)에서 나타납니다. 인공 에이전트는 서로 다른 행동에 따른 미래의 관찰을 예측하고, 과제 목표(Task Objectives)를 달성하면서 동시에 자신의 지식을 향상시키는 행동을 선택할 수 있습니다. 이는 관찰이 부분적이고 물리적 세계에서의 실수 비용이 높은 경우 특히 중요합니다.

따라서 능동 추론(Active Inference)은 예측하는 뇌(Predictive Brain)를 단순히 관찰을 설명하는 시스템에서 미래의 관찰을 능동적으로 형성하는 시스템으로 확장합니다. 내부 모델은 기대를 생성하고, 예측 오차는 불일치를 드러내며, 정밀도(Precision)는 그 중요성을 조절하고, 행동은 증거를 수집하거나 선호 상태를 만들어냅니다. 새로운 관찰은 다시 믿음을 갱신합니다. 이러한 지속적인 순환을 통해 지각(Perception), 학습(Learning), 계획(Planning), 행동(Action)은 하나의 통합된 적응 과정(Adaptive Process)을 구성합니다.

## 04.06 Free Energy Principle [w/Code]

![](images/image8.png){width="7.268055555555556in" height="7.268055555555556in"}

자유 에너지 원리(Free Energy Principle)는 생명 시스템(Living Systems)이 감각 관찰(Sensory Observations)의 원인에 대한 불확실성(Uncertainty)을 지속적으로 감소시킴으로써 제한된 범위의 생존 가능한 상태(Viable States)를 유지한다고 제안합니다. 신경과학(Neuroscience)에서 이 원리는 지각(Perception), 학습(Learning), 행동(Action), 생물학적 자기 유지(Biological Self-Maintenance)를 연결하는 수학적 프레임워크(Mathematical Framework)를 제공합니다. 적응적 생물체는 신체와 환경의 숨겨진 상태(Hidden States)가 만들어내는 감각적 결과를 예측하는 내부 생성 모델(Internal Generative Models)을 유지한다고 설명합니다.

이 프레임워크에서 자유 에너지(Free Energy)라는 용어는 일반적인 물리적 에너지 소비(Physical Energy Consumption)와 직접적으로 혼동해서는 안 됩니다. 변분 자유 에너지(Variational Free Energy)는 감각적 놀람(Sensory Surprise)의 상한(Upper Bound)을 제공하는 수학적 양이며, 여기서 놀람은 특정 감각 상태를 모델 아래에서 관찰할 음의 로그 확률(Negative Log Probability)을 의미합니다. 생물체는 가능한 모든 관찰의 확률을 직접 계산할 수 없기 때문에 변분 자유 에너지를 최소화하는 것은 놀람을 감소시키는 과정을 근사할 수 있는 계산 가능한 방법을 제공합니다.

감각적 놀람(Sensory Surprise)은 주관적으로 놀라는 경험을 의미하지 않습니다. 이는 생물체의 생성 모델(Generative Model)을 기준으로 특정 관찰이 얼마나 발생 가능성이 낮은지를 설명합니다. 오랜 시간 지속되는 생물학적 시스템은 극단적인 체온이나 심각한 에너지 불균형과 같이 발생 가능성이 매우 낮은 생리적 상태(Physiological States)에 장기간 머무르는 것을 피해야 합니다. 따라서 생물체의 조직 자체가 암묵적으로 자신이 존재할 가능성이 높은 상태와 그 상태에 관련된 감각 관찰의 범위를 제약합니다.

생성 모델(Generative Model)은 감각 관찰을 만들어낼 수 있는 숨겨진 원인(Hidden Causes)에 관한 가설을 표현합니다. 뇌는 환경이나 신체의 중요한 상태를 직접 관찰할 수 없는 경우가 많기 때문에 불완전한 증거로부터 이러한 상태를 추론해야 합니다. 숨겨진 상태가 어떻게 관찰을 생성하는지를 예측함으로써 시스템은 예상된 감각 신호(Expected Sensory Signals)를 실제 입력과 비교할 수 있습니다. 이러한 차이는 현재 경험의 원인에 대한 믿음을 개선하는 데 사용할 수 있는 정보를 제공합니다.

변분 추론(Variational Inference)은 이러한 과정의 계산적 기반을 제공합니다. 계산적으로 다루기 어려울 수 있는 모든 가능한 숨겨진 원인에 대한 정확한 사후 확률(Exact Posterior Probability)을 계산하는 대신, 시스템은 숨겨진 상태에 대한 근사 확률 분포(Approximate Probability Distribution)를 유지합니다. 학습과 추론은 이러한 근사값이 관찰된 데이터를 더욱 잘 설명하도록 조정합니다. 따라서 변분 자유 에너지를 최소화하면 내부 믿음(Internal Beliefs)과 감각 증거(Sensory Evidence) 사이의 대응 관계를 개선할 수 있습니다.

예측 오차(Prediction Error)는 자유 에너지 최소화(Free-Energy Minimization)와 예측 부호화(Predictive Coding)를 직관적으로 연결합니다. 예측된 감각 상태가 실제 관찰과 다를 때 예측 오차는 현재의 설명이 충분하지 않다는 것을 나타냅니다. 내부 표현(Internal Representations)을 갱신하면 이러한 불일치를 줄일 수 있습니다. 계층적 예측 처리(Hierarchical Predictive Processing)에서는 여러 수준에서 예측 오차가 발생할 수 있으며, 이를 통해 감각 특징, 객체, 맥락(Context), 더욱 추상적인 원인이 들어오는 증거에 따라 수정될 수 있습니다.

시스템이 관찰을 더 잘 설명하도록 내부 믿음을 변화시키면 지각을 통해 자유 에너지를 감소시킬 수 있습니다. 이러한 과정은 지각적 추론(Perceptual Inference)에 해당합니다. 예상하지 못한 감각 신호가 발생하면 시스템은 해당 신호를 발생시킨 원인에 대한 추정치를 수정할 수 있습니다. 반복적인 믿음 갱신(Belief Updating)은 사전 지식(Prior Knowledge)과 학습된 환경 구조의 제약을 유지하면서 이용 가능한 증거를 더욱 잘 설명하는 해석을 점진적으로 만들어냅니다.

자유 에너지는 행동(Action)을 통해서도 감소시킬 수 있습니다. 생물체는 자신의 믿음만을 변화시키는 대신 환경이나 신체에 행동하여 미래의 관찰이 예상된 상태와 더욱 일치하도록 만들 수 있습니다. 이는 자유 에너지 원리와 능동 추론(Active Inference)을 연결합니다. 지각은 관찰에 맞도록 모델을 변화시키는 반면, 행동은 생존 가능하거나 선호되는 조건(Viable or Preferred Conditions)과 관련된 예측에 더욱 잘 부합하도록 관찰 자체를 변화시킬 수 있습니다.

이러한 관계는 생물학적 조절(Biological Regulation)에서 특히 중요합니다. 생물체는 체온(Temperature), 에너지 가용성(Energy Availability), 수분 상태(Hydration), 신체적 온전성(Bodily Integrity)과 같은 변수를 제한된 범위 내에서 유지합니다. 이러한 상태에 관한 기대는 심각한 편차가 발생하기 전에 행동을 안내할 수 있습니다. 음식으로 이동하고, 위험을 피하며, 피난처를 찾거나, 자세를 교정하는 행동은 지속적인 생존에 필요한 예상된 감각 및 생리적 조건을 유지하기 위한 행동으로 해석할 수 있습니다.

불확실성(Uncertainty)은 생물체가 불완전한 관찰로부터 숨겨진 원인을 추론해야 하기 때문에 이 프레임워크의 핵심입니다. 따라서 내부 믿음은 완전히 확정된 결론이 아니라 확률적으로 표현됩니다. 정밀도(Precision)는 예측 또는 감각 증거의 추정된 신뢰성(Reliability)을 나타내며 이들의 상대적인 영향력을 조절합니다. 신뢰할 수 있는 예측 오차는 믿음을 강하게 갱신할 수 있는 반면, 불확실하거나 잡음이 많은 신호에는 추론과 행동에서 상대적으로 작은 영향력이 부여될 수 있습니다.

자유 에너지 원리(Free Energy Principle)는 탐색(Exploration)을 이해하기 위한 프레임워크도 제공합니다. 행동은 생물체를 선호되는 결과로 직접 이동시키는 것뿐만 아니라 불확실성을 감소시키는 정보를 획득할 수도 있습니다. 장애물 주변을 살펴보거나, 익숙하지 않은 객체에 접근하거나, 시점(Viewpoint)을 변경하면 서로 경쟁하는 가설을 구별할 수 있는 관찰을 얻을 수 있습니다. 따라서 정보 탐색 행동(Information-Seeking Behavior)은 생성 모델을 개선하고 이후 더욱 효과적인 의사결정(Decision Making)을 지원할 수 있습니다.

기대 자유 에너지(Expected Free Energy)는 이러한 개념을 현재의 관찰을 설명하는 것에서 가능한 미래 행동을 평가하는 것으로 확장합니다. 에이전트(Agent)는 여러 대안 정책(Alternative Policies)을 고려하고 각각의 예상 궤적(Predicted Trajectory)에 관련된 불확실성과 선호되는 결과를 추정할 수 있습니다. 바람직한 관찰을 만들어내는 동시에 숨겨진 상태에 관한 불확실성을 감소시킬 것으로 예상되는 정책이 우선될 수 있습니다. 따라서 계획(Planning)은 목표 지향적 행동(Goal-Directed Behavior)과 정보 수집(Information Gathering)을 하나의 공통된 예측 프레임워크 안에서 결합합니다.

학습(Learning)은 생성 모델 자체의 파라미터(Parameters)나 구조를 변화시키면서 더 느린 시간 척도(Slower Timescale)에서 발생합니다. 반복적인 예측 오차는 기존 표현이 충분히 포착하지 못하는 통계적 규칙성(Statistical Regularities)을 드러냅니다. 이후 시냅스 가소성(Synaptic Plasticity)과 기타 적응 메커니즘(Adaptive Mechanisms)이 모델을 수정하여 미래의 관찰을 더욱 쉽게 예측하도록 만들 수 있습니다. 이러한 방식으로 추론은 현재의 숨겨진 상태를 추정하고, 행동은 관찰을 변화시키며, 학습은 경험이 축적됨에 따라 모델 자체를 개선합니다.

인공지능(Artificial Intelligence)의 관점에서 이 프레임워크는 확률적 추론(Probabilistic Inference), 생성 모델링(Generative Modeling), 월드 모델(World Models), 불확실성 인식 계획(Uncertainty-Aware Planning), 체화 에이전트(Embodied Agents)와 개념적으로 연결됩니다. 로봇(Robot)은 부분적인 센서 정보로부터 숨겨진 환경 상태를 추론하고, 행동의 결과를 예측하며, 유용한 관찰을 능동적으로 수집하고, 예측이 실패하면 내부 동역학 모델(Internal Dynamics Model)을 갱신할 수 있습니다. 이러한 개념은 지능형 시스템이 정적인 입력만을 분류하는 것이 아니라 불확실성 속에서 지속적으로 작동해야 하는 경우 특히 중요합니다.

자유 에너지 원리(Free Energy Principle)는 매우 포괄적인 이론이므로 모든 신경 계산(Neural Computation)이 문자 그대로 하나의 동일한 최적화 알고리즘(Optimization Algorithm)을 수행한다는 증거로 이해해서는 안 됩니다. 이 원리의 가치는 예측(Prediction), 추론(Inference), 불확실성(Uncertainty), 행동(Action), 학습(Learning), 생물학적 조절(Biological Regulation)을 연결하는 공통된 수학적 언어를 제공한다는 데 있습니다. 현재의 예측 부호화 구조(Predictive-Coding Structure)에서 이 원리는 예측 처리를 능동 추론(Active Inference)과 미래의 적응 지능(Adaptive Intelligence)을 위한 계산 모델로 확장합니다.

## 04.07 Predictive Coding and Generative AI [w/Code]

![](images/image9.png){width="7.268055555555556in" height="7.268055555555556in"}

예측 부호화(Predictive Coding)와 생성형 인공지능(Generative AI)은 하나의 근본적인 아이디어를 공유합니다. 지능형 시스템(Intelligent Systems)은 입력을 고정된 레이블(Fixed Labels)에 단순히 대응시키는 것보다 관찰(Observations)이 어떻게 생성되는지를 모델링함으로써 유용한 표현(Useful Representations)을 학습할 수 있습니다. 예측 부호화는 기대(Expectations)를 생성하고 예측 오차(Prediction Errors)를 이용해 이를 수정하는 계층적 시스템(Hierarchical Systems)을 설명하는 반면, 생성형 인공지능은 복잡한 관찰을 생성, 복원, 예측 또는 변환할 수 있는 분포(Distributions)를 학습합니다.

예측 부호화(Predictive Coding)에서 내부 생성 모델(Internal Generative Model)은 잠재적 원인(Latent Causes)을 통해 감각 입력(Sensory Input)을 설명하려고 합니다. 높은 수준(Higher Levels)은 세계에 대한 점점 더 추상적인 가설(Hypotheses)을 표현하고 낮은 수준을 위한 예측을 생성합니다. 설명할 수 없는 관찰은 예측 오차를 발생시키며, 이는 표현을 갱신하기 위한 신호를 제공합니다. 따라서 학습은 예측된 정보와 관찰된 정보 사이의 체계적인 차이를 줄임으로써 모델을 개선합니다.

생성형 인공지능(Generative AI)은 데이터 내부의 통계적 구조(Statistical Structure)를 학습한다는 점에서 이와 관련된 계산적 관점(Computational Perspective)을 따릅니다. 관찰이 어떤 범주(Category)에 속하는지만 결정하는 대신, 생성 모델(Generative Model)은 관찰이 발생할 가능성을 결정하는 관계를 포착하려고 합니다. 이러한 관계가 학습되면 모델은 새로운 샘플을 생성하고, 불완전한 데이터를 복원하며, 잠재 변수(Latent Variables)를 추론하고, 누락된 정보를 예측하거나 하나의 표현을 다른 표현으로 변환할 수 있습니다.

잠재 표현(Latent Representations)을 고려하면 이러한 유사성은 더욱 명확해집니다. 이미지, 소리, 언어와 같은 감각 관찰은 방대한 세부 정보를 포함하지만, 많은 변화는 상대적으로 적은 수의 기저 요인(Underlying Factors)으로부터 발생합니다. 예측 시스템은 관찰을 설명하기 위해 이러한 숨겨진 원인(Hidden Causes)을 추론합니다. 생성 모델도 마찬가지로 다양한 관찰 가능한 패턴을 생성할 수 있는 구조를 부호화하는 잠재 표현 또는 분산 표현(Distributed Representations)을 학습합니다.

변분 오토인코더(Variational Autoencoder, VAE)는 이러한 관계를 명시적으로 보여주는 하나의 사례입니다. VAE는 관찰을 복원하거나 생성할 수 있는 잠재 확률 분포(Latent Probability Distribution)를 학습합니다. 인코더(Encoder)는 관찰된 데이터로부터 잠재 원인을 근사하고, 디코더(Decoder)는 이러한 잠재 변수가 어떻게 관찰을 생성할 수 있는지를 모델링합니다. 추론과 생성 사이의 이러한 상호작용은 숨겨진 상태를 추론하고 그 감각적 결과를 예측하는 예측 처리(Predictive Processing)의 보다 광범위한 구분과 유사합니다.

예측 오차(Prediction Error)는 생성 모델 학습(Generative-Model Training)에서도 유사한 개념을 가집니다. 모델은 관찰 또는 그 기저 분포(Underlying Distribution)에 대한 추정값을 생성하고, 예측과 데이터 사이의 불일치에 기반하여 학습 신호(Learning Signal)를 받습니다. 정확한 목적 함수(Objective)는 아키텍처마다 다르지만 일반적인 원리는 중요합니다. 불일치는 모델이 포착하지 못한 부분을 드러내고, 최적화(Optimization)는 미래의 예측이 학습 분포(Training Distribution)의 통계적 규칙성을 더욱 잘 반영하도록 파라미터를 수정합니다.

확산 모델(Diffusion Models)은 반복적 복원(Iterative Reconstruction)을 통해 이러한 원리를 보여줍니다. 학습 과정에서 데이터는 점진적으로 잡음(Noise)에 의해 손상되고, 모델은 이러한 손상을 역으로 되돌리는 데 필요한 정보를 예측하도록 학습합니다. 생성은 잡음에서 시작하여 구조화된 샘플(Structured Samples)에 가까워지는 추정값을 반복적으로 만들어냅니다. 이는 생물학적 예측 부호화와 동일하지 않지만, 두 접근법 모두 반복적인 예측과 수정(Iterative Prediction and Correction)을 통해 불확실한 신호에서 일관된 표현을 구성할 수 있음을 보여줍니다.

자기회귀 생성 모델(Autoregressive Generative Models)은 시간적 예측(Temporal Prediction)을 통해 또 다른 연결점을 제공합니다. 예를 들어 언어 모델(Language Model)은 이전 맥락(Preceding Context)을 바탕으로 이후의 토큰(Subsequent Tokens)을 예측하도록 학습합니다. 학습 과정의 예측 오차는 조건부 분포(Conditional Distributions)가 언어의 패턴을 더욱 잘 표현하도록 모델을 수정합니다. 아키텍처와 학습 메커니즘은 생물학적 예측 부호화와 다르지만, 예측 자체가 강력한 자기 생성 학습 목표(Self-Generated Training Objective)가 됩니다.

이러한 연결은 예측이 자기지도 학습(Self-Supervised Learning)을 지원할 수 있는 이유를 설명합니다. 미래의 관찰(Future Observations), 마스킹된 구성요소(Masked Components), 손상된 입력(Corrupted Inputs), 시퀀스의 인접 요소(Neighboring Elements)는 사람이 직접 만든 레이블 없이 학습 목표를 제공할 수 있습니다. 모델은 누락되거나 미래의 정보를 예측 가능하게 만드는 구조를 발견해야 합니다. 따라서 예측 목표(Predictive Objectives)는 객체, 의미(Semantics), 시간적 의존성(Temporal Dependencies), 맥락적 관계(Contextual Relationships), 잠재 요인(Latent Factors)에 관한 표현의 학습을 촉진할 수 있습니다.

계층적 표현(Hierarchical Representation)은 또 하나의 중요한 연결점입니다. 예측 부호화는 낮은 수준에서 비교적 국소적인 감각 속성을 모델링하고 높은 수준에서 점점 더 추상적인 원인과 맥락을 표현한다고 제안합니다. 심층 생성 시스템(Deep Generative Systems) 역시 여러 계산 계층(Computational Layers)에 걸쳐 변환을 조직합니다. 낮은 수준의 표현은 국소적인 패턴을 포착할 수 있는 반면, 깊은 수준의 표현은 더 광범위한 구조, 의미, 관계 또는 입력의 넓은 범위에 걸친 의존성을 부호화할 수 있습니다.

하향식 생성(Top-Down Generation)은 이러한 비교에서 특히 중요합니다. 예측 부호화에서 높은 수준의 가설은 낮은 수준의 활동에 대한 기대를 생성합니다. 생성형 인공지능에서는 잠재 표현이나 맥락 상태(Contextual States)가 이미지, 텍스트, 오디오, 비디오 또는 기타 데이터와 같은 관찰 가능한 출력(Observable Outputs)으로 변환될 수 있습니다. 두 관점 모두 내부 표현이 해당 표현과 연관된 관찰을 설명하거나 생성할 수 있기 때문에 유용하다는 점을 강조합니다.

그러나 생성형 인공지능(Generative AI)을 생물학적 예측 부호화(Biological Predictive Coding)의 직접적인 구현으로 설명해서는 안 됩니다. 현대 생성 시스템은 일반적으로 역전파(Backpropagation), 대규모 데이터셋(Large Datasets), 트랜스포머 아키텍처(Transformer Architectures), 확산 목적 함수(Diffusion Objectives), 변분 방법(Variational Methods), 적대적 학습(Adversarial Learning) 등을 사용합니다. 반면 신경 예측 처리(Neural Predictive Processing)는 순환적 피질 상호작용(Recurrent Cortical Interactions), 국소 신경 동역학(Local Neural Dynamics), 정밀도 가중(Precision Weighting), 생물학적 가소성(Biological Plasticity)을 포함할 수 있습니다. 따라서 두 분야의 관계는 문자 그대로 동일한 구현이라기보다 개념적이고 계산적인 관계입니다.

생성 모델(Generative Models)은 추론(Inference)을 위한 도구로도 해석할 수 있습니다. 시스템이 숨겨진 변수가 어떻게 관찰을 생성하는지를 학습했다면, 반대 방향으로 추론하여 관찰된 증거로부터 숨겨진 원인을 추정할 수 있습니다. 이는 생성 모델링(Generative Modeling)을 추론으로서의 지각(Perception as Inference)과 연결합니다. 인식(Recognition)은 단순히 레이블을 할당하는 것을 넘어 어떤 내부 설명(Internal Explanation)이 이용 가능한 관찰을 그럴듯하게 설명할 수 있는지를 판단하는 과정이 됩니다.

불확실성(Uncertainty)은 이러한 관점을 특히 중요하게 만듭니다. 결정론적 분류기(Deterministic Classifier)는 하나의 답을 출력할 수 있지만, 확률적 생성 모델(Probabilistic Generative Model)은 여러 가능한 설명이나 미래를 표현할 수 있습니다. 관찰이 불완전하면 여러 잠재 상태(Latent States)가 동시에 가능한 상태로 남을 수 있습니다. 가능성에 대한 분포를 유지하면 지능형 시스템은 하나의 해석을 성급하게 선택하는 대신 모호성(Ambiguity)을 표현할 수 있습니다.

다중모달 생성형 인공지능(Multimodal Generative AI)은 이러한 개념을 서로 다른 정보 형태로 확장합니다. 이미지, 언어, 오디오, 비디오, 행동(Actions), 센서 측정값(Sensor Measurements)은 공유되거나 상호작용하는 표현을 통해 모델링될 수 있습니다. 하나의 감각 양식(Modality)에서 얻은 정보는 다른 감각 양식의 예측을 제약할 수 있습니다. 이는 높은 수준의 가설이 공통된 잠재 원인(Common Latent Causes)을 통해 여러 감각 흐름을 설명할 수 있다는 계층적 예측 처리(Hierarchical Predictive Processing)와 유사합니다.

생성적 예측(Generative Prediction)은 월드 모델(World Models)을 위한 중요한 기반도 제공합니다. 모델은 고립된 샘플을 생성하는 것을 넘어 상태가 시간에 따라 어떻게 변화하고 행동이 미래의 관찰에 어떤 영향을 주는지를 학습할 수 있습니다. 현재 내부 상태(Current Internal State)와 후보 행동(Candidate Action)이 주어지면 시스템은 가능한 미래 상태(Future States)를 예측할 수 있습니다. 이러한 모델을 통해 인공 에이전트(Artificial Agents)는 물리적 환경과 실제로 상호작용하기 전에 내부적으로 결과를 시뮬레이션할 수 있습니다.

이러한 전환은 체화 인공지능(Embodied AI)과 피지컬 AI(Physical AI)에 특히 중요합니다. 로봇(Robot)은 단순히 픽셀이나 언어 토큰만을 예측하는 것이 아니라 객체의 움직임(Object Motion), 접촉(Contact), 기하 구조(Geometry), 주행 가능성(Traversability), 인간 행동(Human Behavior), 자신의 행동이 만들어낼 결과를 추정해야 할 수 있습니다. 생성 모델은 가능한 미래의 관찰을 표현할 수 있으며, 예상 결과와 실제 결과 사이의 예측 오차는 로봇의 내부 모델이 부정확한 부분을 드러낼 수 있습니다.

능동적 지각(Active Perception)은 또 다른 연결점을 제공합니다. 생성 모델이 불확실한 관찰에 대해 여러 가능한 설명을 표현한다면, 에이전트는 이들을 구별할 수 있는 정보를 생성하는 행동을 선택할 수 있습니다. 카메라(Camera)를 움직이거나, 객체에 접근하거나, 시점(Viewpoint)을 변경하거나, 환경과 물리적으로 상호작용하면 생성과 추론을 수동적인 예측 작업이 아니라 능동적인 지각-행동 순환(Perception--Action Loop)으로 전환할 수 있습니다.

따라서 생성형 인공지능(Generative AI)은 경험을 설명하고 예측할 수 있는 모델이 지능에 유용하다는 보다 광범위한 원리와 관련된 하나의 계산적 방향으로 볼 수 있습니다. 예측 부호화(Predictive Coding)는 예측, 계층적 추론(Hierarchical Inference), 오차 수정(Error Correction)을 강조하는 반면, 현대 생성형 인공지능은 복잡한 분포를 학습하고 관찰을 생성하기 위한 확장 가능한 방법(Scalable Methods)을 제공합니다. 두 접근법의 메커니즘은 다르지만, 모두 내부 모델링(Internal Modeling)을 지능적 표현의 중심에 둡니다.

이러한 연결은 기존 생성 시스템을 넘어서는 미래의 발전 방향도 제시합니다. 미래의 에이전트(Future Agents)는 생성 모델에 지속적 기억(Persistent Memory), 불확실성 추정(Uncertainty Estimation), 지속 학습(Continual Learning), 다중모달 지각(Multimodal Perception), 행동 조건부 예측(Action-Conditioned Prediction), 온라인 모델 갱신(Online Model Updating)을 결합할 수 있습니다. 이러한 시스템은 프롬프트가 제공될 때 콘텐츠만 생성하는 것을 넘어 환경 상태를 지속적으로 예측하고, 기대와 관찰을 비교하며, 지속적인 상호작용을 통해 내부 표현을 수정할 수 있습니다.

따라서 예측 부호화(Predictive Coding)와 생성형 인공지능(Generative AI)은 관찰의 이면에 존재하는 숨겨진 구조(Hidden Structure)를 포착하는 모델을 학습한다는 아이디어에서 만납니다. 예측은 이러한 모델을 검증하고, 불일치(Discrepancies)는 개선에 필요한 정보를 제공하며, 잠재 표현(Latent Representations)은 설명 가능한 구조를 부호화하고, 생성(Generation)은 모델이 관찰이 어떤 모습일 것으로 기대하는지를 보여줍니다. 이러한 연결은 생성 모델링에서 월드 모델(World Models), 시간적 예측(Temporal Prediction), 체화 지능(Embodied Intelligence), 적응형 인공지능 시스템(Adaptive AI Systems)으로 자연스럽게 이어집니다.

## 04.08 World Models and Prediction [w/Code]

![](images/image10.png){width="7.268055555555556in" height="7.268055555555556in"}

월드 모델(World Models)은 지능형 시스템(Intelligent System)이 환경이 어떻게 구성되어 있으며 시간이 지남에 따라 어떻게 변화할 수 있는지를 추정하도록 하는 내부 표현(Internal Representations)입니다. 에이전트(Agent)는 현재의 관찰에만 반응하는 대신 상태(States), 관계(Relationships), 동역학(Dynamics), 불확실성(Uncertainty)을 부호화하고 이를 이용해 가능한 미래를 예측할 수 있습니다. 따라서 예측(Prediction)은 지각(Perception), 기억(Memory), 계획(Planning), 행동(Action)을 연결하는 핵심 기능이 됩니다.

월드 모델(World Model)은 일반적으로 관찰(Observations)과 그 기저에 존재하는 상태(Underlying States)를 구분합니다. 센서(Sensors)는 이미지, 소리, 위치, 힘과 같은 부분적인 측정값을 제공하지만 실제 환경 상태(True State of the Environment)는 일부만 관찰 가능할 수 있습니다. 따라서 모델은 모든 감각적 세부 사항을 단순히 재현하는 것이 아니라 미래 예측, 행동, 의사결정(Decision Making)에 필요한 정보를 보존하는 압축된 내부 상태(Compact Internal State)를 추론해야 합니다.

상태 표현(State Representations)은 문제에 따라 여러 형태를 가질 수 있습니다. 학습된 잠재 표현(Learned Latent Representations), 기하학적 지도(Geometric Maps), 구조화된 기호적 기술(Structured Symbolic Descriptions), 의미적 표현(Semantic Representations), 또는 이러한 접근법의 조합이 사용될 수 있습니다. 효과적인 표현은 복잡한 관찰을 압축하면서 객체(Objects), 공간적 관계(Spatial Relationships), 움직임(Motion), 물리적 속성(Physical Properties), 목표(Goals), 그리고 미래의 환경 변화를 예측하는 데 필요한 기타 변수에 관한 정보를 보존합니다.

동역학 모델(Dynamics Model)은 상태가 시간에 따라 어떻게 변화하는지를 예측하는 구성요소입니다. 현재 상태(Current State)와 경우에 따라 행동(Action)이 주어지면 다음 상태 또는 미래 상태의 시퀀스(Sequence of Future States)를 추정합니다. 개념적으로 이러한 관계는 현재 상태와 행동에서 미래 상태로의 전이(Transition)로 표현할 수 있습니다. 유용한 동역학을 학습하면 에이전트는 움직임, 상호작용(Interactions), 환경 변화(Environmental Changes), 행동의 결과를 실제로 발생하기 전에 예측할 수 있습니다.

예측(Prediction)은 관찰 공간(Observation Space)에서 직접 수행되거나 잠재 상태 공간(Latent State Space)에서 수행될 수 있습니다. 미래의 이미지나 센서 측정값을 예측하면 세부적인 학습 신호를 제공할 수 있지만, 고차원 관찰(High-Dimensional Observations)에는 관련성이 낮은 세부 정보가 많이 포함됩니다. 반면 잠재 예측(Latent Prediction)은 압축된 과제 관련 구조(Task-Relevant Structure)에 집중합니다. 따라서 많은 실용적인 월드 모델은 잠재 동역학(Latent Dynamics)을 상세한 출력이 필요할 때 감각 신호를 복원하거나 예측하는 관찰 모델(Observation Models)과 결합합니다.

월드 모델은 여러 가능한 미래(Multiple Possible Futures)를 시뮬레이션할 수 있을 때 특히 강력해집니다. 하나의 결정론적 결과(Deterministic Outcome)만 예측하는 대신 에이전트는 대안 행동(Alternative Actions), 불확실한 환경 변화, 다른 에이전트의 서로 다른 행동을 나타내는 여러 궤적(Trajectories)을 전개할 수 있습니다. 이러한 상상된 미래(Imagined Futures)는 실제 환경에서 행동을 실행하기 전에 그 결과를 평가할 수 있는 계산적 공간(Computational Space)을 제공합니다.

실제 환경은 부분적으로만 예측 가능하기 때문에 불확실성(Uncertainty)을 표현해야 합니다. 센서 잡음(Sensor Noise), 숨겨진 변수(Hidden Variables), 불완전한 지식(Incomplete Knowledge), 확률적 사건(Stochastic Events), 다른 에이전트의 행동으로 인해 동일한 현재 상태에서도 여러 가능한 미래가 발생할 수 있습니다. 확률적 예측(Probabilistic Predictions)과 신뢰도 추정(Confidence Estimates)을 통해 시스템은 발생 가능성이 높은 결과와 불확실한 가능성을 구분하고 위험(Risk)을 계획, 제어(Control), 안전 관련 의사결정에 반영할 수 있습니다.

예측 오차(Prediction Error)는 월드 모델을 개선하기 위한 주요 피드백을 제공합니다. 시스템이 미래 상태 또는 관찰을 예측한 후 실제 결과를 예측과 비교할 수 있습니다. 지속적인 불일치(Persistent Discrepancies)는 상태 표현, 동역학, 관찰 모델링(Observation Modeling), 불확실성 추정(Uncertainty Estimation)의 약점을 나타냅니다. 이후 학습은 이러한 구성요소를 수정하여 다음 예측이 환경의 구조와 변화 과정을 더욱 정확하게 반영하도록 합니다.

예측은 월드 모델을 자기지도 학습(Self-Supervised Learning)과도 연결합니다. 미래의 관찰(Future Observations)은 명시적인 인간 레이블(Human Labels)이 없어도 자연스럽게 학습 목표를 제공합니다. 에이전트는 앞으로의 센서 상태, 객체의 움직임, 마스킹된 정보(Masked Information), 행동의 결과를 예측하고 이후 실제 관찰과 비교할 수 있습니다. 따라서 지속적인 상호작용(Continuous Interaction)은 자체적인 학습 신호를 생성하여 축적된 경험으로부터 표현과 동역학을 개선할 수 있게 합니다.

시간적 구조(Temporal Structure)는 유용한 월드 모델이 개별적인 상태 전이만을 표현해서는 안 되기 때문에 핵심적입니다. 물리적 및 행동적 과정은 빠른 접촉 동역학(Contact Dynamics)부터 객체 궤적(Object Trajectories), 내비게이션 에피소드(Navigation Episodes), 장기적인 과제 진행(Long-Term Task Progression)에 이르기까지 서로 다른 시간 척도(Timescales)에서 전개됩니다. 계층적 시간 모델(Hierarchical Temporal Models)은 단기적인 물리 예측을 더 느린 의미적 사건(Semantic Events), 목표, 계획과 연결하여 제어와 추론 모두에 적합한 표현을 제공할 수 있습니다.

체화된 에이전트(Embodied Agent)는 자신이 예측하는 세계를 능동적으로 변화시키기 때문에 행동(Actions)이 모델에 포함되어야 합니다. 행동 조건부 모델(Action-Conditioned Model)은 서로 다른 후보 행동(Candidate Actions)이 미래 상태에 어떤 영향을 주는지를 추정합니다. 동일한 환경도 로봇이 이동하고, 회전하고, 객체를 파지하고, 기다리거나, 다른 에이전트와 상호작용하는지에 따라 다르게 변화할 수 있습니다. 따라서 예측은 반사실적(Counterfactual)이 되며, 시스템은 서로 다른 행동을 선택하면 어떤 일이 발생할지를 질문할 수 있습니다.

반사실적 시뮬레이션(Counterfactual Simulation)은 에이전트가 실행 전에 대안적인 행동 시퀀스(Alternative Action Sequences)를 비교할 수 있게 함으로써 계획(Planning)을 지원합니다. 가능한 궤적은 목표(Goals), 비용(Cost), 위험(Risk), 제약조건(Constraints), 불확실성, 예상 결과(Expected Outcomes)를 기준으로 평가될 수 있습니다. 이후 에이전트는 예측된 미래가 가장 적절한 행동을 선택할 수 있습니다. 이러한 방식으로 월드 모델은 예측을 수동적인 미래 전망에서 목표 지향적 의사결정(Goal-Directed Decision Making)을 위한 메커니즘으로 전환합니다.

기억(Memory)은 현재의 관찰만으로 환경 상태를 결정하기에 충분하지 않을 수 있기 때문에 월드 모델링(World Modeling)과 밀접하게 연결됩니다. 이전 상태(Previous States), 일화적 경험(Episodic Experiences), 의미적 지식(Semantic Knowledge), 학습된 행동 패턴(Learned Action Patterns)은 추가적인 맥락을 제공할 수 있습니다. 기억을 통해 모델은 숨겨진 변수를 추론하고, 객체 연속성(Object Continuity)을 유지하며, 반복되는 상황을 인식하고, 부분 관찰 환경(Partially Observed Environments)에서 이전 경험을 활용하여 예측을 개선할 수 있습니다.

체화 시스템(Embodied Systems)에서는 에이전트 자체에 대한 모델도 중요합니다. 로봇(Robot)은 외부 환경뿐만 아니라 자신의 신체(Body), 운동학(Kinematics), 동역학(Dynamics), 센서, 에너지 자원(Energy Resources), 페이로드(Payload), 능력(Capabilities), 한계(Limitations)를 표현해야 합니다. 정확한 예측을 위해서는 에이전트 자신의 행동이 물리적 제약조건(Physical Constraints)과 어떻게 상호작용하는지를 이해해야 합니다. 따라서 월드 모델은 환경 모델(Environmental Model)뿐만 아니라 자기 모델(Self Model)의 일부도 포함하는 경우가 많습니다.

지능적인 상호작용(Intelligent Interaction)을 위해서는 다른 에이전트(Other Agents)에 대한 모델이 추가로 필요할 수 있습니다. 인간(Humans), 로봇, 자율 시스템(Autonomous Systems)은 미래 상태에 영향을 주는 목표, 믿음(Beliefs), 의도(Intentions), 행동 패턴(Behavioral Patterns)을 가지고 있습니다. 가능한 행동과 반응을 예측하면 협력(Cooperation), 협상(Negotiation), 충돌 회피(Collision Avoidance), 사회적 상호작용(Social Interaction), 다중 에이전트 협조(Multi-Agent Coordination)를 지원할 수 있습니다. 따라서 월드 모델은 물리적 동역학에서 행동적·사회적 동역학(Behavioral and Social Dynamics)으로 확장됩니다.

생성 모델링(Generative Modeling)은 가능한 미래를 표현하기 위한 유용한 메커니즘을 제공합니다. 생성형 월드 모델(Generative World Model)은 이전 상태와 행동을 조건으로 관찰 또는 잠재 상태를 예측할 수 있으며, 확률적 생성(Probabilistic Generation)을 통해 여러 가능한 궤적을 표현할 수 있습니다. 이는 월드 모델링을 생성형 인공지능(Generative AI)과 연결하지만, 유용한 월드 모델은 단순한 생성 그 자체보다 시간적 일관성(Temporal Consistency), 행동의 결과(Action Consequences), 상호작용에 대한 현실 기반 연결(Grounding in Interaction)을 강조해야 합니다.

월드 모델은 실제 세계에서의 시행착오(Trial-and-Error)가 느리고 비용이 많이 들거나 위험할 수 있기 때문에 로보틱스(Robotics)와 피지컬 AI(Physical AI)에 특히 중요합니다. 내부적으로 결과를 시뮬레이션할 수 있는 로봇은 실제 행동에 앞서 내비게이션 경로(Navigation Paths), 조작 전략(Manipulation Strategies), 접촉(Contact), 장애물(Obstacles), 실패 가능성(Failure Possibilities)을 평가할 수 있습니다. 따라서 예측은 동적 환경에서 데이터 효율성(Data Efficiency), 계획 품질(Planning Quality), 적응형 제어(Adaptive Control), 운영 안전성(Operational Safety)을 향상시킬 수 있습니다.

완전한 월드 모델 순환(World-Model Loop)은 지각(Perception), 예측(Prediction), 계획(Planning), 행동(Action), 관찰(Observation), 학습(Learning)을 통합합니다. 센서는 내부 상태를 갱신하고, 동역학 모델은 가능한 미래를 예측하며, 계획은 행동을 선택하고, 실행은 환경을 변화시키며, 새로운 관찰은 예측 오차를 드러냅니다. 이러한 오차는 다시 표현과 동역학을 갱신합니다. 그 결과 상호작용을 통해 예측이 지속적으로 개선되는 폐쇄형 인지 순환(Closed Cognitive Loop)이 형성됩니다.

따라서 월드 모델(World Models)과 예측(Prediction)은 수동적 패턴 인식(Passive Pattern Recognition)에서 적응형 지능(Adaptive Intelligence)으로 전환하기 위한 연결고리를 제공합니다. 숨겨진 상태를 표현하고, 동역학을 학습하며, 불확실성을 모델링하고, 대안적인 미래를 시뮬레이션하며, 행동의 결과를 통합함으로써 지능형 시스템은 실제 행동을 결정하기 전에 앞으로 어떤 일이 발생할 수 있는지를 추론할 수 있습니다. 이러한 능력은 상상(Imagination), 계획, 의사결정, 모델 기반 학습(Model-Based Learning), 제어, 변화하는 환경에 대한 강건한 적응(Robust Adaptation)을 지원합니다.

## 04.09 Temporal Prediction and State Transitions [w/Code]

![](images/image11.png){width="7.268055555555556in" height="7.268055555555556in"}

시간적 예측(Temporal Prediction)은 지능형 시스템(Intelligent System)이 현재 순간에 무엇이 존재하는지를 표현하는 것뿐만 아니라 상태(States)가 시간에 따라 어떻게 변화할 가능성이 있는지를 표현하도록 합니다. 시스템은 관찰(Observations)을 서로 분리된 스냅샷(Isolated Snapshots)으로 처리하는 대신 시퀀스(Sequences), 의존성(Dependencies), 상태 전이(State Transitions)를 모델링합니다. 이러한 시간적 구조(Temporal Structure)를 통해 지각(Perception)은 예측적 성격을 가지게 되며, 에이전트(Agent)는 사건이 직접 관찰되기 전에 이를 예상할 수 있습니다.

상태(State)는 특정 시점에서 예측과 행동에 관련된 정보를 나타내는 내부 표현(Internal Representation)입니다. 여기에는 감각 특징(Sensory Features), 객체 위치(Object Locations), 속도(Velocities), 관계(Relationships), 목표(Goals), 환경 조건(Environmental Conditions), 또는 관찰로부터 추론된 잠재 변수(Latent Variables)가 포함될 수 있습니다. 유용한 상태 표현(State Representation)의 목적은 모든 세부 정보를 반드시 보존하는 것이 아니라 시스템이 어떻게 변화할 수 있는지를 추정하는 데 충분한 정보를 유지하는 것입니다.

상태 전이(State Transitions)는 하나의 상태가 다른 상태로 어떻게 변화하는지를 설명합니다. 전이 모델(Transition Model)은 개념적으로 현재 상태(Current State)에서 다음 상태(Next State)로의 매핑으로 표현할 수 있으며, 흔히 행동(Action)을 조건으로 포함합니다. 체화 시스템(Embodied Systems)에서는 미래가 환경 동역학(Environmental Dynamics)뿐만 아니라 에이전트가 무엇을 하는지에도 의존하기 때문에 이러한 관계가 특히 중요합니다. 따라서 예측은 수동적인 변화와 행동 의존적 변화(Action-Dependent Change)를 모두 모델링해야 합니다.

시간적 예측은 서로 다른 예측 지평(Prediction Horizons)에서 작동할 수 있습니다. 단기 예측(Short-Term Prediction)은 수 밀리초에서 수 초 후에 발생할 일을 추정하여 운동 제어(Motor Control), 충돌 회피(Collision Avoidance), 즉각적인 상호작용을 지원할 수 있습니다. 장기 예측(Long-Term Prediction)은 내비게이션(Navigation), 조작(Manipulation), 과제(Task), 행동 계획(Behavioral Plans)에 걸친 시퀀스를 표현할 수 있습니다. 시간이 멀어질수록 세부적인 예측의 불확실성이 증가하기 때문에 서로 다른 지평에는 서로 다른 수준의 추상화(Abstraction)가 필요합니다.

마르코프 모델(Markov Models)은 다음 상태가 주로 현재 상태에 의존한다고 가정하는 간단한 형태를 제공합니다. 이러한 가정은 예측을 계산적으로 다루기 쉽게 만들 수 있지만, 실제 세계의 많은 과정은 더 먼 과거까지 이어지는 의존성을 포함합니다. 따라서 충분히 유용한 상태는 관련된 과거 정보를 요약해야 하며, 그렇지 않다면 모델이 더 긴 시간적 의존성(Long Temporal Dependencies)을 표현할 수 있는 명시적인 기억(Memory)을 유지해야 합니다.

순환 신경망(Recurrent Neural Networks)은 새로운 관찰이 들어올 때마다 변화하는 은닉 상태(Hidden States)를 유지함으로써 시간적 모델링(Temporal Modeling)을 확장합니다. LSTM(Long Short-Term Memory)과 GRU(Gated Recurrent Unit)와 같은 아키텍처는 시퀀스 전체에 걸쳐 정보를 유지하고 장기 의존성(Long-Term Dependencies)과 관련된 문제를 완화하도록 설계되었습니다. 이러한 은닉 표현(Hidden Representations)은 이전 관찰을 요약하여 미래 예측이 바로 직전의 입력뿐만 아니라 시간적 맥락(Temporal Context)에 의존하도록 합니다.

트랜스포머(Transformers)는 어텐션 메커니즘(Attention Mechanisms)을 이용하여 시퀀스 내 서로 다른 위치의 정보를 연결하는 또 다른 접근법을 제공합니다. 모든 이전 정보를 하나의 순환 상태(Recurrent State)로 압축하는 대신, 어텐션은 이전 관찰 중 관련된 요소를 선택적으로 참조할 수 있습니다. 이를 통해 장거리 의존성(Long-Range Dependencies)과 관계를 포착할 수 있지만, 시퀀스 길이가 증가함에 따라 계산 요구량(Computational Requirements)이 크게 증가할 수 있습니다.

상태공간 모델(State-Space Models)은 숨겨진 동역학(Hidden Dynamics)과 관찰(Observations)을 연결하는 구조화된 프레임워크를 제공합니다. 잠재 상태(Latent State)는 전이 과정(Transition Process)에 따라 변화하고, 관찰 모델(Observation Model)은 이러한 숨겨진 상태를 측정 가능한 신호로 변환합니다. 이러한 분리는 센서가 기저 시스템에 대해 불완전하거나 잡음이 있는 증거만 제공하는 경우 유용합니다. 예측은 잠재 공간(Latent Space)에서 수행되고, 관찰은 숨겨진 상태의 추정치를 지속적으로 수정할 수 있습니다.

전이가 결정론적(Deterministic)이 아니라 확률적(Stochastic)일 경우 예측은 더욱 어려워집니다. 동일한 현재 상태와 행동에서도 잡음(Noise), 알려지지 않은 변수(Unknown Variables), 환경 변화(Environmental Changes), 다른 에이전트의 영향 때문에 여러 미래 결과가 발생할 수 있습니다. 따라서 확률적 전이 모델(Probabilistic Transition Model)은 하나의 다음 상태만을 출력하는 대신 가능한 다음 상태에 대한 분포(Distribution)를 표현하여 미래 예측에 불확실성이 전파되도록 합니다.

다단계 예측(Multi-Step Prediction)은 전이 모델을 시간 방향으로 반복 적용하여 확장합니다. 예측된 다음 상태는 다시 그 이후 상태를 예측하기 위한 입력이 되어 상상된 궤적(Imagined Trajectory)을 생성합니다. 그러나 작은 오차가 반복적인 롤아웃(Rollout) 과정에서 누적되면 장기 예측(Long-Horizon Prediction)이 현실에서 점차 벗어날 수 있습니다. 따라서 강건한 시간 모델(Robust Temporal Models)은 불확실성을 관리하고, 새로운 관찰을 주기적으로 반영하며, 신뢰할 수 있는 근거리 예측과 점점 더 불확실해지는 장거리 미래를 구분해야 합니다.

계층적 시간 예측(Hierarchical Temporal Prediction)은 여러 시간 척도(Timescales)에서 동역학을 표현함으로써 이러한 문제를 해결하고자 합니다. 낮은 수준에서는 움직임(Motion), 접촉(Contact), 센서 변화(Sensor Variation)와 같은 빠른 변화를 예측할 수 있는 반면, 높은 수준에서는 하나의 기동(Maneuver)을 완료하거나 특정 위치에 도달하거나 과제를 완수하는 것과 같은 더 느린 사건을 표현할 수 있습니다. 계층적 추상화(Hierarchical Abstraction)는 장기간에 걸쳐 모든 저수준 세부 사항을 예측해야 할 필요를 줄이고 보다 효율적인 계획을 지원합니다.

시간적 추상화(Temporal Abstraction)는 시퀀스를 의미 있는 사건(Events)이나 기술(Skills)로 표현할 수도 있습니다. 에이전트는 수백 개의 개별 운동 명령(Motor Commands)을 예측하는 대신 접근(Approach), 파지(Grasp), 운반(Transport), 배치(Place)와 같은 상위 수준 전이를 기준으로 추론할 수 있습니다. 각 추상 상태(Abstract State)는 내부에 더 낮은 수준의 제어기(Controllers) 또는 예측 과정을 포함할 수 있습니다. 이러한 구조는 연속적인 물리 동역학(Continuous Physical Dynamics)을 과제 진행(Task Progression)에 대한 기호적 또는 의미적 추론(Symbolic or Semantic Reasoning)과 연결합니다.

예측 오차(Prediction Errors)는 시간적 동역학(Temporal Dynamics)을 학습하기 위한 피드백을 제공합니다. 실제 전이가 발생한 후 예측된 상태를 실제 관찰 또는 추론된 상태와 비교할 수 있습니다. 이러한 차이는 전이 모델이 부정확한 부분을 드러냅니다. 반복되는 오차는 모델 파라미터(Model Parameters), 표현, 불확실성 추정(Uncertainty Estimates)을 갱신하여 시스템이 경험으로부터 변화하는 동역학을 학습하고 시간이 지남에 따라 예측을 개선하도록 합니다.

시간적 예측(Temporal Prediction)은 미래의 감각 상태에 대한 기대를 들어오는 관찰과 비교할 수 있다는 점에서 예측 부호화(Predictive Coding)와 밀접하게 관련됩니다. 사건이 예상한 대로 전개되면 수정해야 할 정보가 거의 필요하지 않을 수 있습니다. 반대로 예상하지 못한 전이(Unexpected Transitions)는 더 큰 예측 오차를 생성하고 믿음(Belief)이나 모델의 갱신을 유도합니다. 따라서 시간적 예측은 예측을 계층적 감각 처리에서 시간에 따른 상태 변화로 확장합니다.

현재의 관찰만으로 미래를 고유하게 결정할 수 없는 경우에는 기억(Memory)이 필수적입니다. 객체가 장애물 뒤로 일시적으로 사라질 수도 있고, 로봇이 랜드마크(Landmark)를 직접 볼 수 없게 될 수도 있으며, 현재의 상호작용이 수 초 전에 수행된 행동에 의존할 수도 있습니다. 시간적 맥락을 유지하면 시스템은 객체 연속성(Object Continuity)을 보존하고, 숨겨진 상태(Hidden States)를 추론하며, 감각 정보가 일시적으로 사라지는 상황에서도 사건을 예측할 수 있습니다.

행동 조건부 시간 모델(Action-Conditioned Temporal Models)은 계획(Planning)에 특히 중요합니다. 에이전트는 서로 다른 후보 행동(Candidate Actions)에 대응하는 상태 전이를 예측하여 각각을 평가할 수 있습니다. 한 행동은 시스템을 원하는 상태(Desired State)로 이동시킬 수 있는 반면, 다른 행동은 위험이나 불확실성을 증가시킬 수 있습니다. 여러 행동 시퀀스를 내부적으로 롤아웃함으로써 에이전트는 실제 환경에서 정책(Policy)을 선택하고 실행하기 전에 가능한 궤적을 비교할 수 있습니다.

로보틱스(Robotics)와 피지컬 AI(Physical AI)에서는 상태 전이가 환경의 동역학뿐만 아니라 로봇 자체의 물리적 거동(Physical Behavior)도 포착해야 합니다. 관련 변수에는 위치(Position), 속도(Velocity), 자세(Orientation), 관절 구성(Joint Configuration), 객체 움직임(Object Motion), 접촉(Contact), 지형(Terrain), 센서 관찰(Sensor Observations) 등이 포함될 수 있습니다. 유용한 모델은 이러한 변수들이 행동에 따라 어떻게 상호작용하는지를 예측하면서 실시간 지각, 계획, 제어를 지원할 수 있을 만큼 계산적으로 효율적이어야 합니다.

시간적 예측은 월드 모델(World Models)의 기반도 제공합니다. 월드 모델이 의사결정(Decision Making)에 유용하려면 현재의 표현을 가능한 미래 표현으로 변환할 수 있어야 합니다. 상태 추정(State Estimation)은 시스템이 현재 어디에 있는지를 식별하고, 전이 모델링(Transition Modeling)은 어디로 이동할 수 있는지를 예측하며, 관찰 모델은 그 상태에서 무엇을 지각하게 될지를 추정합니다. 이러한 메커니즘을 결합하면 가능한 미래 경험을 내부적으로 시뮬레이션할 수 있습니다.

자기지도 학습(Self-Supervised Learning)은 미래의 경험 자체가 학습 목표를 제공하기 때문에 시간 모델을 자연스럽게 지원합니다. 시스템은 다음 관찰, 미래의 잠재 상태(Future Latent State), 객체 궤적(Object Trajectory), 행동의 결과를 예측한 후 실제로 발생한 결과와 비교할 수 있습니다. 따라서 대규모의 레이블 없는 상호작용 데이터(Unlabeled Interaction Data)는 수작업 주석 없이도 표현과 전이 동역학(Transition Dynamics)을 학습하기 위한 지속적인 지도 신호를 제공할 수 있습니다.

따라서 시간적 예측과 상태 전이(Temporal Prediction and State Transitions)는 현재를 이해하는 것과 미래를 추론하는 것을 연결하는 계산적 가교를 제공합니다. 상태를 표현하고, 동역학을 학습하며, 시간적 맥락을 유지하고, 불확실성을 모델링하며, 행동에 따른 궤적을 시뮬레이션함으로써 지능형 시스템은 단순한 반응적 행동(Reactive Behavior)을 넘어설 수 있습니다. 이러한 능력은 예측(Anticipation), 계획, 적응형 제어(Adaptive Control), 월드 모델링(World Modeling), 동적 환경과의 점점 더 자율적인 상호작용을 지원합니다.
