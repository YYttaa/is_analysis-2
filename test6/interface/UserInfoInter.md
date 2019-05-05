# 接口: userInfo | [返回](../Markdown/UserInfo.md)
用例：查看用户信息

* 功能：查看本用户的信息
* 权限：已登录的用户
* API请求地址：接口基本地址/v1/api/getUserInfo
* 请求方式：GET
* 请求实例:
```json
{
  "user_id": "001",
  "type": "student"
}
```
* 请求参数说明：

| 参数名称 |     说明     |
| :------: | :----------: |
| user_id  |    用户id    |
|   type   | 用户登录类型 |

* 返回实例：
```json
{
  "status": "true",
  "user_id": "001",
  "data": {
       "user_id": "001",
       "student_id": "201610414112",
       "class_id": "2016104141",
       "name": "tyh",
       "github_username": "dztyh",
       "update_date": "2019-05-01",
       "password": "bf2d4040bfe9ce2b6b8a47a75945dad2",
       "disable": "true",
       "web_sum": "true"
  },
  "info":""
}
```
* 返回参数说明:

| 参数名称 |             说明             |
| :------: | :--------------------------: |
|  status  |           请求状态           |
| user_id  |         登录用户的id         |
|   data   |           用户信息           |
|   info   | 额外的信息，可以存放错误信息 |
