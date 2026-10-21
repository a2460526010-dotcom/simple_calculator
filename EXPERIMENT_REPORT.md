# GitHub 协作实验报告

## 1. 实验信息

- 实验日期：2026-10-21
- 实验账号：`a2460526010-dotcom`
- 操作方式：浏览器端图形界面
- 开源项目：[lgiordani/simple_calculator](https://github.com/lgiordani/simple_calculator)
- 项目许可证：MIT License
- 我的 Fork：[a2460526010-dotcom/simple_calculator](https://github.com/a2460526010-dotcom/simple_calculator)

## 2. 实验目标

通过完整的 Fork、分支、代码修改、提交、Pull Request 与合并流程，掌握 GitHub 单人也能独立完成的基础协作方法。

## 3. 实施过程

1. 在 GitHub 检索并选择一个带 MIT 许可证的 Python 开源项目：`lgiordani/simple_calculator`。
2. 将上游仓库 Fork 到个人账号，保留上游来源和许可证信息。
3. 从默认分支创建功能分支：`feature/github-collaboration-demo`。
4. 在 `simple_calculator/main.py` 中新增 `mod(a, b)` 取模运算，并处理除数为零的情况。
5. 在 `tests/test_main.py` 中新增正常取模和除零异常测试。
6. 通过 Pull Request 将包含 3 个提交的功能分支合并到 Fork 的 `master` 分支。
7. 检查变更范围并完成 Merge；因只有单人账号，不执行双人账号的审核评论环节。

## 4. 本次代码改动

- 新增方法：`SimpleCalculator.mod(a, b)`
- 正常情况：返回 `a % b` 的结果
- 异常情况：当 `b == 0` 时抛出带有明确说明的 `ValueError`
- 新增测试：验证 `mod(10, 3) == 1`，以及除数为零时抛出异常

## 5. Pull Request 记录

- 源分支：`feature/github-collaboration-demo`
- 目标分支：`master`
- PR 链接：[#1](https://github.com/a2460526010-dotcom/simple_calculator/pull/1)
- 审核评论：单人账号模式下未执行
- 合并状态：Merged，已合并到 `master`

## 6. 实验结论

GitHub 的 Fork、分支、提交、Pull Request 和合并机制将代码变更与合并记录关联在同一个可追溯的工作流中。本实验完成了单人可独立执行的完整流程；双人互相审核与交叉合并需要第二个 GitHub 账号参与。
