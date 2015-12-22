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
> 
> > Code: 100
 
  
Content:

        { 
            id : 12 
        }
 


* **请求失败:**


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