- [連結中的空格](#連結中的空格)

# 連結中的空格

情況描述：有時候會遇到連結中有空格，導致說Markdown在解析連結的時候，無法解析出來。
情況分析：他把空格當成結束字元了~~爛東西~~。
解決方法：
1. 把連結中的空格，替換成%20。
2. 使用wiki連結。
```md
[[Example]]
```

### 舉例：
今天要連結一個檔案，連結文字顯示成Others，檔案路徑在目錄底下，叫做Markdown Others.md

錯誤示範：
```md
[Others](Markwodn Others.md)
[Others]("Markwodn Others.md")
[Others]('Markwodn Others.md')
```
這三種打法，在Markdown都是無法解析的，所以不能這樣打。

正確示範：
1. 把連結中的空格，替換成%20。
```md
[Others](Markdown%20Others.md)
```
效果展示
[Others](Markdown%20Others.md)

2. 使用Wiki連結
```md
[[Markdown Others]]
```
效果展示
[[Markdown Others]]



#Markdown #MarkupLanguage 