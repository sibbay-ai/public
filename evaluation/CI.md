## 贡献指数（Contribute Index）计算规则

[Sibbay CI 贡献指数定义](https://github.com/sibbay-ai/public/blob/master/ICP%20%E5%A5%96%E5%8A%B1%E6%9C%BA%E5%88%B6.md#51贡献指数contribute-index)

### 计算原则

- 一切基于 github 上有据可查的 issue, commit, pull request 进行计算
- 通过 github API 获取数据作为计算依据
- 计算方法与相关代码完全公开
- 计算结果定期累计，完全公示
- 若计算规则由所调整，调整前已经形成的累计不作溯及以往的调整

### 单期 CI 计算规则（伪代码描述）

1. 查询 sibbay-ai 组织下所有 repo 中，带有 ICP label 的 issue.  
   赋值为 `icp_issues`
   
2. 根据 `icp_issues` 查询与这些 issue 相关的 commit (commit message 中引用了对应 issue).  
   赋值为 `icp_issue_commits`
   
3. 查询 sibbay-ai 组织下所有 repo 中，已经被合并的 pull request.  
   合并日期在统计起止时间内；  
   赋值为 `prs`
   
4. 根据 `prs` 查询与这些 pull request 相关的 commit (commit 出现在 pull request 中).  
   赋值为 `pr_commits`
   
5. 对 `icp_issue_commits` 以及 `pr_commits` 取交集，获得在两边均出现的 commits.  
   赋值为 `result_commits`
   
6. 根据 `result_commits` 找到与其相关的 issue 以及 pull request，形成以下集合（伪代码表示）：
   ```
   [
     { issue: <issue1>, pull_request: <pr1> },
     { issue: <issue2>, pull_request: <pr2> },
     { issue: <issue3>, pull_request: <pr3> },
   ]
   ```
   对该集合进行去重，形成 `result`
   
7. 根据 `result` 生成贡献值统计表格

### 相关统计实现代码位置

https://github.com/sibbay-ai/icp-stat

### CI 累积

CI 针对各个开发者，逐期统计，逐期累积，若因特殊情况导致变化，变化内容需公示。
