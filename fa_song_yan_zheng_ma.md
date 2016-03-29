# 发送验证码

## 接口说明

　注册，找回密码的验证码发送（sms/mail）

## 


* **URL**
        /verifyCode/:source
        
        (source = "sms"/"mail")

* **Method:**
  
  ####<font color=green>`POST`</font>

* **权限:**

  `low`

*  **请求参数**

**键值** | **类型** | **是否必需** | **备注**
---------|----------|--------------|---------
to|string|是|发送对象（手机号/邮箱地址）
use|string|是|用途 （"register"/"forgetPasswd"/"resetPasswd"）

* **请求内容示例:**


        { 
            "to": "gsc1215225@gmail.com",
            "use": "register"
        } 
--- 
*  **返回参数说明**

**键值** | **类型** | **是否必需** | **备注**
---------|----------|--------------|---------
code    |int |是 |结果标志


* **返回成功示例:**


        {
            "code": 200
        } 


