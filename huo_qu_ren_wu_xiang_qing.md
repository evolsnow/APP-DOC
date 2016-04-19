# 获取任务详情

## 接口说明

　获取任务详情

## 


* **URL**
        /missions/:mission

* **Method:**
  
  ####<font color=blue>`GET`</font>

* **权限:**

  `medium`

*  **请求参数**

**键值** | **类型** | **是否必需** | **备注**
---------|----------|--------------|---------
mission|string|是|mission id

* **请求内容示例:**


        /missions/361916bfc04042177f9a0fe8e0a81c62
----------------- 
*  **返回参数说明**

**键值** | **类型** | **是否必需** | **备注**
---------|----------|--------------|---------
code    |int |是 |请求结果
id|     string|是|mission id
createTime|int64|是|创建时间
name|   string|是|名称
desc|string|是|描述
publisherId|string|是|发布者id
receiversName|[]string|否|接收者名称列表
projectId| string |否|所属项目id

* **返回成功示例:**

 
        {
            "code": 0,
            "id": "361916bfc04042177f9a0fe8e0a81c62",
            "createTime": 1460356446,
            "name": "test mission",
            "desc": "test mission desc",
            "publisherId": "5787c1f315347c01899f130de6b4c58c",
            "receiversName": [
                "张三",
                "李四"
            ],
            "projectId": "ab4286092583a315b6c43f3e4317937e"
        } 