<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# 接口：setOneTest  [返回](../README.md)
用例： [发布实验](../用例/发布实验.md)

- 功能：
    发布一条实验信息。
    
    
- 权限：
    老师：给学生布置课后作业。
    
- API请求地址： 
    接口基本地址/v1/api/setOneTest

- 请求方式 ：
    POST
 
- 请求实例：  

        { 
            "status": true,
            "info": null,  
            "course_name":"软件工程分析与设计"
            "data": [
                {
                "test_id":1,
                "title":"实验4：图书管理系统顺序图绘制",
                "summary": "本实验……"
                "update_date":"2018-05-01 13:48:01",
                "teacher_name": "赵卫东"
                }, 
                {
                ...其他实验
                }
            ] 
        }

- 请求参数说明:       
 
  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |status|bool类型，true表示正确的返回，false表示有错误|
  |info|返回结果说明信息|
  |course_name|返回课程信息|      
  |test_id|实验编号|
  |title|实验名称|
  |summary|实验简介|   
  |update_date|批改日期|
  |teacher_name|批改教师|   
