# 更新任务图片

## 接口说明

　更新任务图片

## 


* **URL**
        /missions/pictures/:mission
        

* **Method:**
  
  ####<font color=orange>`PUT`</font>

* **权限:**

  `medium`

*  **请求参数**

**键值** | **类型** | **是否必需** | **备注**
---------|----------|--------------|---------
pictures|[]string|是|图片名

* **请求内容示例:**


        {
            "pictures": ["1.jpg", "2.jpg"...]
        } 
--- 
*  **返回参数说明**

    基本返回