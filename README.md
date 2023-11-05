# 你可能不知道的 TypeScript

## 前言

欢迎你，体操家！本文将从实用角度出发，介绍 TypeScript 中的许多可能不为人所知的理论和特性，希望能够通过这种方式尽可能地抹平我们关于 TypeScript 的一些进阶知识和技巧的信息差，并启发我们使用 TypeScript 解决生产实践中的一些看似无法解决的类型问题。

本文不是所谓的「类型体操」指南。在介绍各种内容时，我会侧重于揭露它的生产价值。我不会涉及很多理论价值高于生产价值的高级技巧，例如使用类型系统写一个正则表达式的 Parser，或者是写一个五子棋游戏。

本文欢迎各位读者共同建设。如果你发现了表述不正确的地方，或者有一些好的 good idea，欢迎发表 issue！

> 作者的博客上面还有很多好康的文章哦，虽然现在不怎么更新了：https://zqy.io

## 参考资料

本文的内容部分参考了下面的文章或书籍，没有它们的作者们的贡献就没有这篇文章。

- [Handbook - The TypeScript Handbook](https://www.typescriptlang.org/docs/handbook/intro.html)
- [The type hierarchy tree](https://www.zhenghao.io/posts/type-hierarchy-tree)
- [https://twitter.com/mattpocockuk](https://twitter.com/mattpocockuk)
- [Transform Any Union in TypeScript with the IIMT](https://www.totaltypescript.com/immediately-indexed-mapped-type)
- Effective TypeScript by Dan Vanderkam

## TODO

本文章编写过程较为仓促，我还有一些想写进来的话题：

- 更多的生产实践
- Optional Variance Annotations 以及函数参数的双向协变
- 聊聊对象类型
  - `type` 和 `interface` 关键字的区别，包括隐式的 [index] 声明（忘记这个叫啥了）
  - `const` 声明的对象字面量不允许 upcast
