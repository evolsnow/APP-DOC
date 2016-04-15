# 新建Project

## 接口说明

　新建Project对象

## 


* **URL**
        /projects

* **Method:**
  
  ####<font color=green>`POST`</font>

* **权限:**

  `medium`

*  **请求参数**

**键值** | **类型** | **是否必需** | **备注**
---------|----------|--------------|---------
name|string|是|名称
desc|string|否|project描述
private| bool|否|是否私有

* **请求内容示例:**


        { 
            "name": "project name",
            "desc": "project desc",
            "private": true
        }
--- 
*  **返回参数说明**

**键值** | **类型** | **是否必需** | **备注**
---------|----------|--------------|---------
id    |string |是 |



* **返回成功示例:**


        { 
            "code": 0,
            "id": "3b6a8cc22882901fe1b800d529a81c19",
        }


