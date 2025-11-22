# 王一然个人网站

![王一然个人网站](astro-supabase-starter-preview.png)

**在线访问:** [https://resumelucasass.netlify.app/](https://resumelucasass.netlify.app/)

这是王一然的个人展示网站，使用 **Astro** 框架构建，部署在 Netlify 平台。

## 项目简介

王一然，永泰小学（十一集团校）五年级四班学生，班级旗手。曾获全国"叶圣陶杯"华人青少年作文大赛一等奖、全国青少年人工智能挑战赛铜奖等多项国家级、省部级荣誉。四年间创作63篇诗歌作品，并使用AI技术开发游戏等作品。

## 网站架构

### 页面结构
- **首页** (`/`) - 个人介绍、核心亮点展示
- **关于我** (`/about`) - 详细个人信息、自荐理由
- **荣誉奖项** (`/awards`) - 各类奖项证书展示
- **诗歌作品** (`/poems`) - 63篇诗歌习作展示
- **学业成绩** (`/academic`) - 学业成绩展示
- **作品展示** (`/projects`) - AI开发作品链接

### 技术栈
- **框架**: Astro 5.1.10
- **样式**: Tailwind CSS 4.0.1
- **部署**: Netlify
- **语言**: TypeScript

### 设计风格
- **色调**: 科技蓝、深空黑、霓虹绿，符合青少年男生审美
- **动画**: 渐变动画、悬浮效果、粒子特效
- **布局**: 响应式设计，移动端优先

## 开发命令

所有命令从项目根目录运行：

| 命令                   | 说明                                           |
| :-------------------- | :-------------------------------------------- |
| `pnpm install`        | 安装依赖                                       |
| `pnpm run dev`        | 启动本地开发服务器 `localhost:4321`              |
| `pnpm run build`      | 构建生产版本到 `./dist/`                        |
| `pnpm run preview`    | 本地预览构建结果                                 |
| `pnpm run astro ...`  | 运行 Astro CLI 命令                            |

## 本地开发

### 前置要求
- Node.js v18.14+
- pnpm (推荐) 或 npm
- Netlify CLI (可选)

### 安装运行

1. 克隆仓库并安装依赖：
```bash
pnpm install
```

2. 启动开发服务器：
```bash
pnpm run dev
```

3. 在浏览器访问 [http://localhost:4321](http://localhost:4321)

### 部署到 Netlify

#### 方式一：通过 Netlify CLI
```bash
# 构建项目
pnpm run build

# 部署到生产环境（分两步执行）
netlify deploy --prod --dir=dist
```

#### 方式二：通过 Git 集成
推送到 GitHub 仓库后，在 Netlify 控制台连接仓库即可自动部署。

## 项目结构

```
resumelucasass/
├── src/
│   ├── components/          # 可复用组件
│   │   ├── Header.astro    # 网站头部导航
│   │   ├── Footer.astro    # 网站页脚
│   │   └── Layout.astro    # 全局布局
│   ├── pages/              # 页面路由
│   │   ├── index.astro     # 首页
│   │   ├── about.astro     # 关于我
│   │   ├── awards.astro    # 荣誉奖项
│   │   ├── poems.astro     # 诗歌作品
│   │   ├── academic.astro  # 学业成绩
│   │   └── projects.astro  # 作品展示
│   └── styles/
│       └── globals.css     # 全局样式
├── public/
│   └── images/             # 静态资源
│       └── awards/         # 奖项证书图片
├── image/                  # 源图片文件
├── resume.md              # 简历内容
├── intruduction.md        # 自荐信
├── poem.md                # 诗歌作品集
└── README.md              # 项目文档
```

## 任务列表 (TASK)

### 当前任务 - 2025年10月19日
- [x] 更新项目README.md，添加王一然个人网站任务
- [ ] 设计网站架构和页面结构
- [ ] 创建全局样式和动画效果
- [ ] 开发Header和Footer组件
- [ ] 开发首页
- [ ] 开发关于我页面
- [ ] 开发荣誉奖项页面
- [ ] 开发诗歌作品页面
- [ ] 开发学业成绩页面
- [ ] 优化配置文件

### 工作中发现的任务
- 需要处理现有的Supabase相关代码（本项目不使用数据库）
- 需要优化图片加载和展示
- 需要添加页面切换动画

## 编码规范

### 命名约定
- 文件名：kebab-case（如：`about-me.astro`）
- 组件名：PascalCase（如：`HeaderNav`）
- 变量名：camelCase

### 代码组织
- 组件按功能分组
- 使用相对导入
- 保持单个文件不超过500行

### 样式指南
- 使用 Tailwind CSS 工具类
- 响应式设计优先
- 移动端优先原则

## 支持

如有问题，请通过 GitHub Issues 反馈。

---

© 2025 王一然 - 版权所有
