# 接口: getStuScore | [返回](../Markdown/SelectCourse.md)
用例：评定成绩，查看成绩

* 功能：查询本学生本课程的实验分数
* 权限：已登录的教师或学生
* API请求地址：接口基本地址/v1/api/getStuScore
* 请求方式：GET
* 请求实例:
```json
{
  "user_id": "001",
  "type": "teacher",
  "select_id": "10000001"
}
```
* 请求参数说明：

|  参数名称   |          说明          |
| :---------: | :--------------------: |
|   user_id   |         用户id         |
|    type     |    当前登录用户类型    |
|    select_id     |    选课id    |

* 返回实例：
```json
{
  "status": "true",
  "user_id": "001",
  "info":"",
  "data": [
      {
         "score_id": "10000001",
         "select_id": "10000001",
         "rules_id": "10000001",
         "test_id": "10000001",
         "result": "85.0"
      },
      {
        "score_id": "10000002",
        "select_id": "10000001",
        "rules_id": "10000002",
        "test_id": "10000001",
        "result": "87.5"
      }
    ]
}
```
* 返回参数说明:

| 参数名称 |             说明             |
| :------: | :--------------------------: |
|  status  |           请求状态           |
| user_id  |         登录用户的id         |
|   data   |    本实验所有分数的信息,类型为一个数组     |
|   info   | 额外的信息，可以存放错误信息 |
