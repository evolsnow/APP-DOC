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
            "msg": "张三邀请你加入项目: pj name",
            "extraInfo": {
                "invitor": "5787c1f315347c01899f130de6b4c58c",
                "projectId": "e2a7af07009a48fce8b0c2646f5089d3",
                "remark": "remark"
            }
        }

* **返回成功示例:**


        {
          "messages": [
          {
            "msg": "张三邀请你加入项目: pj name",
            "extraInfo": {
                "invitor": "5787c1f315347c01899f130de6b4c58c",
                "projectId": "e2a7af07009a48fce8b0c2646f5089d3",
                "remark": "remark"
            }
          },
          {
            "msg": "张三邀请你接受任务: ms name",
            "extraInfo": {
                "invitor": "5787c1f315347c01899f130de6b4c58c",
                "missionId": "e2a7af07009a48fce8b0c2646f5089d3",
                "remark": "remark"
            }
          },
          {
            "msg": "张三发布了一个任务: ms name",
            "extraInfo": {
                "invitor": "5787c1f315347c01899f130de6b4c58c",
                "missionId": "ea2f7341501b894694adce1e40576cb6"
            }
          }
          ]
        }