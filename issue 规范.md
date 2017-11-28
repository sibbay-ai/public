# issue 规范

下文对 issue 的创建，围绕 issue 的 commit/pr 以及 issue 的关闭作出规范说明。

## issue 的创建

- 需求类 issue: 由 committer 创建；
- 具体任务类 issue: 由 committer/contributor 创建；
- bug 报告类 issue: 可由任何人创建；

## issue 的里程碑指定

issue 创建后需尽快指定里程碑，参考[《里程碑规范》](里程碑规范.md)

## issue 的 size label 标记

- issue 创建后需尽快对工作量进行估计，由 committer 标记 size label.  
  size label 包括：`size: 0.1` `size: 0.2` `size: 0.3` …… 等等。  
  建议通过管理工具 codetree 的 points 功能来进行标记。  

- 其中 `size:` 后的数值，代表工作量，`size: 1` 代表一天（八小时）

- 若无法预估工作量，需尽快通过讨论，先推进已经明确的工作；同时对当前 issue 进行拆分；

## issue 的拆分

当一个 issue 较为复杂，需要资源不确定，或需要多人参与时，需要对 issue 进行拆分，方式如下：

- 创建新的 issue, 与原 issue 放入同一里程碑
- 在新的 issue 内引用原 issue，写明 `来源：#<issue 编号>`
- 一般不建议进行多层拆分

## issue 的 assignees 指定

- issue 创建后需尽快指定 assignees. assignees 通常为希望看到并回复此 issue 的开发者；
- ICP 奖励的确定仅与对应 issue 的 pr 有关。assignees 只作为一种跟踪参考；

## 处理 issue 的开发者

- 原则上一个 issue 由一名开发者处理，一个未拆分的 issue 不建议多人同时处理；
- 开发者确定要处理此 issue 时，需在 issue 中留言说明；

## 围绕 issue 的 commit/pr

- 开发者可以通过 github 提交 pull request 来尝试处理这些 issue.  
  pull request 包含的 commit 需要按照以下方式命名：  
  bug 修改类：`fix #<issue 编号> , <描述信息>`  
  开发工作类：`for #<issue 编号> , <描述信息>`  

- 所有带有 ICP 工作量标记的 issue, 必须通过提交 pull request 的方式验收；
  一些工作如需求分析，调研，文档撰写，需要将相关文档整理为 md 文件，或在如 README.md 等文件中添加链接引用，同样以 pull request 的方式提交验收；

- pull request 的验收方式见[《pull request 规范》](pull%20request%20规范.md)

## issue 的关闭

- issue 对应的 pr 被正确合并且关闭后，issue 关闭；  
- 长期无法处理的 issue, 由 committer 给出说明后关闭；  
- issue 关闭时，committer 需重新核实 size label, 并在关闭 issue 时对工作量进行确认；  