# 数据库设计 [首页](../README.md)
* ## students表(学生表)

|      字段       |    类型     | 主键，外键 | 可以为空 | 默认值 |      约束      |          说明          |
| :-------------: | :---------: | :--------: | :------: | :----: | :------------: | :--------------------: |
|     user_id     |   bigint    | 联合主键1  |    否    |  自增  |                |        用户编号        |
|   student_id    |   bigint    | 联合主键2  |    否    |        |                |          学号          |
|    class_id     |   bigint    |    外键    |    否    |        | class.class_id |         班级号         |
|      name       | varchar(50) |            |    否    |        |                |          姓名          |
| github_username | varchar(80) |            |    否    |        |                |     用户GitHub账号     |
|   update_date   |  datetime   |            |    否    |        |                | 用户GitHub账号修改日期 |
|    password     | varchar(50) |            |    否    |        |                |          密码          |
|     disable     | varchar(20) |            |    否    |        |                |      用户是否禁用      |
|     web_sum     | varchar(20) |            |    否    |        |                |    网站正确与否汇总    |
* ## teachers表(教师表)

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

* ## manager表(管理员表)

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

* ## class表(班级表)

|   字段    |    类型     | 主键，外键 | 可以为空 | 默认值 | 约束 |   说明   |
| :-------: | :---------: | :--------: | :------: | :----: | :--: | :------: |
| class_id  |   bigint    |    主键    |    否    |  自增  |      | 班级编号 |
|  college  | varchar(50) |            |    否    |        |      | 所属学院 |
|  subject  | varchar(50) |            |    否    |        |      |   专业   |
|   grade   |     int     |            |    否    |        |      |   年级   |
| class_num |     int     |            |    否    |        |      |  班级号  |

* ## course(课程表)

|     字段      |     类型     | 主键，外键 | 可以为空 | 默认值 |        约束         |   说明   |
| :-----------: | :----------: | :--------: | :------: | :----: | :-----------------: | :------: |
|   course_id   |    bigint    |    主键    |    否    |  自增  |                     | 课程编号 |
|  course_name  | varchar(100) |            |    否    |        |                     | 课程名称 |
| course_detail | varchar(255) |            |    否    |        |                     | 课程描述 |
|  teacher_id   |    bigint    |    外键    |    否    |        | teachers.teacher_id | 教师编号 |

* ## tests(实验表)

|     字段     |     类型     | 主键，外键 | 可以为空 | 默认值 |       约束       |   说明   |
| :----------: | :----------: | :--------: | :------: | :----: | :--------------: | :------: |
|   tests_id   |    bigint    |    主键    |    否    |  自增  |                  | 实验编号 |
|  tests_name  | varchar(100) |            |    否    |        |                  | 实验名称 |
| tests_detail | varchar(255) |            |    否    |        |                  | 实验描述 |
|  course_id   |    bigint    |    外键    |    否    |        | course.course_id | 课程编号 |

* ## score_rules(评分细则表)

|     字段      |     类型     | 主键，外键 | 可以为空 | 默认值 |     约束      |                  说明                  |
| :-----------: | :----------: | :--------: | :------: | :----: | :-----------: | :------------------------------------: |
|   rules_id    |    bigint    |    主键    |    否    |  自增  |               |                细则编号                |
| rules_percent |    float     |            |    否    |        |               | 细则分数占比<br />最大值为1，最小值为0 |
| rules_detail  | varchar(255) |            |    否    |        |               |                细则描述                |
|    test_id    |    bigint    |    外键    |    否    |        | test.tests_id |                实验编号                |

* ## select_course(学生选课表)

|    字段    |     类型     | 主键，外键 | 可以为空 | 默认值 |        约束         |   说明   |
| :--------: | :----------: | :--------: | :------: | :----: | :-----------------: | :------: |
| select_id  |    bigint    |    主键    |    否    |  自增  |                     | 选课编号 |
| student_id |    bigint    |    外键    |    否    |        | students.student_id | 学生编号 |
| course_id  |    bigint    |    外键    |    否    |        |  course.course_id   | 课程编号 |
| all_score  |    float     |            |    是    |   0    |                     |  总分数  |
|    memo    | varchar(255) |            |    是    |        |                     |   评语   |

* ## test_score(实验评分表)

|   字段    |  类型  | 主键，外键 | 可以为空 | 默认值 |          约束           |     说明     |
| :-------: | :----: | :--------: | :------: | :----: | :---------------------: | :----------: |
| score_id  | bigint |    主键    |    否    |  自增  |                         |   分数编号   |
| select_id | bigint |    外键    |    否    |        | select_course.select_id |   选课编号   |
|  test_id  | bigint |    外键    |    否    |        |      tests.test_id      |   实验编号   |
| rules_id  | bigint |    外键    |    否    |        |  score_rules.rules_id   | 评分细则编号 |
|  result   | float  |            |    否    |        |                         |     分数     |



