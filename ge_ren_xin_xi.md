# 个人信息

## 接口说明

　用户个人信息

## 


* **URL**
        /users/personalInfo

* **Method:**
  
  ####<font color=blue>`GET`</font>

* **权限:**

  `medium`

*  **请求参数**

无

-------------------------- 
*  **返回参数说明**

**键值** | **类型** | **是否必需** | **备注**
---------|----------|--------------|---------
code    |int |是 |请求结果
id|     string|是|用户id
name|   string|是|名称
avatar| string |是|头像url
alias|string|否|昵称
mail|string|是|邮箱地址
stuNum|string|否|学号

* **返回成功示例:**


        {
            "code": 0,
            "id": "fasdf24r2",
            "avatar": "http://qiniu_domain/?e=1461405089\u0026token=access_key:GLfl3nGnSzRIYwQUuEv0l0LHGOA",
            "mail": "abc@def.com",
            "name": "李四",
            "stuNum": "1218404004"
        } 