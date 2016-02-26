# 新建Todo

## 接口说明

　新建Todo对象

## 


* **URL**
        /todos

* **Method:**
  
  ####<font color=green>`POST`</font>

* **权限:**

  `medium`

  
*  **请求参数**

**键值** | **类型** | **是否必需** | **备注**
---------|----------|--------------|---------
desc|string|是|todo事件描述
deadline|uint64|是|结束时间
ownerId|string|是|创建者
startTime|string|否|默认则由服务器生成
accomplished|string|否|默认false
missionId|string|否|

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

        Authorization: Bearer abc.defg.hijk