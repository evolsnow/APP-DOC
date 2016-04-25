# 用户登录

## 接口说明

　用户登录，获取令牌

## 


* **URL**
        /accessToken

* **Method:**
  
  ####<font color=green>`POST`</font>

* **权限:**

  `low`

*  **请求参数**

**键值** | **类型** | **是否必需** | **备注**
---------|----------|--------------|---------
phone|string|否|手机号
mail|string|否|邮箱
samId|string|否|sam id
password|string|是|密码
type|string|是|登录方式 "mail"/"phone"/"samId"

* **请求内容示例:**


        { 
            "mail": "gsc1215225@gmail.com",
            "password": "123",
            "type": "mail"
        } 
--- 
*  **返回参数说明**

**键值** | **类型** | **是否必需** | **备注**
---------|----------|--------------|---------
id    |string |是 |用户id
token |string|是|用户令牌，需在http header中设置'Authorization'为该值
avatar|string|否|头像url地址
name|string|是|名称
alias|string|否|昵称
mail|string|是|邮箱地址
stuNum|string|否|学号


* **返回成功示例:**


        {
            "code": 0,
            "id": "3b6a8cc22882901fe1b800d529a81c19",
            "token": "Bearer abc.defg.hijk"，
            "avatar": "http://qiniu_domain/?e=1461405089\u0026token=access_key:GLfl3nGnSzRIYwQUuEv0l0LHGOA",
            "mail": "abc@def.com",
            "name": "李四",
            "stuNum": "1218404004"

        } 


* **Notes:**

　　返回的`token`需要在`http header`中设置,即:

        Authorization: Bearer abc.defg.hijk