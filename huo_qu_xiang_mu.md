# 获取用户项目

## 接口说明

　获取用户加入/创建的项目

## 


* **URL**
        /projects

* **Method:**
  
  ####<font color=blue>`GET`</font>

* **权限:**

  `medium`

*  **请求参数**

**键值** | **类型** | **是否必需** | **备注**
---------|----------|--------------|---------
type|string|否|项目类型

* **请求内容示例:**


        /projects 该用户的所有项目
        
        /projects?type=joined 该用户已加入的所有项目
        
        /projects?type=created 该用户已创建的所有项目
--- 
*  **返回参数说明**

**键值** | **类型** | **是否必需** | **备注**
---------|----------|--------------|---------
available    |bool |是 |是否可用
msg      |string|否 |不可用原因

* **返回成功示例:**


        {
            "available": false,
            "msg": "illegal char: #"
        } 


