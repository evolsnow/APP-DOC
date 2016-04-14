# 上传deviceToken

## 接口说明

　用户首次登陆app,上传推送的deviceToken

## 


* **URL**
        /deviceTokens
        

* **Method:**
  
  ####<font color=green>`POST`</font>

* **权限:**

  `medium`

*  **请求参数**

**键值** | **类型** | **是否必需** | **备注**
---------|----------|--------------|---------
deviceToken|string|是|设备标识

* **请求内容示例:**


        {
            "deviceToken": "r2hjid23eo2j3e231232hnfj"
        } 
--- 
*  **返回参数说明**

    基本返回