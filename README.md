# 📊 E-commerce Analysis Project

基于2010-2011年英国电商交易数据的深度业务分析项目

## 🎯 项目概览

本项目通过**10个核心指标**深度剖析电商业务的销售增长、客户价值与运营效率，提供**数据驱动的战略建议**。

### 核心发现
- 📈 **销售增长**：月度GMV波动剧烈（-69.9%至+47.6%），存在明显季节性
- 🌍 **市场结构**：UK市场占81.42%，海外高价值市场（EIRE人均消费£88,515）待挖掘
- 👥 **客户价值**：Top 10%客户贡献60.2% GMV，复购客户贡献93.8%收入
- 🔁 **留存瓶颈**：首月留存率仅20.6%，30天是关键转化窗口

---

## 📂 项目结构

E-commerce-Analysis/
 ├── README.md                           # 项目介绍
 ├── E-commerce_Analysis_Report.md       # 完整分析报告（Markdown版）
 ├── E-commerce_Analysis_Report.pdf      # 完整分析报告（PDF版）
 ├── notebooks/
 │   ├── 01_data_cleaning.ipynb          # 数据清洗与数据库创建
 │   └── 02_indicator_analysis.ipynb     # 10个核心指标分析与可视化
 ├── results/
 │   ├── 1_monthly_sales.csv             # 月度销售数据
 │   ├── 5_customer_spending.csv         # 客户消费数据
 │   ├── 8_rfm_analysis.csv              # RFM客户分层
 │   ├── 10_customer_ltv.csv             # 客户生命周期价值
 │   └── viz_*.png                       # 所有可视化图表（10+张）
 ├── data/
 │   └── ecommerce.db                    # SQLite数据库（清洗后）
 └── requirements.txt                    # Python依赖包清单



---

## 🚀 快速开始

### 1. 克隆项目

```bash
git clone https://github.com/你的用户名/E-commerce-Analysis.git
cd E-commerce-Analysis
```

### 2. 安装依赖

```
# 创建虚拟环境（推荐）
python -m venv venv
source venv/bin/activate  # Windows用: venv\Scripts\activate

# 安装依赖包
pip install -r requirements.txt
```

### 3. 运行分析

```
# 启动Jupyter Notebook
jupyter notebook

# 依次运行：
# 1. notebooks/01_data_cleaning.ipynb
# 2. notebooks/02_indicator_analysis.ipynb
```

## 🛠️ 技术栈

- **数据处理**：Python 3.11, Pandas, NumPy
- **数据存储**：SQLite
- **数据分析**：SQL（窗口函数、CTE）
- **数据可视化**：Matplotlib, Seaborn
- **开发环境**：Jupyter Notebook

------

## 📄 完整报告

详细分析报告请查看：

- [Markdown版本](E-commerce_Analysis_Report.md)
- [PDF版本](E-commerce_Analysis_Report.pdf)

------

## 👤 作者

**你的名字**
 📧 Email: [your.email@example.com](mailto:your.email@example.com)
 🔗 LinkedIn: [你的LinkedIn主页]
 💼 Portfolio: [你的个人网站]

------

## 📜 许可证

本项目采用 MIT License - 详见 [LICENSE](LICENSE) 文件

------

## 🙏 致谢

- 数据来源：[UCI Machine Learning Repository - Online Retail Dataset](https://archive.ics.uci.edu/ml/datasets/online+retail)
- 分析框架参考：RFM模型、Cohort分析