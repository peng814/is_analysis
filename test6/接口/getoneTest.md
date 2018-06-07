<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# 接口：getOneTest  [返回](../README.md)
用例： [查看实验](../用例/实验信息.md)，[发布实验](../用例/发布实验.md)

- 功能：
    用于查看老师所发布的实验信息。
    
- 权限：
    学生、老师
    
- API请求地址： 
    接口基本地址/v1/api/getOnetest

- 请求方式 ：
    GET

- 请求参数说明:        

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |test_id|实验编号|
    
- 返回实例：

        {         
            "status": true,
            "info": null,    
            "courses_name": "软件工程分析与设计", 
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
 
- 返回参数说明：    
 
  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |status|bool类型，true表示正确的返回，false表示有错误|
  |info|返回结果说明信息|
  |courses_name|课程名|
  |test_id|实验编号|
  |title|实验名称|
  |summary|实验简介|   
  |update_date|批改日期|
  |teacher_name|批改教师|   
