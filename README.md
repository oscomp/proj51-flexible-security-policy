# proj51-Flexible-Security-Policy
### 项目名称
灵活的安全策略

### 项目描述

一个操作系统中集成了大量应用，用户还可以再安装其他第三方应用软件。这些应用来源不同，质量各异，且可能存在各种各样的漏洞(比如，虚拟机或者容器的溢出就是难以容忍的漏洞)，很难保证其行为总是符合用户预期。

然而，对于大多数软件，一旦开发完成，其行为就相对固定，虽然用户不了解其源码，但用户却很了解自己的意图以及自己不想做的事情。基于此，用户可以为应用软件规定可以允许的行为以及必须严格禁止的行为，以此来约束这个软件的行为，这种约束就成为针对这个软件的安全策略。特别地，如果这个安全策略由系统的安全管理员来定义，则显得更有普遍意义（这就成为了一种强制安全策略）。

请开发一种小型的、灵活的针对可执行文件的强制访问控制策略(支持对文件的访问控制、对网络的访问)，并基于开源的openEuler系统或类似操作系统上实现支持这种策略的机制。

### 所属赛道

2021全国大学生操作系统比赛的“OS功能设计”赛道



### 参赛要求

- 以小组为单位参赛，最多三人一个小组，且小组成员是来自同一所高校的本科生（2021年春季学期或之后本科毕业的大一~大四的学生）
- 如学生参加了多个项目，参赛学生选择一个自己参加的项目参与评奖
- 请遵循“2021全国大学生操作系统比赛”的章程和技术方案要求



### 项目导师

卢华歆

* email luhuaxin1@huawei.com



### 难度

较难



### 特征

* 可实现对文件和目录读、写、执行、改名、查询元数据的控制；
* 可实现对网络资源和网络协议的管控；
* 可执行文件的安全策略可以与可执行文件分离保存，也可捆绑保存，取决于使用的文件系统或其它相关因素；
* 安全策略本身应该默认受到该机制的保护；
* 自定义安全策略的语法；
* 可以假设系统管理员及各类用户本身都不受此类安全策略的限制，即只基于应用程序本身进行控制；



### 文档

无

### License

Mulan PSL v1



## 预期目标

### 注意：下面的内容是建议内容，不要求必须全部完成。选择本项目的同学也可与导师联系，提出自己的新想法，如导师认可，可加入预期目标

* 基本目标：自定义策略语法（可支持被允许行为和被禁止行为的白名单），并（在操作系统内核中）实现对策略的支持；

* 扩展目标：针对典型应用（如apache），制定完整的安全策略进行保护；

