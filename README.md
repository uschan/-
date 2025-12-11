# Huberman Protocol - 人体系统调优指南

![Project Status](https://img.shields.io/badge/Status-Active-success)
![Tech Stack](https://img.shields.io/badge/React-TypeScript-blue)
![AI](https://img.shields.io/badge/AI-Gemini_Flash-orange)

这是一个基于神经生物学教授 **Andrew Huberman** (Huberman Lab Podcast) 及抗衰老专家 **David Sinclair** 的研究成果构建的健康生活实践指南 Web 应用。

本项目旨在将复杂的神经科学原理转化为可视化的、可执行的结构化协议，帮助用户像“优化代码”一样优化自己的生理系统（睡眠、专注、饮食、心态与长寿）。

## ✨ 主要功能 (Key Features)

### 1. 🧬 结构化知识库 (Structured Protocols)
将海量的 Podcast 内容提炼为五个核心板块，包含科学原理摘要、可视化图表及行动清单：
- **睡眠 (Sleep):** 昼夜节律校准、皮质醇与褪黑素管理。
- **饮食 (Diet & Fasting):** 间歇性禁食、肠道菌群与自噬机制。
- **专注 (Focus):** 90分钟超日节律、神经可塑性触发机制。
- **多巴胺 (Dopamine):** 痛苦-快乐平衡、奖励预测误差管理。
- **长寿 (Longevity):** 表观遗传信息理论、生活方式干预。

### 2. 🤖 AI 健康评估 (AI Assessment)
- 集成 **Google Gemini 2.5 Flash** 模型。
- 用户在每个板块完成针对性问卷（如光照习惯、手机使用时长等）。
- AI 根据 Huberman 的协议生成个性化的分析报告、优势识别及改进建议。
- **本地持久化:** 报告会自动保存至浏览器 LocalStorage，形成个人健康档案。

### 3. ✅ 每日打卡仪表盘 (Daily Protocol Dashboard)
- 预设基于科学研究的每日任务清单（如：晨间接触阳光、NSDR、生理叹息等）。
- 每日自动重置任务状态。
- 实时追踪完成进度。

### 4. 🧘 实用工具 (Utilities)
- **生理叹息 (Physiological Sigh) 引导:** 内置交互式呼吸动画工具，帮助用户在压力大时快速降低心率并恢复冷静（吸气-再吸气-长呼气）。

### 5. 📱 响应式设计
- 完美适配移动端与桌面端，提供流畅的阅读与交互体验。

---

## 🛠 技术栈 (Tech Stack)

- **Frontend:** React 18, TypeScript
- **Styling:** Tailwind CSS (CDN/Utility classes)
- **AI Integration:** Google GenAI SDK (`@google/genai`)
- **Icons:** Lucide React
- **Charts:** Recharts (可视化数据展示)
- **Build/Runtime:** ES Modules (浏览器原生支持，无需复杂打包配置)

---

## 🚀 快速开始 (Getting Started)

### 前置要求
你需要一个 Google Gemini API Key。请访问 [Google AI Studio](https://aistudio.google.com/) 免费获取。

### 安装与运行

由于本项目结构设计为轻量级 ES Module 模式，你可以通过以下方式运行：

1. **克隆项目**
   ```bash
   git clone https://github.com/your-username/huberman-protocol.git
   cd huberman-protocol
   ```

2. **配置环境变量**
   在项目根目录（或构建配置中）设置 API Key。
   *注意：由于本项目演示环境通常直接在浏览器中运行，代码中通过 `process.env.API_KEY` 调用。在本地开发时，你可能需要配置 `.env` 文件或在构建工具（如 Vite/Webpack）中注入变量。*

3. **安装依赖**
   ```bash
   npm install
   ```

4. **启动开发服务器**
   ```bash
   npm start
   # 或使用 vite
   npm run dev
   ```

---

## 📂 项目结构

```
/
├── index.html              # 入口 HTML，包含 Tailwind CDN 和 Import Maps
├── index.tsx               # React 入口文件
├── App.tsx                 # 主应用逻辑，状态管理与路由
├── constants.tsx           # 静态数据：协议内容、默认任务、图表数据
├── types.ts                # TypeScript 类型定义
├── metadata.json           # 项目元数据
├── components/             # UI 组件库
│   ├── Hero.tsx            # 首页 Banner
│   ├── Sidebar.tsx         # 侧边导航栏
│   ├── Dashboard.tsx       # 仪表盘与档案查看 (核心功能)
│   ├── ContentSection.tsx  # 协议内容详情页
│   ├── SectionCharts.tsx   # Recharts 图表组件
│   ├── AssessmentModal.tsx # AI 问卷与分析模态框
│   └── BreathingExercise.tsx # 呼吸练习工具
└── README.md
```

---

## ⚠️ 免责声明 (Disclaimer)

本项目提供的信息仅供参考，基于 Andrew Huberman 教授及相关科学文献的公开内容整理。**本项目不提供医疗建议、诊断或治疗。**

在开始任何新的饮食、运动或补充剂计划之前，请务必咨询您的医生或其他合格的医疗保健提供者。

---

## 🔗 致谢与引用

- **Huberman Lab Podcast:** [https://www.hubermanlab.com/](https://www.hubermanlab.com/)
- **David Sinclair (Lifespan):** [https://lifespanbook.com/](https://lifespanbook.com/)
- **Google Gemini API:** 提供强大的上下文理解与生成能力。

---

Made with ❤️ and Dopamine.
