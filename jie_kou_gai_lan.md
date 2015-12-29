# 接口概览

##学生

**URL**             | **HTTP**                      | **功能** 
----------------------|-------------------------------|--------------
/students                |<font color=green>`POST`</font> |注册
/accessToken             |<font color=green>`POST`</font>|登陆
/students/{id}/phone     |<font color=blue>`GET`</font> |获取学生{id}的手机号
/students/{id}           |<font color=blue>`GET`</font> |获取学生{id}的所有个人信息
/students/{id}/memos           |<font color=blue>`GET`</font> |获取学生{id}的所有备忘
/verificationCode             |<font color=green>`POST`</font>|发送验证码
/students/{id}/password |<font color=orange>`PUT`</font>|更新学生{id}的密码

