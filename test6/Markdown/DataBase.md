## 数据库设计 [首页](../README.md)
* students表(学生表)

|      字段       |    类型     | 主键，外键 | 可以为空 | 默认值 | 约束 |          说明          |
| :-------------: | :---------: | :--------: | :------: | :----: | :--: | :--------------------: |
|     user_id     |   bigint    | 联合主键1  |    否    |  自增  |      |        用户编号        |
|   student_id    |   bigint    | 联合主键2  |    否    |        |      |          学号          |
|    class_id     |   bigint    |            |    否    |        |      |         班级号         |
|      name       | varchar(50) |            |    否    |        |      |          姓名          |
| github_username | varchar(80) |            |    否    |        |      |     用户GitHub账号     |
|   update_date   |  datetime   |            |    否    |        |      | 用户GitHub账号修改日期 |
|    password     | varchar(50) |            |    否    |        |      |          密码          |
|     disable     | varchar(20) |            |    否    |        |      |      用户是否禁用      |
|     web_sum     | varchar(20) |            |    否    |        |      |    网站正确与否汇总    |

* teachers表(教师表)

|      字段       |    类型     | 主键，外键 | 可以为空 | 默认值 | 约束 |          说明          |
| :-------------: | :---------: | :--------: | :------: | :----: | :--: | :--------------------: |
|     user_id     |   bigint    | 联合主键1  |    否    |  自增  |      |        用户编号        |
|   teacher_id    |   bigint    | 联合主键2  |    否    |        |      |        教师编号        |
|      name       | varchar(50) |            |    否    |        |      |          姓名          |
| github_username | varchar(80) |            |    否    |        |      |     用户GitHub账号     |
|   update_date   |  datetime   |            |    否    |        |      | 用户GitHub账号修改日期 |
|    password     | varchar(50) |            |    否    |        |      |          密码          |
|     disable     | varchar(20) |            |    否    |        |      |      用户是否禁用      |
|     web_sum     | varchar(20) |            |    否    |        |      |    网站正确与否汇总    |
|   department    | varchar(50) |            |    否    |        |      |      老师所属部门      |

* manager表(管理员表)

|      字段       |    类型     | 主键，外键 | 可以为空 | 默认值 | 约束 |          说明          |
| :-------------: | :---------: | :--------: | :------: | :----: | :--: | :--------------------: |
|     user_id     |   bigint    | 联合主键1  |    否    |  自增  |      |        用户编号        |
|   manager_id    |   bigint    | 联合主键2  |    否    |        |      |       管理员编号       |
|      name       | varchar(50) |            |    否    |        |      |          姓名          |
| github_username | varchar(80) |            |    否    |        |      |     用户GitHub账号     |
|   update_date   |  datetime   |            |    否    |        |      | 用户GitHub账号修改日期 |
|    password     | varchar(50) |            |    否    |        |      |          密码          |
|     disable     | varchar(20) |            |    否    |        |      |      用户是否禁用      |
|     web_sum     | varchar(20) |            |    否    |        |      |    网站正确与否汇总    |
