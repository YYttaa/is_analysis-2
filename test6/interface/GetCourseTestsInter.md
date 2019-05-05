# 接口: getCourseTests | [返回](../Markdown/SelectCourse.md)
用例：评定成绩

* 功能：查询本课程的所有实验
* 权限：已登录的教师
* API请求地址：接口基本地址/v1/api/getCourseTests
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
         "tests_id": "10000001",
         "tests_name": "掌握git基本操作",
         "tests_detail": "掌握git基本操作是很重要的",
         "course_id": "10000001"
      },
      {
          "tests_id": "10000002",
          "tests_name": "掌握git高级操作",
          "tests_detail": "掌握git高级操作是很重要的",
          "course_id": "10000001"
      }
    ]
}
```
* 返回参数说明:

| 参数名称 |             说明             |
| :------: | :--------------------------: |
|  status  |           请求状态           |
| user_id  |         登录用户的id         |
|   data   |    所有本课程实验的信息,类型为一个数组     |
|   info   | 额外的信息，可以存放错误信息 |
