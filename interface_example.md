# 接口说明

　用户登陆:server创建token并返回给client

## 


* **URL**
        /accessToken

* **Method:**
  
  ####<font color=green>`POST`</font>
  
*  **请求参数**

**键值** | **类型** | **是否必需** | **备注**
---------|----------|--------------|---------
phone|string|是|
password|string|是|md5 + salt

* **请求内容示例:**


        { 
            phone : "18612341234",
            password : "766aedb5723569cd44e3e7ee1f92a4ea"
        }
--- 
*  **返回参数说明**

**键值** | **类型** | **是否必需** | **备注**
---------|----------|--------------|---------
token    |string |是 |



* **返回内容示例:**


        { 
            code : 0,
            token : "Bearer abc.defg.hijk" 
        }


* **Notes:**

　　返回的`token`需要在`http header`中设置,即:

        Authorization: Bearer abc.defg.hijk