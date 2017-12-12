# icp  奖励机制

## 1、原则

鼓励参与、奖励贡献、淘汰落后。

## 2、参与者

### 2.1、合格参与者

- 个人，不得是组织、团队；
- 赞同小白众和的理念和价值观，并愿为小白的事业做贡献；
- github 账号创建时间超过 6 个月；
- 通过认证流程，见[《贡献者认证流程》](贡献者认证流程.md)

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

#### 2.2.3、Maintainer

- 有Committer的所有权利
- 提名活跃 Committer 升级为 Maintainer

有任何问题可联系： [《通讯录》](通讯录.md)

## 3、奖励机制

小白会对 pr, review 和 bug 付费。

### 3.1、pull request

**合格 pr**：按照规范以 pr 形式提交的，经过 committer 进行 merged，这成为合格 pr  
**成立条件**：以 pr 形式提交的，经过 committer 进行 merged，这成为合格 pr  
**工作量计算**：累计 issue 的size标签

### 3.2、review

**成立条件**：

- 合格 pr 的 review
- 有size标签

**工作量计算**：review 者在 comment 的给出工作量评估，由 committer 在确定后在 pr 上打上 size label

### 3.3、报告 bug

**成立条件**：

- 报告 bug, 并且报告复现方法（以测试代码的方式，或操作描述的方式）
- 此 bug 通过正确的 pull request 得到 fix.
- 若复现条件苛刻，bug 报告者需在开发者进行验收测试时提供必要帮助；
- 由 committer 打上 ICP 的标签

**工作量计算**：固定 size: 0.1D  
**说明**：对于在开发调试期的 bug 不在奖励范畴，尺度由 committer 掌握

### 3.4、issue

**成立条件**：

- 按照规范提交 issue
- 有 size 标签

**说明**：运维建议可以采用运维日志的文档更新的方式进行 pr

## 4、申请与确认

### 4.1、申请方式

committer 会以 issue 的形式发放任务，凡是有 **ICP** 且无 **In Progress** 标签的 issue ，合格参与者均有权申请；  
非指定人员的 ICP issue 会统一放到 public repo 的 issue 中；  
申请者直接在该 issue 上提交留言：**"@committer 申请开发 Size：xx Deadline：2017-12-5"**  
注： 关于deadline，小白的原则是你可以给自己留余量，但不能超期。 

### 4.2、贡献者确认

任务由 committer 指定 contributor，并在 issue 上留言说明并标记 **In Progress** 的标签  

**确认原则**：

- 技术能力
- 工作量
- 历史CI（贡献指数）

参与者如果认为指定方式需要改善，均可向 Maintainer 写issue；

### 4.3、终止

当时间超过 deadline 一个 size（以工作日计），committer 有权终止该参与者，将 issue 标记为"**异常终止**"并关闭；


## 5、评价机制

小白有两个评价指数：贡献指数(CI)和效率指数(EI)
具体指数小白会每周进行一次更新，并公开发布。

### 5.1、贡献指数（Contribute Index）

是 contributor 和 committer 的累计贡献评价值
核心要素：工作量，点赞/点踩 
这是未来小白进行 IPO 或者 ICO 时给予奖励的唯一指标；
具体计算方式采取开源：每半年 review 一次，新的算法不修改以前的结果（欢迎大家给出建议）

### 5.2、效率指数（Efficiency Index)

是 contributor 和 committer 的在单位工作时间效率的评估，这是一个仅仅具有比较意义的指标。

核心要素：

- 单位时间下更新量代码或 review comment 的数量
- 终止 issue 按照：一个申请 size 而 0 提交进行计入

具体计算方式采取开源：每半年 review 一次（欢迎大家给出建议）。   
运维 issue 打上 "**运维**" 不计入 EI 指标。

### 5.3、公示

所有参与者的指数均会进行公布，所有参与小白项目的行为均视为其认同小白拥有公布的权利（以 github 账号显示）。

## 6、淘汰机制

有两种淘汰依据：

### 6.1、EI值

- 连续 3 月 EI 排在倒数 5%（不足一人则以一人计）的账号半年内不得进行奖励统计

### 6.2、违反诚信原则

小白相信每个参与小白项目的同学都会坚守诚信的原则，但是如果出现一下行为：

- 违反小白的版权管理规定
- 数据保密规定
- 虚报工作量
- 删除他人的issue留言
- 以及一切违反小白价值观的行为

一经证实，小白有权停止其贡献资格，并减少甚至取消其 CI 值。

## 7、发放标准及方式

### 7.1、标准

Contributor 每个 D 奖励单价为 RMB500（暂定）  
Commiter 每个 D 奖励单价为 RMB700（暂定）  

### 7.2、方式

每月 15 日统计已经 merge 的 pr  
现金通过 mart.coding.net 或 zbj.com 发放（可以自行选择），税费自负。

#### 说明：以上规范的内容（包含链接引用的部分），上海尘微科技有限公司拥有解释权