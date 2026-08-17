**Volume 44 Neuroscience for AI**


# Chapter 08. Brain Reasoning and Decision Making

##  

## 08.00 Decision System Overview

![](images/image1.png){width="7.268055555555556in" height="7.268055555555556in"}

A decision system transforms perception, memory, goals, internal state, and predicted consequences into selections among possible actions. Decision making is therefore not an isolated reasoning step but a continuous control process linking what an intelligent agent perceives and remembers with what it eventually does. Effective decisions require the system to represent alternatives, estimate their consequences, evaluate their significance, and select actions appropriate to current goals and environmental conditions.

Decision systems operate between cognition and action. Perception provides information about the current environment, memory contributes knowledge derived from previous experience, and internal states specify needs, goals, preferences, and constraints. These information streams are integrated into a decision state from which possible actions can be generated and evaluated. The selected action then changes the environment, producing new observations and beginning another decision cycle.

A central requirement of decision making is the representation of alternatives. An intelligent system rarely faces only one possible response; it may continue, stop, explore, avoid, approach, communicate, manipulate, or postpone action. Decision quality depends not only on selecting correctly among known alternatives but also on constructing a useful set of candidate actions that captures meaningful possibilities without creating unnecessary computational complexity.

Evaluation assigns significance to possible states, actions, or outcomes. Biological systems may evaluate alternatives according to reward, effort, risk, novelty, uncertainty, physiological needs, social consequences, and long-term objectives. Artificial systems similarly require objective functions, utilities, costs, rewards, constraints, or learned value representations. The evaluation mechanism converts diverse consequences into information that can influence action selection.

Value is not necessarily an intrinsic property of an external object or event. The same outcome may have different significance depending on the agent\'s current state, goals, previous experience, and future expectations. A charging station, for example, becomes more valuable to a mobile robot when battery energy is low. Decision systems therefore require context-dependent value representations rather than permanently fixed rankings of all possible outcomes.

Expected consequences are particularly important when actions produce delayed effects. An action that provides an immediate benefit may create a larger future cost, while a temporarily costly action may enable a more valuable future state. Intelligent decision making must therefore consider temporal relationships among actions and outcomes. This creates a close connection between decision systems, prediction, planning, reinforcement learning, and world models.

Uncertainty is unavoidable because agents rarely possess complete information about their environments. Sensor measurements can be noisy, objects can be hidden, other agents may behave unpredictably, and future events may depend on unknown variables. A decision system must therefore operate not only over known states but also over beliefs, probabilities, confidence estimates, or alternative hypotheses about what the current situation might actually be.

Risk emerges when possible actions have uncertain outcomes with different consequences. Two actions with similar expected rewards can be very different if one has predictable results while the other includes a small probability of catastrophic failure. Decision systems therefore often need to represent not only expected value but also variability, downside consequences, safety constraints, and tolerance for uncertainty.

Decision making under uncertainty requires balancing exploitation and exploration. Exploitation selects actions that currently appear most valuable based on existing knowledge, while exploration selects actions partly to acquire information or discover potentially better alternatives. Excessive exploitation can trap an agent in incomplete knowledge, whereas excessive exploration can waste resources or create unnecessary risk. Adaptive intelligence requires a context-sensitive balance between the two.

Attention contributes to decision making by determining which information receives processing priority. Real environments contain far more sensory and remembered information than can be evaluated simultaneously. Attention can emphasize task-relevant objects, events, goals, or uncertainties while suppressing less relevant information. Decision quality therefore depends partly on selecting what should enter the decision process before selecting the final action itself.

Working memory provides an active workspace for maintaining information required during decision making. Current goals, recently observed events, candidate actions, constraints, intermediate conclusions, and predicted outcomes may need to remain temporarily accessible while alternatives are compared. Working memory therefore connects immediate perception with retrieved long-term knowledge and enables multi-step evaluation rather than purely reactive behavior.

Episodic memory allows previous decisions and their consequences to influence current choices. When an agent encounters a familiar situation, related experiences can be retrieved to determine what happened previously, which actions succeeded, and which failures should be avoided. Such memory-based decision making can reduce the need to solve every problem from the beginning and enables rapid adaptation from relatively small numbers of significant experiences.

Semantic memory contributes generalized knowledge about objects, relationships, rules, environments, and likely consequences. Instead of retrieving one specific previous episode, an agent can use accumulated knowledge such as which surfaces are traversable, which actions are dangerous, or which tools are appropriate for particular tasks. Decision systems can therefore combine specific episodic evidence with generalized semantic expectations.

Procedural memory contributes learned action policies and skills. Some decisions that initially require explicit comparison can become increasingly automatic through repeated practice. Once reliable action patterns have been learned, procedural systems can execute them efficiently without reconstructing detailed reasoning for every movement. Higher-level decision systems can then concentrate computational resources on novel, ambiguous, or strategically important choices.

Memory consolidation further improves decision systems by transforming repeated experience into stable knowledge. Successful strategies can be strengthened, recurring relationships generalized, and important failures preserved for later retrieval. Replay can reactivate previous state-action-outcome sequences and provide additional opportunities to learn value relationships without repeating every experience physically. Decision competence can therefore improve during both online interaction and offline learning.

Action selection can be understood as competition among candidate behaviors. Different alternatives accumulate support from sensory evidence, goals, expected values, habits, memories, and contextual constraints. Selection occurs when one alternative becomes sufficiently favored relative to others. This general principle appears in biological models of decision making and in artificial mechanisms ranging from utility-based selection to learned policies and optimization procedures.

Biological decision systems involve distributed interactions rather than a single decision center. Prefrontal regions contribute to goal maintenance, planning, contextual control, and evaluation of alternatives, while basal ganglia circuits are strongly associated with action selection and reinforcement-based learning. Limbic and neuromodulatory systems contribute motivational and value-related signals, allowing cognitive evaluation to interact with reward, emotion, and internal physiological state.

The basal ganglia provide an important conceptual connection between value learning and action selection. Candidate actions can be facilitated or suppressed according to learned relationships between states, actions, and outcomes. Dopamine-related learning signals contribute to updating these relationships when obtained outcomes differ from expectations. Decision systems can therefore adapt their future choices according to prediction errors generated by experience.

Reward prediction error represents the difference between an expected outcome and the outcome actually obtained. A better-than-expected result provides a positive learning signal, whereas a worse-than-expected result produces a negative one. Such errors allow value estimates to change incrementally rather than requiring complete models of every environment. This principle forms an important connection between neuroscience and reinforcement learning.

Model-free decision mechanisms learn values or policies directly from experience without explicitly predicting detailed future state transitions. They can produce fast and efficient behavior after sufficient learning but may adapt slowly when environmental structure changes. Their strengths resemble habitual or procedural control, where previously successful responses can be selected rapidly without extensive prospective simulation.

Model-based decision mechanisms instead use representations of how actions transform states and what outcomes may follow. By internally evaluating alternative future trajectories, they can adapt more flexibly to changed goals or environmental conditions. This flexibility comes at a computational cost because multiple possible futures may need to be represented, predicted, and compared before an action is selected.

Intelligent behavior can benefit from combining model-free and model-based control. Familiar, well-practiced situations may be handled efficiently by learned policies, while unfamiliar, uncertain, or high-consequence situations trigger more deliberate planning. A decision architecture can therefore allocate computational effort according to novelty, uncertainty, risk, and task importance instead of using the same decision mechanism for every situation.

Hierarchical decision making further reduces complexity by separating strategic goals from lower-level actions. A high-level system may decide to reach a destination, inspect an object, recharge, or assist another agent, while lower levels determine routes, motion primitives, and actuator commands. Decisions at different temporal and spatial scales can therefore interact without requiring one optimization process to directly evaluate every possible motor command.

For embodied AI, decisions must respect physical feasibility. An abstract action may appear desirable but remain impossible because of robot geometry, actuator limits, terrain, energy availability, payload, obstacles, or safety constraints. Decision systems must consequently interact with state estimation, motion planning, control, and physical models so that selected actions are not merely logically appropriate but executable in the real world.

World models can strengthen decision making by predicting how candidate actions may change the environment. Rather than evaluating only immediate observations, an agent can simulate future states and compare alternative action sequences internally. The quality of these decisions depends on the accuracy of the model, but uncertainty about model predictions must itself be considered to prevent confident planning based on unreliable imagined futures.

Decision systems also require mechanisms for constraint satisfaction. Safety rules, physical limits, ethical requirements, operational policies, resource budgets, and mission priorities can restrict which actions are permissible regardless of their predicted reward. This distinction is important because maximizing a single objective does not automatically produce acceptable behavior. Practical autonomy requires value optimization within explicit and learned constraints.

Multi-objective decision making becomes necessary when several goals must be satisfied simultaneously. A robot may need to maximize task completion while minimizing energy consumption, travel time, collision risk, equipment wear, and disruption to humans. These objectives may conflict, requiring prioritization, weighting, Pareto reasoning, or context-dependent tradeoffs rather than optimization of one universal scalar objective.

Social environments introduce additional complexity because decisions depend on the intentions and likely responses of other agents. Human-aware robots must predict pedestrian motion, interpret social conventions, preserve personal space, communicate intentions, and sometimes sacrifice locally optimal efficiency for predictable or cooperative behavior. Decision systems therefore increasingly require models of other agents as well as models of the physical environment.

Multi-agent decision making extends this principle to coordinated teams. Each agent may possess incomplete information and different local observations while contributing to a shared objective. Coordination requires decisions about task allocation, communication, formation, resource sharing, conflict resolution, and cooperative planning. Distributed systems must remain effective even when communication is delayed, limited, or temporarily unavailable.

A complete decision architecture therefore forms a closed perception--memory--prediction--decision--action loop. The agent estimates its current state, retrieves relevant knowledge, generates candidate actions, predicts possible outcomes, evaluates value and risk, applies constraints, selects an action, observes the result, and updates its memories and models. Decision making is consequently embedded within continuous learning rather than separated from it.

For advanced AI, the key design challenge is not merely producing a correct choice at one instant but maintaining coherent decisions across time. Goals change, information arrives incrementally, predictions fail, resources decline, and unexpected events require replanning. Robust decision systems must monitor the consequences of their own actions and revise plans when assumptions no longer match the observed world.

The decision system ultimately converts intelligence into purposeful behavior. Perception identifies the current situation, memory provides experience, world models estimate possible futures, value systems define what matters, and action mechanisms change the environment. By integrating these components under uncertainty and constraints, decision systems provide the foundation through which biological organisms, autonomous robots, and intelligent agents transform knowledge into adaptive goal-directed action.

의사결정 시스템(Decision System)은 지각(Perception), 기억(Memory), 목표(Goals), 내부 상태(Internal State), 예측된 결과(Predicted Consequences)를 가능한 행동들 가운데 하나를 선택하는 과정으로 변환합니다. 따라서 의사결정(Decision Making)은 독립적인 추론 단계가 아니라 지능형 에이전트(Intelligent Agent)가 무엇을 지각하고 기억하는지를 실제 행동으로 연결하는 지속적인 제어 과정(Continuous Control Process)입니다. 효과적인 의사결정을 위해서는 대안을 표상하고, 그 결과를 추정하며, 중요성을 평가하고, 현재 목표와 환경 조건에 적합한 행동을 선택해야 합니다.

의사결정 시스템은 인지(Cognition)와 행동(Action) 사이에서 작동합니다. 지각은 현재 환경에 관한 정보를 제공하고, 기억은 이전 경험에서 얻은 지식을 제공하며, 내부 상태는 요구(Needs), 목표, 선호(Preferences), 제약 조건(Constraints)을 규정합니다. 이러한 정보 흐름은 가능한 행동을 생성하고 평가할 수 있는 의사결정 상태(Decision State)로 통합됩니다. 선택된 행동은 다시 환경을 변화시키고 새로운 관찰을 생성하면서 다음 의사결정 순환(Decision Cycle)을 시작합니다.

의사결정의 핵심 요구사항 가운데 하나는 대안(Alternatives)의 표상입니다. 지능형 시스템이 선택할 수 있는 반응은 일반적으로 하나뿐이지 않으며, 계속 진행하거나, 정지하거나, 탐색하거나, 회피하거나, 접근하거나, 통신하거나, 조작하거나, 행동을 연기할 수 있습니다. 의사결정의 품질은 알려진 대안 중에서 올바르게 선택하는 능력뿐 아니라 불필요한 계산 복잡도(Computational Complexity)를 증가시키지 않으면서 의미 있는 가능성을 포함하는 유용한 후보 행동(Candidate Actions) 집합을 구성하는 능력에도 의존합니다.

평가(Evaluation)는 가능한 상태, 행동 또는 결과에 중요성을 부여합니다. 생물학적 시스템(Biological Systems)은 보상(Reward), 노력(Effort), 위험(Risk), 새로움(Novelty), 불확실성(Uncertainty), 생리적 요구(Physiological Needs), 사회적 결과(Social Consequences), 장기 목표(Long-Term Objectives)에 따라 대안을 평가할 수 있습니다. 인공 시스템 역시 목적 함수(Objective Functions), 효용(Utilities), 비용(Costs), 보상, 제약 조건 또는 학습된 가치 표상(Learned Value Representations)이 필요합니다. 평가 메커니즘은 다양한 결과를 행동 선택에 영향을 줄 수 있는 정보로 변환합니다.

가치(Value)는 반드시 외부 객체나 사건이 본질적으로 가지고 있는 고정된 속성은 아닙니다. 동일한 결과도 에이전트의 현재 상태, 목표, 이전 경험, 미래 기대(Future Expectations)에 따라 서로 다른 중요성을 가질 수 있습니다. 예를 들어 이동 로봇(Mobile Robot)의 배터리 에너지가 낮아지면 충전소(Charging Station)의 가치는 더욱 높아집니다. 따라서 의사결정 시스템은 모든 가능한 결과에 대해 영구적으로 고정된 순위를 사용하는 대신 맥락 의존적 가치 표상(Context-Dependent Value Representations)을 필요로 합니다.

행동의 효과가 지연되어 나타나는 경우에는 예상 결과(Expected Consequences)가 특히 중요합니다. 즉각적인 이익을 제공하는 행동이 더 큰 미래 비용을 발생시킬 수도 있고, 일시적으로 비용이 드는 행동이 더 가치 있는 미래 상태를 가능하게 할 수도 있습니다. 따라서 지능적인 의사결정은 행동과 결과 사이의 시간적 관계(Temporal Relationships)를 고려해야 합니다. 이는 의사결정 시스템을 예측(Prediction), 계획(Planning), 강화 학습(Reinforcement Learning), 월드 모델(World Models)과 밀접하게 연결합니다.

에이전트가 환경에 대한 완전한 정보를 가지는 경우는 드물기 때문에 불확실성은 피할 수 없습니다. 센서 측정에는 노이즈(Noise)가 포함될 수 있고, 객체는 가려질 수 있으며, 다른 에이전트의 행동은 예측하기 어려울 수 있고, 미래 사건은 알려지지 않은 변수에 따라 달라질 수 있습니다. 따라서 의사결정 시스템은 알려진 상태뿐만 아니라 현재 상황이 실제로 무엇인지에 관한 신념(Beliefs), 확률(Probabilities), 신뢰도 추정(Confidence Estimates), 대안 가설(Alternative Hypotheses)을 기반으로 작동해야 합니다.

위험은 가능한 행동이 서로 다른 결과를 가진 불확실한 상황에서 발생합니다. 기대 보상(Expected Reward)이 비슷한 두 행동이라도 하나는 결과가 예측 가능한 반면 다른 하나는 낮은 확률이지만 치명적인 실패(Catastrophic Failure)를 포함할 수 있습니다. 따라서 의사결정 시스템은 기대 가치(Expected Value)뿐만 아니라 변동성(Variability), 부정적 결과(Downside Consequences), 안전 제약(Safety Constraints), 불확실성에 대한 허용 수준도 표상해야 하는 경우가 많습니다.

불확실성 하의 의사결정(Decision Making under Uncertainty)은 활용(Exploitation)과 탐색(Exploration) 사이의 균형을 필요로 합니다. 활용은 현재 지식을 기반으로 가장 가치가 높다고 판단되는 행동을 선택하고, 탐색은 정보를 획득하거나 잠재적으로 더 나은 대안을 발견하기 위해 행동을 선택합니다. 지나친 활용은 에이전트를 불완전한 지식에 고착시킬 수 있고, 지나친 탐색은 자원을 낭비하거나 불필요한 위험을 만들 수 있습니다. 적응형 지능(Adaptive Intelligence)은 두 전략 사이의 맥락 의존적인 균형을 요구합니다.

주의(Attention)는 어떤 정보에 처리 우선순위를 부여할지를 결정함으로써 의사결정에 기여합니다. 실제 환경에는 동시에 평가할 수 있는 양보다 훨씬 많은 감각 및 기억 정보가 존재합니다. 주의는 작업과 관련된 객체, 사건, 목표 또는 불확실성을 강조하면서 관련성이 낮은 정보를 억제할 수 있습니다. 따라서 의사결정 품질은 최종 행동을 선택하기 전에 어떤 정보가 의사결정 과정에 들어와야 하는지를 선택하는 능력에도 부분적으로 의존합니다.

작업 기억(Working Memory)은 의사결정 과정에서 필요한 정보를 유지하는 활성 작업 공간(Active Workspace)을 제공합니다. 현재 목표, 최근 관찰된 사건, 후보 행동, 제약 조건, 중간 결론(Intermediate Conclusions), 예측된 결과를 대안과 비교하는 동안 일시적으로 접근 가능한 상태로 유지해야 할 수 있습니다. 따라서 작업 기억은 즉각적인 지각을 검색된 장기 지식(Long-Term Knowledge)과 연결하고, 단순한 반응적 행동을 넘어 다단계 평가(Multi-Step Evaluation)를 가능하게 합니다.

일화 기억(Episodic Memory)은 이전 의사결정과 그 결과가 현재의 선택에 영향을 주도록 합니다. 에이전트가 익숙한 상황에 직면하면 관련 경험을 검색하여 과거에 어떤 일이 발생했는지, 어떤 행동이 성공했는지, 어떤 실패를 피해야 하는지를 판단할 수 있습니다. 이러한 기억 기반 의사결정(Memory-Based Decision Making)은 모든 문제를 처음부터 다시 해결할 필요성을 줄이고, 비교적 적은 수의 중요한 경험에서도 빠르게 적응할 수 있도록 합니다.

의미 기억(Semantic Memory)은 객체, 관계, 규칙, 환경, 예상되는 결과에 관한 일반화된 지식을 제공합니다. 특정한 하나의 과거 일화를 검색하는 대신 에이전트는 어떤 표면이 주행 가능한지, 어떤 행동이 위험한지, 특정 작업에 어떤 도구가 적합한지와 같은 축적된 지식을 활용할 수 있습니다. 따라서 의사결정 시스템은 구체적인 일화적 증거(Episodic Evidence)와 일반화된 의미적 기대(Semantic Expectations)를 결합할 수 있습니다.

절차 기억(Procedural Memory)은 학습된 행동 정책(Action Policies)과 기술(Skills)을 제공합니다. 처음에는 명시적인 비교가 필요했던 일부 의사결정도 반복적인 연습을 통해 점차 자동화될 수 있습니다. 신뢰할 수 있는 행동 패턴이 학습되면 절차 시스템은 모든 움직임마다 상세한 추론을 다시 구성하지 않고도 이를 효율적으로 실행할 수 있습니다. 그러면 상위 수준 의사결정 시스템은 새로운 상황, 모호한 상황 또는 전략적으로 중요한 선택에 계산 자원을 집중할 수 있습니다.

기억 공고화(Memory Consolidation)는 반복적인 경험을 안정적인 지식으로 변환함으로써 의사결정 시스템을 더욱 향상시킵니다. 성공적인 전략은 강화되고, 반복되는 관계는 일반화되며, 중요한 실패는 이후 검색을 위해 보존될 수 있습니다. 재생(Replay)은 과거의 상태--행동--결과(State--Action--Outcome) 시퀀스를 다시 활성화하여 모든 경험을 물리적으로 반복하지 않고도 가치 관계(Value Relationships)를 추가적으로 학습할 기회를 제공합니다. 따라서 의사결정 능력은 온라인 상호작용(Online Interaction)과 오프라인 학습(Offline Learning) 모두에서 향상될 수 있습니다.

행동 선택(Action Selection)은 후보 행동 사이의 경쟁으로 이해할 수 있습니다. 서로 다른 대안은 감각적 증거(Sensory Evidence), 목표, 기대 가치, 습관(Habits), 기억, 맥락적 제약으로부터 서로 다른 수준의 지지를 축적합니다. 하나의 대안이 다른 대안보다 충분히 우세해지면 선택이 이루어집니다. 이러한 일반적인 원리는 생물학적 의사결정 모델뿐만 아니라 효용 기반 선택(Utility-Based Selection), 학습된 정책, 최적화 절차(Optimization Procedures)와 같은 인공 메커니즘에서도 나타납니다.

생물학적 의사결정 시스템은 하나의 단일한 의사결정 중추가 아니라 분산된 상호작용(Distributed Interactions)을 통해 작동합니다. 전전두엽 영역(Prefrontal Regions)은 목표 유지(Goal Maintenance), 계획, 맥락적 제어(Contextual Control), 대안 평가에 기여하며, 기저핵 회로(Basal Ganglia Circuits)는 행동 선택과 강화 기반 학습(Reinforcement-Based Learning)에 강하게 관련됩니다. 변연계(Limbic System)와 신경조절 시스템(Neuromodulatory Systems)은 동기 및 가치 관련 신호를 제공하여 인지적 평가가 보상, 감정(Emotion), 내부 생리 상태와 상호작용하도록 합니다.

기저핵(Basal Ganglia)은 가치 학습(Value Learning)과 행동 선택 사이의 중요한 개념적 연결을 제공합니다. 후보 행동은 상태, 행동, 결과 사이에서 학습된 관계에 따라 촉진되거나 억제될 수 있습니다. 도파민 관련 학습 신호(Dopamine-Related Learning Signals)는 실제로 얻어진 결과가 예상과 다를 때 이러한 관계를 갱신하는 데 기여합니다. 따라서 의사결정 시스템은 경험에서 생성되는 예측 오차(Prediction Errors)를 바탕으로 미래의 선택을 적응적으로 변화시킬 수 있습니다.

보상 예측 오차(Reward Prediction Error)는 예상한 결과와 실제로 얻어진 결과 사이의 차이를 나타냅니다. 예상보다 좋은 결과는 긍정적인 학습 신호(Positive Learning Signal)를 제공하고, 예상보다 나쁜 결과는 부정적인 학습 신호(Negative Learning Signal)를 생성합니다. 이러한 오차를 이용하면 환경 전체에 대한 완전한 모델이 없어도 가치 추정(Value Estimates)을 점진적으로 변경할 수 있습니다. 이 원리는 신경과학(Neuroscience)과 강화 학습을 연결하는 중요한 개념입니다.

모델 프리 의사결정(Model-Free Decision Making)은 미래 상태 전이를 상세하게 명시적으로 예측하지 않고 경험에서 직접 가치 또는 정책을 학습합니다. 충분한 학습 이후에는 빠르고 효율적인 행동을 생성할 수 있지만, 환경 구조가 변화하면 적응 속도가 느릴 수 있습니다. 이러한 특성은 이전에 성공했던 반응을 광범위한 미래 시뮬레이션 없이 빠르게 선택할 수 있는 습관적 또는 절차적 제어(Habitual or Procedural Control)와 유사합니다.

반면 모델 기반 의사결정(Model-Based Decision Making)은 행동이 상태를 어떻게 변화시키고 어떤 결과가 뒤따를지를 나타내는 표상을 이용합니다. 대안적인 미래 궤적(Future Trajectories)을 내부적으로 평가함으로써 목표나 환경 조건이 변화했을 때 더욱 유연하게 적응할 수 있습니다. 그러나 행동을 선택하기 전에 여러 가능한 미래를 표상하고 예측하고 비교해야 할 수 있기 때문에 이러한 유연성에는 추가적인 계산 비용이 따릅니다.

지능적 행동은 모델 프리 제어와 모델 기반 제어를 결합함으로써 이점을 얻을 수 있습니다. 익숙하고 충분히 연습된 상황은 학습된 정책으로 효율적으로 처리하고, 익숙하지 않거나 불확실하거나 결과의 영향이 큰 상황에서는 보다 신중한 계획을 활성화할 수 있습니다. 따라서 의사결정 아키텍처는 모든 상황에 동일한 메커니즘을 적용하기보다 새로움, 불확실성, 위험, 작업 중요도에 따라 계산 노력을 할당할 수 있습니다.

계층적 의사결정(Hierarchical Decision Making)은 전략적 목표와 저수준 행동을 분리함으로써 복잡도를 더욱 줄입니다. 상위 수준 시스템은 목적지에 도달하거나, 객체를 검사하거나, 충전하거나, 다른 에이전트를 지원하는 결정을 내릴 수 있으며, 하위 수준에서는 경로, 모션 프리미티브(Motion Primitives), 액추에이터 명령(Actuator Commands)을 결정합니다. 서로 다른 시간적·공간적 스케일의 의사결정이 상호작용함으로써 하나의 최적화 과정이 모든 가능한 모터 명령을 직접 평가할 필요가 없어집니다.

체화 인공지능(Embodied AI)에서 의사결정은 물리적 실행 가능성(Physical Feasibility)을 준수해야 합니다. 추상적으로는 바람직해 보이는 행동도 로봇의 기하 구조, 액추에이터 한계(Actuator Limits), 지형(Terrain), 사용 가능한 에너지, 페이로드(Payload), 장애물, 안전 제약 때문에 실행할 수 없을 수 있습니다. 따라서 의사결정 시스템은 상태 추정, 모션 계획(Motion Planning), 제어(Control), 물리 모델(Physical Models)과 상호작용하여 선택된 행동이 논리적으로 적절할 뿐 아니라 실제 세계에서 실행 가능하도록 해야 합니다.

월드 모델은 후보 행동이 환경을 어떻게 변화시킬지를 예측함으로써 의사결정을 강화할 수 있습니다. 에이전트는 즉각적인 관찰만 평가하는 대신 미래 상태를 시뮬레이션하고 대안적인 행동 시퀀스를 내부적으로 비교할 수 있습니다. 이러한 의사결정의 품질은 월드 모델의 정확도에 의존하지만, 신뢰할 수 없는 상상된 미래를 지나치게 확신하여 계획하는 문제를 방지하려면 모델 예측 자체의 불확실성도 함께 고려해야 합니다.

의사결정 시스템에는 제약 조건 충족(Constraint Satisfaction)을 위한 메커니즘도 필요합니다. 안전 규칙(Safety Rules), 물리적 한계, 윤리적 요구사항(Ethical Requirements), 운영 정책(Operational Policies), 자원 예산(Resource Budgets), 임무 우선순위(Mission Priorities)는 예상 보상이 높더라도 특정 행동을 허용하지 않을 수 있습니다. 하나의 목적 함수를 최대화하는 것만으로 허용 가능한 행동이 자동으로 만들어지는 것은 아니므로 실제 자율 시스템은 명시적이고 학습된 제약 조건 안에서 가치를 최적화해야 합니다.

여러 목표를 동시에 만족시켜야 할 때는 다목적 의사결정(Multi-Objective Decision Making)이 필요합니다. 로봇은 작업 완료율을 최대화하면서 에너지 소비, 이동 시간, 충돌 위험, 장비 마모(Equipment Wear), 인간에 대한 방해를 최소화해야 할 수 있습니다. 이러한 목표들은 서로 충돌할 수 있으므로 하나의 보편적인 스칼라 목적(Scalar Objective)을 단순히 최적화하기보다 우선순위화(Prioritization), 가중치 부여(Weighting), 파레토 추론(Pareto Reasoning), 맥락 의존적 절충(Context-Dependent Tradeoffs)이 필요합니다.

사회적 환경(Social Environments)은 의사결정이 다른 에이전트의 의도와 예상 반응에 의존하기 때문에 추가적인 복잡성을 만듭니다. 인간 인식 로봇(Human-Aware Robots)은 보행자의 움직임을 예측하고, 사회적 관습(Social Conventions)을 해석하며, 개인 공간(Personal Space)을 보존하고, 자신의 의도를 전달하며, 때로는 예측 가능하거나 협력적인 행동을 위해 국소적으로 최적인 효율성을 포기해야 합니다. 따라서 의사결정 시스템은 물리적 환경뿐만 아니라 다른 에이전트의 모델도 점차 필요로 합니다.

다중 에이전트 의사결정(Multi-Agent Decision Making)은 이러한 원리를 협력 팀으로 확장합니다. 각 에이전트는 불완전한 정보와 서로 다른 지역 관찰(Local Observations)을 가지고 있으면서 공통 목표에 기여할 수 있습니다. 협력을 위해서는 작업 할당(Task Allocation), 통신(Communication), 대형(Formation), 자원 공유(Resource Sharing), 충돌 해결, 협력 계획(Cooperative Planning)에 관한 의사결정이 필요합니다. 분산 시스템(Distributed Systems)은 통신이 지연되거나 제한되거나 일시적으로 사용할 수 없는 경우에도 효과적으로 작동해야 합니다.

완전한 의사결정 아키텍처(Decision Architecture)는 결국 지각--기억--예측--의사결정--행동(Perception--Memory--Prediction--Decision--Action)의 폐루프(Closed Loop)를 형성합니다. 에이전트는 현재 상태를 추정하고, 관련 지식을 검색하고, 후보 행동을 생성하고, 가능한 결과를 예측하고, 가치와 위험을 평가하고, 제약 조건을 적용하고, 행동을 선택하고, 결과를 관찰한 다음 기억과 모델을 갱신합니다. 따라서 의사결정은 지속적인 학습(Continuous Learning) 안에 포함되며 학습 과정과 분리되어 존재하지 않습니다.

고급 인공지능(Advanced AI)에서 핵심적인 설계 과제는 단일 순간에 올바른 선택을 생성하는 것뿐만 아니라 시간에 걸쳐 일관된 의사결정(Coherent Decisions)을 유지하는 것입니다. 목표는 변화하고, 정보는 점진적으로 도착하며, 예측은 실패할 수 있고, 자원은 감소하며, 예상하지 못한 사건은 재계획(Replanning)을 요구합니다. 견고한 의사결정 시스템(Robust Decision Systems)은 자신의 행동 결과를 지속적으로 모니터링하고 기존 가정이 관찰된 세계와 더 이상 일치하지 않을 때 계획을 수정해야 합니다.

궁극적으로 의사결정 시스템은 지능(Intelligence)을 목적 지향적 행동(Purposeful Behavior)으로 변환합니다. 지각은 현재 상황을 식별하고, 기억은 경험을 제공하며, 월드 모델은 가능한 미래를 추정하고, 가치 시스템(Value Systems)은 무엇이 중요한지를 정의하며, 행동 메커니즘(Action Mechanisms)은 환경을 변화시킵니다. 이러한 구성 요소를 불확실성과 제약 조건 아래에서 통합함으로써 의사결정 시스템은 생물학적 유기체, 자율 로봇(Autonomous Robots), 지능형 에이전트가 지식을 적응적이고 목표 지향적인 행동(Adaptive Goal-Directed Action)으로 변환할 수 있도록 하는 핵심 기반을 제공합니다.

##  

## 08.01 Prefrontal Cortex

![](images/image2.png){width="7.268055555555556in" height="7.268055555555556in"}

The prefrontal cortex is a major cortical system for coordinating goal-directed cognition and behavior. Rather than operating as a single decision center, it participates in distributed networks that integrate perception, memory, internal goals, contextual information, and expected consequences. Within the broader decision-system architecture, it is especially associated with working memory, cognitive control, planning, rules, goals, and flexible behavior.

Located in the anterior portion of the frontal lobe, the prefrontal cortex receives and exchanges information with many cortical and subcortical systems. This extensive connectivity allows current sensory evidence to interact with remembered experience, motivational state, action possibilities, and task requirements. Its importance therefore arises less from processing one specific sensory modality than from coordinating information needed to organize behavior.

One of the central functions associated with the prefrontal cortex is working memory. Information that is no longer directly present in sensory input may need to remain actively available while an organism reasons, plans, or performs a task. The prefrontal cortex contributes to maintaining task-relevant representations and coordinating the temporary workspace that connects perception, memory, reasoning, and action.

Working-memory maintenance is selective rather than equivalent to storing every recent observation. Goals and attention determine which representations remain behaviorally relevant. A destination, rule, intermediate calculation, remembered instruction, or recently observed obstacle may need to remain active while irrelevant information is suppressed. Prefrontal control therefore helps allocate limited cognitive resources according to the requirements of the current task.

Cognitive control extends this principle beyond simple maintenance. Intelligent behavior frequently requires selecting information, suppressing inappropriate responses, switching between tasks, and adjusting behavior when circumstances change. The prefrontal cortex contributes to these control processes by maintaining representations of goals and rules that can bias processing elsewhere in the brain toward behavior that is appropriate for the current context.

Rules provide an important mechanism for flexible behavior. The same sensory stimulus can require different actions depending on instructions, context, goals, or previous events. Instead of permanently associating one stimulus with one response, prefrontal representations can help specify conditional relationships such as selecting one action under one rule and another action when the governing rule changes.

This capacity supports behavioral flexibility. Habitual responses are efficient in stable situations, but they can become inappropriate when goals or environmental conditions change. Prefrontal control can help preserve the current task structure and promote behavior consistent with newly relevant information. This establishes an important relationship with later distinctions between habitual and goal-directed decision mechanisms.

Planning requires maintaining goals while organizing intermediate actions. A desired future state may be several steps removed from the present state, requiring the system to represent subgoals, constraints, dependencies, and possible sequences. Prefrontal processing can participate in coordinating these representations so that immediate actions are evaluated not only by their local effects but also by their contribution to longer-term objectives.

The prefrontal cortex is therefore closely connected with prediction and mental simulation. When several actions are possible, decision making may require comparing their expected consequences before execution. Representations of goals and task rules can guide which possibilities deserve consideration, while information from memory and predictive systems supplies knowledge about what may happen under different candidate actions.

Such prospective processing connects the prefrontal cortex with internal models and world models. A useful decision system must represent not only the current state but also possible future states produced by actions. Prefrontal control can help organize this future-oriented reasoning by maintaining objectives, candidate plans, constraints, and intermediate results while predictions are generated and compared.

The prefrontal cortex also interacts strongly with memory systems. The hippocampus rapidly encodes episodic experiences and can retrieve contextually relevant memories, while prefrontal mechanisms can use such retrieved information to guide current reasoning and decisions. Memory is therefore not merely recalled for passive recognition; previous experiences can become active evidence for selecting present actions.

This interaction is especially important when a current situation resembles a previous one. Relevant episodes may reveal which actions succeeded, which failed, and which contextual differences matter. Prefrontal control can integrate retrieved experience with current goals rather than automatically repeating the past. This enables memory-based reasoning to remain flexible when similar situations require different responses.

Semantic knowledge also contributes to prefrontal reasoning. General knowledge about objects, rules, causal relationships, social conventions, and task structures can constrain the set of plausible actions. The prefrontal cortex can coordinate this knowledge with current working-memory contents, allowing decisions to depend simultaneously on immediate observations and information accumulated across many previous experiences.

Attention and prefrontal control are similarly intertwined. Environments contain more information than can be processed with equal priority, so task goals must influence which signals receive additional processing. Top-down control can enhance representations relevant to current objectives and reduce interference from competing information. Attention thus becomes part of the mechanism through which goals influence perception and subsequent decision making.

Response inhibition illustrates another aspect of cognitive control. A strongly activated or previously rewarded action is not necessarily appropriate in the current situation. When context, safety, rules, or changing goals indicate otherwise, the system may need to suppress the dominant response. Prefrontal networks participate in control processes that allow behavior to be withheld, redirected, or replaced by a more appropriate alternative.

However, action selection is not performed by the prefrontal cortex alone. The broader chapter architecture places the basal ganglia immediately after the prefrontal cortex, emphasizing their complementary roles. Cortical systems can provide goals, context, candidate actions, and relevant features, while cortico--basal ganglia loops contribute to facilitating or suppressing actions and processes according to learned values and contextual requirements.

The basal ganglia can therefore be viewed as an important partner in translating cognitive representations into selected behavior. Prefrontal systems may maintain what the agent is trying to achieve and which rules currently apply, while basal ganglia circuits participate in determining which candidate action or cognitive process should be facilitated. Recurrent interactions allow selection outcomes to influence subsequent cortical processing.

Value-related information also shapes prefrontal decision processes. Candidate actions cannot be compared only by their physical possibility; their expected benefits, costs, risks, effort, and relevance to current goals must also be considered. Motivational and reward-related systems provide signals that influence which outcomes matter, enabling cognitive control to operate in relation to the agent\'s needs rather than according to abstract reasoning alone.

The prefrontal cortex is not functionally uniform. Different prefrontal regions participate to different degrees in working memory, cognitive control, valuation, social cognition, monitoring, and action regulation. These functions emerge through interacting networks rather than cleanly isolated modules. Consequently, descriptions of prefrontal function should emphasize distributed specialization and connectivity instead of assigning every cognitive operation to one sharply bounded region.

Dorsolateral prefrontal regions are commonly associated with working memory, task rules, planning, and executive control. They are particularly relevant when information must remain available across delays or be manipulated during multi-step reasoning. Their activity can reflect task variables that are not immediately available in the sensory environment but remain necessary for guiding ongoing behavior.

Ventromedial and orbitofrontal regions contribute strongly to representing value, preferences, and relationships between situations and expected outcomes. These functions help connect cognitive representations with reward and motivational significance. An option that is physically available may nevertheless be rejected because its expected outcome is undesirable, costly, risky, or inconsistent with the current internal state.

Medial frontal systems contribute to monitoring behavior, detecting conflict, evaluating outcomes, and adjusting control. When competing actions are strongly activated or an outcome differs from expectation, additional control may be required. Monitoring mechanisms allow decision systems to recognize that existing strategies are insufficient and increase the resources devoted to resolving uncertainty or correcting behavior.

Prefrontal function is therefore inherently dynamic. Representations can change rapidly when task rules, goals, context, or available evidence change. The same neural populations may participate in different patterns of activity across different tasks. Such context-sensitive distributed representation is consistent with the broader cortical principle that cognition depends on recurrent processing shaped by goals and previous experience.

Recurrent connectivity is important because cognition unfolds over time. A decision may require maintaining information, receiving new evidence, revising an interpretation, comparing alternatives, and eventually committing to an action. Recurrent processing allows internal representations to persist and evolve rather than being transformed through a purely one-directional sequence from input to output.

This temporal persistence is particularly important under partial observability. The environment may not expose every task-relevant variable at the same moment. An agent may need to remember a previously observed instruction, object, location, or event while processing new information. Prefrontal working-memory mechanisms help bridge these temporal gaps so behavior can depend on information distributed across time.

Uncertainty places additional demands on prefrontal control. When evidence is incomplete or conflicting, the system may need to maintain multiple hypotheses, postpone commitment, gather more information, or reconsider an existing plan. Flexible control is therefore valuable not merely for choosing actions but also for deciding when additional reasoning, observation, memory retrieval, or exploration is required.

The same principles are important for embodied intelligence. A robot operating in a changing physical environment must maintain mission goals while reacting to immediate obstacles and unexpected events. High-level control must preserve the objective without rigidly following a plan that has become unsafe or impossible. A prefrontal-like computational function would therefore coordinate persistent goals with continuously changing state estimates.

Hierarchical control provides one useful analogy. High-level representations can encode mission objectives and task rules, intermediate levels can maintain subgoals and plans, and lower levels can execute actions through specialized controllers. Information must flow both downward and upward so that strategic goals influence action while execution failures and environmental changes trigger replanning.

Modern AI systems contain several mechanisms that are functionally analogous to limited aspects of prefrontal processing, although they should not be considered direct replicas of the brain. Agent state, context representations, recurrent networks, attention mechanisms, planning modules, scratchpads, and working-memory systems can maintain task-relevant information and coordinate multi-step computation across time.

An AI agent can, for example, maintain a representation of its current objective while retrieving relevant memories, observing environmental changes, calling specialized tools, evaluating intermediate results, and revising its plan. The functional similarity lies in coordinating information according to goals and context. The underlying computational mechanisms may nevertheless differ substantially from biological prefrontal circuits.

For Physical AI, this coordination function becomes especially important because reasoning must ultimately respect embodiment. Goals must be reconciled with battery state, actuator limits, terrain, obstacles, payload, human presence, safety policies, and mission constraints. A high-level cognitive controller must therefore integrate abstract objectives with continuously updated physical state before committing the robot to behavior.

Prefrontal-inspired AI should consequently emphasize flexible control rather than merely increasing model size or reasoning depth. Useful capabilities include persistent goal representation, selective working memory, context-dependent rules, inhibition of inappropriate actions, hierarchical planning, uncertainty monitoring, switching between strategies, and coordination with memory, prediction, value estimation, and action-selection systems.

The prefrontal cortex ultimately illustrates how intelligence can remain organized around goals while operating in a changing world. It maintains relevant information, applies contextual rules, coordinates planning, regulates competing responses, integrates memory and value, and adjusts behavior when circumstances change. In the decision architecture, it provides a critical bridge between knowing the current situation and controlling what should happen next.

전전두엽 피질(Prefrontal Cortex)은 목표 지향적 인지(Goal-Directed Cognition)와 행동을 조정하는 주요 피질 시스템(Cortical System)입니다. 하나의 단일한 의사결정 중추(Decision Center)로 작동하기보다는 지각(Perception), 기억(Memory), 내부 목표(Internal Goals), 맥락 정보(Contextual Information), 예상 결과(Expected Consequences)를 통합하는 분산 네트워크(Distributed Networks)에 참여합니다. 보다 광범위한 의사결정 시스템 아키텍처(Decision-System Architecture)에서 전전두엽 피질은 특히 작업 기억(Working Memory), 인지 제어(Cognitive Control), 계획(Planning), 규칙(Rules), 목표(Goals), 유연한 행동(Flexible Behavior)과 관련됩니다.

전두엽(Frontal Lobe)의 앞부분에 위치한 전전두엽 피질은 다양한 피질 및 피질하 시스템(Cortical and Subcortical Systems)과 정보를 주고받습니다. 이러한 광범위한 연결성(Connectivity)을 통해 현재의 감각적 증거(Sensory Evidence)는 기억된 경험, 동기 상태(Motivational State), 가능한 행동(Action Possibilities), 작업 요구사항(Task Requirements)과 상호작용할 수 있습니다. 따라서 전전두엽 피질의 중요성은 특정한 하나의 감각 양식(Sensory Modality)을 처리하는 것보다 행동을 조직하는 데 필요한 정보를 조정하는 능력에서 나타납니다.

전전두엽 피질과 관련된 핵심 기능 가운데 하나는 작업 기억입니다. 감각 입력에 더 이상 직접 존재하지 않는 정보도 유기체가 추론(Reasoning), 계획 또는 작업을 수행하는 동안 능동적으로 이용 가능한 상태로 유지되어야 할 수 있습니다. 전전두엽 피질은 작업 관련 표상(Task-Relevant Representations)을 유지하고 지각, 기억, 추론, 행동을 연결하는 일시적인 작업 공간(Temporary Workspace)을 조정하는 데 기여합니다.

작업 기억의 유지는 최근 관찰된 모든 정보를 저장하는 것과 동일하지 않으며 선택적(Selective)으로 이루어집니다. 목표와 주의(Attention)는 어떤 표상이 행동과 관련된 상태로 유지될지를 결정합니다. 목적지(Destination), 규칙, 중간 계산(Intermediate Calculation), 기억된 지시, 최근 관찰된 장애물 등이 활성 상태로 유지되어야 하는 반면 관련 없는 정보는 억제될 수 있습니다. 따라서 전전두엽 제어(Prefrontal Control)는 현재 작업의 요구에 따라 제한된 인지 자원(Cognitive Resources)을 할당하도록 돕습니다.

인지 제어는 이러한 원리를 단순한 정보 유지보다 더 넓은 영역으로 확장합니다. 지능적인 행동은 흔히 정보를 선택하고, 부적절한 반응을 억제하며, 작업 사이를 전환하고, 상황이 변화할 때 행동을 조정해야 합니다. 전전두엽 피질은 목표와 규칙에 대한 표상을 유지하여 뇌의 다른 영역에서 이루어지는 처리가 현재 맥락에 적절한 행동을 향하도록 편향(Bias)시키는 방식으로 이러한 제어 과정에 기여합니다.

규칙은 유연한 행동을 가능하게 하는 중요한 메커니즘입니다. 동일한 감각 자극(Sensory Stimulus)도 지시, 맥락, 목표 또는 이전 사건에 따라 서로 다른 행동을 요구할 수 있습니다. 하나의 자극을 하나의 반응에 영구적으로 연결하는 대신, 전전두엽 표상(Prefrontal Representations)은 특정 규칙에서는 하나의 행동을 선택하고 지배적인 규칙이 변경되면 다른 행동을 선택하는 것과 같은 조건부 관계(Conditional Relationships)를 규정하도록 도울 수 있습니다.

이러한 능력은 행동 유연성(Behavioral Flexibility)을 지원합니다. 습관적 반응(Habitual Responses)은 안정적인 상황에서는 효율적이지만 목표나 환경 조건이 변하면 부적절해질 수 있습니다. 전전두엽 제어는 현재의 작업 구조(Task Structure)를 유지하고 새롭게 중요해진 정보와 일치하는 행동을 촉진할 수 있습니다. 이는 이후 논의되는 습관적 의사결정(Habitual Decision Making)과 목표 지향적 의사결정(Goal-Directed Decision Making) 사이의 구분과 중요한 관계를 형성합니다.

계획은 목표를 유지하면서 중간 행동(Intermediate Actions)을 조직하는 능력을 요구합니다. 원하는 미래 상태(Desired Future State)가 현재 상태에서 여러 단계 떨어져 있다면 시스템은 하위 목표(Subgoals), 제약 조건(Constraints), 의존 관계(Dependencies), 가능한 시퀀스(Possible Sequences)를 표상해야 합니다. 전전두엽 처리는 이러한 표상을 조정하여 즉각적인 행동을 국소적인 효과뿐 아니라 장기 목표에 대한 기여도에 따라 평가할 수 있도록 합니다.

따라서 전전두엽 피질은 예측(Prediction) 및 정신적 시뮬레이션(Mental Simulation)과 밀접하게 연결됩니다. 여러 행동이 가능할 때 의사결정을 위해서는 실행하기 전에 예상되는 결과를 비교해야 할 수 있습니다. 목표와 작업 규칙의 표상은 어떤 가능성을 고려해야 하는지를 안내하고, 기억 및 예측 시스템에서 제공되는 정보는 서로 다른 후보 행동(Candidate Actions)에서 어떤 일이 발생할 수 있는지에 관한 지식을 제공합니다.

이러한 미래 지향적 처리(Prospective Processing)는 전전두엽 피질을 내부 모델(Internal Models) 및 월드 모델(World Models)과 연결합니다. 유용한 의사결정 시스템은 현재 상태뿐 아니라 행동으로 만들어질 수 있는 가능한 미래 상태(Future States)도 표상해야 합니다. 전전두엽 제어는 예측이 생성되고 비교되는 동안 목표, 후보 계획(Candidate Plans), 제약 조건, 중간 결과를 유지하여 이러한 미래 지향적 추론을 조직하는 데 기여할 수 있습니다.

전전두엽 피질은 기억 시스템과도 강하게 상호작용합니다. 해마(Hippocampus)는 일화적 경험(Episodic Experiences)을 빠르게 부호화하고 맥락적으로 관련된 기억을 검색할 수 있으며, 전전두엽 메커니즘은 이렇게 검색된 정보를 현재의 추론과 의사결정을 안내하는 데 활용할 수 있습니다. 따라서 기억은 단순히 수동적인 인식(Recognition)을 위해 회상되는 것이 아니라 과거의 경험이 현재 행동을 선택하기 위한 능동적인 증거(Active Evidence)가 될 수 있습니다.

이러한 상호작용은 현재 상황이 이전의 경험과 유사할 때 특히 중요합니다. 관련된 일화(Episodes)를 통해 과거에 어떤 행동이 성공했는지, 어떤 행동이 실패했는지, 어떤 맥락적 차이가 중요한지를 파악할 수 있습니다. 전전두엽 제어는 과거를 자동적으로 반복하는 대신 검색된 경험을 현재 목표와 통합할 수 있습니다. 이를 통해 유사한 상황에서도 서로 다른 반응이 필요할 때 기억 기반 추론(Memory-Based Reasoning)이 유연성을 유지할 수 있습니다.

의미 지식(Semantic Knowledge) 역시 전전두엽 추론에 기여합니다. 객체, 규칙, 인과 관계(Causal Relationships), 사회적 관습(Social Conventions), 작업 구조에 대한 일반적인 지식은 가능한 행동의 범위를 제한할 수 있습니다. 전전두엽 피질은 이러한 지식을 현재의 작업 기억 내용과 조정하여 즉각적인 관찰과 많은 이전 경험을 통해 축적된 정보가 동시에 의사결정에 영향을 미치도록 할 수 있습니다.

주의와 전전두엽 제어 역시 긴밀하게 연결되어 있습니다. 환경에는 동일한 우선순위로 처리할 수 있는 양보다 훨씬 많은 정보가 존재하기 때문에 작업 목표는 어떤 신호가 추가적인 처리를 받을지를 결정하는 데 영향을 주어야 합니다. 하향식 제어(Top-Down Control)는 현재 목표와 관련된 표상을 강화하고 경쟁하는 정보의 간섭(Interference)을 감소시킬 수 있습니다. 따라서 주의는 목표가 지각과 이후의 의사결정에 영향을 미치는 메커니즘의 일부가 됩니다.

반응 억제(Response Inhibition)는 인지 제어의 또 다른 측면을 보여줍니다. 강하게 활성화되거나 이전에 보상받았던 행동이라고 해서 현재 상황에서도 반드시 적절한 것은 아닙니다. 맥락, 안전, 규칙 또는 변화한 목표가 다른 행동을 요구한다면 시스템은 지배적인 반응(Dominant Response)을 억제해야 할 수 있습니다. 전전두엽 네트워크는 행동을 보류하거나 방향을 변경하거나 보다 적절한 대안으로 대체할 수 있도록 하는 제어 과정에 참여합니다.

그러나 행동 선택(Action Selection)이 전전두엽 피질만으로 이루어지는 것은 아닙니다. 보다 광범위한 구조에서 기저핵(Basal Ganglia)은 전전두엽 피질과 상호보완적인 역할을 수행합니다. 피질 시스템은 목표, 맥락, 후보 행동, 관련 특징을 제공할 수 있고, 피질--기저핵 루프(Cortico--Basal Ganglia Loops)는 학습된 가치(Learned Values)와 맥락적 요구사항에 따라 행동과 처리 과정을 촉진하거나 억제하는 데 기여합니다.

따라서 기저핵은 인지적 표상(Cognitive Representations)을 선택된 행동으로 변환하는 중요한 파트너로 볼 수 있습니다. 전전두엽 시스템은 에이전트가 무엇을 달성하려 하는지, 현재 어떤 규칙이 적용되는지를 유지할 수 있으며, 기저핵 회로는 어떤 후보 행동 또는 인지 과정이 촉진되어야 하는지를 결정하는 데 참여합니다. 반복적인 상호작용(Recurrent Interactions)을 통해 선택 결과가 이후의 피질 처리에 다시 영향을 줄 수 있습니다.

가치 관련 정보(Value-Related Information)도 전전두엽의 의사결정 과정에 영향을 줍니다. 후보 행동은 단순히 물리적으로 가능한지만 비교해서는 안 되며 예상되는 이익, 비용, 위험, 노력, 현재 목표와의 관련성도 고려해야 합니다. 동기 및 보상 관련 시스템(Motivational and Reward-Related Systems)은 어떤 결과가 중요한지를 결정하는 신호를 제공하여 인지 제어가 추상적인 추론에만 의존하지 않고 에이전트의 요구와 관련하여 작동하도록 합니다.

전전두엽 피질은 기능적으로 균일하지 않습니다. 서로 다른 전전두엽 영역은 작업 기억, 인지 제어, 가치 평가(Valuation), 사회적 인지(Social Cognition), 모니터링(Monitoring), 행동 조절(Action Regulation)에 서로 다른 정도로 참여합니다. 이러한 기능들은 명확하게 분리된 모듈(Isolated Modules)이 아니라 상호작용하는 네트워크를 통해 나타납니다. 따라서 전전두엽 기능을 설명할 때는 모든 인지 작용을 하나의 명확하게 구분된 영역에 할당하기보다 분산된 전문화(Distributed Specialization)와 연결성을 강조해야 합니다.

배외측 전전두엽 영역(Dorsolateral Prefrontal Regions)은 일반적으로 작업 기억, 작업 규칙, 계획, 실행 제어(Executive Control)와 관련됩니다. 특히 정보가 일정한 지연 시간 동안 유지되어야 하거나 다단계 추론 과정에서 조작되어야 할 때 중요합니다. 이러한 영역의 활동은 현재 감각 환경에 즉각적으로 존재하지 않지만 지속적인 행동을 안내하기 위해 필요한 작업 변수(Task Variables)를 반영할 수 있습니다.

복내측 및 안와전두엽 영역(Ventromedial and Orbitofrontal Regions)은 가치, 선호(Preferences), 상황과 예상 결과 사이의 관계를 표상하는 데 크게 기여합니다. 이러한 기능은 인지적 표상을 보상 및 동기적 중요성(Motivational Significance)과 연결하는 데 도움을 줍니다. 물리적으로 가능한 선택이라도 예상되는 결과가 바람직하지 않거나, 비용이 높거나, 위험하거나, 현재의 내부 상태와 일치하지 않는다면 거부될 수 있습니다.

내측 전두엽 시스템(Medial Frontal Systems)은 행동을 모니터링하고, 충돌(Conflict)을 감지하고, 결과를 평가하며, 제어 수준을 조정하는 데 기여합니다. 서로 경쟁하는 행동이 강하게 활성화되거나 결과가 예상과 다를 때 추가적인 제어가 필요할 수 있습니다. 모니터링 메커니즘을 통해 의사결정 시스템은 기존 전략이 충분하지 않음을 인식하고 불확실성을 해결하거나 행동을 수정하기 위해 더 많은 자원을 할당할 수 있습니다.

따라서 전전두엽 기능은 본질적으로 동적(Dynamic)입니다. 표상은 작업 규칙, 목표, 맥락 또는 이용 가능한 증거가 변화하면 빠르게 변화할 수 있습니다. 동일한 신경 세포 집단도 서로 다른 작업에서는 서로 다른 활동 패턴에 참여할 수 있습니다. 이러한 맥락 의존적 분산 표상(Context-Sensitive Distributed Representation)은 인지가 목표와 이전 경험에 의해 형성되는 반복 처리(Recurrent Processing)에 의존한다는 보다 광범위한 피질 원리와 일치합니다.

인지가 시간에 걸쳐 진행되기 때문에 반복적 연결성(Recurrent Connectivity)은 중요합니다. 하나의 의사결정을 위해 정보를 유지하고, 새로운 증거를 받아들이고, 해석을 수정하고, 대안을 비교한 다음 최종적으로 행동을 결정해야 할 수 있습니다. 반복 처리를 통해 내부 표상은 입력에서 출력으로 한 방향으로만 변환되는 것이 아니라 시간에 걸쳐 유지되고 변화할 수 있습니다.

이러한 시간적 지속성(Temporal Persistence)은 부분 관찰 가능성(Partial Observability)이 존재하는 환경에서 특히 중요합니다. 환경은 작업에 필요한 모든 변수를 같은 순간에 보여주지 않을 수 있습니다. 에이전트는 이전에 관찰한 지시, 객체, 위치 또는 사건을 기억하면서 새로운 정보를 처리해야 할 수 있습니다. 전전두엽의 작업 기억 메커니즘은 이러한 시간적 간극(Temporal Gaps)을 연결하여 시간적으로 분산된 정보가 행동에 영향을 줄 수 있도록 합니다.

불확실성(Uncertainty)은 전전두엽 제어에 추가적인 요구를 부과합니다. 증거가 불완전하거나 서로 충돌하는 경우 시스템은 여러 가설(Hypotheses)을 유지하거나, 결정을 연기하거나, 추가 정보를 수집하거나, 기존 계획을 다시 검토해야 할 수 있습니다. 따라서 유연한 제어(Flexible Control)는 행동을 선택하는 것뿐 아니라 언제 추가적인 추론, 관찰, 기억 검색(Memory Retrieval), 탐색(Exploration)이 필요한지를 결정하는 데도 중요합니다.

동일한 원리는 체화 지능(Embodied Intelligence)에서도 중요합니다. 변화하는 물리적 환경에서 작동하는 로봇은 즉각적인 장애물과 예상하지 못한 사건에 대응하면서도 임무 목표(Mission Goals)를 유지해야 합니다. 상위 수준 제어는 목표를 지속적으로 유지하는 동시에 안전하지 않거나 실행 불가능해진 계획을 경직되게 따르지 않아야 합니다. 따라서 전전두엽 유사 계산 기능(Prefrontal-Like Computational Function)은 지속적인 목표와 계속 변화하는 상태 추정(State Estimates)을 조정하는 역할을 수행할 수 있습니다.

계층적 제어(Hierarchical Control)는 이러한 기능을 설명하는 유용한 비유를 제공합니다. 상위 수준 표상은 임무 목표와 작업 규칙을 부호화하고, 중간 수준에서는 하위 목표와 계획을 유지하며, 하위 수준에서는 특화된 제어기(Specialized Controllers)를 통해 행동을 실행할 수 있습니다. 전략적 목표가 행동에 영향을 주는 동시에 실행 실패와 환경 변화가 재계획(Replanning)을 유발할 수 있도록 정보는 하향 및 상향 방향으로 모두 흐를 필요가 있습니다.

현대 인공지능 시스템(Modern AI Systems)은 뇌를 직접적으로 복제한 것으로 보아서는 안 되지만, 전전두엽 처리의 제한적인 일부 측면과 기능적으로 유사한 여러 메커니즘을 포함하고 있습니다. 에이전트 상태(Agent State), 맥락 표상(Context Representations), 순환 신경망(Recurrent Networks), 주의 메커니즘(Attention Mechanisms), 계획 모듈(Planning Modules), 스크래치패드(Scratchpads), 작업 기억 시스템은 작업 관련 정보를 유지하고 시간에 걸친 다단계 계산(Multi-Step Computation)을 조정할 수 있습니다.

예를 들어 인공지능 에이전트(AI Agent)는 관련 기억을 검색하고, 환경 변화를 관찰하고, 특화된 도구를 호출하고, 중간 결과를 평가하고, 계획을 수정하면서 현재 목표의 표상을 유지할 수 있습니다. 이러한 기능적 유사성은 목표와 맥락에 따라 정보를 조정한다는 데 있습니다. 그러나 그 기반이 되는 계산 메커니즘(Computational Mechanisms)은 생물학적 전전두엽 회로와 상당히 다를 수 있습니다.

피지컬 AI(Physical AI)에서는 추론이 궁극적으로 체화(Embodiment)의 제약을 준수해야 하기 때문에 이러한 조정 기능이 특히 중요합니다. 목표는 배터리 상태(Battery State), 액추에이터 한계(Actuator Limits), 지형(Terrain), 장애물, 페이로드(Payload), 인간의 존재(Human Presence), 안전 정책(Safety Policies), 임무 제약(Mission Constraints)과 조정되어야 합니다. 따라서 상위 수준 인지 제어기(High-Level Cognitive Controller)는 로봇이 행동을 결정하기 전에 추상적인 목표와 지속적으로 갱신되는 물리적 상태를 통합해야 합니다.

따라서 전전두엽에서 영감을 받은 인공지능(Prefrontal-Inspired AI)은 단순히 모델의 크기나 추론 깊이(Reasoning Depth)를 증가시키는 것보다 유연한 제어 능력을 강조해야 합니다. 유용한 기능에는 지속적인 목표 표상(Persistent Goal Representation), 선택적 작업 기억(Selective Working Memory), 맥락 의존적 규칙(Context-Dependent Rules), 부적절한 행동의 억제, 계층적 계획(Hierarchical Planning), 불확실성 모니터링(Uncertainty Monitoring), 전략 전환(Strategy Switching), 기억·예측·가치 평가·행동 선택 시스템과의 조정이 포함됩니다.

궁극적으로 전전두엽 피질은 변화하는 세계에서 지능이 목표를 중심으로 어떻게 조직된 상태를 유지할 수 있는지를 보여줍니다. 전전두엽 피질은 관련 정보를 유지하고, 맥락적 규칙(Contextual Rules)을 적용하며, 계획을 조정하고, 경쟁하는 반응을 제어하며, 기억과 가치를 통합하고, 상황이 변화할 때 행동을 수정합니다. 의사결정 아키텍처에서 전전두엽 피질은 현재 상황을 이해하는 것과 다음에 무엇을 해야 하는지를 제어하는 것 사이를 연결하는 핵심적인 가교 역할을 수행합니다.

##  

## 08.02 Basal Ganglia and Action Selection [w/Code]

![](images/image3.png){width="7.268055555555556in" height="7.268055555555556in"}

The basal ganglia are a group of interconnected subcortical structures that play a central role in action selection, reinforcement learning, habit formation, motivation, and movement regulation. Within the chapter structure, they follow the prefrontal cortex and precede value-based decision making, positioning them as a critical mechanism through which goals, context, candidate actions, and learned values can influence which behaviors are facilitated or suppressed.

Action selection is necessary because an intelligent organism continuously possesses many possible actions but can execute only a limited subset at any moment. Walking, stopping, reaching, turning, speaking, waiting, or changing strategies may all compete for control. The basal ganglia contribute to resolving this competition by regulating which action-related cortical processes receive sufficient support to proceed and which remain inhibited.

The basal ganglia should not be understood as a simple command center that independently chooses behavior. They participate in recurrent cortico--basal ganglia--thalamic loops through which cortical representations enter subcortical circuits and selection-related signals return toward cortex. This organization allows goals and contextual information represented in cortical systems to interact continuously with learned action preferences and selection mechanisms.

Major components include the striatum, globus pallidus, subthalamic nucleus, substantia nigra, and associated connections with the thalamus and cerebral cortex. The striatum receives extensive cortical input and serves as a major entry point into basal ganglia circuits. Output structures regulate thalamic and brainstem targets, thereby influencing whether particular motor or cognitive processes become facilitated.

The striatum receives information representing goals, context, candidate actions, sensory features, and other task-relevant variables. This input does not necessarily describe one already selected action. Instead, multiple possibilities may be represented simultaneously. Basal ganglia circuits can transform these competing representations according to learned values and current conditions, contributing to selective gating of behavior.

A useful conceptual model distinguishes direct and indirect pathways. The direct pathway is commonly associated with facilitating selected actions by reducing inhibitory output from basal ganglia output nuclei, thereby allowing relevant thalamocortical activity to proceed. The indirect pathway contributes to suppressing competing or inappropriate actions by increasing inhibitory influence through additional circuit stages.

This facilitation--suppression organization provides a useful framework for understanding action selection. Selection does not simply mean activating the desired action; competing alternatives must also be controlled. Reliable behavior therefore depends on simultaneously increasing support for contextually appropriate processes while preventing incompatible responses from interfering with execution.

The subthalamic nucleus contributes another important component of this regulatory architecture. It can influence basal ganglia output broadly and is often associated with mechanisms that increase inhibitory control when competing alternatives or uncertain situations require additional caution. Functionally, this provides a way to delay or regulate commitment when rapid selection could produce an inappropriate action.

Basal ganglia output is largely inhibitory, making disinhibition an important concept for understanding these circuits. Candidate actions can be considered under tonic inhibitory control, with selection involving a reduction of inhibition for favored pathways. This organization creates a gating mechanism in which appropriate actions are released while alternatives remain relatively suppressed.

The thalamus forms an important part of the returning loop. Basal ganglia output influences thalamic activity, while thalamic signals project back toward cortical regions. Consequently, selection is embedded in a recurrent circuit rather than implemented as a one-way sequence. Cortical processing influences basal ganglia activity, and the resulting gating signals reshape subsequent cortical processing and behavior.

These loops are not limited to movement. Parallel cortico--basal ganglia circuits interact with motor, associative, and limbic cortical regions, allowing related principles to influence motor behavior, cognitive processes, motivation, and decision making. Action selection can therefore refer not only to selecting a physical movement but also to selecting strategies, task sets, or other processes that organize behavior.

The relationship with the prefrontal cortex is particularly important. Prefrontal systems can maintain goals, rules, context, candidate actions, and relevant features, while basal ganglia circuits contribute to facilitating or suppressing actions and processes. Together, these systems help transform cognitive goals into selected behavior rather than leaving goals as passive internal representations.

Selection must also adapt through experience. An action that repeatedly produces useful outcomes should generally become easier to select under similar conditions, while actions associated with poor outcomes should become less favored. The basal ganglia are therefore tightly connected with reinforcement learning, through which state--action--outcome relationships modify future behavioral tendencies.

Dopamine provides a major learning-related signal within this architecture. Dopaminergic neurons associated particularly with the substantia nigra pars compacta project strongly to the striatum and modulate plasticity within basal ganglia circuits. Dopamine should not be interpreted simply as a pleasure signal; its computational significance includes communicating information related to unexpected outcomes and changes in expected value.

Reward prediction error provides an important framework for understanding this learning signal. When an obtained outcome is better than expected, a positive prediction error can strengthen relationships that contributed to the successful action. When the result is worse than expected, a negative prediction error can modify those relationships in the opposite direction, progressively changing future action preferences.

Through repeated learning, the system can associate particular states or contexts with actions that tend to produce valuable outcomes. Decision making then becomes increasingly efficient because the agent does not need to reconstruct every action value from the beginning. Learned action tendencies provide a prior structure that can rapidly bias competition among candidate behaviors.

This mechanism connects the basal ganglia with procedural memory. Skills and habits develop through repeated state--action--outcome experience, gradually allowing behavior to become faster and less dependent on deliberate reasoning. The broader memory architecture therefore associates basal ganglia function with habit formation, action selection, and reinforcement learning.

Habit formation demonstrates both the strength and limitation of learned action selection. Repeatedly successful behavior can become efficient and automatic, reducing cognitive demand. However, a strongly learned response can become inappropriate when goals or environmental conditions change. Flexible intelligence consequently requires interaction between habitual mechanisms and systems capable of goal-directed control.

Goal-directed action depends more strongly on current outcomes and their present value. Habitual action depends more strongly on previously learned associations between states and responses. These modes should not be viewed as completely separate systems; behavior can shift between them depending on experience, uncertainty, novelty, task demands, and the stability of the environment.

The basal ganglia therefore contribute to the stability--flexibility balance of decision making. Stable learned policies allow familiar situations to be handled efficiently, while cortical control can intervene when circumstances require reconsideration. An effective decision architecture benefits from preserving well-learned behavior without allowing previous learning to dominate situations in which it is no longer appropriate.

Action selection also depends on motivation. The value of an action changes with internal state and current goals. Seeking food, conserving energy, avoiding danger, or pursuing a learned reward can become more or less important depending on physiological and contextual conditions. Limbic-related basal ganglia circuits allow motivational information to influence which behaviors gain selection priority.

Movement regulation provides a particularly visible expression of basal ganglia function. Voluntary movement requires selecting intended motor programs while preventing competing movements from disrupting execution. The basal ganglia interact with motor and premotor cortical systems to influence initiation, scaling, sequencing, and switching among actions, while other systems such as the cerebellum contribute prediction, timing, coordination, and error correction.

This division of labor is useful for understanding brain-inspired robotics. The basal ganglia are more closely associated with deciding which behavior or policy should gain control, whereas the cerebellum is strongly associated with predicting and refining how movement unfolds. Motor cortical and spinal systems then participate in representing and executing the selected behavior through physical effectors.

Selection operates hierarchically as well. At a high level, an agent may choose between exploration, navigation, manipulation, charging, or waiting. At intermediate levels, it may select routes, skills, or movement primitives. At lower levels, control systems determine detailed motor commands. Basal-ganglia-inspired gating principles can therefore be applied across multiple levels rather than only to individual muscle movements.

Context is essential because the same action can be desirable in one state and inappropriate in another. Reaching may be useful when an object is accessible but unsafe when an obstacle blocks the arm. A learned selection mechanism must therefore condition action preferences on relevant state representations instead of assigning one fixed value to an action independent of circumstances.

Uncertainty further affects selection. When the system has strong evidence that one alternative is preferable, rapid commitment may be appropriate. When several alternatives have similar support or the potential consequences are severe, additional information gathering or delayed commitment may be beneficial. Selection mechanisms must therefore interact with confidence, risk, and monitoring processes rather than maximizing learned value blindly.

In reinforcement-learning terms, action selection can be expressed through a policy that maps states or observations to probabilities or preferences over actions. Experience modifies the policy or underlying value estimates according to rewards and prediction errors. This provides a computational analogy to basal ganglia function, although artificial policies should not be treated as literal replicas of biological circuits.

Actor--critic architectures provide another useful functional analogy. An actor represents or selects behavior, while a critic estimates value and generates learning signals based on differences between expected and obtained outcomes. Basal ganglia and dopaminergic systems have strongly influenced such computational interpretations, linking neuroscience with algorithms for adaptive decision making and control.

For AI agents, basal-ganglia-inspired selection can be implemented as a gating layer between candidate behaviors and execution. Perception, memory, planning, and language systems may propose several actions, while a selection mechanism evaluates their learned utility, context, constraints, and current priorities. Only sufficiently supported actions are allowed to control downstream processes.

This approach becomes especially valuable in embodied AI, where simultaneous execution of incompatible behaviors can create physical failure. A robot cannot safely turn left and right at the same instant, manipulate two unreachable objects with one gripper, or continue forward while an emergency stop requires immediate inhibition. Explicit action gating therefore converts cognitive alternatives into physically coherent behavior.

Safety can be incorporated as an additional inhibitory mechanism. Even when a candidate action has high expected reward, collision risk, actuator limits, energy constraints, human proximity, or operational rules may require suppression. Brain-inspired action selection therefore suggests architectures in which reward-driven facilitation operates together with strong constraint-based inhibition rather than relying on reward maximization alone.

Multi-agent robotics introduces another layer of competition and coordination. Candidate actions must account not only for one robot\'s state but also for teammates, shared resources, communication, and collective goals. Selection mechanisms can combine local action values with team-level constraints, enabling individual agents to choose behaviors that remain compatible with coordinated group activity.

Learning must continue after selection because the outcome provides evidence about whether the chosen action was appropriate. The cycle can be represented as state and context, candidate actions, selection, execution, outcome, prediction error, and value update. This recurrent loop gradually changes future selection preferences and connects action selection directly with continual adaptation.

Memory can strengthen this process by providing examples beyond immediate reinforcement. Episodic memory can retrieve previous successes or failures in similar situations, semantic memory can provide rules and constraints, and procedural memory can supply learned policies. The basal ganglia can therefore be understood as part of a broader decision network in which multiple memory systems influence competition among possible behaviors.

World models add prospective information to this architecture. Instead of relying exclusively on previously learned action values, an agent can predict the consequences of candidate actions and feed expected outcomes into the selection process. This allows model-based planning and model-free learned preferences to cooperate, combining flexible simulation with efficient experience-based action tendencies.

The progression toward value-based decision making follows naturally from this mechanism. Once candidate actions can be selectively facilitated or suppressed, the next question is how their expected outcomes acquire values that permit meaningful comparison. The chapter therefore places value-based decision making immediately after basal ganglia and action selection, connecting neural gating mechanisms with broader principles of utility, reward, cost, and preference.

For AI design, the important lesson is not to reproduce every anatomical pathway literally but to preserve the functional principles of selective gating, competition, inhibition, reinforcement-driven adaptation, context dependence, and recurrent feedback. These principles provide a useful architecture for transforming many possible actions into one coherent behavior while continuously learning from the consequences.

The basal ganglia ultimately illustrate that intelligent behavior requires both selection and suppression. Goals and plans alone cannot control an agent unless one behavior is granted access to execution while incompatible alternatives are restrained. By integrating cortical context with learned values, dopamine-related learning, recurrent gating, and behavioral feedback, basal ganglia circuits provide a biological model for converting decision possibilities into adaptive action.

기저핵(Basal Ganglia)은 행동 선택(Action Selection), 강화 학습(Reinforcement Learning), 습관 형성(Habit Formation), 동기(Motivation), 운동 조절(Movement Regulation)에서 핵심적인 역할을 수행하는 상호 연결된 피질하 구조(Subcortical Structures)의 집합입니다. 전체 장의 구조에서 기저핵은 전전두엽 피질(Prefrontal Cortex) 다음에 위치하고 가치 기반 의사결정(Value-Based Decision Making)에 앞서 등장하며, 목표, 맥락, 후보 행동(Candidate Actions), 학습된 가치(Learned Values)가 어떤 행동을 촉진하거나 억제할지를 결정하는 핵심 메커니즘으로 기능합니다.

지능형 유기체는 지속적으로 많은 가능한 행동을 가지고 있지만 특정 순간에는 그중 제한된 일부만 실행할 수 있기 때문에 행동 선택이 필요합니다. 걷기, 정지하기, 손을 뻗기, 방향 전환하기, 말하기, 기다리기, 전략 변경하기 등이 모두 제어권(Control)을 얻기 위해 경쟁할 수 있습니다. 기저핵은 어떤 행동 관련 피질 과정이 실행될 수 있을 만큼 충분한 지원을 받을지, 그리고 어떤 행동이 억제된 상태로 유지될지를 조절함으로써 이러한 경쟁을 해결하는 데 기여합니다.

기저핵을 행동을 독립적으로 선택하는 단순한 명령 중추(Command Center)로 이해해서는 안 됩니다. 기저핵은 반복적인 피질--기저핵--시상 루프(Cortico--Basal Ganglia--Thalamic Loops)에 참여하며, 이 과정에서 피질 표상(Cortical Representations)이 피질하 회로로 들어가고 선택과 관련된 신호가 다시 피질 방향으로 전달됩니다. 이러한 구조를 통해 피질 시스템에 표상된 목표와 맥락 정보가 학습된 행동 선호도(Action Preferences) 및 선택 메커니즘과 지속적으로 상호작용할 수 있습니다.

주요 구성 요소에는 선조체(Striatum), 창백핵(Globus Pallidus), 시상하핵(Subthalamic Nucleus), 흑질(Substantia Nigra), 그리고 시상(Thalamus) 및 대뇌피질(Cerebral Cortex)과 연결되는 관련 회로가 포함됩니다. 선조체는 광범위한 피질 입력을 받아 기저핵 회로의 주요 입력 지점으로 기능합니다. 출력 구조(Output Structures)는 시상과 뇌간(Brainstem)의 표적을 조절하여 특정 운동 또는 인지 과정이 촉진될 수 있는지에 영향을 줍니다.

선조체는 목표, 맥락, 후보 행동, 감각적 특징(Sensory Features), 기타 작업 관련 변수(Task-Relevant Variables)를 나타내는 정보를 입력받습니다. 이러한 입력이 이미 선택된 하나의 행동만을 나타내는 것은 아닙니다. 여러 가능성이 동시에 표상될 수 있으며, 기저핵 회로는 학습된 가치와 현재 조건에 따라 경쟁하는 표상들을 변환하여 행동을 선택적으로 게이팅(Selective Gating)하는 데 기여할 수 있습니다.

유용한 개념적 모델은 직접 경로(Direct Pathway)와 간접 경로(Indirect Pathway)를 구분합니다. 직접 경로는 일반적으로 기저핵 출력핵(Output Nuclei)의 억제성 출력을 감소시켜 선택된 행동을 촉진하고, 관련 시상--피질 활동(Thalamocortical Activity)이 진행되도록 하는 것과 연관됩니다. 간접 경로는 추가적인 회로 단계를 통해 억제 효과를 증가시켜 경쟁하거나 부적절한 행동을 억제하는 데 기여합니다.

이러한 촉진--억제(Facilitation--Suppression) 구조는 행동 선택을 이해하는 데 유용한 프레임워크를 제공합니다. 선택은 단순히 원하는 행동을 활성화하는 것만을 의미하지 않으며, 경쟁하는 대안들도 함께 제어해야 합니다. 따라서 신뢰할 수 있는 행동은 맥락적으로 적절한 처리 과정에 대한 지원을 증가시키는 동시에 서로 양립할 수 없는 반응이 실행을 방해하지 못하도록 억제하는 데 의존합니다.

시상하핵은 이러한 조절 아키텍처(Regulatory Architecture)의 또 다른 중요한 구성 요소입니다. 시상하핵은 기저핵 출력에 광범위하게 영향을 줄 수 있으며, 경쟁하는 대안이나 불확실한 상황에서 추가적인 주의가 필요할 때 억제 제어(Inhibitory Control)를 증가시키는 메커니즘과 관련되는 경우가 많습니다. 기능적으로 이는 너무 빠른 선택이 부적절한 행동을 초래할 수 있는 상황에서 결정을 지연하거나 조절하는 방법을 제공합니다.

기저핵의 출력은 대부분 억제성(Inhibitory)이므로 탈억제(Disinhibition)는 이러한 회로를 이해하는 데 중요한 개념입니다. 후보 행동은 지속적인 억제 제어(Tonic Inhibitory Control)를 받고 있는 것으로 볼 수 있으며, 선택 과정에서는 선호되는 경로에 대한 억제가 감소합니다. 이러한 구조는 적절한 행동은 해제되도록 하고 다른 대안은 상대적으로 억제된 상태로 유지하는 게이팅 메커니즘(Gating Mechanism)을 형성합니다.

시상은 되돌아오는 루프(Returning Loop)의 중요한 부분을 구성합니다. 기저핵 출력은 시상 활동에 영향을 주고, 시상 신호는 다시 피질 영역으로 투사됩니다. 따라서 선택은 단방향 과정으로 구현되는 것이 아니라 반복 회로(Recurrent Circuit)에 포함됩니다. 피질 처리가 기저핵 활동에 영향을 주고, 그 결과로 생성된 게이팅 신호가 이후의 피질 처리와 행동을 다시 변화시킵니다.

이러한 루프는 운동에만 국한되지 않습니다. 병렬적인 피질--기저핵 회로(Parallel Cortico--Basal Ganglia Circuits)는 운동, 연합, 변연계 피질 영역(Motor, Associative, and Limbic Cortical Regions)과 상호작용하여 관련 원리가 운동 행동뿐 아니라 인지 과정, 동기, 의사결정에도 영향을 주도록 합니다. 따라서 행동 선택은 물리적 움직임뿐 아니라 전략, 작업 세트(Task Sets), 행동을 조직하는 기타 처리 과정을 선택하는 것까지 포함할 수 있습니다.

전전두엽 피질과의 관계는 특히 중요합니다. 전전두엽 시스템은 목표, 규칙, 맥락, 후보 행동, 관련 특징을 유지할 수 있으며, 기저핵 회로는 행동과 처리 과정을 촉진하거나 억제하는 데 기여합니다. 이러한 시스템들이 함께 작동함으로써 인지적 목표(Cognitive Goals)가 수동적인 내부 표상으로만 남지 않고 실제 선택된 행동으로 변환될 수 있습니다.

행동 선택은 경험을 통해서도 적응해야 합니다. 반복적으로 유용한 결과를 만들어내는 행동은 유사한 조건에서 일반적으로 더 쉽게 선택되어야 하며, 좋지 않은 결과와 관련된 행동은 선택 가능성이 낮아져야 합니다. 따라서 기저핵은 상태--행동--결과(State--Action--Outcome) 관계가 미래의 행동 경향(Behavioral Tendencies)을 변화시키는 강화 학습과 긴밀하게 연결되어 있습니다.

도파민(Dopamine)은 이러한 아키텍처에서 중요한 학습 관련 신호를 제공합니다. 특히 흑질 치밀부(Substantia Nigra Pars Compacta)와 관련된 도파민성 뉴런(Dopaminergic Neurons)은 선조체로 강하게 투사하며 기저핵 회로 내부의 가소성(Plasticity)을 조절합니다. 도파민을 단순한 쾌락 신호(Pleasure Signal)로 해석해서는 안 되며, 계산적 의미에는 예상하지 못한 결과와 기대 가치(Expected Value)의 변화에 관련된 정보를 전달하는 기능도 포함됩니다.

보상 예측 오차(Reward Prediction Error)는 이러한 학습 신호를 이해하기 위한 중요한 프레임워크를 제공합니다. 실제로 얻어진 결과가 예상보다 좋으면 긍정적 예측 오차(Positive Prediction Error)가 성공적인 행동에 기여한 관계를 강화할 수 있습니다. 결과가 예상보다 나쁘면 부정적 예측 오차(Negative Prediction Error)가 해당 관계를 반대 방향으로 수정하여 미래의 행동 선호도를 점진적으로 변화시킬 수 있습니다.

반복적인 학습을 통해 시스템은 특정 상태나 맥락을 가치 있는 결과를 만들어내는 경향이 있는 행동과 연관시킬 수 있습니다. 그러면 에이전트가 모든 행동의 가치를 처음부터 다시 계산할 필요가 줄어들기 때문에 의사결정은 점차 효율적으로 이루어질 수 있습니다. 학습된 행동 경향은 후보 행동 사이의 경쟁을 빠르게 편향시킬 수 있는 사전 구조(Prior Structure)를 제공합니다.

이러한 메커니즘은 기저핵을 절차 기억(Procedural Memory)과 연결합니다. 기술(Skills)과 습관(Habits)은 반복되는 상태--행동--결과 경험을 통해 발달하며, 점차 행동을 더 빠르고 명시적인 숙고(Deliberate Reasoning)에 덜 의존하도록 만듭니다. 따라서 보다 광범위한 기억 아키텍처에서 기저핵 기능은 습관 형성, 행동 선택, 강화 학습과 긴밀하게 연관됩니다.

습관 형성은 학습된 행동 선택의 장점과 한계를 동시에 보여줍니다. 반복적으로 성공한 행동은 효율적이고 자동화되어 인지적 부담(Cognitive Demand)을 줄일 수 있습니다. 그러나 강하게 학습된 반응은 목표나 환경 조건이 변화하면 부적절해질 수 있습니다. 따라서 유연한 지능(Flexible Intelligence)을 위해서는 습관적 메커니즘과 목표 지향적 제어(Goal-Directed Control)가 가능한 시스템 사이의 상호작용이 필요합니다.

목표 지향적 행동은 현재의 결과와 그 결과가 지금 가지는 가치에 더욱 강하게 의존합니다. 반면 습관적 행동은 상태와 반응 사이에서 과거에 학습된 연관 관계에 더 크게 의존합니다. 이 두 가지 방식을 완전히 분리된 시스템으로 볼 필요는 없으며, 행동은 경험, 불확실성, 새로움(Novelty), 작업 요구사항, 환경의 안정성에 따라 두 방식 사이에서 전환될 수 있습니다.

따라서 기저핵은 의사결정의 안정성--유연성 균형(Stability--Flexibility Balance)에 기여합니다. 안정적으로 학습된 정책(Policies)을 이용하면 익숙한 상황을 효율적으로 처리할 수 있지만, 상황을 다시 검토해야 하는 경우에는 피질 제어(Cortical Control)가 개입할 수 있습니다. 효과적인 의사결정 아키텍처는 이전 학습이 더 이상 적절하지 않은 상황을 지배하지 않도록 하면서도 충분히 학습된 행동을 유지하는 데서 이점을 얻습니다.

행동 선택은 동기에도 의존합니다. 행동의 가치는 내부 상태와 현재 목표에 따라 변화합니다. 음식 탐색, 에너지 보존, 위험 회피, 학습된 보상 추구 등은 생리적 및 맥락적 조건에 따라 중요도가 높아지거나 낮아질 수 있습니다. 변연계와 관련된 기저핵 회로(Limbic-Related Basal Ganglia Circuits)는 동기 정보를 어떤 행동이 선택 우선순위를 얻을지에 반영할 수 있도록 합니다.

운동 조절은 기저핵 기능이 가장 명확하게 나타나는 사례 가운데 하나입니다. 자발적 운동(Voluntary Movement)을 수행하려면 의도된 운동 프로그램(Motor Programs)을 선택하면서 경쟁하는 움직임이 실행을 방해하지 않도록 해야 합니다. 기저핵은 운동 및 전운동 피질(Motor and Premotor Cortical Systems)과 상호작용하여 행동의 시작, 크기 조절(Scaling), 순서화(Sequencing), 전환(Switching)에 영향을 주며, 소뇌(Cerebellum)와 같은 다른 시스템은 예측, 타이밍, 협응(Coordination), 오차 보정(Error Correction)에 기여합니다.

이러한 역할 분담은 뇌에서 영감을 받은 로보틱스(Brain-Inspired Robotics)를 이해하는 데 유용합니다. 기저핵은 어떤 행동 또는 정책이 제어권을 얻어야 하는지를 결정하는 것과 더 밀접하게 관련되고, 소뇌는 움직임이 어떻게 전개될지를 예측하고 정교화하는 기능과 강하게 관련됩니다. 운동 피질 및 척수 시스템(Motor Cortical and Spinal Systems)은 선택된 행동을 물리적 효과기(Physical Effectors)를 통해 표상하고 실행하는 데 참여합니다.

선택은 계층적(Hierarchical)으로도 작동합니다. 상위 수준에서 에이전트는 탐색(Exploration), 내비게이션(Navigation), 조작(Manipulation), 충전(Charging), 대기(Waiting) 가운데 하나를 선택할 수 있습니다. 중간 수준에서는 경로, 기술, 모션 프리미티브(Motion Primitives)를 선택할 수 있고, 하위 수준에서는 제어 시스템이 세부적인 운동 명령을 결정합니다. 따라서 기저핵에서 영감을 받은 게이팅 원리는 개별 근육 움직임뿐 아니라 여러 수준의 행동 선택에 적용될 수 있습니다.

동일한 행동이라도 어떤 상태에서는 바람직하지만 다른 상태에서는 부적절할 수 있기 때문에 맥락(Context)이 필수적입니다. 예를 들어 물체에 손을 뻗는 행동은 물체에 접근할 수 있을 때는 유용하지만 장애물이 팔을 가로막고 있다면 위험할 수 있습니다. 따라서 학습된 선택 메커니즘은 행동 자체에 상황과 무관한 하나의 고정된 가치를 할당하는 대신 관련 상태 표상(State Representations)에 따라 행동 선호도를 조건화해야 합니다.

불확실성도 행동 선택에 영향을 미칩니다. 하나의 대안이 더 바람직하다는 강한 증거가 있다면 빠르게 결정하는 것이 적절할 수 있습니다. 그러나 여러 대안이 비슷한 수준의 지지를 받거나 잠재적인 결과가 심각하다면 추가적인 정보 수집이나 결정 지연이 더 유리할 수 있습니다. 따라서 선택 메커니즘은 학습된 가치를 무조건 최대화하기보다 신뢰도(Confidence), 위험, 모니터링 과정과 상호작용해야 합니다.

강화 학습의 관점에서 행동 선택은 상태나 관찰을 행동에 대한 확률 또는 선호도로 매핑하는 정책(Policy)으로 표현할 수 있습니다. 경험은 보상과 예측 오차에 따라 정책이나 그 기반이 되는 가치 추정(Value Estimates)을 변화시킵니다. 이는 기저핵 기능에 대한 계산적 유사성(Computational Analogy)을 제공하지만, 인공 정책을 생물학적 회로의 문자 그대로의 복제물로 보아서는 안 됩니다.

액터--크리틱 아키텍처(Actor--Critic Architecture)는 또 다른 유용한 기능적 비유를 제공합니다. 액터(Actor)는 행동을 표상하거나 선택하고, 크리틱(Critic)은 가치를 추정하며 예상 결과와 실제 결과 사이의 차이를 기반으로 학습 신호를 생성합니다. 기저핵과 도파민 시스템은 이러한 계산적 해석에 큰 영향을 주었으며, 신경과학과 적응형 의사결정 및 제어 알고리즘을 연결합니다.

인공지능 에이전트(AI Agents)에서는 기저핵에서 영감을 받은 선택을 후보 행동과 실행 사이의 게이팅 계층(Gating Layer)으로 구현할 수 있습니다. 지각, 기억, 계획, 언어 시스템(Language Systems)이 여러 행동을 제안하면 선택 메커니즘이 학습된 효용(Learned Utility), 맥락, 제약 조건, 현재 우선순위를 평가할 수 있습니다. 충분한 지지를 얻은 행동만 하위 처리 과정에 대한 제어권을 획득하도록 할 수 있습니다.

이러한 접근은 서로 양립할 수 없는 행동을 동시에 실행하면 물리적 실패가 발생할 수 있는 체화 인공지능(Embodied AI)에서 특히 중요합니다. 로봇은 안전하게 왼쪽과 오른쪽으로 동시에 회전할 수 없고, 하나의 그리퍼(Gripper)로 동시에 두 개의 접근 불가능한 객체를 조작할 수도 없으며, 비상 정지(Emergency Stop)가 즉각적인 억제를 요구하는 동안 계속 전진해서도 안 됩니다. 따라서 명시적인 행동 게이팅(Explicit Action Gating)은 인지적 대안을 물리적으로 일관된 행동으로 변환합니다.

안전(Safety)은 추가적인 억제 메커니즘으로 포함될 수 있습니다. 후보 행동의 예상 보상이 높더라도 충돌 위험(Collision Risk), 액추에이터 한계(Actuator Limits), 에너지 제약(Energy Constraints), 인간과의 근접성(Human Proximity), 운영 규칙(Operational Rules)에 따라 해당 행동을 억제해야 할 수 있습니다. 따라서 뇌에서 영감을 받은 행동 선택은 보상 중심의 촉진과 강력한 제약 기반 억제(Constraint-Based Inhibition)가 함께 작동하는 아키텍처를 제안하며, 단순한 보상 최대화에만 의존하지 않습니다.

다중 에이전트 로보틱스(Multi-Agent Robotics)는 경쟁과 협력에 또 다른 계층을 추가합니다. 후보 행동은 하나의 로봇 상태뿐 아니라 팀원(Teammates), 공유 자원(Shared Resources), 통신, 공동 목표(Collective Goals)도 고려해야 합니다. 선택 메커니즘은 지역적 행동 가치(Local Action Values)를 팀 수준 제약(Team-Level Constraints)과 결합하여 개별 에이전트가 협력적인 그룹 행동과 양립할 수 있는 행동을 선택하도록 할 수 있습니다.

선택 이후에도 학습은 계속되어야 합니다. 실행 결과는 선택된 행동이 적절했는지에 관한 증거를 제공하기 때문입니다. 이 과정은 상태와 맥락(State and Context), 후보 행동, 선택, 실행(Execution), 결과(Outcome), 예측 오차, 가치 갱신(Value Update)의 순환으로 표현할 수 있습니다. 이러한 반복 루프(Recurrent Loop)는 미래의 선택 선호도를 점진적으로 변화시키고 행동 선택을 지속적인 적응(Continual Adaptation)과 직접 연결합니다.

기억은 즉각적인 강화 신호를 넘어서는 사례를 제공함으로써 이러한 과정을 강화할 수 있습니다. 일화 기억(Episodic Memory)은 유사한 상황에서 이전에 경험한 성공이나 실패를 검색할 수 있고, 의미 기억(Semantic Memory)은 규칙과 제약 조건을 제공하며, 절차 기억은 학습된 정책을 제공할 수 있습니다. 따라서 기저핵은 여러 기억 시스템이 가능한 행동 사이의 경쟁에 영향을 주는 보다 광범위한 의사결정 네트워크(Decision Network)의 일부로 이해할 수 있습니다.

월드 모델(World Models)은 이러한 아키텍처에 미래 지향적 정보(Prospective Information)를 추가합니다. 에이전트는 이전에 학습한 행동 가치에만 의존하는 대신 후보 행동의 결과를 예측하고 예상 결과를 선택 과정에 제공할 수 있습니다. 이를 통해 모델 기반 계획(Model-Based Planning)과 모델 프리 학습 선호도(Model-Free Learned Preferences)가 협력하여 유연한 시뮬레이션과 효율적인 경험 기반 행동 경향을 결합할 수 있습니다.

가치 기반 의사결정으로의 진행은 이러한 메커니즘에서 자연스럽게 이어집니다. 후보 행동을 선택적으로 촉진하거나 억제할 수 있게 되면 다음 질문은 예상 결과가 어떻게 의미 있는 비교를 가능하게 하는 가치(Value)를 획득하는가입니다. 따라서 가치 기반 의사결정(Value-Based Decision Making)은 기저핵과 행동 선택 이후에 연결되며, 신경 게이팅 메커니즘(Neural Gating Mechanisms)을 효용(Utility), 보상, 비용(Cost), 선호(Preference)라는 보다 광범위한 원리와 연결합니다.

인공지능 설계(AI Design)에서 중요한 교훈은 모든 해부학적 경로(Anatomical Pathways)를 문자 그대로 재현하는 것이 아니라 선택적 게이팅(Selective Gating), 경쟁(Competition), 억제(Inhibition), 강화 기반 적응(Reinforcement-Driven Adaptation), 맥락 의존성(Context Dependence), 반복 피드백(Recurrent Feedback)이라는 기능적 원리를 보존하는 것입니다. 이러한 원리는 많은 가능한 행동을 하나의 일관된 행동으로 변환하면서 그 결과로부터 지속적으로 학습할 수 있는 유용한 아키텍처를 제공합니다.

궁극적으로 기저핵은 지능적인 행동이 선택(Selection)과 억제(Suppression)를 모두 필요로 한다는 것을 보여줍니다. 목표와 계획만으로는 하나의 행동이 실행 권한을 얻고 서로 양립할 수 없는 다른 대안들이 억제되지 않는 한 에이전트를 제어할 수 없습니다. 기저핵 회로는 피질의 맥락 정보와 학습된 가치, 도파민 관련 학습(Dopamine-Related Learning), 반복적 게이팅(Recurrent Gating), 행동 피드백(Behavioral Feedback)을 통합함으로써 다양한 의사결정 가능성을 적응적인 행동(Adaptive Action)으로 변환하는 생물학적 모델을 제공합니다.

##  

## 08.03 Value Based Decision Making [w/Code]

![](images/image4.png){width="7.268055555555556in" height="7.268055555555556in"}

Value-based decision making is the process of selecting among possible actions by estimating and comparing the value of their expected outcomes. It extends action selection beyond simple stimulus-response mappings because alternatives may differ in reward, cost, effort, risk, delay, and relevance to current goals. An intelligent system must therefore determine not only what actions are possible, but which outcome is presently worth pursuing.

Value provides a common decision variable through which otherwise different alternatives can be compared. Food, safety, social interaction, information, energy conservation, or progress toward a goal may have very different physical properties, yet each can influence behavior. Neural and artificial decision systems therefore require mechanisms that transform heterogeneous consequences into representations that support meaningful comparison and choice.

Value should not be understood as a permanent property attached to an object or action. It depends on the relationship between an outcome and the current state of the agent. Food becomes more valuable when an organism is hungry, while energy-efficient behavior becomes more important to a robot when battery capacity is low. Value is therefore dynamic, contextual, and closely coupled to goals and internal state.

Decision value can incorporate both benefits and costs. An action may produce a desirable outcome while requiring substantial energy, time, physical effort, computational resources, or opportunity cost. Rational selection therefore requires considering net consequences rather than reward alone. A highly rewarding outcome may be rejected when the associated cost is sufficiently large relative to available alternatives.

Expected value becomes necessary when outcomes are uncertain. An action may produce several possible consequences, each associated with a different probability and value. Decision systems can combine these possibilities by considering both how desirable each outcome would be and how likely it is to occur. This allows choices to reflect probabilistic expectations rather than assuming that one predicted future is guaranteed.

Expected value alone, however, does not fully capture risk sensitivity. Two alternatives can have similar average expected returns while differing substantially in variability and potential loss. An agent operating in a safety-critical environment may prefer a predictable moderate outcome over a higher-variance alternative that includes a small probability of severe failure. Value-based decisions can therefore depend on risk preferences and safety constraints.

Temporal delay also changes value. A reward available immediately may be preferred over an equivalent reward available much later, a phenomenon commonly described through temporal discounting. However, effective long-term behavior requires avoiding excessive preference for immediate benefits. Decision systems must balance short-term value with delayed consequences when current actions influence future opportunities, resources, or goals.

This temporal dimension connects value-based decision making directly with reinforcement learning. An action can be valuable not only because of its immediate reward but also because it moves the agent into a state from which valuable future outcomes become available. Value functions therefore estimate cumulative future consequences rather than evaluating each action exclusively according to what happens immediately after execution.

State value represents the expected future return associated with being in a particular state, whereas action value represents the expected return associated with performing a particular action in that state. These representations allow an agent to compare possibilities before execution. By learning how states and actions relate to future outcomes, decision systems can progressively improve behavior through accumulated experience.

Reward prediction error provides a central learning mechanism for updating value estimates. When an outcome is better than expected, the corresponding positive prediction error indicates that previous expectations were too low. When the outcome is worse than expected, a negative prediction error indicates that expectations were too high. Repeated updates gradually align predicted values with experienced consequences.

Dopamine-related neural signaling is strongly associated with this learning framework. Dopaminergic activity can reflect differences between expected and obtained outcomes, contributing to plasticity in circuits involved in reinforcement learning and action selection. Dopamine should therefore not be reduced to a simple representation of pleasure; it participates in adaptive learning about changes in expected value and behavioral significance.

The basal ganglia provide an important interface between learned value and action selection. Candidate actions can acquire different levels of support based on their previously learned consequences and current context. Actions associated with favorable outcomes may become easier to facilitate, while alternatives associated with poor outcomes may remain inhibited. Value learning can therefore progressively reshape future behavioral competition.

The prefrontal cortex contributes complementary capabilities by maintaining goals, contextual rules, working-memory contents, and representations of possible outcomes. A previously rewarding action may no longer be desirable when goals change. Prefrontal control allows current objectives and contextual information to modify the significance of learned values, supporting flexible decisions rather than automatic repetition of historically successful behavior.

The orbitofrontal cortex is particularly relevant to representations linking situations, options, and expected outcomes. Such representations allow value to change when the meaning of an outcome changes. If an outcome becomes less desirable because of satiation, changing goals, or altered environmental conditions, flexible decision systems should update behavior even before extensive relearning through repeated failure.

This distinction helps separate goal-directed behavior from habitual behavior. Goal-directed decisions depend strongly on representations of current outcomes and their present value, whereas habits depend more strongly on learned state-response relationships. Goal-directed behavior is flexible but computationally demanding, while habitual behavior can be fast and efficient but less sensitive to changes in outcome value.

Intelligent decision systems benefit from combining both mechanisms. Familiar situations with stable consequences can be handled efficiently through previously learned policies, while novel, uncertain, or changing situations may require explicit evaluation of expected outcomes. The balance between habitual and deliberative control can itself depend on uncertainty, experience, available computation, and the importance of the decision.

Value-based decision making also requires comparison among competing alternatives. Neural decision processes can accumulate evidence supporting different options until one becomes sufficiently favored. The rate of accumulation can depend on sensory evidence, remembered outcomes, expected value, uncertainty, and current goals. Choice therefore emerges dynamically from competition rather than necessarily from one instantaneous calculation.

Choice thresholds provide a way to regulate the tradeoff between speed and accuracy. A low threshold allows rapid decisions but increases the possibility of selecting an inferior option before sufficient evidence has accumulated. A higher threshold allows more evidence to be considered but delays action. Decision systems can adjust thresholds according to urgency, risk, uncertainty, and the consequences of making an error.

Opportunity cost further complicates valuation because selecting one action often prevents another from being executed. Time spent pursuing one goal cannot simultaneously be devoted to another incompatible goal. The value of an action therefore depends partly on what must be abandoned or postponed when that action is selected. Efficient agents must consider alternatives rather than evaluating each option independently.

Information itself can possess value. An action that produces little immediate external reward may be useful because it reduces uncertainty and improves future decisions. Looking around a corner, inspecting an unfamiliar object, requesting clarification, or exploring an unknown route can provide information that changes later action values. This creates a direct connection between valuation and active information gathering.

The value of information is particularly important under partial observability. When the current state is uncertain, committing immediately to a task action may be inferior to first obtaining another observation. A sophisticated decision system can therefore compare actions that directly pursue external goals with actions whose primary purpose is improving the quality of the internal state estimate.

Multi-objective decisions require valuation across several dimensions simultaneously. A robot may need to complete a mission quickly while conserving battery power, minimizing collision risk, reducing mechanical wear, preserving human comfort, and respecting operational constraints. These objectives cannot always be reduced naturally to one physical quantity, requiring explicit tradeoffs or structured preference mechanisms.

Scalar utility functions provide one approach by converting several objectives into a weighted combined value. Although computationally convenient, fixed weights may be insufficient when priorities change with context. Safety may dominate during human interaction, energy efficiency may become critical at low battery levels, and mission completion may dominate under time pressure. Adaptive weighting can therefore be essential.

Constraint-based decision making provides another approach. Instead of assigning every consideration a tradeable numerical value, some requirements can define boundaries that actions must not violate. Collision avoidance, actuator limits, restricted areas, or mandatory safety rules may eliminate candidate actions before reward comparison occurs. Value optimization then operates only within the remaining feasible action set.

This distinction is crucial for embodied AI because physical consequences cannot always be repaired through later learning. A simulated agent may tolerate many failed trials, while a physical robot can damage hardware, injure people, or lose mission capability through one unsafe action. Value-based Physical AI therefore requires explicit integration of utility, uncertainty, physical feasibility, and safety constraints.

World models extend valuation from learned associations toward prospective evaluation. If an agent can predict how actions transform the current state, it can simulate possible future trajectories and estimate their consequences before acting. This supports model-based decision making, where value is assigned not merely from historical experience but also from internally predicted futures.

Model accuracy becomes critical in this setting. A predicted trajectory can appear highly valuable because the world model overlooks an obstacle, underestimates uncertainty, or incorrectly predicts another agent\'s behavior. Decision systems should therefore consider confidence in predictions as part of valuation. Uncertain imagined outcomes may need conservative treatment, additional observation, or alternative planning.

Episodic memory contributes concrete evidence to value estimation. When a current situation resembles a previous experience, the system can retrieve what actions were taken and what consequences followed. Particularly significant successes, failures, hazards, or rare events can influence current decisions even when they are insufficiently frequent to dominate statistical learning.

Semantic memory provides generalized expectations accumulated across many experiences. Instead of recalling one specific event, an agent can know that certain surfaces are hazardous, particular objects are valuable, or specific actions usually require high energy. Semantic knowledge therefore supplies priors that shape valuation before direct experience with the exact current situation is available.

Procedural memory contributes learned policies that embody previous value-based learning. Once repeated decisions consistently favor similar actions, the resulting behavior can become proceduralized and executed with reduced deliberation. Memory consolidation and replay can further strengthen useful state-action-value relationships while preserving important failures that should continue to influence future choices.

Social decision making introduces values that depend on other agents. Cooperation, fairness, predictability, reputation, communication, and the welfare of others can influence which actions are considered desirable. Human-compatible autonomous systems therefore require value representations that extend beyond immediate task efficiency and account for the consequences of behavior within shared environments.

Multi-agent systems add collective value and coordination. An action that appears optimal for one robot independently may reduce overall team performance by creating congestion, duplicating work, consuming shared resources, or interfering with another agent. Decision making can therefore incorporate both local utility and team-level objectives so individual choices contribute to coordinated behavior.

For AI engineering, value-based decision making can be implemented through reward models, value functions, utility estimators, cost functions, learned preferences, constraints, and planning objectives. No single representation is universally sufficient. Practical systems often combine learned values with explicit engineering rules, safety limits, predictive models, memory, and hierarchical control.

Hierarchical valuation can reduce complexity by evaluating decisions at different levels of abstraction. A high-level controller may compare mission goals, an intermediate planner may compare routes or skills, and lower-level systems may evaluate motion alternatives. Each layer can operate with values appropriate to its temporal and physical scale while remaining constrained by higher-level objectives.

The complete value-based decision loop begins with the current state, goals, internal needs, and remembered experience. Candidate actions are generated, their possible consequences are predicted, values and costs are estimated, uncertainty and constraints are considered, and one action is selected. The resulting outcome then produces new evidence that updates memory, predictive models, and future value estimates.

Value-based decision making ultimately provides the mechanism through which an intelligent agent converts the question of what can be done into the more consequential question of what should be done. By integrating reward, cost, risk, delay, uncertainty, information, goals, memory, prediction, and constraints, it connects action selection with adaptive behavior and provides a foundation for increasingly autonomous biological and artificial intelligence.

가치 기반 의사결정(Value-Based Decision Making)은 가능한 행동들의 예상 결과(Expected Outcomes)에 대한 가치를 추정하고 비교하여 행동을 선택하는 과정입니다. 이는 대안들이 보상(Reward), 비용(Cost), 노력(Effort), 위험(Risk), 지연(Delay), 현재 목표와의 관련성에서 서로 다를 수 있기 때문에 단순한 자극--반응(Stimulus--Response) 연결을 넘어 행동 선택(Action Selection)을 확장합니다. 따라서 지능형 시스템(Intelligent System)은 어떤 행동이 가능한지만이 아니라 현재 어떤 결과를 추구할 가치가 있는지도 결정해야 합니다.

가치(Value)는 서로 다른 종류의 대안들을 비교할 수 있도록 하는 공통 의사결정 변수(Common Decision Variable)를 제공합니다. 음식, 안전, 사회적 상호작용(Social Interaction), 정보, 에너지 보존(Energy Conservation), 목표를 향한 진전은 물리적으로 매우 다른 특성을 가지지만 모두 행동에 영향을 줄 수 있습니다. 따라서 생물학적 및 인공 의사결정 시스템은 이질적인 결과(Heterogeneous Consequences)를 의미 있는 비교와 선택을 지원하는 표상으로 변환하는 메커니즘을 필요로 합니다.

가치는 객체나 행동에 영구적으로 부착된 고정된 속성으로 이해해서는 안 됩니다. 가치는 결과와 에이전트(Agent)의 현재 상태 사이의 관계에 따라 달라집니다. 생물체가 배고플 때 음식의 가치가 높아지는 것처럼 로봇의 배터리 용량이 낮아지면 에너지 효율적인 행동의 중요성이 증가합니다. 따라서 가치는 동적(Dynamic)이고 맥락 의존적(Contextual)이며 목표와 내부 상태(Internal State)에 밀접하게 연결됩니다.

의사결정 가치(Decision Value)는 이익과 비용을 모두 포함할 수 있습니다. 하나의 행동이 바람직한 결과를 제공하더라도 상당한 에너지, 시간, 물리적 노력, 계산 자원(Computational Resources), 기회비용(Opportunity Cost)을 요구할 수 있습니다. 따라서 합리적인 선택(Rational Selection)을 위해서는 보상만이 아니라 순수한 결과(Net Consequences)를 고려해야 합니다. 높은 보상을 제공하는 결과라도 관련 비용이 이용 가능한 다른 대안에 비해 충분히 크다면 선택되지 않을 수 있습니다.

결과가 불확실한 경우에는 기대 가치(Expected Value)가 필요합니다. 하나의 행동은 여러 가능한 결과를 만들어낼 수 있으며 각각의 결과에는 서로 다른 확률(Probability)과 가치가 연결됩니다. 의사결정 시스템은 각 결과가 얼마나 바람직한지와 실제로 발생할 가능성이 얼마나 높은지를 함께 고려하여 이러한 가능성을 결합할 수 있습니다. 이를 통해 하나의 예측된 미래가 반드시 발생한다고 가정하지 않고 확률적 기대(Probabilistic Expectations)에 기반하여 선택할 수 있습니다.

그러나 기대 가치만으로는 위험 민감성(Risk Sensitivity)을 완전히 설명할 수 없습니다. 두 대안의 평균적인 기대 수익(Expected Return)이 비슷하더라도 변동성(Variability)과 잠재적 손실(Potential Loss)은 크게 다를 수 있습니다. 안전이 중요한 환경에서 작동하는 에이전트는 심각한 실패 가능성이 조금이라도 포함된 변동성이 높은 대안보다 예측 가능한 중간 수준의 결과를 선호할 수 있습니다. 따라서 가치 기반 의사결정은 위험 선호도(Risk Preferences)와 안전 제약(Safety Constraints)에 따라 달라질 수 있습니다.

시간적 지연(Temporal Delay) 역시 가치를 변화시킵니다. 즉시 얻을 수 있는 보상은 훨씬 나중에 얻을 수 있는 동일한 보상보다 선호될 수 있으며, 이러한 현상은 일반적으로 시간 할인(Temporal Discounting)을 통해 설명됩니다. 그러나 효과적인 장기 행동(Long-Term Behavior)을 위해서는 즉각적인 이익을 지나치게 선호하지 않아야 합니다. 현재 행동이 미래의 기회, 자원 또는 목표에 영향을 미칠 때 의사결정 시스템은 단기 가치와 지연된 결과 사이의 균형을 유지해야 합니다.

이러한 시간적 차원은 가치 기반 의사결정을 강화 학습(Reinforcement Learning)과 직접 연결합니다. 행동은 즉각적인 보상 때문만이 아니라 가치 있는 미래 결과에 접근할 수 있는 상태로 에이전트를 이동시키기 때문에 가치가 있을 수 있습니다. 따라서 가치 함수(Value Functions)는 각 행동을 실행한 직후 발생하는 결과만 평가하는 대신 누적된 미래 결과(Cumulative Future Consequences)를 추정합니다.

상태 가치(State Value)는 특정 상태에 있을 때 기대되는 미래 수익을 나타내며, 행동 가치(Action Value)는 해당 상태에서 특정 행동을 수행했을 때 기대되는 수익을 나타냅니다. 이러한 표상을 통해 에이전트는 행동을 실행하기 전에 여러 가능성을 비교할 수 있습니다. 상태 및 행동과 미래 결과 사이의 관계를 학습함으로써 의사결정 시스템은 축적된 경험을 통해 행동을 점진적으로 개선할 수 있습니다.

보상 예측 오차(Reward Prediction Error)는 가치 추정(Value Estimates)을 갱신하기 위한 핵심적인 학습 메커니즘을 제공합니다. 결과가 예상보다 좋으면 이에 해당하는 긍정적 예측 오차(Positive Prediction Error)는 이전의 기대가 너무 낮았음을 나타냅니다. 결과가 예상보다 나쁘면 부정적 예측 오차(Negative Prediction Error)는 기대가 지나치게 높았음을 의미합니다. 이러한 갱신을 반복함으로써 예측된 가치는 실제 경험된 결과에 점진적으로 맞춰집니다.

도파민 관련 신경 신호(Dopamine-Related Neural Signaling)는 이러한 학습 프레임워크와 강하게 관련됩니다. 도파민성 활동(Dopaminergic Activity)은 예상 결과와 실제로 얻어진 결과 사이의 차이를 반영할 수 있으며, 강화 학습과 행동 선택에 관여하는 회로의 가소성(Plasticity)에 기여합니다. 따라서 도파민을 단순한 쾌락(Pleasure)의 표상으로 축소해서는 안 되며, 기대 가치의 변화와 행동적 중요성(Behavioral Significance)에 관한 적응적 학습에 참여하는 신호로 이해해야 합니다.

기저핵(Basal Ganglia)은 학습된 가치와 행동 선택 사이의 중요한 인터페이스를 제공합니다. 후보 행동(Candidate Actions)은 이전에 학습한 결과와 현재 맥락에 따라 서로 다른 수준의 지지를 받을 수 있습니다. 유리한 결과와 연관된 행동은 더욱 쉽게 촉진될 수 있고, 좋지 않은 결과와 연관된 대안은 억제된 상태로 남을 수 있습니다. 따라서 가치 학습(Value Learning)은 미래의 행동 경쟁(Behavioral Competition)을 점진적으로 변화시킬 수 있습니다.

전전두엽 피질(Prefrontal Cortex)은 목표, 맥락적 규칙(Contextual Rules), 작업 기억(Working Memory)의 내용, 가능한 결과에 대한 표상을 유지함으로써 상호보완적인 기능을 제공합니다. 이전에 보상을 받았던 행동이라도 목표가 변경되면 더 이상 바람직하지 않을 수 있습니다. 전전두엽 제어(Prefrontal Control)는 현재 목표와 맥락 정보가 학습된 가치의 중요성을 변경하도록 하여 과거에 성공했던 행동을 자동적으로 반복하기보다 유연한 의사결정을 지원합니다.

안와전두피질(Orbitofrontal Cortex)은 상황, 선택지, 예상 결과를 연결하는 표상과 특히 관련됩니다. 이러한 표상은 결과의 의미가 변화할 때 가치도 변화할 수 있도록 합니다. 포만(Satiation), 목표의 변화, 환경 조건의 변화로 특정 결과의 바람직함이 감소한다면 유연한 의사결정 시스템은 반복적인 실패를 통한 광범위한 재학습 없이도 행동을 변경할 수 있어야 합니다.

이러한 차이는 목표 지향적 행동(Goal-Directed Behavior)과 습관적 행동(Habitual Behavior)을 구분하는 데 도움을 줍니다. 목표 지향적 의사결정은 현재 결과의 표상과 그 결과가 현재 가지는 가치에 강하게 의존하지만, 습관은 학습된 상태--반응(State--Response) 관계에 더 크게 의존합니다. 목표 지향적 행동은 유연하지만 계산 비용이 높으며, 습관적 행동은 빠르고 효율적일 수 있지만 결과 가치의 변화에 덜 민감합니다.

지능형 의사결정 시스템은 두 메커니즘을 결합함으로써 이점을 얻을 수 있습니다. 결과가 안정적인 익숙한 상황은 이전에 학습된 정책(Policies)을 통해 효율적으로 처리할 수 있지만, 새롭거나 불확실하거나 변화하는 상황에서는 예상 결과에 대한 명시적인 평가가 필요할 수 있습니다. 습관적 제어와 숙고적 제어(Deliberative Control) 사이의 균형 자체도 불확실성, 경험, 이용 가능한 계산 자원, 의사결정의 중요성에 따라 달라질 수 있습니다.

가치 기반 의사결정은 경쟁하는 대안들 사이의 비교도 필요로 합니다. 신경 의사결정 과정(Neural Decision Processes)은 하나의 선택지가 충분히 우세해질 때까지 서로 다른 대안을 지지하는 증거를 축적할 수 있습니다. 이러한 축적 속도는 감각적 증거(Sensory Evidence), 기억된 결과, 기대 가치, 불확실성, 현재 목표에 따라 달라질 수 있습니다. 따라서 선택은 반드시 하나의 순간적인 계산으로 발생하는 것이 아니라 경쟁을 통해 동적으로 형성될 수 있습니다.

선택 임계값(Choice Thresholds)은 속도와 정확도(Speed--Accuracy) 사이의 절충을 조절하는 방법을 제공합니다. 낮은 임계값은 빠른 의사결정을 가능하게 하지만 충분한 증거가 축적되기 전에 열등한 대안을 선택할 가능성을 높입니다. 높은 임계값은 더 많은 증거를 고려할 수 있지만 행동을 지연시킵니다. 의사결정 시스템은 긴급성(Urgency), 위험, 불확실성, 오류 발생 시의 결과에 따라 임계값을 조절할 수 있습니다.

기회비용은 하나의 행동을 선택하면 다른 행동을 수행하지 못하는 경우가 많기 때문에 가치 평가(Valuation)를 더욱 복잡하게 만듭니다. 하나의 목표를 추구하는 데 사용된 시간은 동시에 서로 양립할 수 없는 다른 목표에 사용할 수 없습니다. 따라서 행동의 가치는 해당 행동을 선택함으로써 무엇을 포기하거나 연기해야 하는지에도 부분적으로 의존합니다. 효율적인 에이전트는 각각의 선택지를 독립적으로 평가하기보다 대안들을 함께 고려해야 합니다.

정보 자체도 가치(Value of Information)를 가질 수 있습니다. 즉각적인 외부 보상을 거의 제공하지 않는 행동이라도 불확실성을 감소시키고 미래의 의사결정을 개선한다면 유용할 수 있습니다. 모퉁이 너머를 살펴보거나, 익숙하지 않은 객체를 검사하거나, 추가 설명을 요청하거나, 알려지지 않은 경로를 탐색하는 행동은 이후의 행동 가치를 변화시키는 정보를 제공할 수 있습니다. 이는 가치 평가와 능동적 정보 수집(Active Information Gathering)을 직접 연결합니다.

정보 가치(Value of Information)는 부분 관찰 가능성(Partial Observability)이 존재할 때 특히 중요합니다. 현재 상태가 불확실하다면 즉시 작업 행동에 전념하는 것보다 먼저 추가적인 관찰을 확보하는 것이 더 유리할 수 있습니다. 따라서 정교한 의사결정 시스템은 외부 목표를 직접 추구하는 행동과 내부 상태 추정(Internal State Estimate)의 품질을 향상시키는 것을 주목적으로 하는 행동을 비교할 수 있습니다.

다목적 의사결정(Multi-Objective Decision Making)은 여러 차원에 걸쳐 동시에 가치를 평가해야 합니다. 로봇은 임무를 빠르게 완료하면서 배터리 전력을 절약하고, 충돌 위험을 최소화하고, 기계적 마모(Mechanical Wear)를 줄이고, 인간의 편안함(Human Comfort)을 유지하며, 운영 제약(Operational Constraints)을 준수해야 할 수 있습니다. 이러한 목표들을 항상 하나의 물리량으로 자연스럽게 환산할 수 있는 것은 아니므로 명시적인 절충 또는 구조화된 선호 메커니즘(Structured Preference Mechanisms)이 필요합니다.

스칼라 효용 함수(Scalar Utility Functions)는 여러 목표를 가중 결합된 하나의 가치로 변환하는 방법을 제공합니다. 계산상 편리하지만 우선순위가 맥락에 따라 변화한다면 고정된 가중치(Fixed Weights)만으로는 충분하지 않을 수 있습니다. 인간과 상호작용할 때는 안전이 가장 중요할 수 있고, 배터리가 부족하면 에너지 효율성이 핵심이 되며, 시간 압박이 있을 때는 임무 완료가 우선될 수 있습니다. 따라서 적응적 가중치(Adaptive Weighting)가 필수적일 수 있습니다.

제약 기반 의사결정(Constraint-Based Decision Making)은 또 다른 접근법을 제공합니다. 모든 고려사항에 서로 교환 가능한 수치적 가치를 부여하는 대신 일부 요구사항은 행동이 절대로 위반해서는 안 되는 경계(Boundaries)를 정의할 수 있습니다. 충돌 회피(Collision Avoidance), 액추에이터 한계(Actuator Limits), 제한 구역(Restricted Areas), 필수 안전 규칙은 보상을 비교하기 전에 후보 행동을 제거할 수 있습니다. 이후 가치 최적화(Value Optimization)는 남아 있는 실행 가능한 행동 집합(Feasible Action Set) 안에서만 수행됩니다.

이러한 구분은 물리적 결과를 이후의 학습만으로 항상 복구할 수 없는 체화 인공지능(Embodied AI)에서 매우 중요합니다. 시뮬레이션 에이전트(Simulated Agent)는 많은 실패 시행을 허용할 수 있지만 물리적 로봇은 단 한 번의 안전하지 않은 행동으로 하드웨어를 손상시키거나, 사람을 다치게 하거나, 임무 수행 능력을 잃을 수 있습니다. 따라서 가치 기반 피지컬 AI(Physical AI)는 효용, 불확실성, 물리적 실행 가능성(Physical Feasibility), 안전 제약을 명시적으로 통합해야 합니다.

월드 모델(World Models)은 가치 평가를 학습된 연관 관계에서 미래 지향적 평가(Prospective Evaluation)로 확장합니다. 에이전트가 행동이 현재 상태를 어떻게 변화시키는지 예측할 수 있다면 행동하기 전에 가능한 미래 궤적(Future Trajectories)을 시뮬레이션하고 그 결과를 추정할 수 있습니다. 이는 과거 경험뿐 아니라 내부적으로 예측된 미래에 대해서도 가치를 부여하는 모델 기반 의사결정(Model-Based Decision Making)을 지원합니다.

이러한 상황에서는 모델 정확도(Model Accuracy)가 매우 중요합니다. 월드 모델이 장애물을 놓치거나, 불확실성을 과소평가하거나, 다른 에이전트의 행동을 잘못 예측한다면 실제로는 위험한 궤적이 매우 가치 있는 것으로 평가될 수 있습니다. 따라서 의사결정 시스템은 예측에 대한 신뢰도(Confidence)를 가치 평가의 일부로 고려해야 합니다. 불확실한 가상 결과(Imagined Outcomes)는 보수적으로 처리하거나 추가적인 관찰 또는 대안적 계획(Alternative Planning)을 요구할 수 있습니다.

일화 기억(Episodic Memory)은 가치 추정에 구체적인 증거를 제공합니다. 현재 상황이 이전 경험과 유사하다면 시스템은 과거에 어떤 행동을 수행했고 어떤 결과가 뒤따랐는지를 검색할 수 있습니다. 특히 중요한 성공, 실패, 위험 상황(Hazards), 희귀 사건(Rare Events)은 통계적 학습에서 지배적인 영향을 줄 만큼 자주 발생하지 않았더라도 현재의 의사결정에 영향을 줄 수 있습니다.

의미 기억(Semantic Memory)은 많은 경험을 통해 축적된 일반화된 기대(Generalized Expectations)를 제공합니다. 하나의 특정 사건을 회상하는 대신 에이전트는 특정 표면이 위험하거나, 특정 객체가 가치 있거나, 특정 행동이 일반적으로 많은 에너지를 요구한다는 사실을 알 수 있습니다. 따라서 의미 지식은 현재와 정확히 동일한 상황을 직접 경험하기 전에도 가치 평가를 형성하는 사전 지식(Priors)을 제공합니다.

절차 기억(Procedural Memory)은 이전의 가치 기반 학습을 내포하고 있는 학습된 정책을 제공합니다. 반복적인 의사결정에서 지속적으로 비슷한 행동이 선택되면 해당 행동은 절차화(Proceduralization)되어 숙고를 줄이면서 실행될 수 있습니다. 기억 공고화(Memory Consolidation)와 재생(Replay)은 유용한 상태--행동--가치(State--Action--Value) 관계를 더욱 강화하는 동시에 미래의 선택에 계속 영향을 주어야 하는 중요한 실패 경험을 보존할 수 있습니다.

사회적 의사결정(Social Decision Making)은 다른 에이전트에 따라 달라지는 가치를 추가합니다. 협력(Cooperation), 공정성(Fairness), 예측 가능성(Predictability), 평판(Reputation), 의사소통(Communication), 다른 존재의 복지(Welfare)는 어떤 행동이 바람직한지를 결정하는 데 영향을 줄 수 있습니다. 따라서 인간과 호환되는 자율 시스템(Human-Compatible Autonomous Systems)은 즉각적인 작업 효율성을 넘어 공유 환경에서 행동이 만들어내는 결과를 고려하는 가치 표상을 필요로 합니다.

다중 에이전트 시스템(Multi-Agent Systems)은 집단 가치(Collective Value)와 협력을 추가합니다. 하나의 로봇에게 독립적으로 최적으로 보이는 행동도 혼잡(Congestion)을 발생시키거나, 작업을 중복하거나, 공유 자원을 소비하거나, 다른 에이전트의 행동을 방해함으로써 전체 팀 성능을 감소시킬 수 있습니다. 따라서 의사결정은 지역적 효용(Local Utility)과 팀 수준 목표(Team-Level Objectives)를 함께 포함하여 개별 선택이 협력적 행동에 기여하도록 할 수 있습니다.

인공지능 공학(AI Engineering)에서 가치 기반 의사결정은 보상 모델(Reward Models), 가치 함수(Value Functions), 효용 추정기(Utility Estimators), 비용 함수(Cost Functions), 학습된 선호(Learned Preferences), 제약 조건, 계획 목표(Planning Objectives)를 통해 구현할 수 있습니다. 하나의 표현 방식만으로 모든 문제를 해결할 수는 없습니다. 실제 시스템은 학습된 가치와 명시적인 공학 규칙(Engineering Rules), 안전 한계(Safety Limits), 예측 모델, 기억, 계층적 제어(Hierarchical Control)를 함께 결합하는 경우가 많습니다.

계층적 가치 평가(Hierarchical Valuation)는 서로 다른 추상화 수준에서 의사결정을 평가함으로써 복잡성을 줄일 수 있습니다. 상위 수준 제어기는 임무 목표(Mission Goals)를 비교하고, 중간 수준 계획기는 경로나 기술(Skills)을 비교하며, 하위 수준 시스템은 모션 대안(Motion Alternatives)을 평가할 수 있습니다. 각 계층은 상위 수준 목표의 제약을 받으면서도 자신의 시간적·물리적 스케일에 적합한 가치를 이용할 수 있습니다.

완전한 가치 기반 의사결정 순환(Value-Based Decision Loop)은 현재 상태, 목표, 내부 요구(Internal Needs), 기억된 경험에서 시작합니다. 후보 행동이 생성되고, 가능한 결과가 예측되며, 가치와 비용이 추정되고, 불확실성과 제약 조건이 고려된 후 하나의 행동이 선택됩니다. 그 결과는 다시 기억, 예측 모델(Predictive Models), 미래 가치 추정을 갱신하는 새로운 증거를 생성합니다.

궁극적으로 가치 기반 의사결정은 지능형 에이전트가 "무엇을 할 수 있는가(What Can Be Done)"라는 질문을 더 중요한 "무엇을 해야 하는가(What Should Be Done)"라는 질문으로 변환하는 메커니즘을 제공합니다. 보상, 비용, 위험, 지연, 불확실성, 정보, 목표, 기억, 예측, 제약 조건을 통합함으로써 가치 기반 의사결정은 행동 선택을 적응적 행동(Adaptive Behavior)과 연결하고, 점차 높은 수준의 자율성을 갖는 생물학적 및 인공 지능(Artificial Intelligence)을 위한 핵심 기반을 제공합니다.

##  

## 08.04 Uncertainty and Risk [w/Code]

![](images/image5.png){width="7.268055555555556in" height="7.268055555555556in"}

Uncertainty is a fundamental condition of decision making because intelligent agents rarely possess complete and perfectly accurate information about themselves or their environments. Sensors are noisy, objects can be hidden, future events are not fully predictable, and other agents may behave unexpectedly. A decision system must therefore reason about what might be true rather than assuming that its internal representation exactly matches reality.

Risk emerges when uncertainty is combined with consequences. Uncertainty describes incomplete knowledge about states, events, or outcomes, whereas risk concerns the potential gains and losses associated with those uncertain possibilities. An agent may be uncertain about whether an obstacle exists, but the corresponding risk depends on what could happen if it chooses to move forward despite that uncertainty.

This distinction is important because uncertainty does not always imply significant danger. A robot may be uncertain about the color of a distant object without affecting its mission, while a small uncertainty about whether a human is standing behind an occlusion can be operationally critical. Decision systems therefore need to consider both the degree of uncertainty and the importance of the consequences connected to it.

Uncertainty can arise from several sources. Measurement uncertainty originates from imperfect sensors, calibration errors, limited resolution, environmental interference, and noise. State uncertainty occurs when observations provide only incomplete evidence about the actual condition of the world. Model uncertainty arises when the agent\'s internal representation of environmental dynamics does not accurately describe how states will evolve.

Another useful distinction separates aleatoric uncertainty from epistemic uncertainty. Aleatoric uncertainty reflects variability inherent in the environment, such as unpredictable disturbances or stochastic events that cannot be completely eliminated through additional knowledge. Epistemic uncertainty results from limited knowledge, insufficient observations, or incomplete models and can potentially be reduced by collecting more data or improving the model.

This distinction matters because different uncertainties require different responses. If uncertainty is primarily epistemic, an agent may benefit from exploration, additional sensing, memory retrieval, or model improvement. If uncertainty is largely aleatoric, gathering more observations may provide limited benefit, and the system may instead need robust policies that remain effective across multiple possible outcomes.

Partial observability is a major source of uncertainty for intelligent agents. Important variables may be temporarily hidden, outside the sensor field of view, or impossible to measure directly. The system must then maintain a belief about the hidden state by integrating current observations with previous observations, memory, dynamics, and contextual knowledge rather than relying exclusively on instantaneous sensory input.

A belief state provides a representation of uncertainty over possible states of the world. Instead of asserting that the environment is definitely in one state, the system can maintain several hypotheses with different probabilities or confidence levels. Decision making can then operate over this distribution, allowing actions to reflect both the most likely interpretation and plausible alternatives.

Bayesian reasoning provides a general framework for updating beliefs as new evidence becomes available. Prior beliefs represent what the system expected before receiving a new observation, while likelihood information describes how compatible that observation is with different hypotheses. Combining these sources produces an updated posterior belief that can guide subsequent prediction and decision making.

Probabilistic reasoning is particularly useful when sensor evidence is ambiguous. A robot may combine camera observations, LiDAR measurements, radar, localization estimates, and map information to determine whether a region is traversable. Each source may contain uncertainty, but their combined evidence can produce a more reliable estimate than treating any single measurement as perfectly correct.

Confidence estimation provides another way to represent uncertainty. A perception system can output not only a classification or state estimate but also an indication of how reliable that estimate is. Downstream decision systems can use confidence to determine whether immediate action is appropriate or whether additional sensing, slower motion, human confirmation, or alternative planning is required.

Calibration is important because confidence values are useful only when they correspond reasonably well to actual reliability. A system that reports high confidence when frequently incorrect can be more dangerous than one that openly represents uncertainty. Well-calibrated uncertainty allows decision mechanisms to distinguish between strong evidence and predictions that should be treated cautiously.

Risk assessment combines uncertain outcomes with their potential severity. A low-probability event may still require substantial attention when its consequences are catastrophic. Conversely, a high-probability event with negligible consequences may require little intervention. Risk-sensitive decision making therefore cannot depend only on the probability of failure; it must also consider the magnitude of possible harm.

Expected utility provides one framework for comparing uncertain alternatives. Possible outcomes are assigned probabilities and utilities, and the system evaluates actions according to the probability-weighted value of those outcomes. This enables rational comparison across uncertain choices, but practical systems may need additional mechanisms because equal expected utilities can conceal very different distributions of risk.

Risk preferences describe how an agent treats such distributions. A risk-neutral system primarily considers expected outcomes, while a risk-averse system gives greater importance to avoiding severe losses or variability. Risk-seeking behavior may accept greater uncertainty in exchange for potentially larger gains. Appropriate risk preference depends strongly on mission context and the consequences of failure.

Safety-critical Physical AI generally requires risk-sensitive rather than purely reward-maximizing behavior. An autonomous vehicle, industrial robot, medical robot, or heavy mobile platform should not accept a small probability of catastrophic harm simply because the average predicted reward is high. Hard safety constraints and conservative decision rules may therefore override otherwise attractive actions.

Thresholds can provide simple mechanisms for managing risk. An action may be prohibited when collision probability exceeds a specified limit, localization confidence falls below an acceptable level, or predicted mechanical load approaches a safety boundary. Such thresholds translate uncertain estimates into operational decisions, although poorly chosen thresholds can produce either excessive caution or unsafe behavior.

Chance constraints provide a more probabilistic extension of this idea. Instead of requiring a constraint to hold under every imaginable condition, the system can require that the probability of violating it remain below an acceptable level. This approach is useful when absolute guarantees are impossible but quantified uncertainty allows risk to be bounded during planning and control.

Robust decision making addresses uncertainty by seeking actions that perform acceptably across a range of plausible conditions. Rather than optimizing behavior for one predicted state, robust methods consider variations in model parameters, disturbances, sensor errors, or environmental conditions. The resulting action may sacrifice some nominal performance in exchange for greater reliability when predictions are imperfect.

Worst-case reasoning represents a particularly conservative form of robust decision making. The system evaluates how an action would perform under the most unfavorable plausible conditions and chooses accordingly. This can be valuable in high-consequence situations but may become excessively cautious if extremely unlikely scenarios dominate every decision. Practical autonomy therefore requires an appropriate definition of plausible worst cases.

Uncertainty also influences the speed of decision making. When one alternative has clearly superior evidence, rapid action may be appropriate. When alternatives have similar values or evidence is weak, additional deliberation can improve decision quality. Decision thresholds can therefore adapt according to confidence, urgency, available time, and the cost of making an incorrect choice.

The value of information becomes important when uncertainty can be reduced before commitment. An agent may inspect an object, change viewpoint, request clarification, perform a diagnostic test, or move to obtain better sensor coverage. These actions may provide little immediate task reward, yet they can be valuable because the resulting information improves later decisions and reduces risk.

Active perception applies this principle directly to embodied systems. Instead of treating sensing as a passive process, the robot deliberately selects movements that improve observability. Turning a camera, repositioning around an obstacle, adjusting distance, or approaching from another direction can reduce ambiguity. Perception and action therefore become coupled through uncertainty reduction.

Exploration similarly trades immediate performance for knowledge. An agent operating in an unfamiliar environment may choose actions that reveal new states, dynamics, or rewards. Exploration can reduce epistemic uncertainty and improve future decisions, but uncontrolled exploration can create physical risk. Safe exploration therefore requires balancing information gain against potential harm and resource consumption.

Memory can reduce uncertainty by providing evidence from previous experience. Episodic memory may retrieve a similar situation and its outcome, while semantic memory can supply generalized knowledge about environments, objects, and hazards. However, remembered information can itself become uncertain when environments change, making recency, context, provenance, and confidence important properties of memory retrieval.

World models introduce uncertainty about predicted futures. A model may simulate how an environment changes after a candidate action, but its predictions become less reliable when the state is unfamiliar or the prediction horizon becomes longer. Decision systems should therefore propagate uncertainty through predicted trajectories rather than treating every simulated future state as equally trustworthy.

Long-horizon prediction is especially challenging because small state or model errors can accumulate across successive transitions. Several futures may become plausible even when the current state estimate is relatively precise. Planning systems can represent multiple trajectories, probability distributions, ensembles, or confidence bounds to avoid committing prematurely to one imagined future.

Model uncertainty becomes particularly important when an AI system encounters out-of-distribution conditions. A learned model may produce confident predictions even though the current environment differs substantially from its training experience. Detecting unfamiliar states and reducing confidence can prevent the decision system from treating unsupported predictions as reliable knowledge.

Out-of-distribution detection can therefore function as part of risk management. When observations fall outside familiar operating conditions, the system may reduce speed, increase sensing, switch to a conservative controller, request human assistance, or enter a safe state. Recognizing the limits of learned competence is a central requirement for reliable autonomous behavior.

Uncertainty also arises from other agents. Humans, vehicles, robots, and adversarial agents possess independent intentions that cannot be observed perfectly. Predicting their behavior requires maintaining multiple possible future actions rather than assuming one deterministic trajectory. Social and multi-agent decision systems must therefore combine physical uncertainty with uncertainty about intentions and interactions.

In multi-robot systems, communication creates additional uncertainty. Messages can be delayed, lost, inconsistent, or based on outdated local observations. A robot should not assume that another agent\'s reported state remains perfectly current. Distributed autonomy requires confidence-aware information fusion and decision mechanisms capable of operating safely when communication quality deteriorates.

Risk can accumulate across hierarchical decision levels. A high-level mission decision may appear acceptable while lower-level navigation encounters terrain, localization, energy, or collision uncertainties that make execution unsafe. Information about uncertainty must therefore flow upward as well as downward so that strategic plans can be revised when physical execution becomes unreliable.

Uncertainty-aware hierarchical control can assign different responsibilities to different levels. High-level planning may reason about mission alternatives and long-term uncertainty, intermediate planning may evaluate routes and task feasibility, and low-level control may respond rapidly to disturbances and immediate hazards. Together these layers allow uncertainty to be managed at appropriate temporal and spatial scales.

Learning from failure is essential for improving risk estimates. When an unexpected event occurs, the system can compare predicted and observed outcomes, identify which assumptions were incorrect, and update models or confidence estimates. Near misses can also provide valuable evidence because they reveal dangerous conditions without requiring catastrophic failure to occur before learning.

Replay and memory consolidation can preserve rare but safety-critical experiences. Ordinary data may overwhelmingly represent successful operation, causing rare hazards to have little influence on learning. Prioritized replay can repeatedly expose learning systems to important failures, unusual conditions, and high-risk transitions so that their consequences remain represented in future decisions.

Simulation provides another mechanism for studying risk without exposing physical systems to every dangerous condition. Rare failures, sensor degradation, extreme terrain, communication loss, or unexpected obstacles can be generated virtually. However, simulation itself introduces model uncertainty, so policies trained in simulation must account for the gap between simulated dynamics and the real world.

For Physical AI, uncertainty should be represented throughout the complete perception--prediction--decision--action loop. Perception produces uncertain state estimates, world models generate uncertain futures, decision systems compare risk-sensitive alternatives, planners apply safety constraints, controllers respond to disturbances, and observed outcomes update both knowledge and confidence.

The objective is therefore not to eliminate uncertainty, which is generally impossible, but to make it explicit and operationally useful. An intelligent system should know when evidence is strong, when predictions are unreliable, when more information is valuable, when conservative behavior is appropriate, and when the uncertainty exceeds the level at which autonomous action can safely continue.

Uncertainty and risk ultimately define the boundary between merely selecting a high-value action and making a reliable decision in the real world. By integrating probabilistic beliefs, confidence, consequence severity, information gathering, robust planning, safety constraints, memory, and adaptive learning, decision systems can act effectively even when the world is only partially known and the future remains uncertain.

불확실성(Uncertainty)은 지능형 에이전트(Intelligent Agent)가 자신이나 환경에 대해 완전하고 정확한 정보를 가지는 경우가 거의 없기 때문에 의사결정(Decision Making)의 근본적인 조건입니다. 센서에는 노이즈(Noise)가 존재하고, 객체는 가려질 수 있으며, 미래의 사건은 완전히 예측할 수 없고, 다른 에이전트는 예상과 다르게 행동할 수 있습니다. 따라서 의사결정 시스템(Decision System)은 내부 표상이 현실과 정확히 일치한다고 가정하기보다 무엇이 사실일 가능성이 있는지를 추론해야 합니다.

위험(Risk)은 불확실성이 결과(Consequences)와 결합될 때 발생합니다. 불확실성은 상태, 사건 또는 결과에 대한 불완전한 지식을 의미하는 반면, 위험은 그러한 불확실한 가능성과 연관된 잠재적인 이익과 손실(Potential Gains and Losses)을 의미합니다. 에이전트는 장애물이 존재하는지 확신하지 못할 수 있지만, 그에 따른 위험은 이러한 불확실성에도 불구하고 앞으로 이동하기로 선택했을 때 어떤 일이 발생할 수 있는지에 따라 달라집니다.

이러한 구분은 불확실성이 항상 심각한 위험을 의미하지는 않기 때문에 중요합니다. 로봇은 멀리 있는 객체의 색상에 대해 확신하지 못하더라도 임무에는 아무런 영향을 받지 않을 수 있지만, 가려진 영역 뒤에 사람이 있는지에 관한 작은 불확실성은 운영상 매우 중요할 수 있습니다. 따라서 의사결정 시스템은 불확실성의 정도뿐만 아니라 그것과 연결된 결과의 중요성도 함께 고려해야 합니다.

불확실성은 여러 원인에서 발생할 수 있습니다. 측정 불확실성(Measurement Uncertainty)은 불완전한 센서, 보정 오류(Calibration Errors), 제한된 해상도(Limited Resolution), 환경적 간섭(Environmental Interference), 노이즈에서 발생합니다. 상태 불확실성(State Uncertainty)은 관찰이 실제 세계의 상태에 대한 불완전한 증거만 제공할 때 발생합니다. 모델 불확실성(Model Uncertainty)은 에이전트의 내부 환경 동역학 모델이 상태가 어떻게 변화할지를 정확하게 설명하지 못할 때 발생합니다.

또 다른 유용한 구분은 우연적 불확실성(Aleatoric Uncertainty)과 인식론적 불확실성(Epistemic Uncertainty)을 구분하는 것입니다. 우연적 불확실성은 예측할 수 없는 교란이나 추가 지식으로도 완전히 제거할 수 없는 확률적 사건처럼 환경 자체에 내재된 변동성(Variability)을 반영합니다. 인식론적 불확실성은 제한된 지식, 부족한 관찰 또는 불완전한 모델에서 발생하며 추가 데이터를 수집하거나 모델을 개선함으로써 잠재적으로 감소시킬 수 있습니다.

서로 다른 불확실성은 서로 다른 대응 방법을 요구하기 때문에 이러한 구분은 중요합니다. 불확실성이 주로 인식론적인 경우 에이전트는 탐색(Exploration), 추가적인 감지(Sensing), 기억 검색(Memory Retrieval), 모델 개선을 통해 이점을 얻을 수 있습니다. 반면 불확실성이 주로 우연적인 경우 추가 관찰을 수집하더라도 얻을 수 있는 이점이 제한적일 수 있으며, 시스템은 여러 가능한 결과에서도 효과적으로 작동하는 견고한 정책(Robust Policies)을 필요로 할 수 있습니다.

부분 관찰 가능성(Partial Observability)은 지능형 에이전트의 주요 불확실성 원인입니다. 중요한 변수는 일시적으로 가려지거나 센서의 시야(Field of View) 밖에 존재하거나 직접 측정하는 것이 불가능할 수 있습니다. 이 경우 시스템은 순간적인 감각 입력에만 의존하는 대신 현재 관찰을 이전 관찰, 기억, 동역학(Dynamics), 맥락적 지식(Contextual Knowledge)과 통합하여 숨겨진 상태(Hidden State)에 대한 신념을 유지해야 합니다.

신념 상태(Belief State)는 가능한 세계 상태들에 대한 불확실성을 표상합니다. 환경이 하나의 특정 상태에 있다고 단정하는 대신 시스템은 서로 다른 확률이나 신뢰 수준(Confidence Levels)을 가진 여러 가설(Hypotheses)을 유지할 수 있습니다. 그러면 의사결정은 이러한 분포를 기반으로 수행될 수 있으며, 가장 가능성이 높은 해석뿐만 아니라 충분히 가능한 다른 대안도 행동 선택에 반영할 수 있습니다.

베이지안 추론(Bayesian Reasoning)은 새로운 증거가 제공될 때 신념을 갱신하기 위한 일반적인 프레임워크를 제공합니다. 사전 신념(Prior Beliefs)은 새로운 관찰을 받기 전에 시스템이 예상했던 것을 나타내며, 우도(Likelihood) 정보는 해당 관찰이 서로 다른 가설들과 얼마나 일치하는지를 설명합니다. 이러한 정보들을 결합하면 이후의 예측과 의사결정을 안내할 수 있는 갱신된 사후 신념(Posterior Belief)이 생성됩니다.

확률적 추론(Probabilistic Reasoning)은 센서 증거가 모호할 때 특히 유용합니다. 로봇은 특정 영역이 주행 가능한지 판단하기 위해 카메라 관찰(Camera Observations), 라이다 측정(LiDAR Measurements), 레이더(Radar), 위치 추정(Localization Estimates), 지도 정보(Map Information)를 결합할 수 있습니다. 각각의 정보원에는 불확실성이 포함될 수 있지만, 어느 하나의 측정값을 완전히 정확하다고 가정하는 것보다 여러 증거를 결합하면 더욱 신뢰할 수 있는 추정치를 얻을 수 있습니다.

신뢰도 추정(Confidence Estimation)은 불확실성을 표현하는 또 다른 방법입니다. 지각 시스템(Perception System)은 분류 결과나 상태 추정뿐만 아니라 해당 추정이 얼마나 신뢰할 수 있는지를 함께 출력할 수 있습니다. 하위 의사결정 시스템은 이 신뢰도를 이용하여 즉시 행동하는 것이 적절한지, 아니면 추가 감지, 감속, 인간의 확인(Human Confirmation), 대안적 계획(Alternative Planning)이 필요한지를 결정할 수 있습니다.

보정(Calibration)이 중요한 이유는 신뢰도 값이 실제 신뢰성과 합리적으로 일치할 때만 유용하기 때문입니다. 자주 틀리면서도 높은 신뢰도를 보고하는 시스템은 자신의 불확실성을 명확하게 표현하는 시스템보다 더 위험할 수 있습니다. 잘 보정된 불확실성(Well-Calibrated Uncertainty)을 사용하면 의사결정 메커니즘이 강력한 증거와 신중하게 처리해야 하는 예측을 구분할 수 있습니다.

위험 평가(Risk Assessment)는 불확실한 결과와 그 결과가 초래할 수 있는 잠재적 심각성(Potential Severity)을 결합합니다. 발생 확률이 낮은 사건이라도 그 결과가 치명적이라면 상당한 주의가 필요할 수 있습니다. 반대로 발생 확률이 높은 사건이라도 결과가 미미하다면 큰 개입이 필요하지 않을 수 있습니다. 따라서 위험 민감형 의사결정(Risk-Sensitive Decision Making)은 실패 확률에만 의존할 수 없으며 발생 가능한 피해의 크기도 함께 고려해야 합니다.

기대 효용(Expected Utility)은 불확실한 대안들을 비교하는 하나의 프레임워크를 제공합니다. 가능한 결과에 확률과 효용(Utility)을 부여하고, 시스템은 이러한 결과의 확률 가중 가치(Probability-Weighted Value)에 따라 행동을 평가합니다. 이를 통해 불확실한 선택들을 합리적으로 비교할 수 있지만, 동일한 기대 효용이 매우 다른 위험 분포를 숨길 수 있기 때문에 실제 시스템에서는 추가적인 메커니즘이 필요할 수 있습니다.

위험 선호도(Risk Preferences)는 에이전트가 이러한 분포를 어떻게 다루는지를 설명합니다. 위험 중립적 시스템(Risk-Neutral System)은 주로 기대 결과를 고려하는 반면, 위험 회피형 시스템(Risk-Averse System)은 심각한 손실이나 변동성을 피하는 것을 더 중요하게 평가합니다. 위험 추구형 행동(Risk-Seeking Behavior)은 더 큰 잠재적 이익을 얻기 위해 더 높은 불확실성을 받아들일 수 있습니다. 적절한 위험 선호도는 임무의 맥락과 실패의 결과에 크게 의존합니다.

안전 필수 피지컬 AI(Safety-Critical Physical AI)는 일반적으로 순수한 보상 최대화(Reward Maximization)보다 위험에 민감한 행동을 요구합니다. 자율주행 차량(Autonomous Vehicle), 산업용 로봇(Industrial Robot), 의료 로봇(Medical Robot), 고중량 이동 플랫폼(Heavy Mobile Platform)은 평균적인 예상 보상이 높다는 이유만으로 작은 확률의 치명적 피해를 허용해서는 안 됩니다. 따라서 강제적인 안전 제약(Hard Safety Constraints)과 보수적인 의사결정 규칙(Conservative Decision Rules)이 다른 매력적인 행동보다 우선할 수 있습니다.

임계값(Thresholds)은 위험을 관리하는 단순한 메커니즘을 제공할 수 있습니다. 충돌 확률(Collision Probability)이 지정된 한계를 초과하거나, 위치 추정 신뢰도(Localization Confidence)가 허용 수준 아래로 떨어지거나, 예상 기계적 하중(Predicted Mechanical Load)이 안전 경계에 접근하면 행동을 금지할 수 있습니다. 이러한 임계값은 불확실한 추정을 운영상의 의사결정으로 변환하지만, 부적절하게 설정하면 지나치게 보수적이거나 위험한 행동을 만들 수 있습니다.

확률 제약(Chance Constraints)은 이러한 개념을 보다 확률적인 형태로 확장합니다. 모든 상상 가능한 조건에서 제약이 반드시 만족되어야 한다고 요구하는 대신 제약을 위반할 확률이 허용 가능한 수준 이하로 유지되도록 요구할 수 있습니다. 절대적인 보장이 불가능하지만 정량화된 불확실성(Quantified Uncertainty)을 이용하여 계획과 제어 과정에서 위험을 제한할 수 있는 상황에 유용합니다.

견고한 의사결정(Robust Decision Making)은 가능한 다양한 조건에서 수용 가능한 수준으로 작동하는 행동을 찾음으로써 불확실성을 처리합니다. 하나의 예측된 상태에 맞추어 행동을 최적화하는 대신 모델 파라미터(Model Parameters), 교란(Disturbances), 센서 오류, 환경 조건의 변화를 고려합니다. 이렇게 선택된 행동은 명목상의 성능(Nominal Performance)을 일부 희생하는 대신 예측이 불완전할 때 더 높은 신뢰성을 확보할 수 있습니다.

최악 조건 추론(Worst-Case Reasoning)은 특히 보수적인 형태의 견고한 의사결정입니다. 시스템은 현실적으로 가능한 가장 불리한 조건에서 행동이 어떻게 수행될지를 평가하고 이에 따라 선택합니다. 결과의 영향이 큰 상황에서는 유용할 수 있지만 극히 가능성이 낮은 시나리오가 모든 의사결정을 지배하면 지나치게 보수적으로 변할 수 있습니다. 따라서 실제 자율 시스템(Autonomous System)에서는 현실적으로 가능한 최악 조건을 적절하게 정의해야 합니다.

불확실성은 의사결정 속도에도 영향을 줍니다. 하나의 대안이 명확하게 우수하다는 강력한 증거가 존재한다면 빠르게 행동하는 것이 적절할 수 있습니다. 반대로 대안들의 가치가 비슷하거나 증거가 약하다면 추가적인 숙고(Deliberation)를 통해 의사결정 품질을 향상시킬 수 있습니다. 따라서 의사결정 임계값(Decision Thresholds)은 신뢰도, 긴급성(Urgency), 이용 가능한 시간, 잘못된 선택에 따른 비용에 따라 조정될 수 있습니다.

정보 가치(Value of Information)는 행동을 결정하기 전에 불확실성을 줄일 수 있을 때 중요해집니다. 에이전트는 객체를 검사하거나, 관찰 시점을 변경하거나, 추가 설명을 요청하거나, 진단 시험(Diagnostic Test)을 수행하거나, 더 나은 센서 관측 범위를 확보하기 위해 이동할 수 있습니다. 이러한 행동은 즉각적인 작업 보상을 거의 제공하지 않더라도 이후의 의사결정을 개선하고 위험을 줄이는 정보를 제공하기 때문에 가치가 있을 수 있습니다.

능동 지각(Active Perception)은 이러한 원리를 체화 시스템(Embodied Systems)에 직접 적용합니다. 로봇은 감지를 수동적인 과정으로 취급하는 대신 관찰 가능성(Observability)을 개선하는 움직임을 의도적으로 선택합니다. 카메라를 회전하거나, 장애물 주변으로 위치를 변경하거나, 거리를 조정하거나, 다른 방향에서 접근함으로써 모호성을 감소시킬 수 있습니다. 따라서 지각과 행동은 불확실성 감소(Uncertainty Reduction)를 통해 서로 결합됩니다.

탐색(Exploration) 역시 즉각적인 성능과 지식 획득 사이의 절충을 포함합니다. 익숙하지 않은 환경에서 작동하는 에이전트는 새로운 상태, 동역학 또는 보상을 발견하는 행동을 선택할 수 있습니다. 탐색은 인식론적 불확실성을 줄이고 미래의 의사결정을 향상시킬 수 있지만, 통제되지 않은 탐색은 물리적 위험을 만들 수 있습니다. 따라서 안전한 탐색(Safe Exploration)은 정보 이득(Information Gain)과 잠재적인 피해 및 자원 소비 사이의 균형을 필요로 합니다.

기억(Memory)은 이전 경험의 증거를 제공함으로써 불확실성을 감소시킬 수 있습니다. 일화 기억(Episodic Memory)은 유사한 상황과 그 결과를 검색할 수 있고, 의미 기억(Semantic Memory)은 환경, 객체, 위험 요소(Hazards)에 관한 일반화된 지식을 제공할 수 있습니다. 그러나 환경이 변화하면 기억된 정보 자체도 불확실해질 수 있으므로 최신성(Recency), 맥락, 출처 정보(Provenance), 신뢰도는 기억 검색에서 중요한 속성이 됩니다.

월드 모델(World Models)은 예측된 미래에 관한 불확실성을 도입합니다. 모델은 후보 행동 이후 환경이 어떻게 변화할지를 시뮬레이션할 수 있지만 현재 상태가 익숙하지 않거나 예측 시간 범위(Prediction Horizon)가 길어질수록 예측의 신뢰성이 감소할 수 있습니다. 따라서 의사결정 시스템은 모든 시뮬레이션된 미래 상태를 동일하게 신뢰하기보다 예측 궤적(Predicted Trajectories)을 따라 불확실성을 함께 전파해야 합니다.

장기 예측(Long-Horizon Prediction)은 작은 상태 또는 모델 오차가 연속적인 상태 전이(State Transitions)를 거치면서 누적될 수 있기 때문에 특히 어렵습니다. 현재 상태 추정이 비교적 정확하더라도 여러 미래가 동시에 가능해질 수 있습니다. 계획 시스템은 하나의 상상된 미래에 너무 일찍 고정되지 않도록 여러 궤적, 확률 분포(Probability Distributions), 앙상블(Ensembles), 신뢰 구간(Confidence Bounds)을 표상할 수 있습니다.

모델 불확실성은 인공지능 시스템이 분포 외 조건(Out-of-Distribution Conditions)에 직면할 때 특히 중요합니다. 학습된 모델은 현재 환경이 학습 경험과 상당히 다르더라도 높은 신뢰도의 예측을 생성할 수 있습니다. 익숙하지 않은 상태를 감지하고 신뢰도를 낮추면 의사결정 시스템이 근거가 부족한 예측을 신뢰할 수 있는 지식으로 잘못 취급하는 것을 방지할 수 있습니다.

따라서 분포 외 탐지(Out-of-Distribution Detection)는 위험 관리(Risk Management)의 일부로 기능할 수 있습니다. 관찰이 익숙한 운영 조건(Operating Conditions)을 벗어나면 시스템은 속도를 낮추고, 감지를 강화하고, 보수적인 제어기(Conservative Controller)로 전환하고, 인간의 지원을 요청하거나, 안전 상태(Safe State)로 진입할 수 있습니다. 학습된 능력의 한계를 인식하는 것은 신뢰할 수 있는 자율 행동의 핵심 요구사항입니다.

다른 에이전트로부터도 불확실성이 발생합니다. 인간, 차량, 로봇, 적대적 에이전트(Adversarial Agents)는 완전히 관찰할 수 없는 독립적인 의도를 가지고 있습니다. 이들의 행동을 예측하려면 하나의 결정론적 궤적(Deterministic Trajectory)을 가정하기보다 여러 가능한 미래 행동을 유지해야 합니다. 따라서 사회적 및 다중 에이전트 의사결정 시스템(Multi-Agent Decision Systems)은 물리적 불확실성과 의도 및 상호작용에 관한 불확실성을 함께 처리해야 합니다.

다중 로봇 시스템(Multi-Robot Systems)에서는 통신(Communication)이 추가적인 불확실성을 발생시킵니다. 메시지는 지연되거나, 손실되거나, 서로 일치하지 않거나, 오래된 지역 관찰(Local Observations)을 기반으로 할 수 있습니다. 로봇은 다른 에이전트가 보고한 상태가 계속해서 완벽하게 최신 상태라고 가정해서는 안 됩니다. 분산 자율성(Distributed Autonomy)을 위해서는 신뢰도 인식 정보 융합(Confidence-Aware Information Fusion)과 통신 품질이 저하되더라도 안전하게 작동할 수 있는 의사결정 메커니즘이 필요합니다.

위험은 계층적 의사결정(Hierarchical Decision Making)의 여러 수준에 걸쳐 누적될 수 있습니다. 상위 수준의 임무 결정은 적절해 보이더라도 하위 수준 내비게이션에서 지형, 위치 추정, 에너지 또는 충돌에 관한 불확실성이 발생하여 실행이 위험해질 수 있습니다. 따라서 물리적 실행의 신뢰성이 낮아질 때 전략적 계획을 수정할 수 있도록 불확실성 정보는 하향 방향뿐만 아니라 상향 방향으로도 전달되어야 합니다.

불확실성 인식 계층적 제어(Uncertainty-Aware Hierarchical Control)는 서로 다른 수준에 서로 다른 책임을 할당할 수 있습니다. 상위 수준 계획은 임무 대안과 장기 불확실성을 추론하고, 중간 수준 계획은 경로와 작업 실행 가능성(Task Feasibility)을 평가하며, 하위 수준 제어는 교란과 즉각적인 위험에 빠르게 대응할 수 있습니다. 이러한 계층들이 함께 작동함으로써 불확실성을 적절한 시간적·공간적 스케일에서 관리할 수 있습니다.

실패로부터의 학습(Learning from Failure)은 위험 추정을 향상시키는 데 필수적입니다. 예상하지 못한 사건이 발생하면 시스템은 예측 결과와 실제 관찰 결과를 비교하고, 어떤 가정이 잘못되었는지를 식별하여 모델이나 신뢰도 추정을 갱신할 수 있습니다. 아차 사고(Near Misses) 역시 치명적인 실패가 실제로 발생하기 전에 위험한 조건을 알려주기 때문에 가치 있는 증거를 제공할 수 있습니다.

재생(Replay)과 기억 공고화(Memory Consolidation)는 드물지만 안전에 중요한 경험을 보존할 수 있습니다. 일반적인 데이터는 대부분 성공적인 운영을 나타낼 수 있기 때문에 희귀한 위험이 학습에 미치는 영향이 매우 작아질 수 있습니다. 우선순위 재생(Prioritized Replay)을 사용하면 중요한 실패, 비정상적인 조건, 고위험 상태 전이(High-Risk Transitions)를 학습 시스템에 반복적으로 제공하여 그 결과가 미래의 의사결정에 계속 반영되도록 할 수 있습니다.

시뮬레이션(Simulation)은 물리적 시스템을 모든 위험 조건에 직접 노출하지 않고도 위험을 연구할 수 있는 또 다른 메커니즘을 제공합니다. 희귀한 실패, 센서 성능 저하(Sensor Degradation), 극단적인 지형, 통신 손실, 예상하지 못한 장애물을 가상으로 생성할 수 있습니다. 그러나 시뮬레이션 자체도 모델 불확실성을 포함하기 때문에 시뮬레이션에서 학습된 정책은 시뮬레이션 동역학과 실제 세계 사이의 차이(Sim-to-Real Gap)를 고려해야 합니다.

피지컬 AI(Physical AI)에서는 완전한 지각--예측--의사결정--행동(Perception--Prediction--Decision--Action) 순환 전체에서 불확실성을 표상해야 합니다. 지각은 불확실한 상태 추정을 생성하고, 월드 모델은 불확실한 미래를 생성하며, 의사결정 시스템은 위험에 민감한 대안을 비교하고, 계획기는 안전 제약을 적용하며, 제어기는 교란에 대응하고, 관찰된 결과는 지식과 신뢰도를 다시 갱신합니다.

따라서 목표는 일반적으로 불가능한 불확실성의 완전한 제거가 아니라 불확실성을 명시적으로 표현하고 운영적으로 유용하게 만드는 것입니다. 지능형 시스템은 언제 증거가 강한지, 언제 예측을 신뢰하기 어려운지, 언제 추가 정보가 가치 있는지, 언제 보수적인 행동이 적절한지, 그리고 언제 불확실성이 자율 행동을 안전하게 지속할 수 있는 수준을 넘어섰는지를 판단할 수 있어야 합니다.

궁극적으로 불확실성과 위험은 단순히 높은 가치의 행동을 선택하는 것과 실제 세계에서 신뢰할 수 있는 의사결정(Reliable Decision)을 수행하는 것 사이의 경계를 정의합니다. 확률적 신념(Probabilistic Beliefs), 신뢰도, 결과의 심각성(Consequence Severity), 정보 수집, 견고한 계획(Robust Planning), 안전 제약, 기억, 적응 학습(Adaptive Learning)을 통합함으로써 의사결정 시스템은 세계에 대한 지식이 불완전하고 미래가 불확실한 상황에서도 효과적으로 행동할 수 있습니다.

##  

## 08.05 Planning and Mental Simulation [w/Code]

![](images/image6.png){width="7.268055555555556in" height="7.268055555555556in"}

Planning is the process of organizing actions before execution so that an agent can move from its current state toward a desired future state. It requires more than selecting the action with the highest immediate value because many goals can only be achieved through coordinated sequences of intermediate steps. Effective planning therefore connects goals, memory, prediction, constraints, and action selection across time.

Mental simulation complements planning by allowing possible actions and their consequences to be evaluated internally before they are performed in the external world. Instead of learning exclusively through physical trial and error, an intelligent system can construct hypothetical futures, compare them, reject undesirable possibilities, and select promising trajectories. This capability transforms prediction into a practical mechanism for prospective decision making.

Planning begins with a representation of the current state and a representation of the desired goal state. The difference between these states defines a problem that must be resolved through action. However, the current state is rarely represented perfectly, and goals may contain multiple conditions or priorities. Planning must therefore operate over structured representations rather than simple start-to-finish mappings.

A plan consists of actions whose effects progressively transform the state of the agent and environment. Each action introduces preconditions, expected effects, resource requirements, duration, and possible interactions with other actions. Planning involves discovering sequences in which these relationships remain compatible, allowing later actions to become possible because earlier actions created the necessary conditions.

Intermediate states are essential because complex goals are rarely reachable through one direct action. A robot asked to retrieve an object may first need to localize itself, identify the object, navigate toward it, position its body, prepare a manipulator, grasp the object, and transport it. Planning organizes these dependencies into a coherent sequence that can eventually satisfy the higher-level objective.

Subgoals reduce complexity by decomposing a large objective into smaller and more manageable problems. Rather than searching directly across every possible low-level action sequence, an agent can reason about meaningful intermediate objectives such as reaching a location, acquiring a resource, opening access, or completing a prerequisite task. Hierarchical decomposition therefore makes planning more computationally tractable.

Hierarchical planning represents decisions at several levels of abstraction. High-level planning can determine mission objectives and major task phases, intermediate planning can select skills or routes, and low-level planning can generate detailed motions and control actions. Information must flow between these levels because high-level goals constrain execution while lower-level feasibility can require strategic replanning.

Planning depends fundamentally on an internal model of how actions change the world. If an agent cannot estimate the consequences of an action, it cannot reliably determine whether that action contributes to a goal. Transition models represent how the current state and an action produce a subsequent state, providing the predictive structure required to evaluate possible sequences before execution.

World models generalize this capability by representing objects, agents, spatial relationships, dynamics, and potentially semantic or causal structure. Given a candidate action, a world model can predict possible future states. Planning can then repeatedly apply these predictions to construct imagined trajectories extending from the present toward alternative futures.

Mental simulation can therefore be understood as internally rolling a model forward through time. The agent begins with its current state estimate, considers a possible action, predicts the next state, then considers another action from that imagined state. Repeating this process creates hypothetical trajectories that can be evaluated without physically executing every candidate sequence.

The usefulness of simulation depends strongly on model accuracy. If the internal model incorrectly represents dynamics, object properties, environmental constraints, or other agents, simulated futures can become misleading. Planning systems should therefore represent prediction uncertainty and avoid treating internally generated trajectories as guaranteed descriptions of what will actually occur.

Prediction uncertainty generally increases with simulation depth. Small errors in the current state or transition model can accumulate over many imagined steps, causing long-horizon futures to diverge substantially. Practical planners must balance the benefits of looking farther ahead against declining confidence, computational cost, and the possibility that environmental changes will invalidate detailed predictions.

Branching creates another computational challenge. If several actions are possible at every simulated state, the number of potential future trajectories can grow exponentially with planning depth. Exhaustively evaluating every sequence quickly becomes impossible. Intelligent planning therefore requires mechanisms for focusing computation on promising branches while discarding unlikely, irrelevant, unsafe, or low-value alternatives.

Search algorithms provide one family of mechanisms for navigating this space of possible futures. States can be represented as nodes and actions as transitions, allowing planning to search for a path from the current state toward a goal. Heuristics can estimate which states appear closer or more valuable, directing computational resources toward regions of the search space that are more likely to contain useful plans.

Value information can further guide planning. Rather than treating every candidate trajectory equally, an agent can estimate reward, cost, risk, effort, time, or future opportunity associated with different paths. Planning then becomes closely connected with value-based decision making because candidate futures are compared according to their predicted consequences rather than simply whether they reach a nominal goal.

Planning under uncertainty requires reasoning about multiple possible futures rather than one deterministic trajectory. Sensor ambiguity, stochastic dynamics, incomplete models, and unpredictable agents can cause the same action to produce different outcomes. A robust plan must therefore remain useful across plausible variations or include contingency actions that respond appropriately when the expected future does not occur.

Contingency planning explicitly represents alternative branches. Instead of prescribing one rigid sequence, a plan can specify what to do if particular observations or outcomes arise. This produces conditional policies in which future actions depend on information obtained during execution. Planning thereby becomes a continuing interaction between prediction, observation, decision, and adaptation.

Replanning is essential in dynamic environments because even a well-designed plan can become obsolete. Obstacles move, resources become unavailable, goals change, communication fails, or predictions prove incorrect. An intelligent agent must compare observed states with expected states and revise its plan when the discrepancy becomes operationally significant.

This creates a closed-loop view of planning. The agent plans, executes part of the plan, observes the resulting state, compares it with predictions, updates its internal representation, and plans again when necessary. Such receding-horizon behavior avoids relying on a complete long-term sequence that was calculated once and then followed blindly despite changing conditions.

Model predictive control provides a related engineering principle. A system predicts several future steps, optimizes an action sequence over a limited horizon, executes only the immediate portion, receives new observations, and repeats the optimization. This approach combines prospective simulation with continuous feedback, making it particularly useful when dynamics and disturbances require frequent correction.

Memory contributes strongly to efficient planning. Episodic memory can retrieve previous situations and the plans that succeeded or failed within them. Semantic memory can provide generalized knowledge about objects, environments, rules, and causal relationships. Procedural memory can supply reusable skills that allow the planner to reason in terms of meaningful actions instead of reconstructing low-level behavior from scratch.

Previous plans can therefore function as templates rather than fixed scripts. When a new problem resembles an earlier one, an agent can retrieve a relevant solution and adapt it to current conditions. This reduces search cost while preserving flexibility. Failure memories are equally important because they can prevent the planner from repeatedly exploring trajectories already known to produce undesirable outcomes.

Planning and working memory are closely related because intermediate goals, candidate actions, constraints, and predicted consequences must remain available during deliberation. A complex plan may require comparing several branches while retaining the original objective. Limited working-memory capacity therefore creates pressure for abstraction, external memory, structured representations, and hierarchical decomposition.

The prefrontal cortex provides an important biological connection to these capabilities. Prefrontal systems contribute to maintaining goals, rules, intermediate representations, and task context while alternative actions are considered. Their interaction with memory, basal ganglia, value systems, and predictive mechanisms helps organize behavior across multiple steps rather than allowing immediate stimuli alone to determine action.

The hippocampus also contributes to prospective cognition. Neural mechanisms involved in representing remembered experiences and spatial sequences can participate in constructing or evaluating possible future trajectories. This relationship illustrates an important principle: memory and imagination are not completely separate functions because remembered structures can be recombined to support predictions about situations that have not yet occurred.

Spatial navigation provides a clear example of planning through simulation. An agent can represent its current location, destination, obstacles, and possible routes, then evaluate alternative paths before moving. Cognitive maps support this process by providing relational structure that allows shortcuts, detours, and novel routes to be considered even when the exact trajectory has not previously been experienced.

Mental simulation extends beyond physical navigation. An agent can simulate task sequences, social interactions, resource usage, manipulation outcomes, or strategic choices. The underlying principle remains similar: construct hypothetical state transitions, evaluate their consequences, and use the comparison to guide behavior before irreversible commitment occurs.

Counterfactual reasoning is closely related to mental simulation. After an event, an agent can consider what might have happened if a different action had been selected. Such comparisons can reveal missed opportunities, unsafe alternatives, or better strategies. Counterfactual simulation can therefore improve learning even when the alternative action was never physically executed.

Simulation can also support safety by testing candidate actions internally before granting them access to execution. A robot can reject a trajectory predicted to cause collision, exceed actuator limits, destabilize the platform, violate a restricted zone, or create unacceptable proximity to humans. Internal prediction thus becomes a protective layer between action generation and physical behavior.

However, simulation-based safety is only as reliable as the models and uncertainty estimates supporting it. A trajectory predicted to be safe may still fail when unmodeled conditions occur. Practical systems therefore combine predictive safety evaluation with hard constraints, reactive controllers, monitoring, emergency behaviors, and conservative margins rather than depending on simulation alone.

Planning often involves multiple objectives that compete with one another. A robot may need to minimize travel time while conserving energy, avoiding hazards, maintaining communication, reducing mechanical wear, and completing mission priorities. The planner must therefore evaluate trajectories according to structured utility or constraints rather than optimizing a single simplistic performance measure.

Resource awareness is particularly important for embodied intelligence. Every plan consumes time, energy, computation, actuator lifetime, storage, communication bandwidth, or other finite resources. A theoretically successful plan may be operationally poor if it exhausts the battery before completion or requires computational resources unavailable on the robot. Planning must therefore respect both physical and computational feasibility.

Multi-agent planning introduces additional complexity because the future depends on actions selected by other agents. Robots may cooperate, compete for shared resources, exchange information, divide tasks, or unintentionally interfere with one another. Planning must therefore consider joint states and possible interactions rather than treating each agent as an independent object following a fixed trajectory.

Communication can reduce multi-agent uncertainty but also creates constraints. Shared intentions and planned trajectories can improve coordination, yet communication may be delayed, unavailable, or outdated. Robust multi-robot planning should therefore exploit communication when available while retaining sufficient local autonomy to continue safely when information exchange deteriorates.

Modern AI systems implement planning through many different mechanisms, including symbolic planners, search algorithms, reinforcement-learning policies, tree search, optimization, learned world models, and combinations of these methods. The appropriate architecture depends on state complexity, prediction horizon, uncertainty, computational resources, and whether actions must satisfy strict physical constraints.

Learned world models create the possibility of planning directly within latent representations. Instead of predicting every future sensory detail, a model can represent task-relevant state variables in a compact latent space and simulate their evolution. This can reduce computational cost while preserving information necessary for estimating value, feasibility, uncertainty, and progress toward goals.

Generative models can further represent multiple plausible futures rather than producing only one prediction. When environmental evolution is inherently ambiguous, sampling alternative trajectories can expose several possible consequences of the same action. Planning can then compare these possibilities and select behavior that performs acceptably across the predicted distribution.

For Physical AI, planning and mental simulation form a bridge between cognition and physical execution. Perception estimates the current world, memory supplies previous knowledge, world models predict consequences, value systems evaluate possible futures, planning organizes actions, and controllers execute them. Feedback from the real environment then updates the entire cycle.

The central engineering challenge is to perform enough simulation to improve decisions without allowing planning itself to become too slow. Real-time robots operate under deadlines imposed by motion and environmental change. Effective architectures therefore allocate computation selectively, using fast learned policies for familiar situations and deeper simulation when novelty, uncertainty, risk, or strategic importance justifies additional reasoning.

Planning and mental simulation ultimately allow intelligence to act on futures that have not yet happened. By internally constructing possible trajectories, evaluating their value and risk, organizing intermediate goals, and revising behavior through feedback, an agent can move beyond reactive behavior toward deliberate, adaptive, and increasingly autonomous control of its interaction with the world.

계획(Planning)은 에이전트(Agent)가 현재 상태(Current State)에서 원하는 미래 상태(Desired Future State)로 이동할 수 있도록 실행 전에 행동을 조직하는 과정입니다. 많은 목표는 여러 중간 단계(Intermediate Steps)가 조정된 순서를 통해서만 달성할 수 있기 때문에 계획은 즉각적인 가치가 가장 높은 행동을 선택하는 것 이상을 요구합니다. 따라서 효과적인 계획은 시간의 흐름에 걸쳐 목표(Goals), 기억(Memory), 예측(Prediction), 제약 조건(Constraints), 행동 선택(Action Selection)을 연결합니다.

정신적 시뮬레이션(Mental Simulation)은 가능한 행동과 그 결과를 외부 세계에서 실제로 수행하기 전에 내부적으로 평가할 수 있도록 함으로써 계획을 보완합니다. 지능형 시스템(Intelligent System)은 물리적 시행착오(Physical Trial and Error)에만 의존하지 않고 가상의 미래(Hypothetical Futures)를 구성하고 비교하며, 바람직하지 않은 가능성을 제거하고 유망한 궤적(Promising Trajectories)을 선택할 수 있습니다. 이러한 능력은 예측을 미래 지향적 의사결정(Prospective Decision Making)을 위한 실용적인 메커니즘으로 전환합니다.

계획은 현재 상태의 표상(Representation)과 원하는 목표 상태(Goal State)의 표상에서 시작됩니다. 이 두 상태 사이의 차이는 행동을 통해 해결해야 하는 문제를 정의합니다. 그러나 현재 상태가 항상 완벽하게 표상되는 것은 아니며, 목표에는 여러 조건이나 우선순위가 포함될 수 있습니다. 따라서 계획은 단순한 시작점--종료점 매핑(Start-to-Finish Mapping)이 아니라 구조화된 표상(Structured Representations)을 기반으로 작동해야 합니다.

계획은 에이전트와 환경의 상태를 점진적으로 변화시키는 행동들로 구성됩니다. 각 행동에는 전제조건(Preconditions), 예상 효과(Expected Effects), 자원 요구사항(Resource Requirements), 지속 시간(Duration), 다른 행동과의 잠재적 상호작용이 포함됩니다. 계획 과정에서는 이러한 관계들이 서로 양립할 수 있는 행동 순서를 찾아야 하며, 앞선 행동이 필요한 조건을 만들어냄으로써 이후 행동이 가능해지도록 해야 합니다.

복잡한 목표는 하나의 직접적인 행동만으로 달성되는 경우가 거의 없기 때문에 중간 상태(Intermediate States)가 필수적입니다. 객체를 가져오라는 지시를 받은 로봇은 먼저 자신의 위치를 추정하고, 객체를 식별하고, 객체를 향해 이동하고, 몸체의 위치를 조정하고, 매니퓰레이터(Manipulator)를 준비하고, 객체를 파지한 후 운반해야 할 수 있습니다. 계획은 이러한 의존 관계를 일관된 순서로 조직하여 궁극적으로 상위 수준 목표를 달성하도록 합니다.

하위 목표(Subgoals)는 큰 목표를 더 작고 관리 가능한 문제로 분해하여 복잡성을 줄입니다. 가능한 모든 저수준 행동 순서를 직접 탐색하는 대신 에이전트는 특정 위치에 도달하기, 자원 확보하기, 접근 경로 열기, 선행 작업 완료하기와 같은 의미 있는 중간 목표를 중심으로 추론할 수 있습니다. 따라서 계층적 분해(Hierarchical Decomposition)는 계획을 계산적으로 더 다루기 쉽게 만듭니다.

계층적 계획(Hierarchical Planning)은 여러 추상화 수준(Levels of Abstraction)에서 의사결정을 표현합니다. 상위 수준 계획은 임무 목표(Mission Objectives)와 주요 작업 단계를 결정하고, 중간 수준 계획은 기술(Skills)이나 경로를 선택하며, 하위 수준 계획은 세부적인 움직임과 제어 행동을 생성할 수 있습니다. 상위 목표는 실행을 제약하지만 하위 수준의 실행 가능성(Feasibility)이 전략적 재계획(Replanning)을 요구할 수도 있기 때문에 이러한 계층 사이에서 정보가 양방향으로 흐를 필요가 있습니다.

계획은 행동이 세계를 어떻게 변화시키는지에 대한 내부 모델(Internal Model)에 근본적으로 의존합니다. 에이전트가 행동의 결과를 추정할 수 없다면 해당 행동이 목표 달성에 기여하는지를 신뢰성 있게 판단할 수 없습니다. 전이 모델(Transition Models)은 현재 상태와 행동이 어떻게 다음 상태를 생성하는지를 표현하여 실제 실행 전에 가능한 행동 순서를 평가하는 데 필요한 예측 구조(Predictive Structure)를 제공합니다.

월드 모델(World Models)은 객체, 에이전트, 공간적 관계(Spatial Relationships), 동역학(Dynamics), 그리고 잠재적으로 의미적 또는 인과적 구조(Semantic or Causal Structure)를 표현함으로써 이러한 능력을 일반화합니다. 후보 행동(Candidate Action)이 주어지면 월드 모델은 가능한 미래 상태(Future States)를 예측할 수 있습니다. 계획은 이러한 예측을 반복적으로 적용하여 현재에서 다양한 대안적 미래(Alternative Futures)로 이어지는 가상의 궤적을 구성할 수 있습니다.

따라서 정신적 시뮬레이션은 내부 모델을 시간 방향으로 전개하는 과정으로 이해할 수 있습니다. 에이전트는 현재 상태 추정(Current State Estimate)에서 시작하여 가능한 행동을 고려하고 다음 상태를 예측한 다음, 그 가상 상태에서 또 다른 행동을 고려합니다. 이러한 과정을 반복하면 모든 후보 행동 순서를 물리적으로 실행하지 않고도 평가할 수 있는 가상 궤적(Hypothetical Trajectories)이 생성됩니다.

시뮬레이션의 유용성은 모델 정확도(Model Accuracy)에 크게 의존합니다. 내부 모델이 동역학, 객체 특성(Object Properties), 환경 제약(Environmental Constraints), 다른 에이전트를 잘못 표현하면 시뮬레이션된 미래가 잘못된 판단을 유도할 수 있습니다. 따라서 계획 시스템은 예측 불확실성(Prediction Uncertainty)을 표현하고 내부적으로 생성된 궤적을 실제로 발생할 미래에 대한 확정적인 설명으로 취급하지 않아야 합니다.

예측 불확실성은 일반적으로 시뮬레이션 깊이(Simulation Depth)가 증가할수록 커집니다. 현재 상태나 전이 모델의 작은 오류도 여러 가상 단계를 거치면서 누적되어 장기 미래(Long-Horizon Future)를 크게 변화시킬 수 있습니다. 실제 계획기는 더 먼 미래를 살펴보는 이점과 감소하는 신뢰도(Confidence), 계산 비용(Computational Cost), 환경 변화가 세부 예측을 무효화할 가능성 사이의 균형을 유지해야 합니다.

분기(Branching)는 또 다른 계산적 문제를 발생시킵니다. 각각의 시뮬레이션 상태에서 여러 행동이 가능하다면 잠재적인 미래 궤적의 수는 계획 깊이에 따라 기하급수적으로 증가할 수 있습니다. 모든 행동 순서를 완전히 평가하는 것은 빠르게 불가능해집니다. 따라서 지능형 계획은 유망한 분기에 계산 자원을 집중하면서 가능성이 낮거나 관련성이 없거나 위험하거나 가치가 낮은 대안을 제거하는 메커니즘을 필요로 합니다.

탐색 알고리즘(Search Algorithms)은 가능한 미래 공간을 탐색하는 대표적인 메커니즘입니다. 상태를 노드(Node)로, 행동을 전이(Transition)로 표현하면 계획은 현재 상태에서 목표로 이어지는 경로를 탐색할 수 있습니다. 휴리스틱(Heuristics)은 어떤 상태가 목표에 더 가깝거나 더 가치 있는지를 추정하여 유용한 계획을 포함할 가능성이 높은 탐색 공간에 계산 자원을 집중시킬 수 있습니다.

가치 정보(Value Information)는 계획을 더욱 효과적으로 안내할 수 있습니다. 모든 후보 궤적을 동일하게 취급하는 대신 에이전트는 서로 다른 경로의 보상(Reward), 비용(Cost), 위험(Risk), 노력(Effort), 시간, 미래 기회(Future Opportunity)를 추정할 수 있습니다. 따라서 후보 미래가 단순히 명목상의 목표에 도달하는지만이 아니라 예상되는 결과에 따라 비교되기 때문에 계획은 가치 기반 의사결정(Value-Based Decision Making)과 긴밀하게 연결됩니다.

불확실성하의 계획(Planning under Uncertainty)은 하나의 결정론적 궤적(Deterministic Trajectory)이 아니라 여러 가능한 미래를 고려해야 합니다. 센서의 모호성(Sensor Ambiguity), 확률적 동역학(Stochastic Dynamics), 불완전한 모델, 예측하기 어려운 에이전트 때문에 동일한 행동도 서로 다른 결과를 만들어낼 수 있습니다. 따라서 견고한 계획(Robust Plan)은 여러 현실적인 변화에서도 유효하거나 예상한 미래가 발생하지 않았을 때 적절하게 대응할 수 있는 비상 행동(Contingency Actions)을 포함해야 합니다.

비상 계획(Contingency Planning)은 대안적인 분기를 명시적으로 표현합니다. 하나의 고정된 행동 순서를 규정하는 대신 특정 관찰이나 결과가 발생했을 때 무엇을 해야 하는지를 계획에 포함할 수 있습니다. 이를 통해 미래 행동이 실행 중에 획득한 정보에 따라 달라지는 조건부 정책(Conditional Policies)이 만들어집니다. 따라서 계획은 예측, 관찰, 의사결정, 적응(Adaptation)이 지속적으로 상호작용하는 과정이 됩니다.

동적인 환경에서는 잘 설계된 계획도 빠르게 무효화될 수 있기 때문에 재계획이 필수적입니다. 장애물이 움직이고, 자원을 사용할 수 없게 되며, 목표가 변경되고, 통신이 실패하거나 예측이 잘못될 수 있습니다. 지능형 에이전트는 관찰된 상태와 예상 상태를 비교하고 그 차이가 운영상 중요해질 경우 계획을 수정할 수 있어야 합니다.

이는 계획을 폐루프(Closed-Loop) 관점에서 이해하도록 합니다. 에이전트는 계획을 세우고 일부를 실행한 후 결과 상태를 관찰하고 예측과 비교하며, 내부 표상을 갱신하고 필요하면 다시 계획합니다. 이러한 이동 지평 방식(Receding-Horizon Behavior)은 처음 한 번 계산한 장기 행동 순서를 변화하는 조건과 관계없이 맹목적으로 따르는 것을 방지합니다.

모델 예측 제어(Model Predictive Control)는 이와 관련된 공학적 원리를 제공합니다. 시스템은 몇 단계 앞의 미래를 예측하고 제한된 지평(Horizon)에서 행동 순서를 최적화한 다음 즉각적으로 필요한 일부만 실행합니다. 이후 새로운 관찰을 받아 다시 최적화를 수행합니다. 이러한 접근법은 미래 지향적 시뮬레이션과 지속적인 피드백을 결합하므로 동역학과 교란(Disturbances)에 대한 빈번한 보정이 필요한 환경에서 특히 유용합니다.

기억(Memory)은 효율적인 계획에 크게 기여합니다. 일화 기억(Episodic Memory)은 과거의 유사한 상황과 그 상황에서 성공하거나 실패했던 계획을 검색할 수 있습니다. 의미 기억(Semantic Memory)은 객체, 환경, 규칙, 인과 관계에 관한 일반화된 지식을 제공하며, 절차 기억(Procedural Memory)은 재사용 가능한 기술을 제공하여 계획기가 저수준 행동을 처음부터 재구성하지 않고 의미 있는 행동 단위로 추론할 수 있도록 합니다.

따라서 이전의 계획은 고정된 스크립트(Fixed Scripts)가 아니라 템플릿(Templates)으로 기능할 수 있습니다. 새로운 문제가 과거 문제와 유사하면 에이전트는 관련된 해결책을 검색하여 현재 조건에 맞게 수정할 수 있습니다. 이는 유연성을 유지하면서 탐색 비용(Search Cost)을 줄입니다. 실패 기억(Failure Memories) 역시 계획기가 이미 바람직하지 않은 결과를 만든 것으로 알려진 궤적을 반복적으로 탐색하지 않도록 하기 때문에 중요합니다.

계획과 작업 기억(Working Memory)은 중간 목표, 후보 행동, 제약 조건, 예상 결과가 숙고 과정에서 계속 이용 가능한 상태로 유지되어야 하기 때문에 밀접하게 관련됩니다. 복잡한 계획에서는 원래의 목표를 유지하면서 여러 분기를 비교해야 할 수 있습니다. 따라서 제한된 작업 기억 용량은 추상화(Abstraction), 외부 기억(External Memory), 구조화된 표상, 계층적 분해의 필요성을 증가시킵니다.

전전두엽 피질(Prefrontal Cortex)은 이러한 능력과 중요한 생물학적 연결을 제공합니다. 전전두엽 시스템은 여러 대안 행동을 고려하는 동안 목표, 규칙, 중간 표상, 작업 맥락(Task Context)을 유지하는 데 기여합니다. 기억, 기저핵(Basal Ganglia), 가치 시스템(Value Systems), 예측 메커니즘과의 상호작용을 통해 즉각적인 자극만으로 행동을 결정하는 대신 여러 단계에 걸쳐 행동을 조직하도록 돕습니다.

해마(Hippocampus) 역시 미래 지향적 인지(Prospective Cognition)에 기여합니다. 기억된 경험과 공간적 순서(Spatial Sequences)를 표상하는 신경 메커니즘은 가능한 미래 궤적을 구성하거나 평가하는 데 참여할 수 있습니다. 이러한 관계는 기억과 상상(Imagination)이 완전히 분리된 기능이 아니라는 중요한 원리를 보여줍니다. 기억된 구조를 재결합하여 아직 발생하지 않은 상황에 대한 예측을 지원할 수 있기 때문입니다.

공간 내비게이션(Spatial Navigation)은 시뮬레이션을 통한 계획의 명확한 사례를 제공합니다. 에이전트는 현재 위치, 목적지, 장애물, 가능한 경로를 표상한 후 이동하기 전에 대안 경로를 평가할 수 있습니다. 인지 지도(Cognitive Maps)는 관계적 구조(Relational Structure)를 제공하여 정확히 동일한 궤적을 이전에 경험하지 않았더라도 지름길, 우회로, 새로운 경로를 고려할 수 있도록 합니다.

정신적 시뮬레이션은 물리적인 내비게이션을 넘어 확장됩니다. 에이전트는 작업 순서(Task Sequences), 사회적 상호작용(Social Interactions), 자원 사용(Resource Usage), 조작 결과(Manipulation Outcomes), 전략적 선택(Strategic Choices)을 시뮬레이션할 수 있습니다. 기본 원리는 동일합니다. 가상의 상태 전이를 구성하고 그 결과를 평가한 다음 되돌리기 어려운 행동을 실제로 실행하기 전에 비교 결과를 이용하여 행동을 결정합니다.

반사실적 추론(Counterfactual Reasoning)은 정신적 시뮬레이션과 밀접하게 관련됩니다. 사건이 발생한 이후 에이전트는 다른 행동을 선택했다면 어떤 일이 발생했을지를 고려할 수 있습니다. 이러한 비교를 통해 놓친 기회, 위험한 대안, 더 나은 전략을 발견할 수 있습니다. 따라서 반사실적 시뮬레이션(Counterfactual Simulation)은 대안 행동을 실제로 실행하지 않았더라도 학습을 향상시킬 수 있습니다.

시뮬레이션은 후보 행동을 실제 실행하도록 허용하기 전에 내부적으로 시험함으로써 안전(Safety)을 지원할 수도 있습니다. 로봇은 충돌을 발생시키거나, 액추에이터 한계(Actuator Limits)를 초과하거나, 플랫폼을 불안정하게 만들거나, 제한 구역(Restricted Zone)을 침범하거나, 인간에게 허용할 수 없는 수준으로 접근할 것으로 예측되는 궤적을 제거할 수 있습니다. 따라서 내부 예측은 행동 생성과 물리적 실행 사이에서 보호 계층(Protective Layer)으로 기능할 수 있습니다.

그러나 시뮬레이션 기반 안전(Simulation-Based Safety)은 이를 지원하는 모델과 불확실성 추정(Uncertainty Estimates)의 신뢰성만큼만 효과적입니다. 안전하다고 예측된 궤적도 모델링되지 않은 조건이 발생하면 실패할 수 있습니다. 따라서 실제 시스템은 시뮬레이션에만 의존하지 않고 예측 기반 안전 평가와 강제 제약(Hard Constraints), 반응형 제어기(Reactive Controllers), 모니터링(Monitoring), 비상 행동(Emergency Behaviors), 보수적 안전 여유(Conservative Margins)를 함께 사용합니다.

계획에는 서로 경쟁하는 여러 목표가 포함되는 경우가 많습니다. 로봇은 이동 시간을 최소화하면서 에너지를 보존하고, 위험을 피하고, 통신을 유지하고, 기계적 마모(Mechanical Wear)를 줄이며, 임무 우선순위를 충족해야 할 수 있습니다. 따라서 계획기는 하나의 단순한 성능 지표만 최적화하기보다 구조화된 효용(Structured Utility)이나 제약 조건을 기준으로 궤적을 평가해야 합니다.

자원 인식(Resource Awareness)은 체화 지능(Embodied Intelligence)에서 특히 중요합니다. 모든 계획은 시간, 에너지, 계산 자원, 액추에이터 수명(Actuator Lifetime), 저장 공간, 통신 대역폭(Communication Bandwidth)과 같은 유한한 자원을 소비합니다. 이론적으로 성공 가능한 계획이라도 완료 전에 배터리를 소진하거나 로봇에서 사용할 수 없는 계산 자원을 요구한다면 운영상 좋지 않은 계획입니다. 따라서 계획은 물리적 실행 가능성과 계산적 실행 가능성(Computational Feasibility)을 모두 충족해야 합니다.

다중 에이전트 계획(Multi-Agent Planning)은 미래가 다른 에이전트가 선택하는 행동에도 의존하기 때문에 추가적인 복잡성을 발생시킵니다. 로봇들은 협력하거나 공유 자원을 두고 경쟁하고, 정보를 교환하고, 작업을 분담하거나, 의도하지 않게 서로를 방해할 수 있습니다. 따라서 계획은 각각의 에이전트를 고정된 궤적을 따르는 독립적인 객체로 취급하기보다 공동 상태(Joint States)와 가능한 상호작용을 고려해야 합니다.

통신(Communication)은 다중 에이전트 불확실성을 감소시킬 수 있지만 동시에 제약을 발생시킵니다. 의도와 계획된 궤적을 공유하면 협력을 향상시킬 수 있지만 통신은 지연되거나, 사용할 수 없거나, 오래된 정보를 제공할 수 있습니다. 따라서 견고한 다중 로봇 계획(Robust Multi-Robot Planning)은 통신이 가능할 때 이를 활용하면서도 정보 교환이 악화될 경우 안전하게 계속 작동할 수 있는 충분한 지역 자율성(Local Autonomy)을 유지해야 합니다.

현대 인공지능 시스템(Modern AI Systems)은 기호 계획기(Symbolic Planners), 탐색 알고리즘, 강화 학습 정책(Reinforcement-Learning Policies), 트리 탐색(Tree Search), 최적화(Optimization), 학습된 월드 모델(Learned World Models), 그리고 이들을 결합한 다양한 메커니즘을 통해 계획을 구현합니다. 적절한 아키텍처는 상태 복잡도(State Complexity), 예측 지평(Prediction Horizon), 불확실성, 계산 자원, 행동이 엄격한 물리적 제약을 충족해야 하는지 여부에 따라 달라집니다.

학습된 월드 모델은 잠재 표상(Latent Representations) 내부에서 직접 계획할 수 있는 가능성을 제공합니다. 모든 미래의 감각적 세부 정보를 예측하는 대신 모델은 작업과 관련된 상태 변수를 압축된 잠재 공간(Latent Space)에 표현하고 그 변화를 시뮬레이션할 수 있습니다. 이를 통해 가치, 실행 가능성, 불확실성, 목표를 향한 진행 상황을 추정하는 데 필요한 정보를 유지하면서 계산 비용을 줄일 수 있습니다.

생성 모델(Generative Models)은 하나의 예측만 생성하는 대신 여러 현실적인 미래를 표현할 수 있습니다. 환경 변화가 본질적으로 모호한 경우 여러 대안 궤적(Alternative Trajectories)을 샘플링하면 동일한 행동에서 발생할 수 있는 여러 결과를 확인할 수 있습니다. 계획은 이러한 가능성을 비교하여 예측된 분포(Predicted Distribution) 전반에서 수용 가능한 수준으로 작동하는 행동을 선택할 수 있습니다.

피지컬 AI(Physical AI)에서 계획과 정신적 시뮬레이션은 인지(Cognition)와 물리적 실행(Physical Execution)을 연결하는 가교를 형성합니다. 지각(Perception)은 현재 세계를 추정하고, 기억은 이전 지식을 제공하며, 월드 모델은 결과를 예측하고, 가치 시스템은 가능한 미래를 평가하며, 계획은 행동을 조직하고, 제어기(Controllers)는 이를 실행합니다. 실제 환경에서 얻어진 피드백은 다시 전체 순환을 갱신합니다.

핵심적인 공학적 과제는 의사결정을 향상시키기에 충분한 시뮬레이션을 수행하면서 계획 자체가 지나치게 느려지지 않도록 하는 것입니다. 실시간 로봇(Real-Time Robots)은 움직임과 환경 변화가 부과하는 시간 제약 아래에서 작동합니다. 따라서 효과적인 아키텍처는 익숙한 상황에서는 빠르게 학습된 정책을 사용하고, 새로움(Novelty), 불확실성, 위험, 전략적 중요성이 추가적인 추론을 정당화할 때 더 깊은 시뮬레이션을 수행하도록 계산 자원을 선택적으로 할당합니다.

궁극적으로 계획과 정신적 시뮬레이션은 지능(Intelligence)이 아직 발생하지 않은 미래를 대상으로 행동할 수 있도록 합니다. 가능한 궤적을 내부적으로 구성하고, 그 가치와 위험을 평가하며, 중간 목표를 조직하고, 피드백을 통해 행동을 수정함으로써 에이전트는 단순한 반응적 행동(Reactive Behavior)을 넘어 세계와의 상호작용을 숙고적(Deliberate)이고 적응적(Adaptive)이며 점차 자율적인 방식으로 제어할 수 있습니다.

##  

## 08.06 Habit vs Goal Directed Behavior [w/Code]

![](images/image7.png){width="7.268055555555556in" height="7.268055555555556in"}

Habitual behavior and goal-directed behavior represent two complementary modes of action control that allow intelligent agents to balance efficiency with flexibility. Habitual behavior relies strongly on previously learned associations between situations and responses, whereas goal-directed behavior evaluates actions according to their expected consequences and current goals. Adaptive intelligence requires both mechanisms and the ability to shift between them as conditions change.

Goal-directed behavior is organized around explicit representations of desired outcomes. Before selecting an action, the agent considers what the action is expected to produce and whether that outcome remains valuable under the current circumstances. This makes goal-directed control sensitive to changes in goals, environmental conditions, internal needs, costs, risks, and available alternatives, allowing behavior to be modified rapidly when circumstances change.

Habitual behavior develops when particular actions are repeatedly performed in similar contexts and consistently produce acceptable outcomes. Through repetition, control can gradually shift from deliberate evaluation toward learned state--response relationships. Once established, a familiar cue or context can trigger an appropriate action with relatively little explicit evaluation of its consequences, reducing the cognitive and computational effort required for routine behavior.

The distinction can be expressed as different relationships among states, actions, and outcomes. Goal-directed control emphasizes state--action--outcome relationships because actions are evaluated through their predicted consequences. Habitual control places greater emphasis on state--action associations, allowing familiar situations to activate previously reinforced responses directly. These mechanisms can coexist rather than operating as completely independent systems.

Outcome devaluation provides an important way to distinguish the two forms of control. Suppose an action previously produced an outcome that was highly valuable, but the value of that outcome later decreases. Goal-directed behavior should rapidly reduce selection of the action because the predicted consequence is no longer desirable. A strong habit may continue producing the same response because its control depends less directly on the current value of the outcome.

Contingency degradation provides another distinction. If an action no longer reliably causes the outcome that originally reinforced it, goal-directed control can detect the changed causal relationship and adjust behavior. Habitual responses may persist longer because they are supported by previously learned associations. Flexibility therefore depends partly on whether the system continues to represent the causal consequences of its actions.

Goal-directed behavior requires an internal model capable of representing how actions transform states and lead to outcomes. The agent can use this model to compare alternatives before acting, making goal-directed control closely related to model-based decision making. Planning and mental simulation extend this process across multiple steps by evaluating sequences of actions and their possible future consequences.

Habitual control is more closely related to model-free learning because behavior can be guided by values or policies acquired through repeated experience without explicitly simulating future state transitions during every decision. This makes execution fast and computationally inexpensive. However, the resulting efficiency comes with reduced sensitivity to sudden changes that have not yet been incorporated through new experience.

The contrast between model-based and model-free control should not be treated as an exact biological equivalence to goal-directed and habitual behavior. Nevertheless, the computational distinction is useful. Model-based systems evaluate predicted consequences using an internal transition structure, whereas model-free systems cache useful action tendencies from experience. Intelligent behavior can exploit both forms of knowledge depending on context and available resources.

The basal ganglia are strongly involved in learned action selection and habit formation. Repeated reinforcement can strengthen pathways associated with successful actions, allowing familiar contexts to increasingly bias selection toward previously useful responses. Different corticostriatal circuits contribute to flexible and habitual forms of behavior, illustrating how action control can shift as experience accumulates and tasks become familiar.

The prefrontal cortex contributes strongly to goal-directed control by maintaining goals, rules, contextual information, and intermediate task representations. When familiar responses are inappropriate, prefrontal mechanisms can support alternative actions based on current objectives. This interaction between cortical control and learned action-selection mechanisms allows behavior to remain efficient without becoming completely dominated by automatic responses.

Habit formation provides significant computational advantages. Repeatedly solving a familiar decision from first principles would consume unnecessary time and cognitive resources. Once a reliable solution has been learned, proceduralized control can execute it rapidly while higher-level systems allocate resources to novel or difficult problems. Habit therefore represents an efficient compression of repeated successful decision processes into reusable behavioral policies.

This efficiency is especially important when actions must occur quickly. A system that performs extensive planning before every movement may respond too slowly for real-time interaction. Familiar sensorimotor behaviors, navigation routines, manipulation skills, and operational procedures can therefore benefit from automatic control. Fast habitual mechanisms provide immediate responses while slower deliberative mechanisms remain available when additional reasoning becomes necessary.

However, habits create vulnerability when environments change. A response that was repeatedly successful under previous conditions may become inefficient, unsafe, or inappropriate after goals, rules, physical conditions, or task requirements change. Because habitual control can continue operating from established associations, intelligent systems require mechanisms that detect when automatic behavior is no longer producing expected results.

Prediction error can provide one signal for such detection. When the outcome produced by a familiar action repeatedly differs from expectation, confidence in the existing behavior should decrease. Unexpected obstacles, declining rewards, increasing costs, or violated assumptions can indicate that the current policy is no longer appropriate. These discrepancies can trigger increased monitoring, learning, or transition toward goal-directed control.

Uncertainty also influences the balance between habitual and goal-directed behavior. Familiar environments with predictable dynamics favor efficient reuse of learned policies, while unfamiliar or ambiguous situations increase the value of explicit evaluation. An intelligent agent can therefore allocate more computational resources to planning when uncertainty rises and rely more heavily on cached behavior when confidence in familiar policies is high.

Risk provides another reason to shift control. Even a familiar behavior may deserve deliberate evaluation when the consequences of failure become severe. A mobile robot may normally execute a well-learned navigation routine automatically, but the same route may require additional planning when humans enter the area, localization confidence decreases, or environmental conditions become hazardous. Control strategy should therefore depend on consequence severity as well as familiarity.

Time pressure can produce the opposite effect. When immediate action is necessary, extensive goal-directed evaluation may be impossible. Fast learned policies can provide useful responses when deliberation would take too long. Adaptive control must therefore balance the benefits of careful evaluation against the cost of delayed action, selecting a mode of decision making appropriate to the available time.

Computational resources also influence arbitration. Mental simulation, tree search, trajectory evaluation, and world-model prediction can be expensive, especially when the action space and prediction horizon are large. Habitual policies provide an efficient alternative for situations that have already been solved repeatedly. The system can reserve expensive planning computation for decisions where it is likely to produce meaningful improvement.

Arbitration refers to the mechanism that determines how much control should be assigned to habitual and goal-directed systems. Rather than choosing one permanently, an adaptive agent can estimate which mechanism is more reliable or useful in the current situation. Familiarity, uncertainty, prediction error, risk, novelty, computational cost, urgency, and goal changes can all influence this allocation.

A hierarchical architecture can apply this distinction at multiple levels. High-level mission selection may remain strongly goal-directed, while lower-level locomotion and manipulation skills operate habitually. A robot may deliberately decide to inspect a particular location but execute walking, obstacle avoidance, or grasping through well-learned procedures. This combination reduces planning complexity while preserving strategic flexibility.

Procedural memory is closely connected to habitual control because repeated behaviors can become stored as reusable skills and policies. Instead of explicitly reconstructing every action sequence, the system retrieves and executes learned procedures. This allows previously acquired experience to influence behavior efficiently and provides continuity between memory, reinforcement learning, and action selection.

Episodic memory can support goal-directed behavior by retrieving previous situations in which similar choices produced specific consequences. These memories provide concrete evidence for evaluating current alternatives. A rare failure that is not strongly represented in a habitual policy may still be recalled during deliberation and substantially alter the estimated value or risk of a candidate action.

Semantic memory can provide generalized knowledge that modifies both systems. Rules, object properties, environmental constraints, and learned relationships can influence goal-directed evaluation while also shaping which habitual policies are considered appropriate. Memory systems therefore provide different forms of experience that help determine whether a familiar response should be reused or reconsidered.

Planning naturally favors goal-directed control because it evaluates possible futures before committing to action. World models can predict how candidate actions transform the environment, while value systems assess the desirability of resulting states. When circumstances are novel or important, mental simulation can temporarily replace automatic execution with deeper evaluation of possible consequences.

Habitual behavior can also accelerate planning by supplying reusable action chunks. A planner does not need to reason about every motor command when a complete navigation, grasping, docking, or manipulation skill can be treated as one abstract action. Habit and planning are therefore not necessarily competitors; learned procedures can become building blocks that make higher-level goal-directed reasoning more efficient.

This relationship is important for Physical AI because robots must operate continuously under limited computation, energy, and time. Performing deep planning for every action would be inefficient, while relying entirely on fixed policies would make the system fragile when conditions change. A practical architecture can use learned skills for routine execution and activate deeper reasoning when novelty, uncertainty, or risk exceeds acceptable levels.

For example, an autonomous mobile robot may normally follow a familiar corridor using a learned navigation policy. If the corridor becomes blocked, the habitual policy may no longer be appropriate. The system can detect the unexpected condition, suspend the routine behavior, activate map-based or world-model-based planning, identify an alternative route, and later learn from the successful adaptation.

Manipulation provides a similar example. A robot may use a well-practiced grasping policy for familiar objects under normal conditions. If an object has an unusual shape, uncertain pose, fragile material, or unexpected weight, automatic execution may become risky. Goal-directed evaluation can then incorporate perception, object properties, predicted outcomes, and safety constraints before selecting or modifying the grasp.

Human behavior also demonstrates that habits can be beneficial or problematic depending on context. Automatic routines reduce cognitive workload and support fluent performance, but they can persist even when people consciously recognize that conditions have changed. Intelligent artificial systems should therefore treat automation not simply as greater competence, but as a control mode that requires monitoring and mechanisms for interruption.

Interruptibility is particularly important in safety-critical systems. A habitual policy should not continue merely because it has already begun. New sensor evidence, emergency signals, human intervention, or detected constraint violations must be capable of suppressing the current behavior. Fast inhibitory mechanisms can therefore coexist with automatic policies to prevent efficiency from compromising safety.

Safe habits can be constructed by limiting the conditions under which learned policies are allowed to operate. A policy may be activated only when localization confidence, environmental familiarity, sensor quality, predicted risk, and hardware status remain within validated ranges. Outside this operating envelope, control can transition toward conservative planning, fallback behavior, or human supervision.

Continual learning allows habitual policies to evolve as experience accumulates. Successful repeated adaptations can gradually become new routines, reducing the need for deliberation in situations that were once unfamiliar. Conversely, policies that repeatedly produce poor outcomes should weaken or be revised. The boundary between habit and goal-directed control therefore changes continuously with learning.

Replay and memory consolidation can contribute to this transition. Important experiences can be replayed to strengthen successful state--action relationships or preserve failures that should inhibit future behavior. Through repeated offline or online learning, decisions that initially required expensive planning can become increasingly efficient, effectively transferring knowledge from deliberative problem solving into procedural control.

This creates a useful learning cycle for autonomous agents. Novel situations first trigger goal-directed reasoning and simulation. Successful solutions are stored in memory and reused when similar situations recur. Repetition strengthens efficient policies, allowing behavior to become increasingly automatic. When prediction errors or contextual changes appear, control can shift back toward deliberation and adaptation.

Multi-agent systems require additional caution because a behavior that became habitual in one social configuration may fail when other agents change their strategies. Team roles, communication availability, traffic patterns, and shared-resource conditions can alter the value of previously successful policies. Habitual coordination therefore requires continuous monitoring of the assumptions under which cooperative routines were learned.

The same principle applies to human--robot interaction. A robot may learn efficient interaction patterns for familiar users or environments, but automatic behavior must remain sensitive to human intent, proximity, uncertainty, and changing social context. Goal-directed supervisory mechanisms can prevent learned interaction routines from being applied rigidly when circumstances demand different behavior.

In AI engineering, the distinction can be implemented through hybrid architectures combining reactive policies, reinforcement learning, planning, world models, memory, and supervisory control. Fast policy networks can handle familiar situations, while planning modules evaluate unfamiliar or high-risk cases. An arbitration mechanism determines when control should remain automatic and when deeper reasoning should be activated.

A useful design objective is therefore not to eliminate habits but to make them appropriately conditional. Efficient intelligence depends on transforming repeated successful reasoning into reusable behavior while retaining the ability to reconsider that behavior when evidence changes. Habitual competence without flexibility becomes rigidity, while permanent deliberation without proceduralization becomes computationally inefficient.

Habit and goal-directed behavior ultimately describe a fundamental tradeoff between efficiency and adaptability. Habit allows experience to be compressed into fast, reusable action policies, while goal-directed control uses current goals, predicted outcomes, memory, and world models to reconsider what should be done. Intelligent autonomy emerges when a system can exploit both modes and reliably determine when to switch between them.

습관적 행동(Habitual Behavior)과 목표 지향적 행동(Goal-Directed Behavior)은 지능형 에이전트(Intelligent Agent)가 효율성(Efficiency)과 유연성(Flexibility) 사이의 균형을 유지할 수 있도록 하는 두 가지 상호보완적인 행동 제어 방식입니다. 습관적 행동은 이전에 학습된 상황과 반응 사이의 연관 관계에 크게 의존하는 반면, 목표 지향적 행동은 예상 결과(Expected Consequences)와 현재 목표(Current Goals)에 따라 행동을 평가합니다. 적응적 지능(Adaptive Intelligence)을 위해서는 두 메커니즘과 상황 변화에 따라 이들 사이를 전환하는 능력이 모두 필요합니다.

목표 지향적 행동은 원하는 결과(Desired Outcomes)에 대한 명시적인 표상을 중심으로 구성됩니다. 행동을 선택하기 전에 에이전트는 해당 행동이 어떤 결과를 만들어낼 것으로 예상되는지, 그리고 현재 상황에서도 그 결과가 여전히 가치 있는지를 고려합니다. 따라서 목표 지향적 제어(Goal-Directed Control)는 목표, 환경 조건, 내부 요구(Internal Needs), 비용(Cost), 위험(Risk), 이용 가능한 대안의 변화에 민감하며 상황이 변화하면 행동을 빠르게 수정할 수 있습니다.

습관적 행동은 특정 행동이 유사한 맥락에서 반복적으로 수행되고 지속적으로 수용 가능한 결과를 만들어낼 때 발달합니다. 반복을 통해 제어는 점차 숙고적 평가(Deliberative Evaluation)에서 학습된 상태--반응(State--Response) 관계로 이동할 수 있습니다. 습관이 형성되면 익숙한 단서(Cue)나 맥락이 결과에 대한 명시적인 평가를 거의 거치지 않고 적절한 행동을 유발할 수 있어 일상적인 행동에 필요한 인지적·계산적 부담을 줄입니다.

이러한 차이는 상태(State), 행동(Action), 결과(Outcome) 사이의 서로 다른 관계로 표현할 수 있습니다. 목표 지향적 제어는 행동을 예측된 결과를 통해 평가하기 때문에 상태--행동--결과(State--Action--Outcome) 관계를 강조합니다. 반면 습관적 제어는 상태--행동(State--Action) 연관 관계를 더욱 강조하여 익숙한 상황이 이전에 강화된 반응을 직접 활성화하도록 합니다. 이러한 메커니즘들은 완전히 독립적으로 작동하기보다 서로 공존할 수 있습니다.

결과 가치 저하(Outcome Devaluation)는 두 가지 제어 방식을 구분하는 중요한 방법을 제공합니다. 어떤 행동이 이전에는 매우 가치 있는 결과를 만들어냈지만 이후 그 결과의 가치가 감소했다고 가정할 수 있습니다. 목표 지향적 행동은 예측된 결과가 더 이상 바람직하지 않기 때문에 해당 행동의 선택을 빠르게 줄여야 합니다. 반면 강한 습관은 현재 결과 가치에 대한 의존도가 상대적으로 낮기 때문에 동일한 반응을 계속 만들어낼 수 있습니다.

우발성 저하(Contingency Degradation)는 또 다른 차이를 보여줍니다. 행동이 원래 강화했던 결과를 더 이상 안정적으로 만들어내지 못하면 목표 지향적 제어는 변화된 인과 관계(Causal Relationship)를 감지하고 행동을 조정할 수 있습니다. 습관적 반응은 이전에 학습된 연관 관계의 지원을 받기 때문에 더 오래 지속될 수 있습니다. 따라서 유연성은 시스템이 자신의 행동과 결과 사이의 인과적 결과를 지속적으로 표상하는지에 부분적으로 의존합니다.

목표 지향적 행동에는 행동이 상태를 어떻게 변화시키고 결과로 이어지는지를 표상할 수 있는 내부 모델(Internal Model)이 필요합니다. 에이전트는 이 모델을 이용하여 실제 행동 전에 대안들을 비교할 수 있으므로 목표 지향적 제어는 모델 기반 의사결정(Model-Based Decision Making)과 밀접하게 관련됩니다. 계획(Planning)과 정신적 시뮬레이션(Mental Simulation)은 행동 순서와 가능한 미래 결과를 여러 단계에 걸쳐 평가함으로써 이러한 과정을 확장합니다.

습관적 제어는 모든 의사결정에서 미래 상태 전이(Future State Transitions)를 명시적으로 시뮬레이션하지 않고 반복 경험을 통해 획득한 가치나 정책(Policies)을 기반으로 행동할 수 있기 때문에 모델 프리 학습(Model-Free Learning)과 더욱 밀접하게 관련됩니다. 이는 실행을 빠르고 계산적으로 저렴하게 만듭니다. 그러나 이러한 효율성은 새로운 경험을 통해 아직 반영되지 않은 갑작스러운 변화에 대한 민감성이 감소하는 대가를 수반합니다.

모델 기반 제어(Model-Based Control)와 모델 프리 제어(Model-Free Control)의 차이를 목표 지향적 행동과 습관적 행동의 정확한 생물학적 등가물로 간주해서는 안 됩니다. 그럼에도 이러한 계산적 구분은 유용합니다. 모델 기반 시스템은 내부 전이 구조(Internal Transition Structure)를 이용하여 예측 결과를 평가하는 반면, 모델 프리 시스템은 경험을 통해 유용한 행동 경향(Action Tendencies)을 저장합니다. 지능적 행동은 맥락과 이용 가능한 자원에 따라 두 형태의 지식을 모두 활용할 수 있습니다.

기저핵(Basal Ganglia)은 학습된 행동 선택(Learned Action Selection)과 습관 형성(Habit Formation)에 강하게 관여합니다. 반복적인 강화(Reinforcement)는 성공적인 행동과 관련된 경로를 강화하여 익숙한 맥락에서 이전에 유용했던 반응을 점차 더 쉽게 선택하도록 만들 수 있습니다. 서로 다른 피질--선조체 회로(Corticostriatal Circuits)는 유연한 행동과 습관적 행동에 기여하며, 경험이 축적되고 작업이 익숙해짐에 따라 행동 제어가 어떻게 변화할 수 있는지를 보여줍니다.

전전두엽 피질(Prefrontal Cortex)은 목표, 규칙, 맥락 정보(Contextual Information), 중간 작업 표상(Intermediate Task Representations)을 유지함으로써 목표 지향적 제어에 크게 기여합니다. 익숙한 반응이 적절하지 않은 경우 전전두엽 메커니즘은 현재 목표에 기반한 대안 행동을 지원할 수 있습니다. 이러한 피질 제어(Cortical Control)와 학습된 행동 선택 메커니즘의 상호작용은 행동이 자동적 반응에 완전히 지배되지 않으면서도 효율성을 유지하도록 합니다.

습관 형성은 상당한 계산적 이점(Computational Advantages)을 제공합니다. 익숙한 의사결정 문제를 매번 처음부터 다시 해결하는 것은 불필요한 시간과 인지 자원을 소비합니다. 신뢰할 수 있는 해결책이 학습되면 절차화된 제어(Proceduralized Control)를 통해 이를 빠르게 실행하면서 상위 수준 시스템은 새롭거나 어려운 문제에 자원을 할당할 수 있습니다. 따라서 습관은 반복적으로 성공한 의사결정 과정을 재사용 가능한 행동 정책(Behavioral Policies)으로 효율적으로 압축한 것으로 볼 수 있습니다.

이러한 효율성은 행동을 빠르게 수행해야 할 때 특히 중요합니다. 모든 움직임 전에 광범위한 계획을 수행하는 시스템은 실시간 상호작용(Real-Time Interaction)에 필요한 속도를 확보하지 못할 수 있습니다. 따라서 익숙한 감각운동 행동(Sensorimotor Behaviors), 내비게이션 루틴(Navigation Routines), 조작 기술(Manipulation Skills), 운영 절차는 자동 제어의 이점을 얻을 수 있습니다. 빠른 습관적 메커니즘은 즉각적인 반응을 제공하면서 추가 추론이 필요한 경우 더 느린 숙고적 메커니즘을 사용할 수 있도록 합니다.

그러나 환경이 변화하면 습관은 취약성을 만들 수 있습니다. 이전 조건에서 반복적으로 성공했던 반응도 목표, 규칙, 물리적 조건, 작업 요구사항이 변화하면 비효율적이거나 위험하거나 부적절해질 수 있습니다. 습관적 제어는 이미 형성된 연관 관계를 기반으로 계속 작동할 수 있으므로 지능형 시스템은 자동화된 행동이 더 이상 예상한 결과를 만들어내지 못하는 시점을 감지하는 메커니즘을 필요로 합니다.

예측 오차(Prediction Error)는 이러한 변화를 감지하는 하나의 신호를 제공할 수 있습니다. 익숙한 행동으로 생성된 결과가 반복적으로 예상과 달라지면 기존 행동에 대한 신뢰도가 감소해야 합니다. 예상하지 못한 장애물, 감소하는 보상, 증가하는 비용, 위반된 가정은 현재 정책이 더 이상 적절하지 않다는 것을 나타낼 수 있습니다. 이러한 불일치는 모니터링 강화, 추가 학습 또는 목표 지향적 제어로의 전환을 유발할 수 있습니다.

불확실성(Uncertainty) 역시 습관적 행동과 목표 지향적 행동 사이의 균형에 영향을 줍니다. 예측 가능한 동역학을 가진 익숙한 환경에서는 학습된 정책을 효율적으로 재사용하는 것이 유리하지만, 익숙하지 않거나 모호한 상황에서는 명시적 평가의 가치가 증가합니다. 따라서 지능형 에이전트는 불확실성이 증가하면 계획에 더 많은 계산 자원을 할당하고 익숙한 정책에 대한 신뢰도가 높을 때는 저장된 행동을 더욱 적극적으로 사용할 수 있습니다.

위험 역시 제어 방식을 전환해야 하는 또 다른 이유입니다. 익숙한 행동이라도 실패 결과가 심각해지면 숙고적 평가가 필요할 수 있습니다. 이동 로봇(Mobile Robot)은 일반적으로 잘 학습된 내비게이션 루틴을 자동적으로 실행할 수 있지만, 사람이 해당 영역에 들어오거나 위치 추정 신뢰도(Localization Confidence)가 낮아지거나 환경이 위험해지면 동일한 경로에 추가적인 계획이 필요할 수 있습니다. 따라서 제어 전략은 익숙함뿐 아니라 결과의 심각성(Consequence Severity)에도 의존해야 합니다.

시간 압박(Time Pressure)은 반대 방향의 효과를 만들 수 있습니다. 즉각적인 행동이 필요한 경우 광범위한 목표 지향적 평가를 수행할 시간이 없을 수 있습니다. 빠르게 학습된 정책은 숙고에 지나치게 많은 시간이 필요한 상황에서 유용한 반응을 제공할 수 있습니다. 따라서 적응적 제어(Adaptive Control)는 신중한 평가의 이점과 행동 지연의 비용 사이에서 균형을 유지하고 이용 가능한 시간에 적합한 의사결정 방식을 선택해야 합니다.

계산 자원(Computational Resources) 역시 중재(Arbitration)에 영향을 줍니다. 정신적 시뮬레이션, 트리 탐색(Tree Search), 궤적 평가(Trajectory Evaluation), 월드 모델 예측(World-Model Prediction)은 특히 행동 공간과 예측 지평(Prediction Horizon)이 클 때 많은 계산 비용을 요구할 수 있습니다. 습관적 정책은 이미 반복적으로 해결된 상황에 효율적인 대안을 제공합니다. 따라서 시스템은 실제 개선 가능성이 높은 의사결정에만 비용이 큰 계획 계산을 사용할 수 있습니다.

중재(Arbitration)는 습관적 시스템과 목표 지향적 시스템에 어느 정도의 제어권을 부여할지를 결정하는 메커니즘입니다. 하나의 방식을 영구적으로 선택하는 대신 적응형 에이전트는 현재 상황에서 어떤 메커니즘이 더 신뢰할 수 있고 유용한지를 평가할 수 있습니다. 익숙함(Familiarity), 불확실성, 예측 오차, 위험, 새로움(Novelty), 계산 비용, 긴급성(Urgency), 목표 변화 등이 이러한 제어권 배분에 영향을 줄 수 있습니다.

계층적 아키텍처(Hierarchical Architecture)는 이러한 구분을 여러 수준에 적용할 수 있습니다. 상위 수준의 임무 선택(Mission Selection)은 강하게 목표 지향적으로 유지하면서 하위 수준의 이동과 조작 기술은 습관적으로 작동할 수 있습니다. 로봇은 특정 위치를 검사하기로 숙고하여 결정하면서도 걷기, 장애물 회피, 파지(Grasping)는 잘 학습된 절차를 통해 실행할 수 있습니다. 이러한 조합은 전략적 유연성을 유지하면서 계획 복잡도를 줄입니다.

절차 기억(Procedural Memory)은 반복적인 행동이 재사용 가능한 기술과 정책으로 저장될 수 있기 때문에 습관적 제어와 밀접하게 연결됩니다. 시스템은 모든 행동 순서를 명시적으로 다시 구성하는 대신 학습된 절차를 검색하여 실행할 수 있습니다. 이를 통해 이전 경험이 행동에 효율적으로 영향을 줄 수 있으며 기억, 강화 학습(Reinforcement Learning), 행동 선택 사이의 연속성을 제공합니다.

일화 기억(Episodic Memory)은 유사한 선택이 특정한 결과를 만들어냈던 과거 상황을 검색함으로써 목표 지향적 행동을 지원할 수 있습니다. 이러한 기억은 현재 대안을 평가하는 구체적인 증거를 제공합니다. 습관적 정책에 강하게 반영되지 않은 희귀한 실패도 숙고 과정에서 회상되면 후보 행동의 예상 가치 또는 위험을 크게 변화시킬 수 있습니다.

의미 기억(Semantic Memory)은 두 시스템 모두를 수정할 수 있는 일반화된 지식을 제공합니다. 규칙, 객체의 특성(Object Properties), 환경 제약(Environmental Constraints), 학습된 관계는 목표 지향적 평가에 영향을 주는 동시에 어떤 습관적 정책이 적절한지를 결정할 수 있습니다. 따라서 기억 시스템은 익숙한 반응을 재사용할 것인지 다시 검토할 것인지를 결정하는 데 도움이 되는 다양한 형태의 경험을 제공합니다.

계획은 행동을 실제로 실행하기 전에 가능한 미래를 평가하기 때문에 자연스럽게 목표 지향적 제어를 선호합니다. 월드 모델은 후보 행동이 환경을 어떻게 변화시키는지 예측할 수 있고, 가치 시스템(Value Systems)은 결과 상태의 바람직함을 평가할 수 있습니다. 상황이 새롭거나 중요한 경우 정신적 시뮬레이션은 자동 실행을 일시적으로 대체하여 가능한 결과에 대한 더 깊은 평가를 수행할 수 있습니다.

습관적 행동은 재사용 가능한 행동 청크(Action Chunks)를 제공함으로써 계획을 가속할 수도 있습니다. 완전한 내비게이션, 파지, 도킹(Docking), 조작 기술을 하나의 추상적인 행동으로 취급할 수 있다면 계획기는 모든 모터 명령을 개별적으로 추론할 필요가 없습니다. 따라서 습관과 계획은 반드시 경쟁 관계에 있는 것이 아니며, 학습된 절차는 상위 수준의 목표 지향적 추론을 더욱 효율적으로 만드는 구성 요소가 될 수 있습니다.

이러한 관계는 로봇이 제한된 계산 자원, 에너지, 시간 안에서 지속적으로 작동해야 하는 피지컬 AI(Physical AI)에서 중요합니다. 모든 행동에 대해 깊은 계획을 수행하면 비효율적이지만 고정된 정책에만 의존하면 조건 변화에 취약해집니다. 실제적인 아키텍처는 일상적인 실행에는 학습된 기술을 사용하고 새로움, 불확실성 또는 위험이 허용 수준을 초과하면 더 깊은 추론을 활성화할 수 있습니다.

예를 들어 자율 이동 로봇(Autonomous Mobile Robot)은 일반적으로 익숙한 복도에서 학습된 내비게이션 정책을 사용할 수 있습니다. 복도가 차단되면 기존의 습관적 정책은 더 이상 적절하지 않을 수 있습니다. 시스템은 예상하지 못한 상황을 감지하고 일상적인 행동을 중단한 다음 지도 기반 또는 월드 모델 기반 계획(World-Model-Based Planning)을 활성화하여 대체 경로를 찾고, 이후 성공적인 적응 경험을 다시 학습할 수 있습니다.

조작(Manipulation)에서도 유사한 사례를 확인할 수 있습니다. 로봇은 일반적인 조건에서 익숙한 객체를 대상으로 잘 연습된 파지 정책(Grasping Policy)을 사용할 수 있습니다. 그러나 객체의 형태가 특이하거나 자세(Pose)가 불확실하거나 재질이 깨지기 쉽거나 예상하지 못한 무게를 가진다면 자동 실행은 위험해질 수 있습니다. 이때 목표 지향적 평가는 파지를 선택하거나 수정하기 전에 지각, 객체 특성, 예상 결과, 안전 제약(Safety Constraints)을 통합할 수 있습니다.

인간 행동 역시 습관이 맥락에 따라 유용하거나 문제가 될 수 있음을 보여줍니다. 자동화된 일상 행동은 인지 부하(Cognitive Workload)를 감소시키고 유창한 수행을 지원하지만, 사람이 조건이 변화했다는 사실을 의식적으로 인식한 이후에도 지속될 수 있습니다. 따라서 지능형 인공 시스템은 자동화를 단순히 더 높은 능력으로 간주하기보다 모니터링과 중단 메커니즘을 필요로 하는 하나의 제어 방식으로 다루어야 합니다.

중단 가능성(Interruptibility)은 안전 필수 시스템(Safety-Critical Systems)에서 특히 중요합니다. 습관적 정책은 이미 실행을 시작했다는 이유만으로 계속 진행되어서는 안 됩니다. 새로운 센서 증거, 비상 신호(Emergency Signals), 인간의 개입(Human Intervention), 감지된 제약 위반은 현재 행동을 억제할 수 있어야 합니다. 따라서 빠른 억제 메커니즘(Inhibitory Mechanisms)은 자동화된 정책과 공존하여 효율성이 안전을 훼손하는 것을 방지할 수 있습니다.

안전한 습관(Safe Habits)은 학습된 정책이 작동할 수 있는 조건을 제한함으로써 구성할 수 있습니다. 정책은 위치 추정 신뢰도, 환경 친숙도(Environmental Familiarity), 센서 품질(Sensor Quality), 예상 위험, 하드웨어 상태가 검증된 범위 안에 있을 때만 활성화될 수 있습니다. 이러한 운영 영역(Operating Envelope)을 벗어나면 제어는 보수적인 계획(Conservative Planning), 폴백 행동(Fallback Behavior), 인간 감독(Human Supervision)으로 전환될 수 있습니다.

지속 학습(Continual Learning)은 경험이 축적됨에 따라 습관적 정책을 발전시킬 수 있습니다. 성공적인 적응이 반복되면 새로운 일상 행동으로 점차 변화하여 과거에는 익숙하지 않았던 상황에서도 숙고의 필요성을 줄일 수 있습니다. 반대로 반복적으로 좋지 않은 결과를 만드는 정책은 약화되거나 수정되어야 합니다. 따라서 습관과 목표 지향적 제어 사이의 경계는 학습과 함께 지속적으로 변화합니다.

재생(Replay)과 기억 공고화(Memory Consolidation)는 이러한 전환에 기여할 수 있습니다. 중요한 경험을 재생하여 성공적인 상태--행동(State--Action) 관계를 강화하거나 미래 행동을 억제해야 하는 실패를 보존할 수 있습니다. 반복적인 오프라인 또는 온라인 학습(Offline or Online Learning)을 통해 처음에는 많은 비용의 계획이 필요했던 의사결정이 점차 효율적으로 변하면서 숙고적 문제 해결의 지식이 절차적 제어(Procedural Control)로 이전될 수 있습니다.

이는 자율 에이전트를 위한 유용한 학습 순환(Learning Cycle)을 형성합니다. 새로운 상황은 먼저 목표 지향적 추론과 시뮬레이션을 유발합니다. 성공적인 해결책은 기억에 저장되고 유사한 상황이 반복될 때 재사용됩니다. 반복은 효율적인 정책을 강화하여 행동을 점차 자동화합니다. 이후 예측 오차나 맥락 변화가 나타나면 제어는 다시 숙고와 적응으로 전환될 수 있습니다.

다중 에이전트 시스템(Multi-Agent Systems)은 하나의 사회적 구성에서 습관화된 행동이 다른 에이전트의 전략 변화에 따라 실패할 수 있기 때문에 추가적인 주의를 필요로 합니다. 팀 역할(Team Roles), 통신 가용성(Communication Availability), 이동 패턴(Traffic Patterns), 공유 자원의 상태가 변화하면 이전에 성공했던 정책의 가치도 달라질 수 있습니다. 따라서 습관적 협력(Habitual Coordination)은 협력적 행동이 학습되었던 전제조건을 지속적으로 모니터링해야 합니다.

동일한 원리는 인간--로봇 상호작용(Human--Robot Interaction)에도 적용됩니다. 로봇은 익숙한 사용자나 환경에 대해 효율적인 상호작용 패턴을 학습할 수 있지만 자동 행동은 인간의 의도(Human Intent), 근접성(Proximity), 불확실성, 변화하는 사회적 맥락에 계속 민감해야 합니다. 목표 지향적 감독 메커니즘(Goal-Directed Supervisory Mechanisms)은 상황이 다른 행동을 요구할 때 학습된 상호작용 루틴이 경직되게 적용되는 것을 방지할 수 있습니다.

인공지능 공학(AI Engineering)에서는 반응형 정책(Reactive Policies), 강화 학습, 계획, 월드 모델, 기억, 감독 제어(Supervisory Control)를 결합한 하이브리드 아키텍처(Hybrid Architectures)를 통해 이러한 구분을 구현할 수 있습니다. 빠른 정책 네트워크(Policy Networks)는 익숙한 상황을 처리하고 계획 모듈(Planning Modules)은 익숙하지 않거나 위험도가 높은 상황을 평가할 수 있습니다. 중재 메커니즘은 언제 자동 제어를 유지하고 언제 더 깊은 추론을 활성화할지를 결정합니다.

따라서 유용한 설계 목표는 습관을 제거하는 것이 아니라 적절한 조건에서 작동하도록 만드는 것입니다. 효율적인 지능은 반복적으로 성공한 추론을 재사용 가능한 행동으로 변환하면서 증거가 변화할 때 해당 행동을 다시 검토할 수 있는 능력을 유지하는 데 달려 있습니다. 유연성이 없는 습관적 능력은 경직성(Rigidity)이 되고, 절차화 없이 지속되는 숙고는 계산적으로 비효율적이 됩니다.

궁극적으로 습관적 행동과 목표 지향적 행동은 효율성과 적응성(Adaptability) 사이의 근본적인 절충 관계를 설명합니다. 습관은 경험을 빠르고 재사용 가능한 행동 정책으로 압축할 수 있도록 하며, 목표 지향적 제어는 현재 목표, 예측 결과, 기억, 월드 모델을 이용하여 무엇을 해야 하는지를 다시 검토합니다. 지능형 자율성(Intelligent Autonomy)은 두 가지 방식을 모두 활용하면서 상황에 따라 언제 전환해야 하는지를 신뢰성 있게 결정할 수 있을 때 형성됩니다.

##  

## 08.07 AI Agents and Brain Decision Systems [w/Code]

![](images/image8.png){width="7.268055555555556in" height="7.268055555555556in"}

AI agents and biological decision systems share a fundamental computational problem: they must transform incomplete observations, internal states, goals, memories, and predicted consequences into actions. Although artificial and neural systems operate through very different physical mechanisms, comparing their functional organization reveals common principles such as perception--action loops, value evaluation, memory-guided reasoning, planning, learning, and adaptive control.

The brain does not contain a single centralized decision module that independently determines every action. Decision making emerges from interactions among distributed neural systems responsible for perception, memory, valuation, executive control, action selection, emotion, and motor execution. Information circulates continuously among these systems, allowing decisions to reflect both immediate sensory conditions and knowledge accumulated through previous experience.

AI agents can similarly be understood as distributed decision architectures rather than isolated prediction models. An agent receives observations from an environment, constructs or updates an internal state, evaluates possible actions, selects an action, observes the resulting consequences, and modifies future behavior. This repeated perception--decision--action cycle provides the basic structure through which artificial agents interact adaptively with changing environments.

The prefrontal cortex provides an important biological reference for executive control. It contributes to maintaining goals, task rules, contextual information, working-memory contents, and alternative courses of action. These functions resemble supervisory components in AI agents that maintain task objectives, coordinate specialized modules, determine priorities, and regulate when deeper reasoning or planning should replace routine behavior.

The basal ganglia provide another important comparison because they participate in action selection, reinforcement learning, and the regulation of competing behavioral alternatives. Candidate actions can receive different levels of support according to learned value and current context. In artificial agents, policy selection, action-value estimation, reinforcement-learning mechanisms, or arbitration modules can perform functionally related roles without reproducing the biological circuitry itself.

Dopaminergic signaling illustrates how decision systems can learn from discrepancies between expectation and experience. Reward prediction errors provide information about whether outcomes were better or worse than expected, enabling value estimates and future action preferences to change. Reinforcement-learning agents use mathematically related error signals to update value functions, policies, or models from interaction experience.

The hippocampus contributes memory and relational structure to decision making. Previous episodes, spatial relationships, and sequences can provide information for evaluating current situations and imagining future possibilities. AI agents can implement related functions through episodic memory stores, vector retrieval, structured databases, maps, trajectories, or experience buffers that make previous interactions available during current reasoning.

Semantic knowledge also influences decisions by providing generalized information that extends beyond individual experiences. Humans can use concepts, rules, object properties, causal relationships, and social knowledge when evaluating unfamiliar situations. AI agents similarly benefit from pretrained representations, knowledge bases, language models, world knowledge, and structured memory that allow prior information to constrain and guide new decisions.

Working memory provides temporary access to information needed during ongoing reasoning. Goals, intermediate results, relevant observations, candidate plans, and constraints must remain available while a complex decision unfolds. Artificial agents require comparable temporary computational workspaces, such as context windows, scratch representations, state buffers, or structured task memories, to preserve information across multi-step reasoning processes.

Perception supplies the state information upon which decisions depend, but neither biological nor artificial systems receive perfectly complete descriptions of the world. Sensory noise, occlusion, ambiguity, and limited observation create uncertainty. Decision systems must therefore combine current evidence with prior knowledge, memory, prediction, and confidence estimates to construct a useful internal representation of the situation.

Attention helps manage the enormous amount of potentially available information. Biological attention prioritizes sensory signals, memories, goals, and internal representations according to current relevance. AI agents similarly require mechanisms that select which observations, retrieved memories, tools, tokens, objects, or environmental features deserve computational resources, preventing decision processes from treating every piece of information as equally important.

Value systems determine why one possible outcome should be preferred over another. Biological decisions can reflect reward, effort, danger, physiological needs, social consequences, and long-term objectives. Artificial agents may represent preferences through reward functions, utility models, cost functions, learned evaluators, constraints, or human-provided objectives. In both cases, action selection requires some mechanism for distinguishing desirable futures from undesirable ones.

Goal-directed decision making depends on evaluating actions through their expected consequences. Biological systems can use internal models and memory to consider what may happen before acting. Model-based AI agents similarly use transition models, simulators, search procedures, or learned world models to generate possible futures and compare candidate actions according to predicted value, feasibility, uncertainty, and risk.

Habitual behavior provides a complementary mode of control. Frequently repeated actions can become efficient responses that require less deliberation, allowing cognitive resources to be allocated elsewhere. AI agents can achieve similar efficiency through learned policies, cached actions, reusable skills, procedural memory, or reactive controllers. Familiar situations can then be handled rapidly without reconstructing a complete plan every time.

Adaptive intelligence requires arbitration between these modes. Deep planning is unnecessary for every familiar action, while automatic policies may fail in novel or dangerous situations. Both biological organisms and advanced AI agents benefit from mechanisms that allocate more reasoning when uncertainty, novelty, prediction error, risk, or goal conflict increases and rely on efficient learned behavior when conditions remain familiar and predictable.

Mental simulation provides another major connection between biological cognition and agentic AI. Humans can imagine alternative actions and possible consequences without physically performing them. Artificial agents equipped with world models can similarly simulate candidate trajectories internally. Such prospective computation allows failures to be rejected, opportunities to be identified, and plans to be evaluated before resources or physical actions are committed.

However, internal simulation introduces its own uncertainty. Imagined futures depend on the accuracy of the models used to generate them, and prediction errors can accumulate as the simulation horizon increases. Both biological and artificial decision systems therefore need mechanisms that limit confidence in distant predictions, incorporate feedback, and revise plans when observations diverge from expectations.

Closed-loop control is essential because intelligent decisions cannot end when an action is selected. After acting, the system must observe what actually happened and compare the result with what was expected. Prediction errors, environmental changes, and unexpected consequences then modify subsequent decisions. Intelligence therefore emerges from continuous cycles of sensing, prediction, action, observation, and learning.

Emotion and affect provide biological mechanisms that rapidly influence attention, valuation, memory, and action readiness. Artificial agents do not need biological emotions to perform decision making, but functionally related control variables can prioritize urgent conditions, amplify safety concerns, modify risk tolerance, or redirect computational resources. The comparison is functional rather than a claim that artificial systems experience emotional states.

Metacognition adds another level of control by allowing a system to evaluate aspects of its own reasoning. Humans can recognize uncertainty, conflict, unfamiliarity, or insufficient knowledge and alter their strategy accordingly. AI agents can approximate such functionality through confidence estimation, uncertainty monitoring, verification, self-evaluation, consistency checking, or policies that determine when external information or additional computation is required.

Tool use extends an agent\'s effective decision capability beyond its internal model. Humans use external artifacts, instruments, written records, and other people to overcome limitations in memory and computation. AI agents can similarly invoke search systems, databases, calculators, simulators, software tools, sensors, and specialized models. Decision making then includes not only choosing environmental actions but also choosing useful cognitive operations.

Memory retrieval itself can therefore become an action. An agent deciding what to do may first determine that additional information is needed, retrieve a relevant episode, query semantic knowledge, inspect a map, or search an external database. The retrieved information modifies the internal state and may change the preferred action. Agentic reasoning thus includes information acquisition as part of the decision process.

Language provides a powerful mechanism for representing goals, rules, plans, explanations, and abstract relationships. In humans, language interacts with broader cognitive systems rather than replacing perception, memory, or action control. Language-model-based agents likewise become more capable when linguistic reasoning is connected with persistent memory, grounded perception, world models, tools, planning systems, and mechanisms for physical or digital action.

Large language models can provide high-level reasoning and semantic knowledge within an agent architecture, but next-token prediction alone does not constitute a complete autonomous decision system. Persistent goals, environmental state tracking, memory, action interfaces, feedback, verification, and safety mechanisms are required to transform a language model from a conversational predictor into a component of an adaptive agent.

Embodied AI makes this distinction especially important because physical actions have irreversible consequences. A robot cannot treat every generated action proposal as executable. Candidate actions must be checked against geometric feasibility, dynamics, hardware limits, collision risk, human safety, energy availability, and environmental uncertainty. Cognitive reasoning must therefore connect with lower-level perception, planning, and control systems.

Hierarchical control provides an effective architecture for integrating these capabilities. A high-level agent may interpret goals and select tasks, an intermediate system may generate plans and choose reusable skills, and lower-level controllers may execute trajectories and stabilize physical behavior. Feedback from lower levels can invalidate high-level assumptions, requiring plans or even mission objectives to be reconsidered.

Brain decision systems are also highly parallel. Perception, memory retrieval, valuation, motor preparation, and monitoring can proceed simultaneously rather than as one strictly sequential algorithm. Artificial agent architectures can benefit from comparable modularity, allowing specialized processes to operate concurrently while coordination mechanisms integrate their outputs into coherent behavior.

Multi-agent interaction further expands the decision problem. Humans reason about other individuals\' goals, intentions, knowledge, and likely actions. Artificial agents operating with humans or other robots must similarly predict interactions, communicate intentions, negotiate shared resources, coordinate tasks, and revise plans when another agent behaves unexpectedly. Decision making therefore becomes relational rather than purely individual.

Social decision systems also require values that extend beyond immediate individual reward. Cooperation, trust, fairness, predictability, safety, and shared objectives can influence which actions are acceptable. Human-compatible AI agents require mechanisms that represent constraints and preferences associated with other people rather than optimizing only narrow task performance or short-term reward.

Learning allows the architecture to improve across repeated interactions. Successful decisions can strengthen reusable policies, unexpected outcomes can update world models, important episodes can enter memory, and repeated planning solutions can become proceduralized skills. The decision system therefore changes not only its current action but also the internal structures that determine future decisions.

Replay and consolidation can further transform experience into durable decision competence. Important trajectories can be revisited after execution, allowing value estimates, predictive models, and policies to improve without repeating every physical event. Rare failures can receive additional learning emphasis, while successful strategies can gradually become efficient procedures available for future situations.

An integrated AI agent can therefore be described as a continuous cognitive control loop. Perception estimates the world, attention prioritizes relevant information, memory supplies previous knowledge, world models predict possible futures, value mechanisms evaluate alternatives, planning organizes actions, policies provide efficient skills, and monitoring determines whether execution remains consistent with goals and safety constraints.

No single brain region corresponds directly to a modern AI module, and no AI architecture should be interpreted as a literal digital copy of the brain. The useful comparison exists at the level of computational functions and system organization. Biological intelligence demonstrates how specialized processes can cooperate dynamically, while AI engineering provides alternative mechanisms for implementing related capabilities in software and machines.

The comparison also highlights an important limitation of purely feedforward intelligence. Systems that simply map an input to an output cannot easily maintain goals, reconsider assumptions, retrieve relevant experience, simulate alternatives, detect their own uncertainty, or adapt plans through feedback. Agentic intelligence requires recurrent interaction among state estimation, memory, evaluation, prediction, action, and learning.

For Physical AI, these principles converge in autonomous systems that must continuously perceive, remember, predict, decide, act, and learn while remaining grounded in physical reality. Brain-inspired functional organization suggests that robust autonomy is unlikely to emerge from one monolithic algorithm. Instead, intelligence can arise from coordinated subsystems operating across different timescales and levels of abstraction.

AI agents and brain decision systems ultimately illustrate the same broad principle: adaptive behavior requires more than producing an answer to a stimulus. An intelligent system must maintain goals, integrate memory with current evidence, evaluate uncertainty and value, anticipate consequences, select and execute actions, observe their effects, and use experience to improve future decisions.

인공지능 에이전트(AI Agents)와 생물학적 의사결정 시스템(Biological Decision Systems)은 근본적으로 동일한 계산적 문제에 직면합니다. 즉, 불완전한 관찰(Incomplete Observations), 내부 상태(Internal States), 목표(Goals), 기억(Memories), 예측된 결과(Predicted Consequences)를 행동(Actions)으로 변환해야 합니다. 인공 시스템과 신경 시스템은 매우 다른 물리적 메커니즘으로 작동하지만, 기능적 조직을 비교하면 지각--행동 순환(Perception--Action Loops), 가치 평가(Value Evaluation), 기억 기반 추론(Memory-Guided Reasoning), 계획(Planning), 학습(Learning), 적응적 제어(Adaptive Control)와 같은 공통 원리를 확인할 수 있습니다.

뇌에는 모든 행동을 독립적으로 결정하는 하나의 중앙집중식 의사결정 모듈(Centralized Decision Module)이 존재하지 않습니다. 의사결정은 지각(Perception), 기억(Memory), 가치 평가(Valuation), 실행 제어(Executive Control), 행동 선택(Action Selection), 감정(Emotion), 운동 실행(Motor Execution)을 담당하는 분산된 신경 시스템(Distributed Neural Systems) 사이의 상호작용에서 나타납니다. 정보는 이러한 시스템 사이를 지속적으로 순환하여 즉각적인 감각 조건과 과거 경험을 통해 축적된 지식이 모두 의사결정에 반영되도록 합니다.

인공지능 에이전트 역시 고립된 예측 모델(Isolated Prediction Models)이 아니라 분산형 의사결정 아키텍처(Distributed Decision Architectures)로 이해할 수 있습니다. 에이전트는 환경으로부터 관찰을 받아 내부 상태를 구성하거나 갱신하고, 가능한 행동을 평가하고, 하나의 행동을 선택한 후 그 결과를 관찰하여 미래 행동을 수정합니다. 이러한 반복적인 지각--의사결정--행동 순환(Perception--Decision--Action Cycle)은 인공 에이전트가 변화하는 환경과 적응적으로 상호작용하는 기본 구조를 제공합니다.

전전두엽 피질(Prefrontal Cortex)은 실행 제어(Executive Control)에 대한 중요한 생물학적 참고 모델을 제공합니다. 전전두엽은 목표, 작업 규칙(Task Rules), 맥락 정보(Contextual Information), 작업 기억(Working Memory)의 내용, 대안적 행동 경로를 유지하는 데 기여합니다. 이러한 기능은 작업 목표를 유지하고, 전문화된 모듈을 조정하며, 우선순위를 결정하고, 언제 일상적 행동을 대신하여 더 깊은 추론이나 계획을 수행할지를 조절하는 인공지능 에이전트의 감독 구성요소(Supervisory Components)와 유사합니다.

기저핵(Basal Ganglia)은 행동 선택, 강화 학습(Reinforcement Learning), 경쟁하는 행동 대안의 조절에 관여하기 때문에 또 다른 중요한 비교 대상입니다. 후보 행동(Candidate Actions)은 학습된 가치와 현재 맥락에 따라 서로 다른 수준의 지지를 받을 수 있습니다. 인공지능 에이전트에서는 정책 선택(Policy Selection), 행동 가치 추정(Action-Value Estimation), 강화 학습 메커니즘 또는 중재 모듈(Arbitration Modules)이 생물학적 회로 자체를 복제하지 않으면서 기능적으로 관련된 역할을 수행할 수 있습니다.

도파민성 신호(Dopaminergic Signaling)는 의사결정 시스템이 기대와 경험 사이의 차이를 통해 어떻게 학습할 수 있는지를 보여줍니다. 보상 예측 오차(Reward Prediction Errors)는 결과가 예상보다 좋았는지 나빴는지에 대한 정보를 제공하여 가치 추정과 미래 행동 선호도가 변화하도록 합니다. 강화 학습 에이전트는 수학적으로 관련된 오차 신호(Error Signals)를 이용하여 상호작용 경험으로부터 가치 함수(Value Functions), 정책(Policies), 모델(Models)을 갱신합니다.

해마(Hippocampus)는 기억과 관계적 구조(Relational Structure)를 의사결정에 제공합니다. 이전의 사건, 공간적 관계(Spatial Relationships), 행동 순서는 현재 상황을 평가하고 가능한 미래를 상상하는 데 필요한 정보를 제공할 수 있습니다. 인공지능 에이전트는 일화 기억 저장소(Episodic Memory Stores), 벡터 검색(Vector Retrieval), 구조화된 데이터베이스(Structured Databases), 지도(Maps), 궤적(Trajectories), 경험 버퍼(Experience Buffers)를 통해 관련 기능을 구현하여 과거 상호작용을 현재 추론에서 사용할 수 있습니다.

의미 지식(Semantic Knowledge) 역시 개별 경험을 넘어 일반화된 정보를 제공함으로써 의사결정에 영향을 줍니다. 인간은 익숙하지 않은 상황을 평가할 때 개념, 규칙, 객체 특성(Object Properties), 인과 관계(Causal Relationships), 사회적 지식(Social Knowledge)을 사용할 수 있습니다. 인공지능 에이전트도 사전학습된 표상(Pretrained Representations), 지식 베이스(Knowledge Bases), 언어 모델(Language Models), 월드 지식(World Knowledge), 구조화된 기억을 활용하여 사전 지식이 새로운 의사결정을 제한하고 안내하도록 할 수 있습니다.

작업 기억은 진행 중인 추론에 필요한 정보에 일시적으로 접근할 수 있도록 합니다. 복잡한 의사결정이 진행되는 동안 목표, 중간 결과, 관련 관찰, 후보 계획(Candidate Plans), 제약 조건(Constraints)이 계속 이용 가능한 상태로 유지되어야 합니다. 인공지능 에이전트도 여러 단계의 추론 과정에서 정보를 보존하기 위해 컨텍스트 윈도(Context Windows), 임시 추론 표상(Scratch Representations), 상태 버퍼(State Buffers), 구조화된 작업 기억(Structured Task Memories)과 같은 임시 계산 작업공간(Computational Workspaces)을 필요로 합니다.

지각은 의사결정에 필요한 상태 정보를 제공하지만 생물학적 시스템과 인공 시스템 모두 세계에 대한 완전한 설명을 제공받지는 못합니다. 감각 노이즈(Sensory Noise), 가림(Occlusion), 모호성(Ambiguity), 제한된 관찰(Limited Observation)은 불확실성(Uncertainty)을 발생시킵니다. 따라서 의사결정 시스템은 현재 증거를 사전 지식, 기억, 예측, 신뢰도 추정(Confidence Estimates)과 결합하여 상황에 대한 유용한 내부 표상(Internal Representation)을 구성해야 합니다.

주의(Attention)는 잠재적으로 이용 가능한 막대한 양의 정보를 관리하도록 돕습니다. 생물학적 주의는 현재의 관련성에 따라 감각 신호, 기억, 목표, 내부 표상의 우선순위를 결정합니다. 인공지능 에이전트 역시 어떤 관찰, 검색된 기억, 도구(Tools), 토큰(Tokens), 객체 또는 환경 특징(Environmental Features)에 계산 자원을 할당해야 하는지를 선택하는 메커니즘이 필요하며, 이를 통해 모든 정보를 동일하게 중요하게 처리하는 것을 방지할 수 있습니다.

가치 시스템(Value Systems)은 가능한 결과 가운데 왜 하나의 결과가 다른 결과보다 선호되어야 하는지를 결정합니다. 생물학적 의사결정은 보상(Reward), 노력(Effort), 위험(Danger), 생리적 요구(Physiological Needs), 사회적 결과(Social Consequences), 장기 목표(Long-Term Objectives)를 반영할 수 있습니다. 인공지능 에이전트는 보상 함수(Reward Functions), 효용 모델(Utility Models), 비용 함수(Cost Functions), 학습된 평가기(Learned Evaluators), 제약 조건, 인간이 제공한 목표를 통해 선호를 표현할 수 있습니다. 두 경우 모두 행동 선택에는 바람직한 미래와 바람직하지 않은 미래를 구분하는 메커니즘이 필요합니다.

목표 지향적 의사결정(Goal-Directed Decision Making)은 행동의 예상 결과를 기반으로 행동을 평가하는 데 의존합니다. 생물학적 시스템은 내부 모델과 기억을 이용하여 실제 행동 전에 어떤 일이 발생할 수 있는지를 고려할 수 있습니다. 모델 기반 인공지능 에이전트(Model-Based AI Agents) 역시 전이 모델(Transition Models), 시뮬레이터(Simulators), 탐색 절차(Search Procedures), 학습된 월드 모델(Learned World Models)을 사용하여 가능한 미래를 생성하고 예측된 가치, 실행 가능성(Feasibility), 불확실성, 위험에 따라 후보 행동을 비교합니다.

습관적 행동(Habitual Behavior)은 상호보완적인 제어 방식을 제공합니다. 자주 반복되는 행동은 숙고(Deliberation)를 덜 요구하는 효율적인 반응으로 발전하여 인지 자원을 다른 곳에 할당할 수 있도록 합니다. 인공지능 에이전트도 학습된 정책(Learned Policies), 캐시된 행동(Cached Actions), 재사용 가능한 기술(Reusable Skills), 절차 기억(Procedural Memory), 반응형 제어기(Reactive Controllers)를 통해 유사한 효율성을 얻을 수 있습니다. 이를 통해 익숙한 상황은 매번 완전한 계획을 재구성하지 않고도 빠르게 처리할 수 있습니다.

적응적 지능(Adaptive Intelligence)을 위해서는 이러한 제어 방식 사이의 중재(Arbitration)가 필요합니다. 모든 익숙한 행동에 깊은 계획이 필요한 것은 아니며, 자동화된 정책은 새롭거나 위험한 상황에서 실패할 수 있습니다. 생물학적 유기체와 고급 인공지능 에이전트 모두 불확실성, 새로움(Novelty), 예측 오차(Prediction Error), 위험 또는 목표 충돌(Goal Conflict)이 증가하면 더 많은 추론을 할당하고, 조건이 익숙하고 예측 가능할 때는 효율적인 학습 행동에 의존하는 메커니즘으로부터 이점을 얻습니다.

정신적 시뮬레이션(Mental Simulation)은 생물학적 인지와 에이전트형 인공지능(Agentic AI) 사이의 또 다른 중요한 연결점을 제공합니다. 인간은 가능한 행동과 결과를 실제로 수행하지 않고도 상상할 수 있습니다. 월드 모델을 갖춘 인공지능 에이전트도 후보 궤적(Candidate Trajectories)을 내부적으로 시뮬레이션할 수 있습니다. 이러한 미래 지향적 계산(Prospective Computation)을 통해 물리적 행동이나 자원을 투입하기 전에 실패 가능성을 제거하고, 기회를 식별하며, 계획을 평가할 수 있습니다.

그러나 내부 시뮬레이션 자체도 불확실성을 발생시킵니다. 상상된 미래는 이를 생성하는 모델의 정확도에 의존하며, 예측 오차는 시뮬레이션 지평(Simulation Horizon)이 길어질수록 누적될 수 있습니다. 따라서 생물학적 의사결정 시스템과 인공지능 의사결정 시스템 모두 먼 미래의 예측에 대한 신뢰도를 제한하고, 피드백을 반영하며, 실제 관찰이 예상과 달라지면 계획을 수정하는 메커니즘을 필요로 합니다.

폐루프 제어(Closed-Loop Control)가 중요한 이유는 지능적 의사결정이 행동을 선택하는 순간 끝나는 것이 아니기 때문입니다. 행동한 이후 시스템은 실제로 어떤 일이 발생했는지를 관찰하고 그 결과를 예상했던 것과 비교해야 합니다. 예측 오차, 환경 변화, 예상하지 못한 결과는 이후의 의사결정을 수정합니다. 따라서 지능은 감지(Sensing), 예측, 행동, 관찰, 학습이 지속적으로 반복되는 순환에서 나타납니다.

감정(Emotion)과 정서(Affect)는 주의, 가치 평가, 기억, 행동 준비도(Action Readiness)에 빠르게 영향을 미치는 생물학적 메커니즘을 제공합니다. 인공지능 에이전트가 의사결정을 수행하기 위해 생물학적 감정을 가질 필요는 없지만, 기능적으로 유사한 제어 변수(Control Variables)를 사용하여 긴급한 상황의 우선순위를 높이고, 안전 문제를 강화하며, 위험 허용도(Risk Tolerance)를 변경하거나 계산 자원을 재배분할 수 있습니다. 이러한 비교는 기능적 비교이며 인공 시스템이 감정 상태를 경험한다는 의미는 아닙니다.

메타인지(Metacognition)는 시스템이 자신의 추론 일부를 평가할 수 있도록 함으로써 또 다른 제어 계층을 추가합니다. 인간은 불확실성, 충돌, 익숙하지 않은 상황, 지식 부족을 인식하고 그에 따라 전략을 변경할 수 있습니다. 인공지능 에이전트는 신뢰도 추정, 불확실성 모니터링(Uncertainty Monitoring), 검증(Verification), 자기 평가(Self-Evaluation), 일관성 검사(Consistency Checking), 외부 정보나 추가 계산이 필요한 시점을 결정하는 정책을 통해 이러한 기능에 근접할 수 있습니다.

도구 사용(Tool Use)은 에이전트의 효과적인 의사결정 능력을 내부 모델의 한계 이상으로 확장합니다. 인간은 기억과 계산의 한계를 극복하기 위해 외부 인공물(External Artifacts), 도구, 기록, 다른 사람을 이용합니다. 인공지능 에이전트 역시 검색 시스템(Search Systems), 데이터베이스, 계산기, 시뮬레이터, 소프트웨어 도구, 센서, 전문화된 모델을 호출할 수 있습니다. 따라서 의사결정에는 환경에 대한 행동뿐만 아니라 유용한 인지적 연산(Cognitive Operations)을 선택하는 것도 포함됩니다.

따라서 기억 검색(Memory Retrieval) 자체도 하나의 행동이 될 수 있습니다. 무엇을 해야 할지 결정하는 에이전트는 먼저 추가 정보가 필요하다고 판단하고 관련된 사건을 검색하거나, 의미 지식을 조회하거나, 지도를 확인하거나, 외부 데이터베이스를 검색할 수 있습니다. 검색된 정보는 내부 상태를 변경하고 선호되는 행동을 바꿀 수 있습니다. 따라서 에이전트형 추론(Agentic Reasoning)은 정보 획득(Information Acquisition)을 의사결정 과정의 일부로 포함합니다.

언어(Language)는 목표, 규칙, 계획, 설명, 추상적 관계(Abstract Relationships)를 표현하는 강력한 메커니즘을 제공합니다. 인간에서 언어는 지각, 기억, 행동 제어를 대체하는 것이 아니라 더 광범위한 인지 시스템과 상호작용합니다. 언어 모델 기반 에이전트(Language-Model-Based Agents) 역시 언어적 추론이 지속 기억(Persistent Memory), 현실에 기반한 지각(Grounded Perception), 월드 모델, 도구, 계획 시스템, 물리적 또는 디지털 행동 메커니즘과 연결될 때 더 높은 능력을 발휘할 수 있습니다.

대규모 언어 모델(Large Language Models)은 에이전트 아키텍처에서 상위 수준 추론(High-Level Reasoning)과 의미 지식을 제공할 수 있지만, 다음 토큰 예측(Next-Token Prediction)만으로 완전한 자율 의사결정 시스템이 구성되는 것은 아닙니다. 언어 모델을 대화형 예측기(Conversational Predictor)에서 적응형 에이전트의 구성요소로 전환하려면 지속적인 목표, 환경 상태 추적(Environmental State Tracking), 기억, 행동 인터페이스(Action Interfaces), 피드백, 검증, 안전 메커니즘이 필요합니다.

체화 인공지능(Embodied AI)에서는 물리적 행동이 되돌릴 수 없는 결과를 만들 수 있기 때문에 이러한 구분이 특히 중요합니다. 로봇은 생성된 모든 행동 제안을 실행 가능한 것으로 취급할 수 없습니다. 후보 행동은 기하학적 실행 가능성(Geometric Feasibility), 동역학(Dynamics), 하드웨어 한계(Hardware Limits), 충돌 위험(Collision Risk), 인간 안전(Human Safety), 에너지 가용성(Energy Availability), 환경 불확실성을 기준으로 검증되어야 합니다. 따라서 인지적 추론은 하위 수준의 지각, 계획, 제어 시스템과 연결되어야 합니다.

계층적 제어(Hierarchical Control)는 이러한 능력을 통합하기 위한 효과적인 아키텍처를 제공합니다. 상위 수준 에이전트는 목표를 해석하고 작업을 선택하며, 중간 수준 시스템은 계획을 생성하고 재사용 가능한 기술을 선택하고, 하위 수준 제어기(Lower-Level Controllers)는 궤적을 실행하고 물리적 행동을 안정화할 수 있습니다. 하위 수준의 피드백이 상위 수준의 가정을 무효화하면 계획이나 임무 목표 자체를 다시 검토해야 할 수도 있습니다.

뇌의 의사결정 시스템 역시 매우 병렬적(Parallel)입니다. 지각, 기억 검색, 가치 평가, 운동 준비(Motor Preparation), 모니터링은 하나의 엄격한 순차 알고리즘으로만 수행되는 것이 아니라 동시에 진행될 수 있습니다. 인공지능 에이전트 아키텍처도 이러한 모듈성(Modularity)의 이점을 활용하여 전문화된 프로세스들이 병렬로 작동하고 조정 메커니즘이 그 결과를 일관된 행동으로 통합하도록 할 수 있습니다.

다중 에이전트 상호작용(Multi-Agent Interaction)은 의사결정 문제를 더욱 확장합니다. 인간은 다른 사람의 목표, 의도(Intentions), 지식, 예상 행동을 추론합니다. 인간이나 다른 로봇과 함께 작동하는 인공지능 에이전트 역시 상호작용을 예측하고, 의도를 전달하고, 공유 자원을 조정하며, 작업을 협력하고, 다른 에이전트가 예상과 다르게 행동하면 계획을 수정해야 합니다. 따라서 의사결정은 순수하게 개인적인 문제가 아니라 관계적(Relational) 문제가 됩니다.

사회적 의사결정 시스템(Social Decision Systems)은 즉각적인 개인 보상을 넘어서는 가치도 필요로 합니다. 협력(Cooperation), 신뢰(Trust), 공정성(Fairness), 예측 가능성(Predictability), 안전, 공유 목표(Shared Objectives)는 어떤 행동이 허용 가능한지에 영향을 줄 수 있습니다. 인간 호환 인공지능 에이전트(Human-Compatible AI Agents)는 좁은 작업 성능이나 단기 보상만 최적화하는 것이 아니라 다른 사람과 관련된 제약과 선호를 표현하는 메커니즘을 필요로 합니다.

학습은 반복적인 상호작용을 통해 전체 아키텍처가 향상되도록 합니다. 성공적인 의사결정은 재사용 가능한 정책을 강화하고, 예상하지 못한 결과는 월드 모델을 갱신하며, 중요한 사건은 기억에 저장되고, 반복적으로 사용되는 계획 해결책은 절차화된 기술(Proceduralized Skills)로 발전할 수 있습니다. 따라서 의사결정 시스템은 현재 행동만 변경하는 것이 아니라 미래 의사결정을 결정하는 내부 구조 자체를 변화시킵니다.

재생(Replay)과 공고화(Consolidation)는 경험을 지속적인 의사결정 능력으로 더욱 발전시킬 수 있습니다. 중요한 궤적을 실행 이후 다시 처리함으로써 모든 물리적 사건을 반복하지 않고도 가치 추정, 예측 모델, 정책을 개선할 수 있습니다. 드물게 발생하는 실패에는 추가적인 학습 중요도를 부여하고, 성공적인 전략은 미래 상황에서 사용할 수 있는 효율적인 절차로 점차 변화시킬 수 있습니다.

따라서 통합된 인공지능 에이전트(Integrated AI Agent)는 지속적인 인지 제어 순환(Cognitive Control Loop)으로 설명할 수 있습니다. 지각은 세계를 추정하고, 주의는 관련 정보에 우선순위를 부여하며, 기억은 이전 지식을 제공하고, 월드 모델은 가능한 미래를 예측하며, 가치 메커니즘은 대안을 평가하고, 계획은 행동을 조직하며, 정책은 효율적인 기술을 제공하고, 모니터링은 실행이 목표와 안전 제약에 계속 부합하는지를 판단합니다.

하나의 뇌 영역이 현대 인공지능의 특정 모듈과 직접적으로 일대일 대응하는 것은 아니며, 어떤 인공지능 아키텍처도 뇌를 문자 그대로 디지털 복제(Digital Copy)한 것으로 해석해서는 안 됩니다. 유용한 비교는 계산 기능(Computational Functions)과 시스템 조직(System Organization)의 수준에서 이루어집니다. 생물학적 지능은 전문화된 과정들이 어떻게 역동적으로 협력할 수 있는지를 보여주며, 인공지능 공학(AI Engineering)은 관련 기능을 소프트웨어와 기계에서 구현하기 위한 다른 메커니즘을 제공합니다.

이러한 비교는 순수한 순방향 지능(Feedforward Intelligence)의 중요한 한계도 보여줍니다. 단순히 입력을 출력으로 매핑하는 시스템은 목표를 지속적으로 유지하거나, 가정을 다시 검토하거나, 관련 경험을 검색하거나, 대안을 시뮬레이션하거나, 자신의 불확실성을 감지하거나, 피드백에 따라 계획을 적응시키기 어렵습니다. 에이전트형 지능(Agentic Intelligence)은 상태 추정(State Estimation), 기억, 평가, 예측, 행동, 학습 사이의 순환적 상호작용을 필요로 합니다.

피지컬 AI(Physical AI)에서는 이러한 원리들이 물리적 현실에 기반을 두면서 지속적으로 지각하고, 기억하고, 예측하고, 결정하고, 행동하고, 학습해야 하는 자율 시스템(Autonomous Systems)으로 수렴합니다. 뇌에서 영감을 받은 기능적 조직(Brain-Inspired Functional Organization)은 강건한 자율성(Robust Autonomy)이 하나의 거대한 단일 알고리즘에서 발생하기보다는 서로 다른 시간 척도(Timescales)와 추상화 수준에서 작동하는 여러 하위 시스템의 조정을 통해 형성될 가능성이 높다는 점을 보여줍니다.

궁극적으로 인공지능 에이전트와 뇌의 의사결정 시스템은 동일한 광범위한 원리를 보여줍니다. 적응적 행동(Adaptive Behavior)은 단순히 자극에 대한 답을 생성하는 것 이상을 요구합니다. 지능형 시스템은 목표를 유지하고, 기억과 현재 증거를 통합하며, 불확실성과 가치를 평가하고, 결과를 예상하며, 행동을 선택하고 실행하고, 그 효과를 관찰하며, 경험을 활용하여 미래의 의사결정을 지속적으로 개선할 수 있어야 합니다.
