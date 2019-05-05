# 接口：getClass  [返回](../README.md)
用例： [选课](../用例/选课.md)

- 功能：
    选择老师所教授的课程。
    
- 权限：    
    老师和同学都可以选多门课程，但必须是老师先选，学生后选。
    
- API请求地址： 
    接口基本地址/v1/api/getClass /<is_next>/<student_id>

- 请求方式 ：
    GET

- 请求参数说明:        

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |student_id|学生的学号|
  |class_id|NUMBER(6,0)|主键|否| | | 课程编号|
  |class_name|VARCHAR2(400 BYTE)| |否| | |课程名称|
  |teacher_id|VARCHAR2(50 BYTE)| 外键|否| | |所教授的老师名字|
    
- 返回实例：

        {         
            "status": true,
            "info": null,    
            "student_id": "201510315203"
            "class_id":023
            "class_name":java基础入门
            "teacher_id":张志强
        }
 
- 返回参数说明：    
 
  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |status|bool类型，true表示正确的返回，false表示有错误|
  |info|返回结果说明信息|
  |student_id|学号|
  |class_id|课程编号|
  |class_name|课程名称|
  |teacher_id|所教授的老师名字|

