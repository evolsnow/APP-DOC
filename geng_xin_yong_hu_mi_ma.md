# 更新用户密码

## 接口说明

　更新用户密码

##


* **URL**
        /users/:identify
        
        （identify为用户手机号/邮箱/samId）

* **Method:**
  
  ####<font color=orange>`PUT`</font>

* **权限:**

  `low`

*  **请求参数**

**键值** | **类型** | **是否必需** | **备注**
---------|----------|--------------|---------
phone|string|否|手机号
mail|string|否|邮箱
samId|string|否|samId
password|string|是|密码
source|string|是|识别方式 "mail"/"sms"/"samId"
verifyCode|string|是|验证码

* **请求内容示例:**


        {
            "mail": "gsc1215225@gmail.com",
            "password": "123",
            "source": "mail",
            "verifyCode": "434887"
        } 
--- 
*  **返回参数说明**

    基本返回