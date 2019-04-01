# 实验1:业务流程建模

|学号|班级|姓名|
|----|------|----|
|201610414112|软件（本）16-1|唐银浩|

### 1.图书管理系统用例图
* **PlantUML源码如下:**
```puml
@startuml
:图书管理员:as admin
:读者:as reader
left to right direction
rectangle 管理员操作{
    (借出图书)
    (归还图书)
    (维护书目)
    (维护读者信息)
    (更改读者信息)
}
rectangle 读者操作{
    (查询书目)
    (查询借阅情况)
    (预定图书)
    (取消预定)
    (反馈信息)
}
'left to right direction
admin -down->(借出图书)
admin -down->(归还图书)
admin -down->(维护书目)
admin -down->(维护读者信息)
reader -up->(查询书目)
reader -up->(查询借阅情况)
reader -up->(预定图书)
reader -up->(取消预定)
reader -up->(反馈信息)
(维护读者信息).>(更改读者信息):<<include>>

@enduml
```

* **用例图:**

![img](./picture/test2-1.png)

<br>


### 2.用例规约表

* **反馈信息:**

    [反馈信息](./markdown/usercase1.md)
    
* **取消预约:** 

    [取消预约](./markdown/usercase2.md)
    
* **预定图书:** 

    [取消预约](./markdown/usercase3.md)