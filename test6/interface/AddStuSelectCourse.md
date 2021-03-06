# 接口: addStuSelectCourse | [返回](../Markdown/SelectCourse.md)
用例：学生选课

* 功能：添加学生选课信息
* 权限：已登录的学生
* API请求地址：接口基本地址/v1/api/addStuSelectCourse
* 请求方式：POST
* 请求实例:
```json
{
  "user_id": "001",
  "type": "student",
  "data": {
    "course_name": "信息系统",
    "course_detail": "信息系统是一门好课",
    "teacher_id": "001"
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

