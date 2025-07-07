---
layout:       post
title:        "gemini-cli"
author:       "WHY"
header-style: text
catalog:      true
tags:
    - gemini
---
# Gemini CLI 部署与使用指南

Gemini CLI 是一款为开发者设计的开源命令行界面（Command Line Interface, CLI）工具，它如同一个AI代理，可以直接在终端中使用 [3]。本文将指导您如何安装和使用 Gemini CLI，并解决一些常见的安装问题。

![Gemini CLI Logo](https://storage.googleapis.com/gweb-uniblog-publish-prod/images/Gemini_CLI_Hero_Final.width-200.format-webp.webp)

## 安装 Gemini CLI

安装 Gemini CLI 的前提是你的系统中已经安装了 Node.js 和 NPM [2]。

你可以通过 NPM（Node Package Manager）在全局环境中安装 Gemini CLI。打开您的终端或命令行工具，运行以下命令：

```bash
npm install -g @google/gemini-cli
```
或  
```
npx https://github.com/google-gemini/gemini-cli
```

## 如何使用 Gemini CLI

安装成功后，就可以在终端中直接与 Gemini 模型进行交互了。Gemini CLI 作为一个强大的AI助手，可以帮助开发者提高工作效率。

你可以通过 `gemini` 命令加上您想提问或执行的指令来使用它。例如，向 Gemini 提问：

```bash
gemini "请解释一下什么是命令行界面"
```

或者让它帮助您生成代码：

```bash
gemini "用 python 写一个快速排序算法"
```

## 使用限制
只要有谷歌账号就能用，请求也基本没什么限制,除非你一分钟请求超过60次或你一天请求超过1000次。真的有人有这么大的需求吗？  
详见官方仓库<a href="https://github.com/google-gemini/gemini-cli" target="_blank">gemini-api/gemini-cli</a>