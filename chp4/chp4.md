第四章 跟着数据走
========================================================
#### 侦探这行有句谚语“跟着钱走。”在数据科学，成功的一个关键是“跟着数据走。”在多数情形，一个数据科学家不会去从无到有的设计一个信息系统。反而，在一些或者许多已有的系统中，就有数据；数据科学家面临的很大一部分挑战就是如何整合这些系统。


我讨厌唠叨，但是你最近做过体检吗？如果你去看过医生，不管是为什么原因，你可能会记得医生的办公室被数据湮没了。首先，医生有大量的数字传感器，从血压监测器到超声波机器应有尽有，所有这些都会产生大量的数据。也许，对于现在引起广泛关注的关于健康保险的争论，金融和保险数据的一个很重要的出发点就可以是医生的办公室。美国医疗保健体系有一个著名的“特点”，就是我们的医疗保健服务的普遍做法是：按照流程付钱。当你在医生的办公室经历一次“流程”时，不管是一次咨询，一次检查，一次化验，或者其它什么，这是一系列会产生深远结果的数据事件的开端。

如果你的医生是典型的医生，这些事件的起点是一张纸质的表格。你曾经详细的看过它们吗？这些表格上多半填的是由流程和代码组成的矩阵。虽然许多设备先进的地方可能会用平板电脑或者其它电脑将这些表格数字化，但是纸质表格仍然是普遍存在的。如果要进行保单赔付或者付款，纸质表格的数据会被输进一个系统，这个过程会在医生办公室或者在一个外包公司里进行。

这些流程数据去哪儿了呢？哪些其它种类的数据（比如病人账号信息）可以在接下来的流程中和它们连接？这些连在一起的数据形成了什么样的网络？或者它们的安全性如何？在这些数据到达保险公司之前，处理数据要多少步骤？保险公司在考虑理赔之前是怎样处理和分析数据的？当保险公司的系统同意理赔之后钱是怎么转账的？这些问题仅仅是从表面上考虑的：还有几十种上百种处理步骤我们连想都想不到。

我们很容易从这个例子中看到，根本不可能把已有的系统扔掉，然后去设计一个更好的或者至少更标准化的系统。但是如果你的工作是提高系统的效率，或者审查保险理赔以确保它们和保险记录相符，或者使用数据去探测和预测疾病的爆发和流行，或者给顾客提供反馈告诉他们一些流程的期望花费是多少，那么你该怎么办呢？

你的项目的关键的出发点在于要跟着数据走。你应该像一个侦探一样，充分的弄清楚细节，包括内容，格式，发送人，接收人，转账方法，仓库，还有过程中每一步数据的使用者以及进行数据处理和存储的组织。

幸运的是，已经有一个广泛的研究和实践领域叫做“数据模型”，它给出理论，策略和工具以帮助实现数据科学家“跟着数据走”的目标。这些想法开始于70年代早期，是由计算机科学家Ed Yourdon提出的称之为数据流程图方法。一个更现代的方法叫做实体关系模型，它和建立关系型数据库的方法有很强的关系。专家们使用这个模型发明了实体关系图（ERDs）来描述一个系统的结构和数据的移动。

实体关系模型在不同层面出现，从抽象概念侧面到实际存储层面。在概念层面一个实体是一个对象或者东西，通常是真实世界中存在的东西。在医生办公室的例子中，一个重要的“对象”是病人。另一个实体是医生。病人和医生通过一个关系相连：在现代医疗保健术语中这是“供应”关系。如果病人是X先生，医生是Y医生，供应关系提供一个双向的连接：

- Y医生是X先生的提供者
- X先生的提供者是Y医生

自然的，有一些数据可以描述X先生：名字，地址，年龄，等等。同样的，也有描述Y医生的数据：医龄，专业领域，资质证书，执照。重要的是，有一大块数据用来描述X和Y的联系，这就是关系。

建立一个ERD需要调查和枚举所有的实体，比如病人和医生，还有它们之间可能存在的所有的关系。就像本章的开始提到的，这可能发生在许多组织上（比如，医生办公室和保险公司），这取决于信息系统被设计出来的目标。最终，ERDs必须足够详细，这样它们才能被用作一个数据库的物理存储的说明书。

在医疗保健这样的应用领域中，如何设计数据有太多不同的选择了，以至于建立一个好用的系统要求一些经验和一些“艺术”。“艺术”一部分体现在理解用户的现有信息需求以及这些需求在未来预期的变化。如果一个组织在重新设计一个系统，补充一个系统，或者设计新系统，他们这样做是为了未来的利益。这个利益可能是更高的效益，错误/不精确的减少，或者增强的信息能力带来的做出新产品或新服务的可能性。

不管目标是什么，数据科学家现在在方法上面临重要且困难的挑战，包括纸质表格和手工数据录入，想象一下将来的方法。跟着数据走！

在下一章，我们介绍组织数据的最普遍也是最有用的方法，叫做矩形结构，它包含行和列。这种把数据布置成矩形的做法出现在电子表格和数据库，被很多应用所使用。理解这些行和列如何组织的，这是数据科学中多数任务的关键。

#### 参考资料

[http://en.wikipedia.org/wiki/Data_modeling](http://en.wikipedia.org/wiki/Data_modeling )

[http://en.wikipedia.org/wiki/Entity-relationship_diagram](http://en.wikipedia.org/wiki/Entity-relationship_diagram)