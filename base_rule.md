# 基本规定

尽量采用rest风格

##1.请求地址
(https配置已完成,暂不启用)

**api请求地址前缀在测试期间为:**

        http://samaritan.tech/api/1.0
**接口示例中不再重复书写,即:**

        /students/123
**实际代表:**

        http://samaritan.tech/api/1.0/students/123

##2.请求方法
基本对应关系:


**请求方法** | **含义** | **服务器操作** 
---------|----------|--------------
<font color=blue>`POST`</font>|CREATE|创建一个对象
<font color=green>`GET`</font>|READ|读取对象
<font color=orange>`UPDATE`</font>|UPDATE|更新对象
<font color=red>`DELETE`</font>|DELETE|删除一个对象

* <font color=blue>`POST`</font>