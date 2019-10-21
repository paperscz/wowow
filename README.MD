# wowow
一个给你的javascript项目快速集成ESlint, prettier, lint-staged,commitlint([Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0-beta.2/#why-use-conventional-commits))的命令行工具。

## installation
```bash
yarn add wowow -g
# or
npm install wowow -g
```
## usage
只需要在你的项目下面执行以下命令
```bash
wowow
```
然后就可以轻松愉快地写代码了，wowow...


## why
在javascript项目中，
* 使用ESlint可以帮助我们减少语法错误
* prettier可以让我们在合作开发中统一代码风格
* lint-staged可以在每一次git 提交的时候都自动使用ESlint和prettier
* commitlint可以规范我们的提交，让commit message更易读和管理

**推荐在每一个javascript项目中集成上述的工具。**

但是在一个新项目中要集成上述的特性，难免繁琐。

不仅需要在命令行中手动打出大量安装包的名字，还要一个一个配置工具的rc，ignore文件。
最关键的是因为这些工具的配置频率不是很频繁，我们不一定时刻记得我们应该安装什么，ESlint和prettier一起使用应该怎么办，commitlint的husky命令应该怎么写。这时候我们又要在网上搜索一番，就会很浪费时间，即便我们前不久就已经这么做过了。
我们应该专注于代码上面，而不是将起始的热情精力花费在这些重复工作上。

所以这个工具提供了一个简单的命令让我们的项目轻松集成这些令人愉悦的功能。

## advanced
```bash
# 安装全部特性
wowow
# 只安装eslint，prettier, lint-statge
wowow eslint
# 只安装commitlint
wowow commitlint
```