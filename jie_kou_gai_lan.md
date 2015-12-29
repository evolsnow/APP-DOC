# 接口概览

##学生

**URL**             | **HTTP**                      | **功能** 
----------------------|-------------------------------|--------------
/users                |<font color=blue>`POST`</font> |注册
/users/{name}/token   |<font color=green>`POST`</font>|登陆
/users/{name}         |<font color=green>`GET`</font> |获取{name}的学生信息
/users/{name}/password|<font color=orange>`PUT`</font>|重置{name}学生的密码