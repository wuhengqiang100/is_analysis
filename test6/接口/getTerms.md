﻿# 接口：getTerms[返回](../README.md)
用例： [查询学期](../用例/查询学期.md)，[查询学期](../用例/查询学期.md)

- 功能：
    查询不同的学期有哪些学期.
    
- 权限：
    无,都可以查询学期
    
- API请求地址： 
    接口基本地址/v1/api/getCourses

- 请求方式 ：
    GET

- 请求参数说明:        

     无
    
- 返回实例：

        {         
            "status": true,
            "info": null,
            "data": [
                {
                    "term_id":"1",
                    "name":"大三下学期",
                },
                 {
                    "term_id":"2",
                    "name":"大三上学期",
                },
                {
                    ...其他学期信息
                }       
            ] 
        }
 
- 返回参数说明：    
 
  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |status|bool类型，true表示正确的返回，false表示有错误|
  |info|返回结果说明信息|
  |term_id|学期编号|
  |name|学期名称|   

