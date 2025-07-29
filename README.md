# AI-STOCK: Your AI Investment Strategy Committee

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python Version](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/)

An advanced, multi-agent AI system that provides comprehensive, multi-faceted investment analysis by simulating a world-class investment committee.

---

## 📖 关于项目 (About The Project)

在当今瞬息万变的金融市场中，投资者常常面临信息过载、分析片面和情绪偏见等挑战。专业的投研工具不仅昂贵，而且往往缺乏深度的、多维度的洞察力。

**AI-STOCK** 正是为此而生。它不仅仅是一个数据聚合工具或简单的AI“黑箱”，而是一个透明的、由多个AI专家组成的“玻璃盒”决策辅助系统。受到 `ai-hedge-fund` 项目的启发，我们将其理念进一步深化，从一个自动交易系统演变为一个专注于为人类用户提供深度投研报告的“AI副驾”。

我们的核心理念是：**为每一位投资者，配备一个世界级的、永不休息的、由投资传奇组成的投研团队。**

### ✨ 核心亮点 (Key Features)

*   **🤖 多Agent协同分析 (Multi-Agent Analysis):** 系统由十多个拥有不同“人格”和分析框架的AI Agent组成，并行工作，确保分析的广度和深度。
*   **🧠 传奇投资人视角 (Legendary Investor Personas):** 借助沃伦·巴菲特的价值洞察、凯茜·伍德的创新远见、彼得·林奇的成长嗅觉，从经过时间检验的投资哲学中获得智慧。
*   **📄 综合策略报告 (Comprehensive Reporting):** 最终输出一份详尽的“投资委员会会议纪要”，清晰呈现每位专家的观点、分歧与共识，以及最终的综合策略建议。
*   **💬 智能查询与交互 (Intelligent Query & Interaction):** 不仅能进行深度分析，还能理解用户的日常查询，如“苹果公司最近有什么新闻？”或“给我看一下特斯拉近一年的股价图”。
*   **🌐 动态数据聚合 (Dynamic Data Aggregation):** 自动从网页、API等多种渠道获取最新的财务报表、新闻和市场数据，确保分析的时效性。

---

## 🏛️ 系统架构与工作流程 (Architecture & How It Works)

AI-STOCK 的工作流程旨在模拟一个高效的投研团队从接收任务到提交报告的全过程。

1.  **用户输入 (User Query):** 用户通过自然语言提出需求（例如：“帮我分析一下英伟达”）。
2.  **智能识别与数据获取 (NLU & Data Aggregation):** 系统精准识别目标公司，并启动数据爬虫和API调用程序，从全网抓取最新的公司财报、新闻、股价等信息。
3.  **任务分发至Agent核心 (Task Distribution):** 干净、结构化的数据被分发给所有AI Agent。
4.  **并行分析 (Parallel Analysis):**
    *   **传奇投资人Agent (Investor Legends):** 从各自的投资哲学出发，进行定性与定量分析。
    *   **功能性Agent (Functional Agents):** 对估值、风险、技术面、基本面等进行专项量化分析。
5.  **整合与生成 (Synthesis & Generation):**
    *   **AI首席投资官 (Chief Investment Strategist):** 收集所有Agent的分析报告，主持一场“虚拟投委会”，提炼共识、聚焦分歧，并撰写最终的综合报告。
6.  **输出详实报告 (Report Delivery):** 一份结构清晰、内容详实的“投资委员会会议纪要”被呈现给用户。

### 认识我们的AI团队 (Meet the AI Team)

*   **传奇投资人 (The Legends):**
    *   **Warren Buffett:** 寻找拥有护城河的伟大企业。
    *   **Ben Graham:** 挖掘具有巨大安全边际的“烟蒂股”。
    *   **Cathie Wood:** 投资于颠覆性创新的未来。
    *   **Peter Lynch:** 在普通人视角中发现“十倍股”。
    *   *(以及更多...)*
*   **功能性专家 (The Specialists):**
    *   **Valuation Agent:** 精确计算内在价值。
    *   **Risk Advisor:** 揭示所有潜在风险。
    *   **Fundamentals Agent:** 审计财务健康状况。
    *   **Technicals Agent:** 解读图表和市场时机。
    *   **Sentiment Agent:** 量化市场情绪。

---

## 🚀 开始使用 (Getting Started)

请按照以下步骤在您的本地环境中设置并运行本项目。

### 先决条件 (Prerequisites)

*   Python 3.9+
*   pip 包管理器

### 安装步骤 (Installation)

1.  **克隆仓库**
    ```sh
    git clone https://github.com/your-username/project-synapse.git
    cd project-synapse
    ```

2.  **安装依赖**
    ```sh
    pip install -r requirements.txt
    ```

3.  **配置环境变量**
    *   将 `.env.example` 文件复制为 `.env`。
        ```sh
        cp .env.example .env
        ```
    *   在 `.env` 文件中填入您从以下服务获取的API密钥：
        ```env
        # 例如:
        OPENAI_API_KEY="sk-..."
        ALPHA_VANTAGE_API_KEY="your_alpha_vantage_key"
        # ...其他API密钥
        ```

---

## 💻 使用示例 (Usage)

您可以通过命令行或导入模块的方式与系统交互。

**示例1：进行一次完整的股票分析**

```python
from synapse import analyze

# 启动分析
report = analyze("分析一下苹果公司(AAPL)") 

# 打印报告
print(report)
```
*这将输出一份完整的“投资委员会会议纪要”报告。*

**示例2：查询特定信息**

```python
from synapse import query

# 查询新闻
news = query("特斯拉最近有什么关于自动驾驶的新闻？")
print(news)

# 获取股价图
chart_path = query("帮我生成一张微软从年初至今的股价图")
print(f"图表已保存至: {chart_path}")
```

---

## 🗺️ 未来路线图 (Roadmap)

*   [x] 核心多Agent分析框架
*   [ ] 引入更多传奇Agent（如 Ray Dalio, George Soros）
*   [ ] 支持投资组合级别的诊断与分析
*   [ ] 引入宏观经济Agent，提供自上而下的市场洞察
*   [ ] 开发Web前端界面，提供更友好的交互体验

查看[开放的问题](https://github.com/your-username/project-synapse/issues)列表，了解更多计划中的功能。

---

## 🤝 贡献 (Contributing)

我们欢迎任何形式的贡献！如果您有好的想法，请先创建一个Issue或Pull Request。

1.  Fork 本项目
2.  创建您的特性分支 (`git checkout -b feature/AmazingFeature`)
3.  提交您的更改 (`git commit -m 'Add some AmazingFeature'`)
4.  推送到分支 (`git push origin feature/AmazingFeature`)
5.  打开一个 Pull Request

---

## 📄 许可证 (License)

本项目采用 MIT 许可证。详情请见 `LICENSE` 文件。

---

## ⚠️ **重要免责声明 (Important Disclaimer)**

**本项目提供的所有信息、数据、分析和报告仅用于学术研究和技术演示目的，不构成任何形式的投资建议、财务建议、交易建议或任何其他类型的建议。**

所有内容均基于公开数据和AI模型的分析，可能存在错误、延迟或不完整之处。您不应将本项目的任何输出作为您做出任何投资决策的唯一依据。

**投资有风险，入市需谨慎。** 请在做出任何财务决策前，咨询专业的财务顾问。对于因使用或依赖本项目信息而造成的任何直接或间接损失，本项目作者及贡献者概不负责。

---

## 🙏 致谢 (Acknowledgments)

*   本项目的灵感和基础源于 Virat Singh (virattt) 的 [ai-hedge-fund](https://github.com/virattt/ai-hedge-fund) 项目。
*   感谢所有提供免费金融数据的API服务商。
*   感谢所有开源社区的贡献者。