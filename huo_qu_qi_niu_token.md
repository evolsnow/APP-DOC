# 获取七牛token


## 接口说明

　上传图片至七牛时，从服务器获取token

## 


* **URL**
        /qiniu/uploadTokens
        

* **Method:**
  
  ####<font color=blue>`GET`</font>

* **权限:**

  `medium`

*  **请求参数**


无

* **请求内容示例:**

无

--- 
*  **返回参数说明**

**键值** | **类型** | **是否必需** | **备注**
---------|----------|--------------|---------
uploadToken |string|是|七牛上传令牌
expire|int|是|有效期,单位为秒



* **返回成功示例:**


        {
            "code": 0,
            "uploadToken": "3b6a8cc22882901fe1b800d529a81c19",
            "expire": 3600
        } 