## 项目简介

这是一个房屋租赁管理全栈 Monorepo 项目，包含 app 应用、用户权限系统（RBAC + 多租户）、管理后台。基于 React 19 + PostgreSQL + Drizzle。

## 开发指南

### 前置要求

- Node.js >= 22
- pnpm >= 10
- PostgreSQL

### 安装与运行

```bash
# 安装依赖
pnpm install

# 开发模式
pnpm dev
```

### 项目结构

```
apps/
  app/          # React Native 移动端应用
  admin/        # 管理后台
  server/       # NestJS 后端服务
packages/
  schema/       # 共享 Zod 验证 Schema
docs/           # 设计文档与计划
infra/
  compose/      # Docker Compose（一次命令启动 admin+server）
```
