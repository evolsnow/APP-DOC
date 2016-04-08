# Models
（持续更新中）

##User

**字段名** | **类型** | **备注**
 ----------------|--------|------
 	`Id         `|string        | 混淆id
 	`SamId      `|string        | samaritan 唯一 id
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
 	`Name       `|string        | 名称
 	`CreateTime `|int64         | 创立时间
 	`Desc       `|string        | 项目描述
 	`Private    `|bool          | 是否私有
 	`Creator    `|`User`        | 创立者
 	`Members    `|[...]`User`   | 项目成员列表
 	
 
 ##Mission

**字段名** | **类型** | **备注**
 ----------------|--------|------
 	`Id         `|string        |    
 	`Name       `|string        | 名称
 	`CreateTime `|int64         | 创建时间
 	`Desc       `|string        | 任务描述
 	`Publisher  `|`User`        | 任务发布者
 	`Receivers `|[...]`User`   | 所有任务接受者
 	`completionNum`|int         | 已完成人数
 	`completedTime`|int64       | 任务完成时间
 	`Comments   `|Comment       | 评论
 	`Project    `|`Project`     | 所属项目
 	
 	
 ##Todo

**字段名** | **类型** | **备注**
 ----------------|---------|----
 	`Id         `|string        |
 	`StartTime  `|int64         | 开始时间
 	`Repeat     `|bool          | 是否重复
 	`AllDay     `|bool          | 是否全天
 	`RepeatMode `|int           | 重复模式
 	`Place      `|string        | 地点
 	`Pictures   `|[]string      | 图片地址
 	`Desc       `|string        | 描述
 	`Remark     `|string        | 备注
  	`Owner      `|`User`        | 所属者   
 	`FinishTime `|int64         | 完成时间
 	`Mission    `|`Mission`     | 所属任务
 	