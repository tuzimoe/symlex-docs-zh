# 我应该使用 Symlex 吗?

如果您已经喜欢 Symfony 并想以更精简，更灵活的方式工作，请尝试一下。

!!! quote
    选择是生产力的敌人。 换句话说，如果你的解决方案做了所有事情，并且没有任何意见，那么它什么也解决不了。
    <br> ― *Asim Aslam*

## 优点 ##

  - 到目前为止最快的PHP框架依据 [phpbenchmarks.com](http://www.phpbenchmarks.com/en/)
  - 在许多大型商业项目中经过实战测试
  - 代码和内存占用非常小
  - 建立在经过充分记录和测试的标准组件之上
  - 设计简单，只需要理解的概念很少
  - 比许多其他框架更容易学习
  - 使用 Symlex 会产生更易于维护和可测试的代码，这对敏捷开发至关重要
  - 它已被证明非常适合快速构建微服务， CLI 和单页面应用程序
  - 它配有工作示例，这是最好的文档形式
  - 包含创建全功能 Web 应用程序的所有内容：服务容器， REST 路由和 Twig 模板引擎
  - 尽可能使用普通类来避免 vendor lock-in 并启用框架无关代码重用（其他框架通常会尝试使用专有注释和必须继承的特定基类来锁定）
  - 您可以将它与 Symfony Components 和任何其他 PHP 库一起使用
  - 即使您选择不使用 Symlex，您也可能会发现自己的项目有很多灵感（例如，您可以构建自己的框架基于 [微内核](https://github.com/symlex/di-microkernel) 或者学习如何将 JavaScript 与 PHP 集成)
  - 易于升级到 Symfony 的新版本
  - 如果您想要完全控制并且因任何原因不信任社区，您可以自由创建分支

## 缺点 ##

  - 当你在选择获取 [商业支持](https://blog.liquidbytes.net/contact/) 的时候，Symlex 没有大公司的支持，因为我们是一个小社区：开发开始为 FOSRestBundle 提供高性能替代品，我们的目标永远不是商业化。
  - 对于那些不习惯阅读至少少量框架代码的开发人员来说，这并不好，因为并非所有内容都是 100％ 记录的（欢迎您通过电子邮件寻求帮助或发送其他文档作为提交 PR ）
  - Symfony Bundles 中的 Symlex 没有提供支持
    - 使用它们通常会增加整体架构的复杂性：它们隐藏了引导程序/配置细节，并鼓励构建膨胀的应用程序
    - Symlex 旨在构建专注，精益和完全可测试的应用程序
    - 如果某些功能仅在框架配置文件中编码或由 bundle 神奇地生成，则无法编写有意义的单元测试
    - 可以创建验收测试，但它们很慢并且不适合测试驱动开发（TDD）和重构
  - 由于我们发现难以维护和测试，因此也不支持注释
    - 我们更喜欢使用一小段代码或使用服务容器来配置我们的应用程序
  - 从 Stack Overflow 或 Symfony 文档中复制和粘贴代码有时无法使用。理解它并稍微调整它，例如 在服务配置或路由方面
