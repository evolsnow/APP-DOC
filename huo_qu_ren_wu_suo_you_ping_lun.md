# 获取任务所有评论


## 接口说明

　获取某任务所有评论

## 


* **URL**
        /missions/comments/:mission

* **Method:**
  
  ####<font color=blue>`GET`</font>

* **权限:**

  `medium`

*  **请求参数**

**键值** | **类型** | **是否必需** | **备注**
---------|----------|--------------|---------
type|string|否|项目类型

* **请求内容示例:**


        /missions/comments/djio23ejdo2jdrqwerqewqeqw
------------------------------------------- 
*  **返回参数说明**

**键值** | **类型** | **是否必需** | **备注**
---------|----------|--------------|---------
comments    |[]comment |是 |任务数组

* **ms内容示例:**


        {
            "id": "361916bfc04042177f9a0fe8e0a81c62",
            "userId": "213r2qgfr43fg4",
            "userName": "user name",
            "when": 147258369
        }

* **返回成功示例:**


        {
            "code": 0,
            "comments": [
                {
                    "id": "361916bfc04042177f9a0fe8e0a81c62",
                    "userId": "213r2qgfr43fg4",
                    "userName": "user name",
                    "when": 147258369
                },
                {
                    "id": "361916bfc04042177f9a0fe8e0a81c62",
                    "userId": "213r2qgfr43fg4",
                    "userName": "user name",
                    "when": 147258369
                }
            ]
        } 