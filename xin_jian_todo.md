# 新建Todo

## 接口说明

　新建Todo对象

## 


* **URL**
        /todos

* **Method:**
  
  ####<font color=green>`POST`</font>

* **权限:**

  `medium`

*  **请求参数**

**键值** | **类型** | **是否必需** | **备注**
---------|----------|--------------|---------
desc|string|是|todo事件描述
deadline|uint64|是|结束时间
startTime|uint64|否|默认则由服务器生成
accomplished|string|否|默认false
missionId|int|否|

* **请求内容示例:**


        { 
            desc : "to do something",
            deadline: 147258369123,
            missionId: 1
        }
--- 
*  **返回参数说明**

**键值** | **类型** | **是否必需** | **备注**
---------|----------|--------------|---------
code    |int |是 |



* **返回成功示例:**


        { 
            code : 0 
        }

