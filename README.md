# 📊 E-commerce Analysis Project

基于2010-2011年英国电商交易数据的深度业务分析项目

## 🎯 项目概览

本项目通过**10个核心指标**深度剖析电商业务的销售增长、客户价值与运营效率，提供**数据驱动的战略建议**。

### 核心发现

- 📈 **销售增长**：月度GMV波动剧烈（-69.9%至+47.6%），存在明显季节性
- 🌍 **市场结构**：UK市场占81.42%，海外高价值市场（EIRE人均消费£88,515）待挖掘
- 👥 **客户价值**：Top 10%客户贡献60.2% GMV，复购客户贡献93.8%收入
- 🔁 **留存瓶颈**：首月留存率仅20.6%，30天是关键转化窗口

------

## 📂 项目结构

```bash
E-commerce-Analysis/
├── README.md                               # 项目介绍
├── E-commerce Analysis Report.md           # 完整分析报告（Markdown版）
├── E-commerce Analysis Report.pdf          # 完整分析报告（PDF版）
├── notebooks/
│   └── E-commerce_Analysis.ipynb           # 完整数据分析代码（清洗+10个指标+可视化）
├── results/
│   ├── 1_monthly_sales.csv                 # 月度销售数据
│   ├── ......
│   ├── 5_customer_spending.csv             # 客户消费数据
│   ├── 8_rfm_analysis.csv                  # RFM客户分层
│   ├── 10_customer_ltv.csv                 # 客户生命周期价值
│   └── viz_*.png                           # 所有可视化图表（10+张）
├── data/
│   └── data.csv                            # 原始数据集
└── requirements.txt                        # Python依赖包清单
```

------

## 🚀 快速开始

### 1. 克隆项目

```bash
git clone https://github.com/wanter0407/E-commerce-Analysis.git
cd E-commerce-Analysis
```

### 2. 安装依赖

```bash
# 创建虚拟环境（推荐）
python -m venv venv
source venv/bin/activate  # Windows用: venv\Scripts\activate

# 安装依赖包
pip install -r requirements.txt
```

### 3. 运行分析

```bash
# 启动Jupyter Notebook
jupyter notebook

# 打开并运行 notebooks/E-commerce_Analysis.ipynb
# 按顺序执行所有单元格即可完成：
# 1. 数据清洗与数据库创建
# 2. 销售增长与结构分析（指标1-4）
# 3. 客户价值深度分析（指标5-10）
```

------

## 📊 核心分析指标

### 销售增长与结构（4个指标）

1. **月度销售趋势** - 识别季节性规律与异常波动
2. **商品结构分析** - 验证帕累托法则，优化SKU组合
3. **国家市场表现** - 识别高价值市场与增长机会
4. **时间维度分析** - 优化运营时间与资源配置

### 客户价值深度（6个指标）

1. **客户消费分布** - 识别高/中/低价值客户群体
2. **复购率分析** - 评估客户粘性与复购价值
3. **购买间隔分析** - 定位流失预警关键节点
4. **RFM客户分层** - 精细化运营策略制定
5. **留存率分析** - Cohort分析识别流失瓶颈
6. **客户LTV量化** - 客户生命周期价值估算

------

## 📈 可视化示例

### 月度销售趋势

![月度销售趋势](./results/viz_1_monthly_trend.png)

### RFM客户分层

![RFM客户分层](./results/viz_8_rfm_segments.png)

### 留存率分析

![留存率分析](./results/viz_9_retention_analysis.png)

------

## 🛠️ 技术栈

- **数据处理**：Python 3.11, Pandas, NumPy
- **数据存储**：SQLite
- **数据分析**：SQL（窗口函数、CTE）
- **数据可视化**：Matplotlib, Seaborn
- **开发环境**：Jupyter Notebook

------

## 📄 完整报告

详细分析报告请查看：

- **Markdown版本**：[E-commerce Analysis Report.md](./E-commerce Analysis Report.md)
- **PDF版本**：[E-commerce Analysis Report.pdf](./E-commerce Analysis Report.pdf)

------

## 👤 作者

**Wanting Zhang**
 📧 Email: [wantingz185@gmail.com](mailto:wantingz185@gmail.com)
 🔗 GitHub: [@wanter0407](https://github.com/wanter0407)

------

## 📜 许可证

本项目采用 MIT License - 详见 [LICENSE](LICENSE) 文件

------

## 🙏 致谢

- 数据来源：[UCI Machine Learning Repository - Online Retail Dataset](https://archive.ics.uci.edu/ml/datasets/online+retail)
- 分析框架参考：RFM模型、Cohort分析

------

**如果觉得这个项目对你有帮助，请给个⭐Star支持一下！**