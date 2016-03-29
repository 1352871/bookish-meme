# 复用文档

### 可复用组件
- 系统的构件
	- 系统体系结构：
		- 前后端通过EventBus机制解耦
		- 将功能划分为不同的低耦合、高内聚的模块单独实现（channel中有一系列顺序流过的handler来分别实现不同的功能，而不是一个handler实现所有的功能）
	- UI设计构件
	- 配置文件读取构件（需要根据类进行适当修改才能复用）
	- 数据库连接构件
	 	
- 项目管理和文档 
	- 项目管理模式
	- 文档构件：项目管理文档，项目计划表
	- 测试数据：测试用例设计

### 冗余检查
- 测试用例
- 过程冗余：由于登陆消息和聊天消息公用一条pipeline，所以消息在channel中流动时会有冗余，但这种冗余反而降低了设计的复杂度，是可接受的。