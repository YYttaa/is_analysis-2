# 接口: getTestsRules | [返回](../Markdown/SelectCourse.md)
用例：评定成绩

* 功能：查询选择本实验的所有评分标准
* 权限：已登录的教师
* API请求地址：接口基本地址/v1/api/getTestsRules
* 请求方式：GET
* 请求实例:
```json
{
  "user_id": "001",
  "type": "teacher",
  "test_id": "10000001"
}
```
* 请求参数说明：

|  参数名称   |          说明          |
| :---------: | :--------------------: |
|   user_id   |         用户id         |
|    type     |    当前登录用户类型    |
|    course_id     |    实验id    |

* 返回实例：
```json
{
  "status": "true",
  "user_id": "001",
  "info":"",
  "data": [
      {
         "rules_id": "10000001",
         "rules_percent": "0.25",
         "rules_detail": "格式规范",
         "test_id": "10000001"
      },
      {
           "rules_id": "10000002",
           "rules_percent": "0.25",
           "rules_detail": "完成度",
           "test_id": "10000001"
      }
    ]
}
```
* 返回参数说明:

| 参数名称 |             说明             |
| :------: | :--------------------------: |
|  status  |           请求状态           |
| user_id  |         登录用户的id         |
|   data   |    本实验所有评分标准的信息,类型为一个数组     |
|   info   | 额外的信息，可以存放错误信息 |
