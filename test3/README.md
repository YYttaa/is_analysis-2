# 实验2:图书管理系统用例建模

|学号|班级|姓名|
|----|------|----|
|201610414112|软件（本）16-1|唐银浩|
## 1.图书管理系统类图
### 1.1PlantUML源码如下:
```puml
@startuml
package person #DDDDDD {
 abstract class 人物{
    -姓名
    -用户名
    -密码
    -性别
 }
 class 学生<extends 人物>{
    -学号
    -类别
 }
 class 图书管理员<extends 人物>{
    -管理员编号
    -职务
    -负责区域
 }

 class 超级管理员{
     -ID
     -姓名
     -用户名
     -密码
  }
}

package book #FFF8DC {
 class 书籍{
    -图书编号
    -书名
    -作者
    -价格
    -国际出版号
    -简介
    -馆藏位置
    -馆藏数量
    -可借数量
    -图书类别
 }
 class 图书种类{
    -类别编号
    -类别名称
    -类别描述
 }
 class 馆藏{
    -馆藏编号
    -地点
 }
}

package operation #BCEE68 {
 class 借阅图书{
    -借阅编号
    -借阅人
    -借阅书籍编号
    -借阅日期
    -应还日期
    -还书日期
 }
 class 预定图书{
    -预定编号
    -预定人
    -预定图书
    -预定日期
 }
 class 逾期记录{
    -逾期编号
    -逾期人
    -逾期书籍
    -逾期天数
 }
}
图书管理员 "1"-down-"*" 借阅图书:登记
学生 "1"-down-"*" 预定图书:预定
馆藏 "1" *-right- "*" 书籍:馆藏
书籍 "1" -right- "*" 预定图书:被预定
图书种类 "1" *-up- "*" 书籍:分类
借阅图书 "0..1" -down- "1" 书籍:借阅
借阅图书 "1" -right- "0..1" 逾期记录:记录
借阅图书 "*"--"1" 学生:借阅
图书管理员 "1" -up- "*"书籍:维护
人物 <|-right- 学生
人物 <|-left- 图书管理员
@enduml
```
<br>

### 1.2类图如下:
![img](./picture/libraryManager.png)

<br>

### 1.3类图说明:
* 学生类与图书管理员类均**继承于抽象类人物**。
* 超级管理员为独立的类，可以对整体数据进行操作。
* 学生与预定图书的关系为**学生预定图书**，且**一对多**。
* 学生与借阅图书的关系为**学生借阅图书**，且**一对零或一**。
* 图书管理员与借阅图书的关系为**管理员登记借阅图书**，且**一对多**。
* 图书管理员与书籍的关系为**管路员维护书籍**，且**一对多**。