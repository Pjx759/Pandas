### 第四周笔记
#### 一、用法
* split：多个字符用列表框起来
* len：查看长度
* lamda：匿名函数，可省略定义函数的步骤（不同新增的列，可以有不同的方法/函数/功能）
#### 二、数据框重塑
1. stack实现数据透视，一个独角兽对应多个值（一对多）
2. marge使用“,”隔开
3. split使用stack拆分
```
str.split→‘[，,、]’→相对完整   # 一对多简单透视
```
4. series使用：将index、values作为值
5. marge合并（效果）：左边因多个而产生复制
#### 三、取值   
> （字符串→列表）→表格
