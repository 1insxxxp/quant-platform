# 项目架构

> 本文档描述 quant-platform 的架构与目录职责。**请在修改项目结构、新增应用或包时同步更新此文件。**

## 概览

```
quant-platform/
├── apps/                    # 应用层
│   └── backend/             # 后端 API 服务
│       ├── index.js         # 入口
│       └── package.json
├── packages/                # 共享包（预留）
├── docs/                    # 文档
│   └── ARCHITECTURE.md
├── package.json
├── .gitignore
└── README.md
```

## 目录职责

### `apps/`

可运行的应用，每个子目录为独立应用：

| 应用 | 说明 | 技术 |
|------|------|------|
| `backend` | 后端 API 服务 | Express 5.x |

### `packages/`

共享库，供多个应用引用：

| 包 | 说明 | 状态 |
|----|------|------|
| （待添加） | | 预留 |

### `docs/`

项目文档：

| 文件 | 说明 |
|------|------|
| `ARCHITECTURE.md` | 本架构文档 |

## 后端 (backend)

- **框架**: Express 5.x
- **端口**: 3000
- **入口**: `apps/backend/index.js`

当前提供根路径 `GET /` 健康检查接口。

## 扩展规划

- [ ] 增加 `packages/` 下的共享工具或类型包
- [ ] 增加前端应用（如 `apps/web`）
- [ ] 后端 API 路由与业务模块化
