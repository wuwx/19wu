# 19wu

19wu - 卖活动票的小屋

这是一个基于 Rails3 的开源电子商务项目，主要是为了方便会议活动（e.g.RubyConfChina）网上卖票，项目上线后将完全免费。

之前做 ShopQi 时，项目功能太多，后期不少朋友想要贡献代码非常困难，新手学习门槛也高。
对于这个项目我决定推迟 2 周，将在 **12月24日** 正式开始，并持续利用业余时间进行完善，欢迎关注或加入。

### 项目特色

* 完全免费
* 支持即时到帐网上支付
* 代卖公司票（提供发票）

### 基本需求

* `主办方`发起活动，卖票，发放电子票
* `参与者`可以在线购票，退票
* 个人票、公司票的库存可以联合计算，总数在 n 以内
* 支持调价规则，如11月1日起 118 元，或者第200张开始 118 元
* 支持手机、平板、网站访问

### 扩展需求

* 参与者关注`主办方`（下次RubyConfChina办活动你将得到邮件通知）

### 技术选型

* Rails 3
* 数据库支持 PostgreSQL 和 MySQL
* 后台任务使用 delayed_job，而不使用 resque，避免对 redis 的依赖
* 前端基于 [Bootstrap](http://twitter.github.com/bootstrap) 和 [Spine.js](http://spinejs.com)

## 开发计划

开发时会针对一个个小的功能点提出 issue，提交的代码要与相应 issue 关联。

### Week #1

做出最小可用原型，不涉及支付流程等。

* 主办方用户注册、发起免费活动
* 普通用户报名参加
* 主办方用户查看参与者用户列表

域名备案通过即上线内部试用。

### Week #2

加入签到功能，先只支持二三十人左右的小型会议，不涉及电子票码生成。

* 参与者用户到达会场后，由主办方用户直接勾选签到

### Week #3

支持手机访问。

* 参与者用户查看活动时间、地点
* 参与者用户查看参与者列表（独立列表，带头像），对其他参与者有个基本了解。


以上为初步计划，待进一步讨论细化。

## 团队

### 管理团队

* [@saberma](https://github.com/saberma)
* [@lgn21st](https://github.com/lgn21st)

### 贡献者

* 持续招募中。。。
* 加入条件：无，只要你有时间参与就行

### 如何参与

* 在 [Issue](https://github.com/saberma/19wu/issues) 发起讨论
* 对提交的代码有任何疑问时发起讨论
* 开发一些功能（需要带测试，以保证此功能在后续开发时不被破坏）
* 试用已有的功能，提出建议
* 向身边的朋友介绍 19wu

## License

[GNU  Affero GPL 3](http://www.gnu.org/licenses/agpl-3.0.html)