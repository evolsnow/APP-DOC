# 获取项目所有任务

## 接口说明

　获取某项目的所有任务

## 


* **URL**
        /projects/missions/:id

* **Method:**
  
  ####<font color=blue>`GET`</font>

* **权限:**

  `medium`

*  **请求参数**

**键值** | **类型** | **是否必需** | **备注**
---------|----------|--------------|---------
type|string|否|项目类型

* **请求内容示例:**


        /projects/missions/djio23ejdo2jdrqwerqewqeqw
---------------------------------------------------- 
*  **返回参数说明**

**键值** | **类型** | **是否必需** | **备注**
---------|----------|--------------|---------
missions    |[]mission |是 |任务数组

* **ms内容示例:**


        {
            "id": "361916bfc04042177f9a0fe8e0a81c62",
            "name": "ms name",
            "desc": "ms desc",
            "pictures":["...1.jpg", "...2.jpg", ...],
            "receiversName": ["张三", "李四"],
            "deadline": 12342542345,
            "creatorName": "evol",
            "creatorName": "123ui1ohr4ui2h4u13",
            "createTime": 1324123423

        }

* **返回成功示例:**


        {
            "code": 0,
            "missions": [
                {
                    "id": "361916bfc04042177f9a0fe8e0a81c62",
                    "name": "ms name",
                    "desc": "ms desc",
                    "pictures":["...1.jpg", "...2.jpg", ...],
                    "receiversName": ["张三", "李四"],
                    "deadline": 12342542345,
                    "creatorName": "evol",
                    "creatorName": "123ui1ohr4ui2h4u13",
                    "createTime": 1324123423
                },
                {               {
                    "id": "rqwfeqw2177f9a0fedasdew8e0a81c62",
                    "name": "ms name 2",
                    "desc": "ms desc 2",
                    "pictures":["...1.jpg", "...2.jpg", ...],
                    "receiversName": ["张三", "李四"],
                    "deadline": 12342542345,
                    "creatorName": "evol",
                    "creatorName": "123ui1ohr4ui2h4u13",
                    "createTime": 1324123423
                }
            ]
        } 