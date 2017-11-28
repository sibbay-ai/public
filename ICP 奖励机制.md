# ICP 奖励机制

## 1、原则

## 2、参与者

### 2.1、合格参与者

- 个人，不得是组织、团队
- 赞同小白众和的理念和价值观，并愿为小白的事业做出贡献
- github 账号创建时间超过 6 个月

### 2.2、角色

#### 2.2.1、Contributor

熟悉Sibbay的流程

- issue
- commit
- review
- pull request

#### 2.2.2、Committer

- 有 Contributor 的所有权利
- push
- merge
- 工作量核定
- 提名活跃 Contributor 升级为 Committer

## 3、奖励机制

小白会对 pr, review 和 bug 付费。

### 3.1、pull request

合格 pr：按照规范以 pr 形式提交的，经过 committer 进行 merged，这成为合格 pr
成立条件：以 pr 形式提交的，经过 committer 进行 merged，这成为合格 pr
工作量计算：累计 fix 和 for 的 issue 工作量值

### 3.2、review

成立条件：合格 pr 的 review
工作量计算：review 者在 comment 的给出工作量评估，由 committer 在确定后在 pr 上打上 size label

### 3.3、bug

成立条件：合格 pr fix 的 bug
工作量计算：固定 size: 0.1D

### 3.4、issue

小白为：需求实现、fix bug 和文档付费。
说明：运维建议可以采用运维日志的文档更新的方式进行 pr

## 4、评价机制

小白有两个评价指数：贡献指数(CI)和效率指数(EI)
具体指数小白会每周进行一次更新，并公开发布。

### 4.1、贡献指数（Contribute Index）

是 contributor 和 committer 的累计贡献评价值
核心要素：工作量，点赞/点踩 
这是未来小白进行 IPO 或者 ICO 时给予奖励的唯一指标；
具体计算方式采取开源：每半年 review 一次，新的算法不修改以前的结果（欢迎大家给出建议）

### 4.2、效率指数（Efficiency Index)

是 contributor 和 committer 的在单位工作时间效率的评估，这是一个仅仅具有比较意义的指标
核心要素：单位时间下代码或 review comment 的数量
具体计算方式采取开源：每半年 review 一次（欢迎大家给出建议）

## 5、淘汰机制

有两种淘汰依据：

### 5.1、EI值

- 连续 3 月 EI 排在倒数 5%（不足一人则以一人计）的账号半年内不得进行奖励统计

### 5.2、违反诚信原则

小白相信每个参与小白项目的同学都会坚守诚信的原则，但是如果出现一下行为：

- 违反小白的版权管理规定
- 数据保密规定
- 工作量造假

一经查实，小白停止其贡献资格，并减少甚至取消其 CI 值。