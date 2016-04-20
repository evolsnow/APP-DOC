# 更新Todo

## 接口说明

　更新Todo内容的基本内容, 包含图片

## 


* **URL**
        /todos/:tid
        

* **Method:**
  
  ####<font color=orange>`PUT`</font>

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
done|bool|否|是否完成
finishTime|int64|否|完成时间
pictures|[]string|否|图片名
* **请求内容示例:**


        { 
            "startTime" : 147258369123,
            "place": "somewhere",
            "repeat": true,
            "repeatmode": 1,
            "desc": "do sth",
            "remark": "some remark",
            "missionId": "1dacc22882901fe1b800d529a81c19",
            "done": true,
            "finishTime": 147258369123,
            "pictures": ["1.jpg", "2.jpg"]
        }
--- 
*  **返回参数说明**

    基本返回
