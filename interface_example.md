# 接口说明

　用户登陆:server创建token并返回给client

## 


* **URL**
        /accessToken

* **Method:**
  
  ####<font color=green>`POST`</font>
  
*  **请求参数**

**键值** | **类型** | **可否为空** | **备注**
---------|----------|--------------|---------
phone|string|否|
password|string|否|

* **请求内容示例:**


        { 
            phone : "18612341234",
            password : "766aedb5723569cd44e3e7ee1f92a4ea"
        }
--- 
*  **返回参数说明**

**键值** | **类型** | **可否为空** | **备注**
---------|----------|--------------|---------
token    |string |否 |



* **返回内容示例:**


        { 
            token : "Bearer abc.defg.hijk" 
        }


* **Notes:**

　　返回的`token`需要在`http header`中设置,即:

        `Authorization: Bearer abc.defg.hijk`