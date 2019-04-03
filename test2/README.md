# 实验2:图书管理系统用例建模

|学号|班级|姓名|
|----|------|----|
|201610414112|软件（本）16-1|唐银浩|

## 1.图书管理系统用例图
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
    (增加书目信息)
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
(维护书目).>(增加书目信息):<<include>>

@enduml
```

* **用例图:**

![img](./picture/test2-1.png)

<br>

## 2.参与者说明

#### 2.1图书管理员
主要职责是维护及管理图书，并负责图书的外借与归还。

#### 2.2读者
主要职责是查看自己的借阅情况，搜索图书并预定借书。

<br>

## 3.用例规约表

#### 【读者规约表】

* **反馈信息规约表:**

    [反馈信息](./markdown/usercase1.md)
    
* **取消约定规约表:** 

    [取消约定](./markdown/usercase2.md)
    
* **预定图书规约表:** 

    [预定图书](./markdown/usercase3.md)
    
* **查询借阅情况规约表:** 
    
    [查询借阅情况](./markdown/usercase4.md)
        
* **查询书目规约表:** 
    
    [查询书目](./markdown/usercase5.md)
    
   <br>
    
#### 【图书管理员规约表】
        
* **增加图书信息规约表:** 
    
    [增加图书信息](./markdown/usercase6.md)
        
* **维护书目规约表:** 
    
    [维护书目](./markdown/usercase7.md)
        
* **借出图书规约表:** 
    
    [借出图书](./markdown/usercase8.md)
        
* **归还图书规约表:** 
    
    [归还图书](./markdown/usercase9.md)
            
* **维护读者信息规约表:** 
    
    [维护读者信息](./markdown/usercase10.md)