# Scrum 估算与规划

当我们在开发一个产品时，总要向相关方解释什么时候可以完成产品，或者在什么时间节点达成产品的某个阶段性目标。 Scrum 框架有专门的估算（Estimation）方法帮助团队掌控进度、传递信息并建立与客户之间的信任。与传统软件开发模式不同的是，Scrum 中的估算具备如下特性：

## 关注规模而非用时

传统的软件开发团队以时间为单位来估算工作量，如最常见的“人天”。这种方式的优点在于更容易向非技术人员解释开发计划，但是由于开发人员通常在客观上存在能力差异，因此对于绝对工作时间的估算往往不准，可能会影响整个迭代 / Sprint 周期的计划安排。

目前在 Scrum 实践中，更为普遍的做法是估算“故事点（Story Point）”或“规模（Effort）” 。故事点是一个产品待办事项达到完成定义所对应的相对数值，表示团队对于投入的工作量、工作的复杂度，以及可能遇到的风险或不确定性的综合考虑。这种数值没有单位，是相对的，例如产品待办事项A的故事点为1，B的故事点为2，则说明B的工作量、复杂度和风险的加成是A的两倍。一个 Sprint 待办列表所有事项的故事点之和不能超过开发团队在这个 Sprint 周期内的交付能力，这样可以帮助团队更客观地分析每个被放入当前 Sprint 的事项的交付价值与完成思路，并在 Sprint 过程中保持专注。

Scrum 团队会利用最开始的1、2个 Sprint 进行磨合，确定故事点为“1”的标准。如果团队对于故事点的概念接受起来存在困难，可以先仅考虑工作量因素，再逐渐兼顾其它因素 —— 这种情况下，团队可将水平居中的开发人员正常状态用一天能够确保完成的产品待办事项当作“故事点为1”，作为实际估算的“参照物”。

## 估算是一项团队工作

在 Scrum 的开发过程中，开发团队共同承担责任，因此 Scrum 中的估算并非由某个人说了算，而是开发团队共同参与讨论，形成共识的结果。“计划扑克”是最流行的集体估算工具，它由一组类似于斐波那契数列的卡牌组成，包括：0，0.5，1，2，3，5，8，20，40，?，∞，每张牌代表一种故事点数。通常在 Sprint 计划会上，产品负责人向开发团队逐一介绍准备放入 Sprint 待办列表的产品待办事项，并对开发团队的问题予以解答。当所有开发人员都对某个事项有充分和一致的理解时，每人按照自己的实现想法所对应的估算数值，选择卡牌，并将数字面朝下扣在桌字上。开发人员同时展示估算结果，如果选取的数值不一样，则需要轮流说明自己的思路，并安排重新估算，直到开发团队达成一致，再进行下一个事项的介绍、答疑和估算。值得再次重申的是，在这个过程中，估算一定要将满足完成定义作为 Sprint 结束时的交付标准。

由于开发团队的每名成员的专业背景和经验不同，因此尽管集体估算相对费时，却能让团队考虑问题足够全面，基于充分讨论，在开发前形成统一思路。而如果将思路差异留到开发过程中，就很难把控开发进度和质量，一旦引起返工，必将破坏团队士气。

## 估算是动态的

产品待办列表上的所有产品待办事项都需要被估算。按照优先级顺序，一部分靠前的事项被安排进当前的 Sprint ，团队在 Sprint 计划会上共同确定这些事项的估算结果；剩下的事项则在平时的产品待办列表精化活动中，由产品负责人根据过往经验对其进行相对粗略的估算，以此预估整个产品的开发周期长度或阶段性目标的时间节点。

因此就 Scrum 的整体而言，估算是一个从粗到细、从不确定到周全而明确的动态过程。当一个产品待办事项被放入新的 Sprint，就意味着必须要在 Sprint 的时限范围内满足完成定义的的全部要求，普遍的限制是不超过20个故事点或两个工作日。如果过大，则说明该事项过于“粗糙”，还不具备被放入 Sprint 的条件。这时产品负责人就需要将其拆分成颗粒度更小的若干事项，重新描述和排序。

用史诗（Epic）、特性（Feature / Theme）、用户故事\(User Story\)分别代表不同颗粒度级别的产品待办事项（以用户需求为主），是较为常见的一种实践。

* **史诗**是颗粒度最大的用户需求，通常涵盖范围较广而细节描述较少，例如某类用户在使用服务过程中经历的某短较长的流程，显然需要花费多个 Sprint 来开发和测试，才能完成最终交付。
* **特性**，是一组由某个史诗拆分出来的、具有相关性的用户故事的集合。例如史诗被拆成足够小的用户故事，其中某些用户故事在共同场景或功能区中，或构成某段子流程。利用特性分组，产品负责人可以优化 Sprint 的交付价值。
* **用户故事**，是敏捷开发中描述用户需求的最小单元，在被放入 Sprint 之前，需要符合“ [INVEST 标准](https://worktile.com/blog/scrum/Worktile-xuemj-product%20backlog) ”，即独立的（Idependent）、便于沟通的（Negotiable）、有价值的（Valuable）、可估算的（Estimable）、规模足够小的（Small）、可测试的（Testable）。

确定被放入 Sprint 的产品待办事项还要在 Sprint 计划会上被分解成具体、可执行的任务，每个任务应确保能在一天内被搞定，这样团队就可以在每日站会上同步客观的开发进度。

## 借助估算形成规划

Scrum 团队在一个 Sprint 中实际完成的产品待办事项的故事点数之和，即为团队速率（Velocity），反映着团队的交付能力。在前几个 Sprint 的执行过程中，团队需要记录每个 Sprint 的速率，从而得出平均速率。一方面，团队可以利用平均速率作为参考标准，判断接下来每个 Sprint 待办列表的容量，更合理地安排计划；另一方面，产品负责人估算出产品待办列表剩余事项的故事点总数，又知道了开发团队的平均速率，那么就可以推算出大概需要多少个 Sprint 能将产品做完，而 Sprint 的时间范围是固定的，也就很容易知道剩余开发工作所需的周期长度。在此基础上，产品负责人就可以制定出产品版本发布的整体规划。

需要强调的是，Scrum 中的估算并非对于任何一方的承诺，而是 Scrum 团队共同管理和优化工作效率的抓手。理想状态下，一个 Sprint 中实际完成的故事点数等于其计划的故事点数，也就是团队平均速率，但事实上，尤其是在实施 Scrum 的早期，很难保证两者之间没有差距。Scrum 团队需要保持良好的心态，利用 Sprint 回顾会来分析导致实际完成低于预期的原因，并讨论出融入下次 Sprint 之中的解决方案和行动计划。经过一个相互磨合、建立信任和改善工作方式的过程，团队一定能够更为有效地使用估算、计划和速率，对产品开发和交付的进展更有把握。关于 Sprint 规划的更多内容可以查看博客文章：《[敏捷开发中如何做好Sprint规划](https://worktile.com/blog/scrum/agile-sprint-planning)》。

