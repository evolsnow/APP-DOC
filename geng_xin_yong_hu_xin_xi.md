# 更新用户信息

## 接口说明

　更新User个人中心内容

## 


* **URL**
        /users/personalInfo
        

* **Method:**
  
  ####<font color=orange>`PUT`</font>

* **权限:**

  `medium`

*  **请求参数**

**键值** | **类型** | **是否必需** | **备注**
---------|----------|--------------|---------
alias|string|否|昵称
name|string|否|名称
avatar|string|否|头像(仅支持七牛)

*  **请求内容示例:**


        { 
            "alias": "new_alias",
            "avatar": "fjsiodfjiower.jpg",
        }
--- 
*  **返回参数说明**

    基本返回
