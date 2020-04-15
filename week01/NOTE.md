1. 怎么建立知识体系
2. 工作环境怎么给自己做职业规划


# 学习方法 0407

## 整理法

* 顺序 [编译] 词法分析、(语义分析)、语法分析、代码优化、代码生成
* 组成 [CSS规则] 选择器 属性 值
* 维度关系 [JavaScript] 文法(词法、语法) 语义 运行时(类型、执行过程)
* 分类关系 [CSS简单选择器] ID Class 通用 属性 元素 伪类 伪元素

## 追溯法 源头|标准|大师

* Closure
* MVC
* OOP

# 前端技术 知识体系整体案例

* HTML
* JavaScript
  * runtime
    * 类型
      * Undefined
      * Null
      * Boolean
      * String
      * Number
      * Symbol
      * Object
        * Prototype
        * Property
    * 执行过程
  * 文法
* CSS
* API

# 面试官怎么想

区分度
覆盖面
深度

* 打断
  * 不感兴趣
  * 提示
* 争论
  * 故意产生压力
  * 技巧
* 难题
  * 展示分析过程
  * 缩小规模

项目 / 知识 / 开放 / 案例 / 有趣

# 0409 建立知识体系

## HTML
技术实现文档
Latest published version https://www.w3.org/TR/html53/
Living Standard https://html.spec.whatwg.org/multipage/

emit
~~~
<html>
lang=en
lang=""
lang=''
abc
</html>
~~~

* HTML as 计算机语言
  * 语法
  * 词法
* HTML as SGML
  * DTD
    * https://www.w3.org/TR/html4/strict.dtd
    * https://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd
  * [Entity](https://www.w3.org/TR/xhtml1/DTD/...)
    * xhtml-lat1.ent
    * xhtml-symbol.ent
    * xhtml-special.ent
* HTML as XML
  * Namespace <html xmlns="http://www.w3.org/1999/xhtml" ></html>
    * SVG
    * MathML
    * ARIA (Accessible Rich Internet Applications)
      * https://www.w3.org/TR/html-aria/
      * https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA
  * Tag
    * https://html.spec.whatwg.org
      * 4 The elements of HTML
        * Array.prototype.map.call(, e => e.innerText).join("\n");
          * $0.querySelectorAll('code')

## JavaScript
https://www.ecma-international.org/publications/standards/Ecma-262.htm

* Grammar 语法
  * lexical 词法
  * Syntax
* Semantics 语义
* Runtime 运行时
  * Type 类型
    * Undefined
    * Null
    * Boolean
    * String
    * Number
    * Symbol
    * Object
      * Prototype
      * Property
  * 执行过程

### Grammar
#### lexical 词法
* WhiteSpace "var\uFEFFa = 1" => "vara = 1"
* LineTerminator
* Comment
* Token
  * Identifier
  * Keywords
  * Punctuator
  * NumericLiteral
  * StringLiteral
  * RegularExpressionLiteral
  * Template

#### Syntax
Lexical
Expression
Statements
Functions and Classes
Scripts and Modules

~~~
if(a<100)
  b += a++
~~~
IfStatement
  Expression
  Statement
    Expression
      =
        b
        Expression
          a++

### Semantics 与 Syntax 一一对应
### Runtime
Type
* Undefined
* Null
* Boolean
* String
* Number
* Symbol
* Object
  * Prototype
  * Property
* 内部类型
  * Reference
  * Completion Record

Job
~~~
Script / Module
Promise
Function
Statement
Expression
Literal
Identifier    
~~~

## CSS
2.1 最完整 
https://www.w3.org/TR/CSS2/
https://www.w3.org/TR/CSS22/

多少属性
多少值

* 语法/词法
* @规则
* 普通规则
  * 选择器 #id a>.cls[attr], #id2
    * 简单选择器：.class, #id, tagname, *, [attr=v]
    * 复合选择器：
    * 复杂选择器：子孙(空格)
    * 选择器列表：逗号
  * Property
  * Value
* 机制
  * 排版
  * 伪元素
  * 动画
  * 优先级

## API
* Browser
  * DOM
    * Nodes <-> HTML
    * Ranges
    * Events
  * BOM https://en.wikipedia.org/wiki/Browser_Object_Model
* Node
* Electron
* 小程序

https://www.w3.org/TR/WebCryptoAPI/

### Web Platform API
https://webplatform.github.io/
https://platform.html5.org/
https://flaviocopes.com/web-platform/
https://webplatformcourse.com/

## 作业
哪些标准对windows对象进行了扩展

# 0411 前端与工程体系
小互动 - 我眼中优秀的前端工程师

* 领域知识（上节课
* 前端知识
* 3大能力
编程 能
架构 规模大 组件化
工程 协作 工具链+持续集成

* 潜力 基于职业规划

## 怎么展示成就
I wrote Python.
我在xxx项目里担任什么角色，具体干了什么。

Who is the owner of your career ? You are the owner of your career.

### 职业发展总纲
成长 -> 成就 -> 晋升 -> 成长

学习能力很强 - 现在啥也不会，kpi 是啥？

### 业务成就
* 业务目标
  * 理解公司业务的核心目标 - 怎么挣钱
  * 目标转化为指标 - 引导成交 gmv 1流量 2转化率 3客单价
* 技术方案
  * 业务指标到技术指标的转化
  * 形成纸面方案、完成小规模实验
* 实施方案
  * 确定实施目标、参与人
  * 管理实施进度
* 结果评估
  * 数据采集、数据报表
  * 向上级汇报

* 案例：应用手势

### 技术难题
目标：公认的技术难点
方案与实施：编程+架构
结果

* 案例：爬取商品价格

### 工程型
目标：质量、效率
方案与实施：规章制度 库 工具 系统
结果：线上监控
* 案例：XSS

工程：不一定是搞个系统，可能只是规章，唯一的标准就是有效。

* 插播答疑
数组 线性表
二叉树 排序
数据结构80%的需求都是排序，大部分排序场景都可hash。分层hash，可排序hash。不可hash就是二叉树。
链表练习不实用。
wildcard 很难，正则会超时。

## 数据驱动的思考方式：一个小故事
* 目标：分析业务目标，定数据目标。
* 现状：采集数据，建立数据展示系统。 - 技术(加载时间 错误数据)
* 方案：设计技术方案，预估数据。 - 方便和其他部门配合
* 实施：小规模实验，推广全公司落地，形成制度。
* 结果：统计最终效果，汇报。

活跃度：日活/月活
页面加载时间 平均时长 - 转化率 点击率
秒开率

技术好 业务敏感度 老板赏识
加班 老板不安
核心指标高速增长时，没人让你加班

## 工具链
* 工具链(套件)的作用
* 工具的分类
  * 脚手架 init
  * 本地调试 run
    * build
  * 单元测试 test
  * 发布 publish
* 工具链体系的设计
  * 版本问题
  * 数据统计
    * 研发阶段

## 持续(最终)集成
|       | 客户端软件                    | 前端              |
| ----- | ----------------------------- | ----------------- |
| build | Daily build                   | Check-in build    |
| test  | BVT (Build Verification Test) | Lint + Rule Check |

整包 = 单张 * 4

## 技术架构
客户端架构：解决软件需求规模带来的复杂性
服务端架构：解决大量用户访问带来的复杂性
前端架构：解决大量页面需求带来的重复劳动问题 - 复用

Library 库：有复用价值的代码 utility - URL AJAX(时间戳...) ENV
Component 组件：UI 上多次出现的元素 - 轮播 Tab
Module 模块：经常被使用的业务区块 - 登陆

* 插播答疑
vue cli 工具链

AB
发布，页面_a/_b cookie(CDN)
埋点，

单测 mocha
前端之巅
https://github.com/spritejs/spritejs
JavaScript 高级程序设计
编译 - 龙书

SPA SSR

Code Review

## 作业
URL 正则