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
 	`Receiverss `|[...]`User`   | 所有任务接受者
 	`completionNum`|int         | 已完成人数
 	`completedTime`|int64       | 任务完成时间
 	`Comments   `|Comment       | 评论
 	
 	
 ##Todo

**字段名** | **类型** | **备注**
 ----------------|---------|----
 	`Id         `|string        |
 	`StartTime  `|int64         | 开始时间
 	`TaskTime   `|int64        | 姓名
 	`Repeat     `|bool        | 手机号
 	`RepeatPeriod`|int64        | 密码
 	`Place      `|string        | 邮箱
 	`Deadline   `|int64        | 头像地址
 	`Desc       `|string        | 学校
 	`Remark     `|string        | 院系
  	`Owner      `|`User`           | 年级   
 	`FinishTime `|int64        | 班级
 	`Mission    `|`Mission`        | 学号
 	