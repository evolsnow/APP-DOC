# 基本规定

请求尽量采用rest风格

##1.请求地址
(https配置已完并强制采用)

**api请求地址前缀在测试期间为:**

        https://samaritan.tech/api/1.0
**接口示例中不再重复书写,即:**

        /students/123
**实际代表:**

        https://samaritan.tech/api/1.0/students/123

##2.请求权限
`low`：任意访问

`medium`：登录访问


##2.请求内容
a. 双方以`json`传输(`GET`方法除外),字段参考对象属性;

b. client需设置`Accept`为`application/json`;

c. client在登陆成功后,会获取到服务器返回的token值,
请将`header`中的`Authorization`设置为该值,否则无权操作需要授权的接口;

##3.请求方法
基本对应关系:


**请求方法** | **含义** | **服务器操作** 
---------|----------|--------------
<font color=green>`POST`</font>|CREATE|创建一个对象
<font color=blue>`GET`</font>|READ|读取对象
<font color=orange>`PUT`</font>|UPDATE|更新对象
<font color=red>`DELETE`</font>|DELETE|删除一个对象
---

* <font color=green>POST</font>

POST方法用于向server申请**创建**内容

示例: 

学生注册

        POST /students

---
* <font color=blue>GET</font>

GET方法用于向server**请求**内容

示例:

a.请求id为123学生的信息

        GET /students/123
b. 请求所有课程的信息,限制为10条

        GET /courses?limit=10

---
* <font color=orange>PUT</font>

PUT方法用于向server申请**更新**内容

示例: 

更新id为123的学生手机号

        PUT /students/123/phone

---

* <font color=red>DELETE</font>

PUT方法用于向server申请**删除**内容

示例: 

删除id为123的学生

        DELETE /students/123


##4.返回内容
请求默认以`http status code`来标志请求状态

`200`: 请求成功执行

`400`: 请求格式错误,详情查看`error`字段

`401`: 未授权请求,查看请求`header`中`Authorization`字段

`403`: 请求禁止,用户信息与授权信息不匹配

`500`: 服务器错误,客户端通知服务器解决

其次，所有失败的请求都会返回错误信息

        {
            code: 400/401...,
            error 错误描述...
        }

`code`为错误状态码，为`0`时表示无错误; error为错误描述信息

注意：请求成功且除`code`外有其他返回内容时，`code`字段会省略。

即：

    无其他内容，返回
    
        {code: 0}
        
    有其他内容，返回
    
        {
            key: value,
            foo: bar
        }