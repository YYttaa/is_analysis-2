# 接口: getSelectCourseStu | [返回](../Markdown/SelectCourse.md)
用例：评定成绩

* 功能：查询选择本课程的学生
* 权限：已登录的教师
* API请求地址：接口基本地址/v1/api/getSelectCourseStu
* 请求方式：GET
* 请求实例:
```json
{
  "user_id": "001",
  "type": "teacher",
  "course_id": "10000001"
}
```
* 请求参数说明：

|  参数名称   |          说明          |
| :---------: | :--------------------: |
|   user_id   |         用户id         |
|    type     |    当前登录用户类型    |
|    course_id     |    课程id    |

* 返回实例：
```json
{
  "status": "true",
  "user_id": "001",
  "info":"",
  "data": [
      {
          "user_id": "001",
          "student_id": "201610414112",
          "class_id": "2016104141",
          "name": "tyh",
          "github_username": "scdztyh",
          "update_date": "2019-05-01",
          "password": "bf2d4040bfe9ce2b6b8a47a75945dad2",
          "disable": "true",
          "web_sum": "true"
      },
      {
          "user_id": "002",
          "student_id": "201610414111",
          "class_id": "2016104141",
          "name": "tyh",
          "github_username": "dztyh",
          "update_date": "2019-05-01",
          "password": "bf2d4040bfe9ce2b6b8a47a75945dad2",
          "disable": "true",
          "web_sum": "true"
      }
    ]
}
```
* 返回参数说明:

| 参数名称 |             说明             |
| :------: | :--------------------------: |
|  status  |           请求状态           |
| user_id  |         登录用户的id         |
|   data   |    所有选择本课程学生的信息,类型为一个数组     |
|   info   | 额外的信息，可以存放错误信息 |
