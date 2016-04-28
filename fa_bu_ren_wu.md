# 发布任务

## 接口说明

　新建mission对象

## 


* **URL**
        /missions

* **Method:**
  
  ####<font color=green>`POST`</font>

* **权限:**

  `medium`

*  **请求参数**

**键值** | **类型** | **是否必需** | **备注**
---------|----------|--------------|---------
name|string|是|任务名
desc|string|否|任务描述
receiversId|[]string|否|预期接收者
deadline|int64|否|截止日期
projectId|string|是|所属项目id

* **请求内容示例:**


        { 
            "name": "ms name",
            "desc": "ms desc",
            "receiversId": ["abc", "def"],
            "deadline": 1232154325,
            "projectId": "32a8cc22882901fe1b800d529a81c19"
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

*  **备注**

用户收到的推送内容为

**键值** | **类型** | **是否必需** | **备注**
---------|----------|--------------|---------
message    |string |是 |推送展示消息
invitor    |string |是 |邀请人id
invitorAvatar|string|是|邀请人头像
invitorName|string|是|邀请人姓名
time|int64|是|时间
targetId    |string |是 |任务id
targetName    |string |是 |任务名字
projectId|string|是|所属项目

        {
            "message": "张三邀请你接受任务 - 任务名",
            "invitor": "5787c1f315347c01899f130de6b4c58c",
            "invitorAvatar": "fsdafas.jpg",
            "invitorName": "张三",
            "time":41289412438,
            "targetId": "e2a7af07009a48fce8b0c2646f5089d3",
            "targetName": "任务名",
            "projectId": "3243092jf0342kjf3",
        }