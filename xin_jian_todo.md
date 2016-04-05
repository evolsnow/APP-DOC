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
startTime|int64|是|开始时间
place|string|否|地点
repeat|bool|否|是否重复,默认为false
repeatMode|int|否|重复模式
allDay|bool|否|是否为全天
desc|string|是|todo事件描述
remark|string|否|备注
missionId|string|否|所属任务id

* **请求内容示例:**


        { 
            "startTime" : 147258369123,
            "place": "somewhere",
            "repeat": true,
            "repeatmode": 1,
            "desc": "do sth",
            "remark": "some remark",
            "missionId": "32a8cc22882901fe1b800d529a81c19"
        }
--- 
*  **返回参数说明**

**键值** | **类型** | **是否必需** | **备注**
---------|----------|--------------|---------
id    |string |是 |



* **返回成功示例:**


        { 
            "id": "3b6a8cc22882901fe1b800d529a81c19",
        }

