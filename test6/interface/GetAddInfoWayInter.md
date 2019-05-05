# 接口: getAddInfoWay | [返回](../Markdown/MaintainUserInfo.md)
用例：用户列表

* 功能：获取可添加信息方式
* 权限：已登录的管理员
* API请求地址：接口基本地址/v1/api/getAddInfoWay
* 请求方式：GET
* 请求实例:
```json
{
  "user_id": "001",
  "type": "manager"
}
```
* 请求参数说明：

|   参数名称   |       说明       |
| :----------: | :--------------: |
|   user_id    |      用户id      |
|     type     | 当前登录用户类型 |

* 返回实例：
```json
{
  "status": "true",
  "user_id": "001",
  "info":"",
  "data": [
    {
      "way": "xml"
    },
    {
      "way": "sql"
    }
  ]
}
```
* 返回参数说明:

| 参数名称 |             说明             |
| :------: | :--------------------------: |
|  status  |           请求状态           |
| user_id  |         登录用户的id         |
|   data   |     所有的可添加方式,类型为一个数组    |
|   info   | 额外的信息，可以存放错误信息 |
