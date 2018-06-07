<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# 接口：getcourses  [返回](../README.md)
用例： [实验信息](../用例/实验信息.md)，[课程信息](../用例/课程信息.md)

- 功能：
    查看老师发布的实验信息、课程信息
    
- 权限：
    学生/老师：查看老师发布的实验信息，必须先登录，不能查看的信息。    
    
- API请求地址： 
    接口基本地址/v1/api/getcourses

- 请求方式 ：
    GET
      
- 请求参数说明:        

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |courses_id|课程编号|
  
- 返回实例：

        {         
            "status": true,
            "info": null,
            "courses_id":km0,
            "courses_name":软件工程分析与设计,
            "summary":该课程……,
            "teacher_name":赵卫东,          
        }
 
- 返回参数说明：    
 
  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |status|bool类型，true表示正确的返回，false表示有错误|
  |info|返回结果说明信息|
  |courses_id|课程编号|
  |courses_name|课程名|
  |summary|课程简绍|
  |teacher_name|发布课程教师的姓名|  
