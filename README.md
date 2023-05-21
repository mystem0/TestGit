# DogCatHome
	宠物信息统一管理系统
本项目主要功能为宠物猫和宠物狗的信息展示，所有业务只针对管理员权限。管理员可以完成本项目
的所有权限操作，例如新增宠物、移除宠物、修改宠物信息、查询宠物信息等。
本项目完全采用 ssm 纯注解方式进行开发。由于开发时考虑到数据库信息的后期移动，未在代码中直
接写入数据库的驱动、库名、账号和密码，而是采用了读取配置文件的形式来间接连接数据库。通过
mybatis 创建 bean 对象交给 spring 管理，利用 SpringMVC 的 @RequestBody/@ResponseBody 注解
对传来/传出 的 JSON 格式转成目标格式，dao 层使用 mybatis 注解执行 sql 操作。
