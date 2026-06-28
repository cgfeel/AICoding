# 项目名称

AICoding

## 项目概述

通过 `Claude Code` 完成 `Claude Code` 项目，使用的技术栈是 `NextJS` + `TypeScript` + `Prisma`

## 技术栈

- 前端 `NextJS 14` + `TypeScript` + `Tailwind CSS`
- 后端：`Next.js API Routes`
- 数据库：`Prisma` + `SQLite`
- 部署：`Vercel`

## 项目结构

```
src/
├── app/            # NextJS App Router 页面
│   ├── api/        # API 路由
│   ├── layout.tsx  # 全局布局
│   └── page.tsx    # 首页
├── components/     # React 组件
│   ├── ui/         # 通用 UI 组件
│   └── features/   # 业务组件
├── lib/            # 工具函数和配置
├── prisma/         # 数据库 schema 和迁移
└── types/          # TypeScript 类型定义
```

## 编码规范

- 使用函数式组件 + `React Hooks`
- 组件文件使用 `PascalCase` 命名（如 `BookmarkCard.tsx`）
- 工具函数使用 `camelCase` 命名
- `API` 路由返回统一的格式：`{ success: boolean, data?: unknown, error?: string }`
- 所有数据库操作通过 `Prisma Client` 执行

## 当前开发状态

- 项目初始化完成
- 数据库 `Schema` 设计完成
- 书签 `CRUD API` 开发中
- 前端页面持续开发
- 搜索功能持续开发

## 注意事项

- `SQLite` 数据库文件在 `prisma/dev.db`，不要提交到 `Git` 仓库
- 环境变量再 `.env` 文件中，不要提交到 `Git` 仓库
- 所有新功能先创建 `Git` 分支再开发，完成后合并到 `main` 分支
