# pull request 规范

下文对 pull request 的创建，以及对 review 工作作出规范说明；
小白采用双分支的方式进行代码的管理。master和develop，所有的contributor仅仅只能向develop上推送pr。
icp的统计仅仅针对已经进入master分支的所有关联issue和pr

## pull request 的创建

- 完成代码编写或文档编写工作后，提交 pull request 来进行验收；

- 一个 pull request 必须针对一个到多个 issue;  
  换言之，不接受不针对 issue 的 pull request;

- pull request 中包含的 commit 需正确命名，声明 `#<issue 编号>`.

- pull 对应的分支应该按照 `类型/开发者-目的` 命名。  
  可取的类型包括：`bugfix`(修 BUG) `feature`(功能特性开发) `doc`(文档工作)  
  例如，ben7th 修正图表显示不正确的 bug，可以表示为：  
  `bugfix/ben7th-chart-error`

## pull request 的验收(review)

- 可由多人对一个 pull request 进行验收


## pull request 的更新

- 验收存在问题的 pull request 不进行合并；
- 开发者收到验收意见后，在同一分支上继续提交 commit, 更新 pull request. 直到验收通过；

## pull request 的合并与关闭

- 原则上，确定 pull request 解决了对应 issue 时才进行合并与关闭；  
  避免反复为一个 issue 提交不同的 pull request.
- pull request 由 committer 合并到开发分支；
- 若出现冲突，根据具体情况解决代码冲突后合并；