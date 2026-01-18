---
title: "Python 办公自动化：像 Excel 一样玩转 Pandas 数据分析"
date: 2026-01-18 13:00:00 +0800
categories: [技术, 办公辅助]
tags: [Python, Pandas, 办公自动化]
---

> 如果你每天还在处理没完没了的 Excel 表格，那么 Pandas 库将是你打开自动化办公大门的钥匙。

## 1. 读取数据

```python
import pandas as pd
df = pd.read_excel("data.xlsx")
print(df.head())
```

## 2. 数据过滤

```Python
# 筛选金额大于 500 的订单
result = df[df['金额'] > 500]
result.to_excel("result.xlsx", index=False)
```

## 3. 分组统计
```Python
# 统计各部门业绩总和
summary = df.groupby('部门')['业绩'].sum()
print(summary)
```

欢迎在下方留言交流！

  
