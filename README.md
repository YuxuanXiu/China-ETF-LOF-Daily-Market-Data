# China ETF & LOF Daily Market Data · 中国 ETF 与 LOF 日行情数据集

**[English](#english)** | **[中文](#chinese)**

---

<a id="english"></a>

## English

### Overview

This dataset contains **daily OHLCV (Open, High, Low, Close, Volume, Amount) market data** for **1,710 exchange-traded funds (ETFs) and listed open-ended funds (LOFs)** listed on the **Shanghai Stock Exchange (SSE)** and **Shenzhen Stock Exchange (SZSE)** in China, spanning from the earliest listing dates through **November 17, 2025**.

### Data Structure

- **Format**: CSV files, stored under `data_up_to_2025-11-17/`
- **File naming convention**: `{code}_{start_date}_to_{end_date}.csv`
  - Example: `510050_2005-02-23_to_2025-11-17.csv` (SSE 50 ETF, from Feb 2005 to Nov 2025)
- **Encoding**: UTF-8

Each CSV file contains the following columns:

| Column | Description | Unit |
|--------|-------------|------|
| `date` | Trading date (YYYY-MM-DD) | — |
| `OPEN` | Opening price | CNY |
| `HIGH` | Highest price of the day | CNY |
| `LOW` | Lowest price of the day | CNY |
| `CLOSE` | Closing price | CNY |
| `VOLUME` | Trading volume | Shares |
| `AMT` | Trading amount (turnover) | CNY |



### Temporal Coverage

- **Latest data**: November 17, 2025
- Data length varies by product depending on its listing date.

### Usage Notes

1. **Currency**: All prices and amounts are denominated in **Chinese Yuan (CNY)**.
2. **Price precision**: Prices are quoted to 3 decimal places, consistent with Chinese market conventions for ETFs.
3. **Suspensions & holidays**: Non-trading days (weekends, holidays, and individual security trading halts) are omitted — only active trading days appear in the files.
4. **Date gaps**: If a security was suspended for a period, those dates simply do not appear in its CSV file.

### Updates

This dataset may be updated periodically with newer data. Each update will be placed in a separate folder named by the cutoff date (e.g., `data_up_to_YYYY-MM-DD/`), so that previous versions remain available and citable.

### License

This dataset is made available under the **[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)** license. You are free to share and adapt the data for any purpose, provided you give appropriate credit.

---

<a id="chinese"></a>

## 中文

### 概述

本数据集包含在**上海证券交易所**和**深圳证券交易所**上市的 **1,710 只 ETF（交易型开放式指数基金）和 LOF（上市型开放式基金）** 的**日频 OHLCV 行情数据**，涵盖开盘价、最高价、最低价、收盘价、成交量与成交额。时间范围从最早上市日期起，至 **2025 年 11 月 17 日**止。

### 数据结构

- **格式**：CSV 文件，存放于 `data_up_to_2025-11-17/` 目录下
- **文件命名规则**：`{代码}_{起始日期}_to_{结束日期}.csv`
  - 示例：`510050_2005-02-23_to_2025-11-17.csv`（上证 50 ETF，2005 年 2 月至 2025 年 11 月）
- **编码**：UTF-8

每个 CSV 文件包含以下字段：

| 字段 | 含义 | 单位 |
|------|------|------|
| `date` | 交易日期（YYYY-MM-DD） | — |
| `OPEN` | 开盘价 | 人民币（元） |
| `HIGH` | 当日最高价 | 人民币（元） |
| `LOW` | 当日最低价 | 人民币（元） |
| `CLOSE` | 收盘价 | 人民币（元） |
| `VOLUME` | 成交量 | 份/股 |
| `AMT` | 成交额 | 人民币（元） |



### 时间跨度

- **最新数据**：2025 年 11 月 17 日
- 各产品数据长度视其上市日期而定。

### 使用说明

1. **计价货币**：所有价格与金额均以**人民币（CNY）**计价。
2. **价格精度**：价格保留 3 位小数，符合中国 ETF 市场的报价惯例。
3. **停牌与节假日**：非交易日（周末、节假日及个股停牌期间）不包含在文件中——仅实际交易日有记录。
4. **日期不连续**：若某只证券因停牌等原因在一段时间内无交易，对应日期不会出现在其 CSV 文件中。

### 更新说明

本数据集视情况可能后续更新。每次更新会以截止日期命名的独立文件夹存放（如 `data_up_to_YYYY-MM-DD/`），以确保历史版本可追溯、可引用。

### 许可协议

本数据集采用 **[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)** 许可协议。您可以自由分享和改编本数据用于任何目的，但须注明出处。