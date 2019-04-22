# 实验4:图书管理系统数据库设计与界面设计

|学号|班级|姓名|
|----|------|----|
|201610414112|软件（本）16-1|唐银浩|

## 1.数据库表设计
### 1.1馆藏表(collect)
|  字段   |     类型     | 主键，外键 | 可以为空 | 默认值 | 约束 |   说明   |
| :-----: | :----------: | :--------: | :------: | :----: | :--: | :------: |
|   id    |     bigint   |    主键    |    否    |  自增  |      | 馆藏编号 |
| address | varchar(150) |            |    否    |   ""   |      | 馆藏地点 |

### 1.2图书表(book)
|     字段     |     类型     | 主键，外键 | 可以为空 | 默认值 |    约束    |    说明    |
| :----------: | :----------: | :--------: | :------: | :----: | :--------: | :--------: |
|   book_id    |    bigint    |    主键    |    否    |  自增  |            |  图书编号  |
|  book_name   | varchar(150) |            |    否    |   ""   |            |    书名    |
|    author    | varchar(150) |            |    否    |   ""   |            |    作者    |
|    pirce     |    float     |            |    否    |  0.0   |            |    价格    |
|     ISBN     | varchar(150) |            |    否    |   ""   |            | 国际出版号 |
|    detail    | varchar(255) |            |    是    |   ""   |            |    简介    |
| collect_add  |    bigint    |    外键    |    否    |        | collect.id |  馆藏位置  |
| collect_num  |    bigint    |            |    否    |   0    |            |  馆藏数量  |
| borrowed_num |    bigint    |            |    否    |   0    |            |  可借数量  |
|  book_kind   |    bigint    |    外键    |    否    |        |  kind.id   |  图书类别  |

### 图书种类表(kind)
|   字段    |     类型     | 主键，外键 | 可以为空 | 默认值 | 约束 |   说明   |
| :-------: | :----------: | :--------: | :------: | :----: | :--: | :------: |
|    id     |    bigint    |    主键    |    否    |  自增  |      | 类别编号 |
| kind_name | varchar(150) |            |    否    |   ""   |      | 类别名称 |
|  detail   | varchar(150) |            |    是    |   ""   |      | 类别描述 |