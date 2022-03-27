# software-testing-cn
wikipedia 上 软件测试(中文) 和 software testing(英文) 页面内容有一些区别, 包括 目录、参考文献等.
但由于 software testing 英文wikipedia **篇幅过于巨大**, , 故只能对 software testing 的篇幅一笔带过 改天另起一文记录, 本文只是对于 中文wikipedia 的 软件测试 进行探讨.

## reference
1. wikipedia 的 软件测试 中文界面:
https://zh.wikipedia.org/wiki/%E8%BD%AF%E4%BB%B6%E6%B5%8B%E8%AF%95

2. wikipedia 的 软件测试 英文界面:
https://en.wikipedia.org/wiki/Software_testing


## difference about contents and references between cn and en 
来自于 [wikipedia 的 软件测试 中文界面](https://zh.wikipedia.org/wiki/%E8%BD%AF%E4%BB%B6%E6%B5%8B%E8%AF%95):

**tips:** 中文wikipedia 上写着: 
>**参考文献:** 郑人杰 《计算机软件测试技术》，清华大学出版社

软件测试 wikipedia 中文目录:
1. 测试的进程;
    1.1. Alpha测试
    1.2. Beta测试
        1.2.1. 封测与公测
    1.3. Gamma测试
2. 测试的方法
    2.1. 黑盒测试
    2.2. 白盒测试
3. 测试的类型
    3.1. 压力测试与性能测试
4. 测试的阶段
5. 测试用例、测试脚本和测试场景
6. 测试过程示例
    6.1.  软件测试活动
7. 代码覆盖率
8. 自动化测试
9. 参考文献
10. 参见
---

**tips:** software testing 英文wikipedia 上的 [reference条目](https://en.wikipedia.org/wiki/Software_testing#References) 则多到86条, 不一一列出.

英文wikipedia 的目录也不尽相同:

Contents:
1.	Overview
    1.1.	Faults and failures
    1.2.	Input combinations and preconditions
    1.3.	Economics
    1.4.	Roles
2.	History
3.	Testing approach
    3.1.	Static, dynamic, and passive testing
    3.2.	Exploratory approach
    3.3.	The "box" approach
        3.3.1	White-box testing
        3.3.2	Black-box testing
            3.3.2.1	Visual testing
        3.3.3	Grey-box testing
4.	Testing levels
    4.1.	Unit testing
    4.2.	Integration testing
    4.3.	System testing
    4.4.	Acceptance testing
5.	Testing types, techniques and tactics
    5.1.	Installation testing
    5.2.	Compatibility testing
    5.3.	Smoke and sanity testing
    5.4.	Regression testing
    5.5.	Acceptance testing
    5.6.	Alpha testing
    5.7.	Beta testing
    5.8.	Functional vs non-functional testing
    5.9.	Continuous testing
    5.10.	Destructive testing
    5.11.	Software performance testing
    5.12.	Usability testing
    5.13.	Accessibility testing
    5.14.	Security testing
    5.15.	Internationalization and localization
    5.16.	Development testing
    5.17.	A/B testing
    5.18.	Concurrent testing
    5.19.	Conformance testing or type testing
    5.20.	Output comparison testing
    5.21.	Property testing
    5.22.	Metamorphic testing
    5.23.	VCR testing
6.	Testing process
    6.1.	Traditional waterfall development model
    6.2.	Agile or XP development model
    6.3.	A sample testing cycle
7.	Automated testing
    7.1.	Testing tools
    7.2.	Capture and replay
8.	Measurement in software testing
    8.1.	Hierarchy of testing difficulty
9.	Testing artifacts
10.	Certifications
11.	Controversy
12.	Related processes
    12.1.	Software verification and validation
    12.2.	Software quality assurance
13.	See also
14.	References
15.	Further reading
16.	External links

关于 contents 和 references 的对比到此结束.
后面只针对 软件测试 的中文wikipedia内容.

## detail
主要针对一些重要的名词做定义和解释.

### testing approachs
**测试方法** 分为 黑盒测试 和 白盒测试.

#### black-box testing
- **黑盒测试**(black-box testing), 又名 功能测试、数据驱动测试、基于功能说明的测试.
    
    - 目的: 测试应用程序的功能, 而不是其内部结构或运作.
    - 测试者要求: 测试者不需具备应用程序的代码、内部结构和编程语言的专门知识。测试者只需知道什么是系统应该做的事，即当键入一个特定的输入，可得到一定的输出.
    - 测试案例: 测试案例是依应用系统应该做的功能，照规范、规格或要求等设计。测试者选择有效输入和无效输入来验证是否正确的输出.
    - 适用范围: 可适合大部分的软件测试，例如集成测试（integration testing）以及系统测试（system testing）.

#### white-box testing
- **白盒测试**（white-box testing，又称 透明盒测试 glass box testing、结构测试structural testing等）是一个测试软件的方法.
    
    - 目的: 测试应用程序的内部结构或运作，而不是测试应用程序的功能。
    - 测试案例: 在白盒测试时，以编程语言的角度来设计测试案例。测试者输入资料验证资料流在程序中的流动路径，并确定适当的输出，类似测试电路中的节点.
    - 适用范围: 白箱测试可以应用于单元测试（unit testing）、集成测试（integration testing）和系统的软件测试流程，可测试在集成过程中每一单元之间的路径，或者主系统跟子系统中的测试。尽管这种测试的方法可以发现许多的错误或问题，它可能无法检测未使用部分的规范.

### testing types
测试的类型 有 功能测试、系统测试、极限值测试、性能测试、压力测试. 其中, 压力测试 和 性能测试 容易混淆, 其实**有区别**.
- **功能测试**: 按照测试软件的各个功能划分进行有条理的测试，在功能测试部分要保证测试项覆盖所有功能和各种功能条件组合。
- **系统测试**: 对一个完整的软件以用户的角度来进行测试，系统测试和功能测试的区别是，系统测试利用的所有测试数据和测试的方法都要模拟成和用户的实际使用环境完全一样，测试的软件也是经过系统集成以后的完整软件系统，而不是在功能测试阶段利用的每个功能模块单独编译后生成的可执行程序。
- **极限值测试**: 对软件在各种特殊条件，特殊环境下能否正常运行和软件的性能进行测试。
特殊条件一般指的是软件规定的最大值，最小值，以及在超过最大、最小值条件下的测试。
特殊环境一般指的是软件运行的机器处于CPU高负荷，或是网络高负荷状态下的测试，根据软件的不同，特殊环境也有过不同。
- **性能测试**: 性能测试是对 软件性能 的评价。简单的说，软件性能衡量的是软件具有的响应及时度能力。因此，性能测试是采用测试手段对软件的响应及时性进行评价的一种方式。根据软件的不同类型，性能测试的侧重点也不同。

#### stress testing and peformance testing
压力测试常常和性能测试相混淆。
它们**主要不同点**是，压力测试要求进行超过规定性能指标的测试。例如一个网站设计容量是100个人同时点击，压力测试就要是采用120个同时点击的条件测试。
压力测试的通常判断准则：
1. 系统能够恢复。
2. 压力过程中不要有明显性能下降。

### tesing levels
**测试阶段/级别** 分为4个，单元测试、集成测试、系统测试、回归测试。

#### unit testing
**单元测试**是对软件组成单元进行测试，其目的是检验软件基本组成单位的正确性，测试的对象是软件设计的最小单位：函数。
并且使用假资料测试不同状况下功能使用情况，单元测试还有助于开发人员编写更好的代码。
单元测试是基于code的:可读性、可测试性，它们与开发代码的构建方式密切相关。因此开发人员最清楚哪些测试最有意义。

#### integration testing
**集成测试**集成测试也称综合测试、组装测试、联合测试，将程序模块采用适当的集成策略组装起来，对系统的接口及集成后的功能进行正确性检测的测试工作。其主要目的是检查软件单位之间的接口是否正确，集成测试的对象是已经经过单元测试的模块。

#### system testing
**系统测试**主要包括功能测试、界面测试、可靠性测试、易用性测试、性能测试。 功能测试主要针对包括功能可用性、功能实现程度（功能流程&业务流程、数据处理&业务数据处理）方面测试。

#### regression testing
回归测试(regression test)指在软件维护阶段，为了检测代码修改而引入的错误所进行的测试活动。回归测试是软件维护阶段的重要工作，有研究表明，回归测试带来的耗费占软件生命周期的1/3总费用以上。

与普通的测试不同，在回归测试过程开始的时候，测试者有一个完整的测试用例集可供使用，因此，如何根据代码的修改情况对已有测试用例集进行有效的复用是回归测试研究的重要方向，此外，回归测试的研究方向还涉及自动化工具，面向对象回归测试，测试用例优先级，回归测试用例补充生成等。

- 测试原有功能
- 测试新加入的功能是否有side effect

### code coverage
代码覆盖率原本是种白箱测试活动。目标软件通过特殊选项或者函数馆编译并且/或者在特殊环境（程序里每个函数都被映射回源代码里函数起点）下执行。这个过程允许开发员与品管员查看系统中在正常情况下极少或从未被读写的部分（例如：异常处理之类）并且帮助测试员确认最重要的情况（函数点）都被测过了。

测试员可查看代码覆盖率测试结果来设计测试个案、相对应的输入或者设置组以增加重要函数的代码覆盖率。两种测试员常用的代码覆盖率形式：语句覆盖率（或称行覆盖率）以及路径覆盖率（或称边覆盖率）。行覆盖率回报到测试完成时，执行过哪些行，或者存储器大小。边覆盖率回报到测试完成时，哪些分支，或者程序决定点被执行过。正如覆盖率的“率”字所言，这两个都以百分比为单位。

通常代码覆盖率的工具与函数馆要求的性能、存储器、或者其他资源开销不为正常的软件营运接受。因此它们通常只存在实验室里。又，你可能会想到软件里的许多类无法一一通过这些代码覆盖率测试，虽然代码覆盖程度可通过分析但不是直接测试。

有些瑕疵也会受这些工具的影响。个别来说某些竞态条件（race condition）或者类似的对即时（real time）敏感度高的操作几乎不可能在代码覆盖率测试环境下侦知；相反的这类的瑕疵只会带来更多的测试码开销。

### automated testing
测试自动化是使用软件工具和既定程序，对软件所进行的测试活动。