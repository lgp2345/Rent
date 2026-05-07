# 后端服务

基于 NestJS + Fastify 的房屋租赁管理后端服务。

## 技术栈

### 核心框架

| 类别 | 选型 |
|------|------|
| 运行时 | Node.js 22+ |
| 框架 | NestJS + Fastify |
| 语言 | TypeScript 5+ |

### 认证与验证

| 类别 | 选型 |
|------|------|
| 认证 | Passport JWT（`@nestjs/passport` + `@nestjs/jwt`） |
| 验证 | nestjs-zod（与 `packages/schema` 共享 Zod schema） |

### 数据库

| 类别 | 选型 |
|------|------|
| 数据库 | PostgreSQL 16+ |
| ORM | Drizzle ORM |
| 迁移 | drizzle-kit |

### 中间件与安全

| 类别 | 选型 |
|------|------|
| 配置管理 | `@nestjs/config` + Zod 校验 env |
| 安全头 | `@fastify/helmet` |
| CORS | `@fastify/cors` |
| 限流 | `@nestjs/throttler` |

### 业务支撑

| 类别 | 选型 |
|------|------|
| 定时任务 | `@nestjs/schedule` |
| 健康检查 | `@nestjs/terminus` |
| 日志 | `nestjs-pino` |

### 开发工具链

| 类别 | 选型 |
|------|------|
| API 文档 | `@nestjs/swagger` + `@fastify/swagger` |
| 测试框架 | `vitest` + `@nestjs/testing` |
| 代码质量 | `biome` |

### 本地开发

| 类别 | 选型 |
|------|------|
| 容器化 | `Dockerfile` + `docker-compose`（含 PostgreSQL） |

## 端口

| 服务 | 端口 |
|------|------|
| NestJS Server | 3000 |
| PostgreSQL | 5432 |

## 测试策略

- 单元测试：Service 层，覆盖核心业务逻辑
- 集成测试：Controller 层 E2E 测试，使用 `supertest`
