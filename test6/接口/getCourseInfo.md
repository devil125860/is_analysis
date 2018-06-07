# 接口：getCourseInfo  [返回](../../README.md)
用例： [查看课程信息](../用例/查看课程信息.md),[修改课程信息](../用例/修改课程信息.md)

- 功能：
    查看指定课程的信息。
    
- 权限：
    学生/老师：查看所修/所任教课程信息，不能查看其他课程的信息。    
    
- API请求地址： 
    接口基本地址/v1/api/getCourseInfo/<course_id>

- 请求方式 ：
    GET
      
- 请求参数说明:        

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |course_id|课程的ID号。对应表COURSES.COURSE_ID的值|
  
- 返回实例：

        {         
            "status": true,
            "info": null,
            "data": {
                "course_id": "0123456"
                "course_name": "JAVA"
                "course_content": "JAVA是一门基础的语言。"
                "course_term": "2015-2016学年第1学期"
                "course_major": "软件工程"
            }          
        }
 
- 返回参数说明：    
 
  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |status|bool类型，true表示正确的返回，false表示有错误|
  |info|返回结果说明信息|
  |data|返回主体信息JSON串|
  |course_id|课程编号|
  |course_name|课程名称|  
  |course_content|课程简介|
  |course_class|开课班级|