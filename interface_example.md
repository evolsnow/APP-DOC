# 接口说明

这里是说明

## 


* **URL**
        /book/id

* **Method:**
  
  ####<font color=red>`GET` | `POST` | `DELETE` | `PUT`</font>
  
*  **请求参数**

**键值** | **类型** | **可否为空** | **备注**
---------|----------|--------------|---------
foo|int|是|
key|value|否|
a|b|否|

* **请求成功示例:**


        { 
            name : "c book",
            price: 12
        }
 
*  **返回参数说明**

**键值** | **类型** | **可否为空** | **备注**
---------|----------|--------------|---------
name    |string |否 |
price   |float  |否 |
author  |string |否 |


* **请求失败示例:**


        { 
            error : "unauthorized" 
        }



* **Sample Call:**


* **Notes:**