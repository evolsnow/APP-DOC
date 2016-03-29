# 用户注册

## 接口说明

　新建用户，用户注册

## 


* **URL**
        /users

* **Method:**
  
  ####<font color=green>`POST`</font>

* **权限:**

  `low`

*  **请求参数**

**键值** | **类型** | **是否必需** | **备注**
---------|----------|--------------|---------
name|string|是|姓名
phone|string|否|手机号
mail|string|否|邮箱
password|string|是|密码
source|string|是|注册方式 "mail"/"sms"
verifyCode|string|是|验证码

* **请求内容示例:**


        { 
            "name": "evolsnow",
            "mail": "gsc1215225@gmail.com",
            "password": "123",
            "source": "mail",
            "verifyCode": "434887"
        } 
--- 
*  **返回参数说明**

**键值** | **类型** | **是否必需** | **备注**
---------|----------|--------------|---------
id    |string |是 |用户id
token |string|是|用户令牌，需在http header中设置'Authorization'为该值



* **返回成功示例:**


        {
            "id": "3b6a8cc22882901fe1b800d529a81c19",
            "token": "Bearer abc.defg.hijk"
        } 


* **Notes:**

　　返回的`token`需要在`http header`中设置,即:

        Authorization: Bearer abc.defg.hijk

