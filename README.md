TypeScript
===

## 简介

### 什么是 TypeScript

``TypeScript`` 是 ``JavaScript`` 的类型的超集，它可以编译成纯 ``JavaScript``。编译出来的``JavaScript`` 可以运行在任何浏览器上。``TypeScript`` 编译工具可以运行在任何服务器和任何系统上。``TypeScript`` 是开源的。

### 为什么选择 TypeScript

TypeScript 官网列举了一些优势，不过我更愿意自己总结一下：

#### TypeScript 增加了代码的可读性和可维护性

类型系统实际上是最好的文档，大部分的函数看看类型的定义就可以知道如何使用了
可以在编译阶段就发现大部分错误，这总比在运行时候出错好
增强了编辑器和 IDE 的功能，包括代码补全、接口提示、跳转到定义、重构等

### TypeScript 非常包容

TypeScript 是 JavaScript 的超集，.js 文件可以直接重命名为 .ts 即可
即使不显式的定义类型，也能够自动做出类型推论
可以定义从简单到复杂的几乎一切类型
即使 TypeScript 编译报错，也可以生成 JavaScript 文件
兼容第三方库，即使第三方库不是用 TypeScript 写的，也可以编写单独的类型文件供 TypeScript 读取

### TypeScript 的缺点

任何事物都是有两面性的，我认为 TypeScript 的弊端在于：
- 有一定的学习成本，需要理解接口（Interfaces）、泛型（Generics）、类（Classes）、枚举类型（Enums）等前端工程师可能不是很熟悉的概念
- 短期可能会增加一些开发成本，毕竟要多写一些类型的定义，不过对于一个需要长期维护的项目，TypeScript 能够减少其维护成本
- 集成到构建流程需要一些工作量
- 可能和一些库结合的不是很完美

## 安装

TypeScript 的命令行工具安装方法如下：
```sh
npm install -g typescript
```
以上命令会在全局环境下安装 tsc 命令，安装完成之后，我们就可以在任何地方执行 tsc 命令了。
编译一个 TypeScript 文件很简单：
```
tsc hello.ts
```
我们约定使用 TypeScript 编写的文件以 .ts 为后缀，用 TypeScript 编写 React 时，以 .tsx 为后缀。

## 编辑器

TypeScript 最大的优势便是增强了编辑器和 IDE 的功能，包括代码补全、接口提示、跳转到定义、重构等。
主流的编辑器都支持 TypeScript，这里我推荐使用 Visual Studio Code。

它是一款开源，跨终端的轻量级编辑器，内置了 TypeScript 支持。
另外它本身也是用 TypeScript 编写的。
下载安装：[https://code.visualstudio.com/](https://code.visualstudio.com/)
获取其他编辑器或 IDE 对 TypeScript 的支持：

- Sublime Text
- Atom
- WebStorm
- Vim
- Eclipse
- Visual Studio 2013及以上版本