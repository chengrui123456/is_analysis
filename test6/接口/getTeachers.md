# 接口：getTeachers  [返回](../README.md)
用例： [老师列表](../用例/老师列表.md)

- 权限：<br>
    学生/访客：不能看到RESULT_SUM，WEB_SUM<br>
    老师/管理员：可以看到RESULT_SUM，WEB_SUM。

- 功能：
    返回所有老师的列表。

- API请求地址：
   接口基本地址/v1/api/getTeachers

- 请求方式 ：
    GET

- 请求参数说明:
    无

- 返回实例：

        {
            "status": true,
            "info": null,
            "total": 121,
            "data": [
                {
                "TEACHER_ID": "201610414404",
                "USER_ID": "02356",
                "NAME": "陈少义",
                "DEPARTMENT": "IT类"
                "GITHUB_USERNAME": "**********"
                },
                {
                ...其他老师
                }
            ]
        }

- 返回参数说明：

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |status|bool类型，true表示正确的返回，false表示有错误|
  |info|返回结果说明信息|
  |total|返回老师人数|
  |data|所有老师的数组|
  |TEACHER_ID|GITHUB 用户名|
  |USER_ID|学号|
  |NAME| 名字|
  |DEPARTMENT|所属部门|
  |GITHUB_USERNAME|github 用户名|
