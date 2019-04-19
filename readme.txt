MAT(MyAutoTesting)
目的：为了了解docker、jenkins等自动化部署架构
实现jmeter、loadrunner、selenium等自动化工具自动管理和部署脚本、自动提取用例、自动运行脚本、自动记录测试结果，并以数据库形式及html等形式保存。
实现环境：python作为开发语言
					postgresql作为数据库
					jenkins作为自动化部署工具
					jemter作为实现工具					
期望实现：docker 集群管理
					postgresql集群管理
					spring boot云管理（*）
数据库设计：库名：MATdb
						表：testcase:用例表  列：tcid name descripte step expect date author other
						表：result:测试结果  列：resid bug descripter caseid tools date runner
						表：user:用户				 列：usrid usrname 
						表：file:文件				 列：fid tools path use
脚本设计：文件读取
					数据库处理						