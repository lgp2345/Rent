## 项目概览

| 模块              | 描述                                 | 端口 |
| ----------------- | ------------------------------------ | ---- |
| `apps/app`        | React Native 房屋租赁移动端 app 应用 | —    |
| `apps/admin`      | React 管理后台（用户/角色/权限）     | 5173 |
| `apps/server`     | NestJS 用户/认证/RBAC 服务           | 3000 |
| `packages/schema` | 共享 Zod 验证 Schema                 | —    |

## 快速导航

- [产品与业务设计总览](./DESIGN.md)
- [后端服务总览](./apps/server/CLAUDE.md)

### 硬性规则

- 单文件不超过 300 行
- 新增代码必须有对应测试
- 禁止 `console.log`，使用结构化日志
- 当需要查阅任何库或框架的文档时，自动使用 Context7 MCP。
- 提交规范：`feat:`、`fix:`、`refactor:`、`docs:`、`test:`
