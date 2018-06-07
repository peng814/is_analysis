<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# 接口：setOneStudentResults  [返回](../README.md)
用例： [评定成绩](../用例/评定成绩.md)

- 功能：
    设置一个学生的部分实验成绩和评语。
    
    输入参数result不为空，自动设置update_date为当前日期，表示同时设置批改日期。
    
    输入参数result为空，自动设置update_date为空，表示未批改。
    
- 权限：
    老师：可以查看所有学生的成绩。
    
- API请求地址： 
    接口基本地址/v1/api/etOneStudentResults

- 请求方式 ：
    POST
 
- 请求实例：  

        { 
            "status": true,
            "info": null,  
            "course_name":"软件工程分析与设计"
            "student_id": "201510315203", 
            "github_username": "chinajuedui", 
            "class": "软件(本)15-1", 
            "name": "陈松华", 
            "total": 6,
            "data": [
                {
                "test_id":1,
                "standard":
                    "1.实验完成程度是否达标（20分）","18",
                    "2.各图是否相互联系（20分）"，"18",
                    "3.……（20）","18",
                    "4.……（20）","18",
                    "5.……（20）","18",
                "result": 90, 
                "memo":"本实验做得好",
                "update_date": "2018-04-02 13:48:01"
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
  |student_id|学号|
  |github_username|学生的gitHub用户名|
  |class|班级|
  |name|真实姓名|  
  |total|本次批改的所有实验的总数，小于等于全部实验的总数|
  |data|实验的成绩和评语|
  |test_id|实验编号|
  |standard|评分标准|
  |result|本实验成绩，可以为空，为空表示没有批改。|
  |memo|本实验老师的评价，可以为空|
  |update_date|本实验老师的批改日期，可以为空|   
 
