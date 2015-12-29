# 接口概览

##学生

**URL**             | **HTTP**                      | **功能** 
----------------------|-------------------------------|--------------
/user                |<font color=green>`POST`</font> |注册
/accessToken             |<font color=green>`POST`</font>|登陆
/user/{id}/phone     |<font color=blue>`GET`</font> |获取学生{id}的手机号
/user/{id}           |<font color=blue>`GET`</font> |获取学生{id}的所有个人信息
/user/{id}/memos           |<font color=blue>`GET`</font> |获取学生{id}的所有备忘
/verificationCode             |<font color=green>`POST`</font>|发送验证码
/user/{id}/password |<font color=orange>`PUT`</font>|更新学生{id}的信息(密码等)

