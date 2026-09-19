---
name: helloworld
description: 最小可用的测试 skill：按需打印一句 Hello World 问候，并回报本次加载的 skill 名称与所在路径。
whenToUse: 当用户要求测试 skill 是否生效、想看到 Hello World 输出，或显式调用 /helloworld 时使用。
---

# Hello World 测试 Skill

这是一个用于验证 DSH skill 发现与加载链路是否正常的最小 skill。

## 执行步骤

1. 回复一句问候：`Hello, World! 🌍`
2. 回报本次加载信息，格式如下：

   ```
   skill name   : helloworld
   skill source : .dsh/skills/helloworld/SKILL.md
   status       : loaded successfully
   ```

3. 补充一行说明：该 skill 是通过项目级根目录 `.dsh/skills/` 被发现的。

## 约束

- 不要修改任何文件，这是一个只读的验证用 skill。
- 不要执行网络请求。
- 如果用户同时提供了其他任务，先完成本 skill 的问候输出，再继续处理用户的任务。
