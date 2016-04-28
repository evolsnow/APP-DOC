# 任务邀请

## 接口说明

　邀请用户接收任务

## 


* **URL**
        /invitations/mission

* **Method:**
  
  ####<font color=green>`POST`</font>

* **权限:**

  `medium`

*  **请求参数**

**键值** | **类型** | **是否必需** | **备注**
---------|----------|--------------|---------
invitee|string|是|被邀请人id
MissionId|string|是|任务id
MissionName|string|是|任务名称
remark|string|否|备注

* **请求内容示例:**


        { 
            "invitee" : "r423fjewfo43f",
            "missionId": "41235432rfwef432f",
            "missionName": "任务名",
            "remark": "some remark"
        }
--- 
*  **返回参数说明**

    基本返回
    
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
remark    |string |否 |备注

        {
            "message": "张三发布了一个任务 - 任务名",
            "invitor": "5787c1f315347c01899f130de6b4c58c",
            "invitorAvatar": "fsdafas.jpg",
            "invitorName": "张三",
            "time":41289412438,
            "targetId": "e2a7af07009a48fce8b0c2646f5089d3",
            "targetName": "任务名",
            "projectId": "3243092jf0342kjf3",
            "remark": "remark"
        }