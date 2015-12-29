# 接口概览

##学生

**URL**             | **HTTP**                      | **功能** 
----------------------|-------------------------------|--------------
/user                |<font color=blue>`POST`</font> |注册
/session             |<font color=green>`POST`</font>|登陆
/user/{id}           |<font color=green>`GET`</font> |获取{id}的学生信息
/user/{id}/password|<font color=orange>`PUT`</font>|更新{id}学生的密码