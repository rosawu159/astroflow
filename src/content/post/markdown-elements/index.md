---
title: "Two Sum"
description: "This post is for testing and listing a number of different markdown elements"
publishDate: "22 Feb 2023"
updatedDate: 22 Jan 2024
tags: ["test", "leetcode"]
---

## 需求

1. Two Sum 問題的要求是找到兩個數字的和等於目標值，並且返回它們的索引
2. 返回的是這兩個數字的索引，而不是數字本身
3. 索引跟數字本身之間的配對關係

## 思路

知道 target且已經用迴圈遍歷到某個數字 num，那只需要檢查「有沒有一個數字可以和 num 相加等於 target」

```
target = num + 另一個數字
另一個數字 = target - num = complement
```

基於字典的查詢方法是：**找什麼就把什麼放key**

→ 因為要在遍歷過的num中，尋找complement 

→ 把num放key

## 資料結構

Key：數字 num（方便快速查找）。

Value：索引 index（方便在找到 complement 時快速返回索引值）。
