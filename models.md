# Models
（持续更新中）

##User

**字段名** | **类型** | **备注**
 ----------------|--------|------
 	`Id         `|string        | 混淆id
 	`Alias      `|string        | 昵称
 	`Name       `|string        | 姓名
 	`Phone      `|string        | 手机号
 	`Password   `|string        | 密码
 	`Email      `|string        | 邮箱
 	`Avatar     `|string        | 头像地址
 	`School     `|string        | 学校
 	`Department `|string        | 院系
  	`Grade      `|int           | 年级   
 	`Class      `|string        | 班级
 	`StudentNum `|string        | 学号
	

##Project

**字段名** | **类型** | **备注**
 ----------------|---------|----
 	`Id         `|string        |    
 	`Name       `|string        |  
 	`CreateTime `|int64         | 
 	`Desc       `|string        | 
 	`Private    `|bool          |
 	`Creator    `|`User`        | 
 	`Members    `|[...]`User`   |    user 列表
 	
 