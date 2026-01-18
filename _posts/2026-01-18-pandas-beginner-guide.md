---
title: "Python 办公自动化：像 Excel 一样玩转 Pandas 数据分析"
date: 2026-01-18 13:00:00 +0800
categories: [技术, 办公辅助]
tags: [Python, Pandas, 办公自动化, 入门教程]
---

> 如果你每天还在处理没完没了的 Excel 表格、重复性的复制粘贴，那么 Python 的 Pandas 库将是你打开“自动化办公”大门的钥匙。

很多初学者觉得 Pandas 很难，其实它就是一个**“没有界面的超级 Excel”**。今天我们不讲高深算法，只讲最实用的三个核心技能，帮你摆脱加班。

---

## 1. 读取与观察：给数据做个“体检”

在 Excel 中，我们要看数据得先双击打开。在 Pandas 里，我们只需要两行代码即可完成加载和预览。

```python
import pandas as pd

# 读取 Excel 文件
df = pd.read_excel("你的表格.xlsx")

# 看看前 5 行长什么样
print(df.head())

# 看看数据概况（列名、数据类型、是否有空值）
print(df.info())
