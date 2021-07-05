# Markdown
* 整理from: [菜鸟教程](https://www.runoob.com)
## 簡介  
字尾為 .md 或是 .markdown。  
Markdown的目標是實現「易讀易寫」。  
不過最需要強調的便是它的可讀性。一份使用Markdown格式撰寫的文件應該可以直接以純文字發佈，並且看起來不會像是由許多標籤或是格式指令所構成。Markdown語法受到一些既有text-to-HTML格式的影響，包括Setext、atx、Textile、reStructuredText、Grutatext 和 EtText，然而最大靈感來源其實是純文字的電子郵件格式。

因此Markdown的語法全由標點符號所組成，並經過嚴謹慎選，是為了讓它們看起來就像所要表達的意思。像是在文字兩旁加上星號，看起來就像*強調*。Markdown的清單看起來，嗯，就是清單。假如你有使用過電子郵件，區塊引言看起來就真的像是引用一段文字。

## 標題
```
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题
```
## 段落
兩個空格加Enter  
實現跳行  

或是新增一個空行

我是沒有
使用上面
方法得例子

## 列表
程式碼
```
* 第一项
+ 第二项
- 第三项
4. 第四項
    - 小項
```
結果
* 第一项
+ 第二项
- 第三项
4. 第四項
    - 小項

## 區塊
```
>外
>>中
>>>內
```
>外
>>中
>>>內

## 顯示code
        四個空格 
        或是tab

```
前後使用```
可以很大段
```
就這樣

## 連結
1. 顯示文字 [菜鸟教程](https://www.runoob.com)  
```
顯示文字 [菜鸟教程](https://www.runoob.com)
```

2. 直接顯示網址  <https://www.runoob.com>  
```
<https://www.runoob.com>
```

## 圖片
1. 使用!+[]+(位址)  
```
![alt Markdown-mark](img/Markdown-mark.png "Markdown-mark")
```
![alt Markdown-mark](img/Markdown-mark.png "Markdown-mark")

2. 或是 img 標籤
```
<img src="img/Markdown-mark.png" width="50%">
```
<img src="img/Markdown-mark.png" width="50%">

## 表格
```
| 表頭 | 表頭 | 表頭 |
| :---- | ----: | :----: |
| 置左 | 置右 | 置中 |
| 內容 | 內容 | 內容 |
```
| 表頭 | 表頭 | 表頭 |
| :---- | ----: | :----: |
| 置左 | 置右 | 置中 |
| 內容 | 內容 | 內容 |

## 其他

1. **文本加粗** 
```
**文本加粗**  
```
2. 前面加上反斜杠来帮助插入普通的符号：  
\*\* 正常显示星号 \*\*
