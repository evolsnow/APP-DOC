# 获取离线消息

## 接口说明

　获取用户离线消息

## 


* **URL**
        /offlineMessages

* **Method:**
  
  ####<font color=blue>`GET`</font>

* **权限:**

  `medium`

*  **请求参数**

无


------------------------------------------- 
*  **返回参数说明**

**键值** | **类型** | **是否必需** | **备注**
---------|----------|--------------|---------
msgs    |[]msg |是 |消息数组

* **msg内容示例:**


       {
            "id": "3er2fefs",
            "msg": "张三邀请你加入项目: pj name",
            "time": 31278034432,
            "type": 4,
            "dealt": false,
            "extraInfo": {
                "invitor": "5787c1f315347c01899f130de6b4c58c",
                "invitorAvatar": "e23r432.jpg",
                "invitorName": "张三",
                "projectId": "e2a7af07009a48fce8b0c2646f5089d3",
                "remark": "remark"
            }
        }

* **返回成功示例:**


        {
          "messages": [
          {
            "id": "werersf3r324",
            "msg": "张三邀请你加入项目: pj name",
            "type": 4,
            "dealt": true,
            "extraInfo": {
                "invitor": "5787c1f315347c01899f130de6b4c58c",
                "invitorAvatar": "e23r432.jpg",
                "invitorName": "张三",
                "projectId": "e2a7af07009a48fce8b0c2646f5089d3",
                "remark": "remark"
            }
          },
          {
            "id": "werersf3r324",
            "msg": "张三邀请你接受任务: ms name",
            "type": 7,
            "dealt": true,
            "extraInfo": {
                "invitor": "5787c1f315347c01899f130de6b4c58c",
                "invitorAvatar": "e23r432.jpg",
                "invitorName": "张三",
                "missionId": "e2a7af07009a48fce8b0c2646f5089d3",
                "remark": "remark"
            }
          },
          {
            "id": "werersf3r324",
            "msg": "张三发布了一个任务: ms name",
            "type": 6,
            "dealt": true,
            "extraInfo": {
                "invitor": "5787c1f315347c01899f130de6b4c58c",
                "invitorAvatar": "e23r432.jpg",
                "invitorName": "张三",
                "missionId": "ea2f7341501b894694adce1e40576cb6"
            }
          }
          ]
        }

* **Notes:**

　　msg类型：

**类型** | **说明**
---------|----------
0| 私信
1|群聊
2|其他用户加入项目
3|其他用户离开项目
4|被邀请加入项目
5|被踢出项目
6|任务发布
7|被邀请接受任务