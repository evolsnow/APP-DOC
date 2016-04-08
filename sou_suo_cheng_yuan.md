# 搜索成员

## 接口说明

　成员搜索

## 


* **URL**
        /users/:mail

* **Method:**
  
  ####<font color=blue>`GET`</font>

* **权限:**

  `low`

*  **请求参数**

**键值** | **类型** | **是否必需** | **备注**
---------|----------|--------------|---------
samId|string|是|sam id

* **请求内容示例:**


        /users/abc@def.com
-------------------------- 
*  **返回参数说明**

**键值** | **类型** | **是否必需** | **备注**
---------|----------|--------------|---------
code    |int |是 |请求结果
id|     string|是|用户id
name|   string|是|名称
avatar| string |是|头像url

* **返回成功示例:**


        {
            "code": 0,
            "id": "fasdf24r2",
            "name": "张三",
            "avatar": "https://img.samaritan.tech/abc.jpg"
        } 