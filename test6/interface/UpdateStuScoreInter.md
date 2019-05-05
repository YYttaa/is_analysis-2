# 接口: updateStuScore | [返回](../Markdown/SelectCourse.md)
用例：评定成绩，查看成绩

* 功能：查询本学生本课程的实验分数
* 权限：已登录的教师或学生
* API请求地址：接口基本地址/v1/api/updateStuScore
* 请求方式：UPDATE
* 请求实例:
```json
{
  "user_id": "001",
  "type": "teacher",
  "data": {
    "select_id": "10000001",
    "rules_id": "10000003",
    "test_id": "10000003",
    "result": "85.0"
  }
}
```
* 请求参数说明：

|  参数名称   |          说明          |
| :---------: | :--------------------: |
|   user_id   |         用户id         |
|    type     |    当前登录用户类型    |
|     data     |    添加课程信息    |

* 返回实例：
```json
{
    "status": "true",
    "user_id": "001",
    "info":""
}
```
* 返回参数说明:

| 参数名称 |             说明             |
| :------: | :--------------------------: |
|  status  |           请求状态           |
| user_id  |         登录用户的id         |
|   info   | 额外的信息，可以存放错误信息 |
