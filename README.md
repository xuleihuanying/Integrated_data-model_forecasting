
本文综述了时空预测方法、不确定性、数据-模型耦合以及时空预测未来方向的一些内容。


时空预测问题是指对未知系统状态在时间和空间上的预测。时空预测被广泛应用于现实世界的众多应用中，如天气预测、交通流预测、地震预测等等。时空预测的区域不仅限于地理空间，还可以是社会空间和虚拟空间。相比传统的时间序列预测和空间插值，时空预测在空间和时间维度上对时空依赖关系进行建模并开展预测。现有的时空预测方法可以分为三种类型（图1）：时空统计、人工智能和物理模型。
![image](https://user-images.githubusercontent.com/16514945/218958596-17a6737c-f3f6-4fbc-9c43-3de0b3ba5561.png)

图1 时空预测方法分类

时空统计基于统计理论（如概率论）进行预测，例如地理加权回归、时空自回归综合移动平均、时空克里金和贝叶斯最大熵。人工智能方法，如机器学习和深度学习，可以从数据驱动的角度对时空依赖性进行建模。人工智能模型在天气预报、交通预测、视频预测等方面具有良好的预测性能。物理模型基于物理机制，可以合理地解释预测结果，尽管当前物理模型的预测精度可能在一些实例中差于统计机器学习方法。人工智能和物理模型可以结合起来，利用各自的优势来提高模拟和预测的准确性。目前三种模型广泛应用于时空预测问题，时空预测的精度取决于预测问题、方法、预测时间和参数。在厄尔尼诺/南方涛动预测问题中，人工智能模型在时序长期记忆建模方面比当前的物理模型具有一定优势。在降水临近预报中，空间卷积和长短记忆网络的集成优于传统的数值光流方法。然而，人工智能模型在学习数据集内不可预测的噪声时，可能会出现过度拟合并削弱泛化能力。

时空预测不确定性包括数据（偶然）和模型（认知）不确定性。数据不确定性是指由于观测手段和处理算法的局限性，使得数据中存在系统误差、偶然误差、粗差及未知误差。模型不确定性是指预测方法或模型难以完全模拟现实世界的系统动态。数据不确定性通常是通过一个概率分布进行建模，模型不确定性通常基于贝叶斯定理来估计参数的后验分布（图2）。
![image](https://user-images.githubusercontent.com/16514945/218958884-19ce0399-52cc-4e5f-b41a-73d597cb8237.png)

图2 不确定性建模方法

可预测性一般是指一个变量在理论上的预测能力。通常有两种量化可预测性的方法（图 3）：分析型可预测性和试验型可预测性。分析型可预测性是通过诊断的方法来分析理论上的可预测性，如潜在可预测性，是理论上的潜在预测能力。试验型可预测性是指通过试验测量得到的可预测性。例如，使用数值模型分析降水可预测性。试验型可预测性取决于模型模拟真实物理过程的能力。可预测性随时间而变化，例如，在气候变化的背景下，降雨的可预测性随之变化。随着模型结构和参数化方案的不断发展，变量的试验型可预测性可能会进一步提高。

![image](https://user-images.githubusercontent.com/16514945/218958924-d3199a06-c711-4992-8e6d-6a098b58a80f.png)

图3 可预测性相关理论

物理模型和人工智能模型可以进行集成，以提高物理过程理解和时空预测的准确性（图4）。例如，复杂的物理模型在计算上需要校准参数，而人工智能模型可以实现快速参数校准、灵敏度分析和区间估计。人工智能模型可以通过模型-观测的映射和降尺度得到更精细的物理模型结果。物理模型中的参数化方案可以被使用人工智能模型代替，以相对简单的模型结构加速计算。人工智能模型可以通过加入一些限制，来生成富含物理意义的中间和最终结果。

![image](https://user-images.githubusercontent.com/16514945/218958997-e0ffec3b-a466-4ad8-b045-d961935ca201.png)

图4 物理和人工智能模型的耦合

随着人工智能技术的发展，现代社会的时空预测系统越来越智能化。智能时空预测系统应能够实时自动收集用于模型训练的各种数据集、知识和规则（图5），可以自动从已知数据中学习，具有灵活的模型结构和即时训练能力，能够实时或接近实时地作出预测。时空预测服务应该是用户友好的，以智能方式提供预测信息。从用户的角度来看，智能时空预测系统可以为用户提供确定性、概率性、演绎性和结论性的信息，最终服务于决策支持。

![image](https://user-images.githubusercontent.com/16514945/218959046-7771884f-4737-4f12-90b6-d4bad7e91582.png)

图5 智能时空预测系统展望

论文信息：
Xu, L., Chen, N., Chen, Z., Zhang C., Yu H. (2021). Spatiotemporal forecasting in earth system science: Methods, uncertainties, predictability and future directions. Earth-Science Reviews, 103828. doi: 10.1016/j.earscirev.2021.103828
