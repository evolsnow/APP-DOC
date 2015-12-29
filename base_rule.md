# 基本规定

请求尽量采用rest风格

##1.请求地址
(https配置已完成,暂不启用)

**api请求地址前缀在测试期间为:**

        http://samaritan.tech/api/1.0
**接口示例中不再重复书写,即:**

        /students/123
**实际代表:**

        http://samaritan.tech/api/1.0/students/123

##2.请求内容
双方以`json`传输,字段参考对象属性

客户端需设置`Content-type`与`Accept`为`application/json`

##3.请求方法
基本对应关系:


**请求方法** | **含义** | **服务器操作** 
---------|----------|--------------
<font color=blue>`POST`</font>|CREATE|创建一个对象
<font color=green>`GET`</font>|READ|读取对象
<font color=orange>`PUT`</font>|UPDATE|更新对象
<font color=red>`DELETE`</font>|DELETE|删除一个对象
---

* <font color=blue>POST</font>

POST方法用于向服务器申请**创建**内容

示例: 

学生注册

        POST http://samaritan.tech/api/1.0/students

---
* <font color=green>GET</font>

GET方法用于向服务器**请求**内容

示例:

a.请求id为123学生的信息

        GET http://samaritan.tech/api/1.0/students/123
b. 请求所有课程的信息

        GET http://samaritan.tech/api/1.0/courses

---
* <font color=orange>PUT</font>

PUT方法用于向服务器申请**更新**内容

示例: 

更新id为123的学生信息

        PUT http://samaritan.tech/api/1.0/students/123

---

* <font color=orange>DELETE</font>

PUT方法用于向服务器申请**删除**内容

示例: 

删除id为123的学生信息

        DELETE http://samaritan.tech/api/1.0/students/123


##4.返回内容
请求默认以`http status code`来标志请求状态

`200`:请求成功执行

`400`:请求格式错误,详情查看`error`字段

`401`:未授权请求,详情查看`error`字段

`500`:服务器错误,客户端通知服务器解决
