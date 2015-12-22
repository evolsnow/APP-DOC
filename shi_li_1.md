# 接口说明

这里是说明

## 


* **URL**
        /user/id

* **Method:**
  
  `GET` | `POST` | `DELETE` | `PUT`
  
*  **请求参数**

**键值** | **类型** | **可否为空** | **备注**
---------|----------|--------------|---------
foo|int|是|
key|value|否|
a|b|否|

* **请求成功:**
>#####Code: 200
>#####Content:

        { 
            id : 12 
        }
 


* **请求失败:**
>#####Code: 401 UNAUTHORIZED
>#####Content:
        { 
            error : "Log in" 
        }



* **Sample Call:**


* **Notes:**