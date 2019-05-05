# 接口: addClass | [返回](../Markdown/MaintainUserInfo.md)
用例：维护用户数据

* 功能：添加班级
* 权限：已登录的管理员
* API请求地址：接口基本地址/v1/api/addClass
* 请求方式：POST
* 请求实例:
```json
{
  "user_id": "001",
  "type": "manager",
  "data": {
    "college": "信息科学与工程学院",
    "subject": "软件工程",
    "grade": "2016",
    "class_num": "1"
  }
}
```
* 请求参数说明：

|   参数名称   |          说明          |
| :----------: | :--------------------: |
|   user_id    |         用户id         |
|     type     | 用户信息的类型 |
|     data     |    添加班级信息    |

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
