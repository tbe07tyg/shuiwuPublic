# 部署说明

## 项目概述
这是一个基于 Vue3 + Ant Design Vue 的项目管理系统，使用 Vite 作为构建工具。

## 技术栈
- Vue 3.3.0
- Ant Design Vue 4.0.0
- Vue Router 4.2.0
- Pinia 2.1.0
- Vite 4.4.0
- ECharts 6.0.0

## Vercel 部署步骤

### 1. 准备工作
确保项目已经推送到 GitHub 仓库：https://github.com/tbe07tyg/shuiwuPublic.git

### 2. Vercel 部署配置
项目已配置 `vercel.json` 文件，包含：
- 构建命令：`npm run build`
- 输出目录：`dist`
- SPA 路由配置

### 3. 部署步骤
1. 访问 [Vercel](https://vercel.com)
2. 使用 GitHub 账号登录
3. 点击 "New Project"
4. 导入 GitHub 仓库 `tbe07tyg/shuiwuPublic`
5. 配置部署设置：
   - Framework Preset: Vite
   - Build Command: `npm run build`
   - Output Directory: `dist`
   - Install Command: `npm install`
6. 点击 "Deploy"

### 4. 环境变量（如需要）
如果项目需要环境变量，可以在 Vercel 项目设置中添加。

### 5. 自定义域名（可选）
部署完成后，可以在 Vercel 项目设置中配置自定义域名。

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

## 项目结构
```
├── api/           # API 接口定义
├── assets/        # 静态资源
├── components/    # 公共组件
├── layout/        # 布局组件
├── router/        # 路由配置
├── store/         # 状态管理
├── styles/        # 全局样式
├── utils/         # 工具函数
├── views/         # 页面组件
├── App.vue        # 根组件
├── main.js        # 入口文件
├── index.html     # HTML 模板
├── vite.config.js # Vite 配置
├── vercel.json    # Vercel 部署配置
└── package.json   # 项目配置
```