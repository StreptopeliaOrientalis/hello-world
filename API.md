# Application Programming Interface

来源：CSDN

> Application Programming Interface
>
> [APIs are] a set of subroutine definitions, protocols, and tools for building application software. In general terms, it’s a set of clearly defined methods of communication between various software components.

## 1 假设你有一个银行

银行:| 仓库 | 记账本 | 顾客

你有一个仓库来存钱，一个记账本来记各种业务。一个简单的管理银行的方法是直接将权限给所有人，让客户自己动手完成各种业务。

这种模式下，一个客户想要存钱的话，他需要：

1. 拿着钱去银行
2. 打开仓库把钱放进去
3. 把这笔业务写到记帐本上
4. 离开银行

显然这存在着问题：

1. 想开开仓库门需要废很大力气，并不是所有的人都能打开，还有些人不识字不会记账。
2. 在这个模式下，我们假定所有人都是诚实的，显然这并不成立。（说不定哪一个人存了100块钱记账的时候写了10000块）。

这时你遇到麻烦了。

## 2 雇一个柜员

要是我们雇一个体格棒、办事还麻利的人来处理开仓库，记账的问题呢？ 

小娜登场了。

现在模式为：建一个柜台将仓库和记账本和顾客分开，这样顾客就不需要再去管仓库和记账本了。想存钱的话直接找小娜就行。

银行: 仓库 | 记账本 | 顾客 | 小娜 | 柜台

这种模式下，要是有人想存钱，他们必须：

1. 拿钱去银行
2. 告诉小娜我是 MMM 我想要存￥￥￥。
3. 小娜打开仓库把钱放进去
4. 小娜把业务（transaction ）记录好
5. 告诉你业务办好了
6. 顾客离开银行

现在不会发生打不开仓库门或者是记错账的情况了，你觉得很满意。

到此我们引出今天的主角**API**（ Application Programming Interface），它能够帮你实现轻松的和其他软件组件（如服务器，操作系统等）的交互。

在上面举的例子中，我们雇一个收纳员帮顾客解决了开仓门，放钱，记账这一系列繁琐的过程。这大大节省了顾客的时间，同时提高了银行的效率。同理，如果我们将操作的具体实施步骤抽象化，这将会大大降低开发人员的负担（去记忆所有的步骤花费的力气），从而大大提高了效率。

另外的好处是，**只要他们遵循了同一个协议，组件可以交换或者是改变。**银行不需要知道时哪一个顾客或者说顾客是怎么进来的，顾客也不需要知道银行拿自己的钱去做什么了。只要负责的柜员在这里并做好工作，整个流程将会继续工作。

API 应用范围很广：从操作系统中简单的 fork() 到我们接触的百度地图API，和风天气API，又或者是邢远分享的段子，这些 API 都大大简化了程序员的工作。

## 3 银行里有什么

银行: 仓库 | 记账本 | 顾客 | 小娜 | 柜台

你可能已经注意到了银行分成了两个区域：顾客在前台排好队来办理业务，后台完成各种对钱的操作。在中间层，前台和后台发生了交互，  **双方都不能越界** ，交互只能发生在中间的区域。

在 API 术语里面，我们管中间的这块区域叫做接口 *Interface* ；在这里各个部分发生交互。在我们的银行中，前台和后台都同意并且规定**使用 Interface 来交换信息。**

现在，我们假定 Bob 想要取钱。他到了柜台找到了小娜，小娜知道该怎样去取钱，她取好了之后告诉了 Bob。

```mermaid
sequenceDiagram
    Bob->>Nana: Withdraw $500
    Nana-->>Bob: OK
```



Bob 这时候又问：“你知道今天的股票行情吗”

小娜：？？？？WTF ?

在这个例子里面，小娜知道怎样取钱和存钱 , 但是她不知道如何去给Bob查查今天的股票行情是怎样的。这个例子引出了另一个概念**协议**（Protocol）。

在 API 术语中，**协议是规定了各部分之间如何进行交流的一系列规则的集合。**各部分之间想要完成交互必须理解并且遵守同一个协议。

同时，我们注意到了交换时用的是中文。如果Bob 对小娜说「我想撳五百蚊出嚟呀唔該」，小娜不懂广东话，所以没法理解Bob说的是什么，这又引出了另一个概念**格式**（Format）

在程序员的世界里，通用的格式包含 *XML* 和  *JSON*。

最后，让我们假设银行想要扩展业务到股市，这时候就需要一位特殊的接待员来处理与股票相关的业务了，这时，小冰就登场啦。 

```mermaid
sequenceDiagram
    Bob->>Ice: Buy stocks in ACME Frozen Foods
    Ice-->>Bob: OK
```

在 API 术语里面， **API 端点** 通常是指在同一个接口中提供特定功能子集的服务提供者。在这种情况下，小冰和小娜都是端点。（**小冰和小娜是同一个柜台不同功能的提供者**）不同的端点可以有不同的协议和不同的格式。

总结起来：**接口是不同组件进行交互的地方。协议是一系列规定了他们之间怎样进行交互的规则。格式定义了他们通过什么进行交流（JSON或者是XML），端点可以在同一个接口里面提供不同的功能。**

## 4 柜员还能干什么？

到现在我们把 API 的基础知识过了一遍，接下来我们再来谈一谈 API　的其他特征。w(ﾟДﾟ)w

现在又有客户来取钱了，他想要取￥10000。 

首先，我们可以指示小娜在操作前先去确认一下 Bob 是否真的有这么多钱。（**API 能确认所有的操作都是合法的。**）

小娜查到 Bob 账户里只有一百块了，告诉 Bob 余额不足。（**在发生错误的时候 API 会根据错误报告机制发出指示，减轻开发人员的负担。**）

Bob 认为肯定是哪里出错了，他要求银行给他列一张表，给出他所拥有的每个账户上的余额。结果显示一共有 200 个账户。把他们一下子全给列出来不太实际，所以小娜每次给 Bob 看十个账户，看完了之后再来十个。（**这叫做分页（pagination），可以节省带宽和服务器资源，因为你不需要一次获取数据集中的所有内容。**）

如果 Bob 只想要知道他某一个账户中的余额的话，他可以要求小娜只给她看那个的（**这称为过滤（filtering），它还有助于节省带宽和资源，并且更易于导航。**）

在检查完所有账户之后，鲍勃现在知道他的帐户中确实没有10000美元。他知道爱丽丝购买股票并获得了大量资金，于是伪装成爱丽丝并重新进入银行。他告诉莎莉：“我是爱丽丝，我想从我的账户中提取10000美元。” 小娜识破了他的骗局。（**API中内置授权和访问控制，以确保只有授权人员才能访问特定数据。**）

最后，在试图从银行拿到10000美元失败后，他想报复小娜，他进入银行并多次从账户中提取0.01美元。 （**我们可以实施速率限制来控制服务器资源的使用，以确保用户不会滥用服务。**）

API 通常都会被设计具有这些功能，它可以充当**防火墙**，在保护您的资源免受滥用的同时允许合法请求通过。

## 5 再读Wiki

**API 是用于构建应用程序软件的一组子程序定义，协议和工具。一般来说，这是一套明确定义的各种软件组件之间的通信方法。**

> Application Programming Interface
>
> [APIs are] a set of subroutine definitions, protocols, and tools for building application software. In general terms, it’s a set of clearly defined methods of communication between various software components.

现在是不是头脑里对这个概念清晰多了呢。