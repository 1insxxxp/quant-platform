# Quant Platform

量化交易平台 monorepo 项目。

## 技术栈

- **运行时**: Node.js
- **包管理**: npm workspaces
- **后端**: Express 5.x

## 项目结构

```
quant-platform/
├── apps/
│   └── backend/          # 后端 API 服务 (Express)
├── packages/             # 共享包（预留）
├── docs/                 # 文档
├── package.json          # 根配置与 workspaces
└── README.md
```

## 快速开始

### 安装依赖

```bash
npm install
```

### 启动后端

```bash
cd apps/backend && node index.js
```

服务默认运行在 http://localhost:3000

### 验证

访问 http://localhost:3000 应返回 `Quant Platform Running`

## Workspaces

- `apps/*` - 应用（后端、前端等）
- `packages/*` - 共享库（工具、类型、配置等）

## 文档

- [项目架构](docs/ARCHITECTURE.md) - 架构说明与目录职责
