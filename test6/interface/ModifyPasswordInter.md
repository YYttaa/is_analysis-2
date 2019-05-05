# 接口: modifyPassword | [返回](../Markdown/ModifyPassword.md)
用例：修改密码

* 功能：修改本用户的密码
* 权限：已登录的用户
* API请求地址：接口基本地址/v1/api/modifyPassword
* 请求方式：UPDATE
* 请求实例:
```json
{
  "user_id": "001",
  "type": "student",
  "old_password": "aaa321",
  "new_password": "aaa321!",
  "re_password": "aaa321!"
}
```
* 请求参数说明：

|   参数名称   |     说明     |
| :----------: | :----------: |
|   user_id    |    用户id    |
|     type     | 用户登录类型 |
| old_password |    旧密码    |
| new_password |    新密码    |
| re_password  |   确认密码   |

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
