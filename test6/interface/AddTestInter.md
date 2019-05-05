# 接口: addTest | [返回](../Markdown/AddTests.md)
用例：设定实验

* 功能：添加实验信息
* 权限：已登录的教师
* API请求地址：接口基本地址/v1/api/addTest
* 请求方式：POST
* 请求实例:
```json
{
  "user_id": "001",
  "type": "teacher",
  "data": {
    "tests_name": "掌握git基本操作",
    "tests_detail": "掌握git基本操作是很重要的",
    "course_id": "10000001"
  }
}
```
* 请求参数说明：

|   参数名称   |          说明          |
| :----------: | :--------------------: |
|   user_id    |         用户id         |
|     type     | 用户信息的类型 |
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
