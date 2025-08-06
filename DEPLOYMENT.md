# 部署说明

## 项目概述
这是一个基于 Vue3 + Ant Design Vue + Vite 的前端项目管理系统。

## 技术栈
- Vue 3.3.0
- Ant Design Vue 4.0.0
- Vite 4.4.0
- Pinia 2.1.0 (状态管理)
- Vue Router 4.2.0
- ECharts 6.0.0 (图表库)

## 本地开发
```bash
# 安装依赖
npm install

# 启动开发服务器
npm run dev

# 构建生产版本
npm run build

# 预览构建结果
npm run preview
```

## Vercel 部署

### 自动部署
1. 将代码推送到 GitHub 仓库
2. 在 Vercel 中连接 GitHub 仓库
3. Vercel 会自动检测到 Vue 项目并配置构建设置

### 手动部署
```bash
# 安装 Vercel CLI
npm i -g vercel

# 登录 Vercel
vercel login

# 部署项目
vercel

# 生产环境部署
vercel --prod
```

### 部署配置
项目已配置 `vercel.json` 文件，包含：
- 构建命令：`npm run build`
- 输出目录：`dist`
- SPA 路由配置

## 环境变量
如需配置环境变量，可在 Vercel 项目设置中添加。

## 注意事项
- 确保所有依赖都已正确安装
- 构建前请运行 `npm run build` 确保构建成功
- 如遇到路由问题，检查 `vercel.json` 中的路由配置