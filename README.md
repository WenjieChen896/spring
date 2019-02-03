# spring
# Mybatis
(1)
ORM框架
MyBatis是一个优秀的持久层框架，对JDBC操作数据库进行了封装，封装后的Mybatis使应用程序开发者只需要关注SQL本身
完全不需要再次花精力去处理例如注册驱动、创建connection、创建statement、手动设置参数、结果集检索等jdbc繁杂的过程代码（最初的Mybatis环境搭建只需要立项之初配置即可）

	* 
要求通过xml或注解的方式将要执行的各种statement（statement、preparedStatemnt、CallableStatement）配置起来
	* 
并通过java对象和statement中的sql进行映射生成最终执行的sql语句
	* 
mybatis框架执行sql并将结果映射成java对象并返回。




(2)
以上为Mybatis配置文件中各个模块的简单介绍，重在介绍模块的功能，具体用法还需要参考官方文档
从配置文件也可以看得出来，Mybatis的配置条理清晰，各个模块各司其职，而且非常的灵活

	* 
通过properties可以对元素进行设置
	* 
通过environments对环境进行指定
	* 
通过mappers对映射文件进行定位
	* 
通过settings设置可以对Mybatis进行高级调优
	* 
通过typeAliases别名可以简化名称，简捷使用
	* 
通过typeHandlers类型处理可以对数据与Java类型的转换进行高级设置
	* 
通过plugins插件可以在Mybatis执行逻辑中植入逻辑功能
	* 
通过databaseIdProvider数据库厂商标识符 可以灵活应用部署多数据库
	* 
通过objectFactory对象工厂可以个性化对象的创建


以上各个模块都是configuration的子元素，放置于configuration内
需要注意的是各个元素之间也是有顺序的，有顺序的，在DTD文件中可以看到

https://www.cnblogs.com/noteless/p/10332784.html
