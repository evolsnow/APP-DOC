# 获取项目详情

## 接口说明

　获取项目详细信息

## 


* **URL**
        /projects/:pid

* **Method:**
  
  ####<font color=blue>`GET`</font>

* **权限:**

  `medium`

*  **请求参数**

**键值** | **类型** | **是否必需** | **备注**
---------|----------|--------------|---------
pid|string|是|项目id

* **请求内容示例:**


        /projects/r28rjiewqj2jej2
        
--- 
*  **返回参数说明**

**键值** | **类型** | **是否必需** | **备注**
---------|----------|--------------|---------
id    |string |是 |项目数组
name|string|是|项目名称
desc|string|否|项目描述
creatorId|string|是|创建者id
creatorName|string|是|创建者姓名
private|bool|否|是否私有
members|[]user|否|成员

* **返回成功示例:**


        {
            "id": "adjapfdjp3q2wekp2",
            "name": "项目名称",
            "desc": "项目描述",
            "creatorId": "eq23dfwejfpw",
            "creatorName": "evol",
            "private": false,
            "members": [{
                         "id": "e12e1",
                         "name": "张三",
                         "avatar": "http://qdwqwq.jpg"
                        },
                         "id": "afdsfwe",
                         "name": "李四",
                         "avatar": "http://qdwqfew.jpg"
                        }]
        } 

