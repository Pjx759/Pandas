## WEEK02笔记
### 数据的输入输出
#### 一、片语化和视觉化记忆
* read_* → to_*
* 从数据中挖去故事
* 读写表格，书写电子讲义
#### 二、Pandas如何处理数据
1. 数据表被称为DataFrame
   * 竖列column通常为**变数variablies**
   * 横行row通常为**观察observation**
2. 数据类型
   * 表格数据
   * 树状文本数据：HTML/XML最主流的查询语言是*xpath*
#### 三、数据框
* 数据框本质是多种变数及其多个观察序列的数据所构成
* 主流使用字典，在pandas情景下“,”可以方便数据的缩进不引起格式错误
   1. 对于数据的处理现实更加方便，读取文件方式“pd.read_csv/tsv/excel”
#### 四、读取数据
1. 档案安全：档案打开时，只允许一个软件进行读取改写
2. 尽量不要使用Excel另存为的csv文件，会容易出现代码错误
3. 数据框功能
   * df.head()：表格前三
   * df.info()：数据观察，各种变量的数据列，可以快速总观数据
   * df.shape()：数据框的大小（数据的含量）
   * df.describe(include=“all”)：描述性统计，所有变量的最大最小值的数据
     > df.describe()：运行生成数据框
#### 五、代码片段切片（code sinppets）
1. 列子集：
```python

df.loc()
df.iloc()
df.set_index()
df.head(n)
df.tail(n)
df.nlargest(n, '变量')
df.nsmallest(n, '变量')
df[df.估值（亿人民币）> 10]
```
2.行子集：（只取变量【数字】）
```python

df[['变量X','变量Y','变量Z']]
df[['变量X']]
df['变量X']
```
3.列+行子集：
```python

df.loc[:,['变量X':'变量Z']]    # 注意中括号里的: 和 ,的使用
df.iloc[:,[1,2,5]]    # iloc一定是数字
df.loc[df['变量X']>10, ['变量X','变量Z'] ]   
```
#### 六、绘制数据表
* 绘制代码：
```python
df.plot()
```




    
   
