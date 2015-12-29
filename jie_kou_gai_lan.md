# 接口概览

##学生

**URL**             | **HTTP**                      | **功能** 
----------------------|-------------------------------|--------------
/user                |<font color=blue>`POST`</font> |注册
/session             |<font color=green>`POST`</font>|登陆
/user/{id}/phone     |<font color=green>`GET`</font> |获取学生{id}的手机号
/user/{id}           |<font color=green>`GET`</font> |获取学生{id}的所有信息
/verification code             |<font color=green>`POST`</font>|发送验证码
/user/{id} |<font color=orange>`PUT`</font>|更新学生{id}的信息(密码等)

