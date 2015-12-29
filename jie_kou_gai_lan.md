# 接口概览

##学生

**URL**             | **HTTP**                      | **功能** 
--------------------|-------------------------------|--------------
/users              |<font color=blue>`POST`</font> |注册
/loginsession       |<font color=green>`POST`</font>|登陆
/users/{id}         |<font color=green>`GET`</font> |获取{id}的学生信息
/users/{id}/password|<font color=orange>`PUT`</font>|重置{id}学生的密码