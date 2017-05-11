- 术语：A/B测试
- 印象：为同一个目标制定两个方案，让一部分用户使用A方案，另一个用户使用B方案，记录下使用情况，看哪个方案更符合设计目标。
    - 核心思想：
        1. 多个方案并行测试。
        2. **每个方案只有一个变量不同** 。A/B测试应用范围必须是单变量，因为多变量之间会相互干扰，很难通过A/B测试Z找出各个变量对结果的影响。
        3. 以某种规则优胜略汰。
    - AB测试示意图：
       ![AB测试示意图](https://raw.githubusercontent.com/dragon86yq/photo/master/AB%E6%B5%8B%E8%AF%95%E7%A4%BA%E6%84%8F%E5%9B%BE.png)
    - A/B测试需要完成的工作：
        1. 开发两个（或多个）不同的版本并部署；
        2. 收集数据；
        3. 分析数据，得出结果。
    - AB测试部署概念图：
        ![AB测试部署概念图](https://raw.githubusercontent.com/dragon86yq/photo/master/ABtest%E9%83%A8%E7%BD%B2%E6%A6%82%E5%BF%B5%E5%9B%BE.png)
        - 上图是AB测试实现的原理。
          - 从左到右分别代表AB测试中的四个关键角色：客户端(Client)、服务器(Server)、数据层(Data)、数据仓库(Data-Warehouse)。
          - 从上到下代表三种测试形式：无A/B测试的普通访问流程(No-AB-test)、基于后端的A/B测试访问流程(Back-end AB test)、基于前端的A/B测试访问流程(Front-end AB test)
- 出处：[A/B测试：基本概念](https://blog.oldj.net/2010/07/27/ab-testing-basic-concept/)、[A/B测试：实现方法](https://blog.oldj.net/2010/07/29/ab-testing-method/)