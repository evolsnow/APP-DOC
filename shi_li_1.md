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

* **Success Response:**
  

  * **Code:** 200
 
  
  * **Content:** 
        { 
            id : 12 
        }
 
* **Error Response:**


  * **Code:** 401 UNAUTHORIZED <br />
    **Content:** 
        { 
            error : "Log in" 
        }

  OR

  * **Code:** 422 UNPROCESSABLE ENTRY <br />
    **Content:** 
        { 
            error : "Email Invalid" 
        }

* **Sample Call:**


* **Notes:**