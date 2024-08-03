# xxl-job使用手册
## 1. 部署配置调度中心
#### 步骤一： 执行数据库初始化SQL脚本
> 脚本位置 /xxl-job/doc/db/tables_xxl_job.sql
#### 步骤二： 修改配置，启动xxl-job-admin(调度中心)
> 修改application.properties文件
#### 步骤三： 登陆http://localhost:8080/xxl-job-admin
> 用户名/密码 ---> admin/123456
## 2. 部署执行器项目
#### 步骤一： 引入xxl-job-core的依赖
#### 步骤二： 创建xxl-job-executor的配置项
> 调度中心URL
> xxl.job.executor.address=http://127.0.0.1:9999
> 执行器内部IP
> xxl.job.executor.ip=127.0.0.2
> 执行器监听端口
> xxl.job.executor.port=9999 
#### 步骤三： 创建XxlJobSpringExecutor
#### 步骤四： 调度中心执行器管理配置执行器(可自动发现)
#### 步骤五： 调度中心任务管理配置任务(有很多模式)

