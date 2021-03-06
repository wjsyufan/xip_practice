# xip_practice
## XIP培训积累文档和资料总结

本仓库主要用于同方软银渠道业务事业部的培训积累文档，用于不断的更新和分享最新的相关新人培训、在职培训等文档。

完成的功能希望大家积极编写，已完成的欢迎大家补充，修正。

---

目录的初步说明

PDF/ 用来放生成的文档，可以是PDF，也可以是mhtml等
MOV/ 用来放视频
SRC/ 用来放MARKDOWN和图片的源代码。



## 计划完成如下功能

#### 1. 基础前提知识点

- 培训引言（PPT）  -- 已完成

  - 组织架构介绍：部门名称、部门定位、部门领导、各条线负责人、产品线初步介绍、地区负责人制度、项目经理
  - 交流共享：QQ群、论坛、微信群、内部FTP地址
  - 纪律规定：着装+耳机+游戏+视频、124标准加班+邮件格式+请假要求
  - 培训介绍：培训要求、考试要求、基本环境、整体培训课表

- linux基本操作（文档)   -- 已完成

  - linux系统介绍，用户，ssh和telnet服务，环境变量说明.
  - 初级命令 cd  ls  mv cp(-r) ps(-ef) mkdir rm grep、find . -name、env|grep HOME、chmod、tail、tar
  - 查看进程,停启服务,shell是啥 
  - ping, telnet,ftp(工具，命令都可以) 

- vim基本操作（文档） -- 已完成

  - vim介绍(vi和vim的区别)
  - 上下左右
  - ESC两种模式
  - i,x,yy,p,dd,:wq

- xip用户系统环境介绍（说明文档） — 待完成

  - ```
    bin/  etc/ keys/  log/ src/  txt/
    binsh/    files/  lib/   tmp/  user/
    ```

- 柜面交易配置（视频+操作文档）— 已完成

  - 画屏幕
  - 查询配置
  - 打印配置  

- 渠道交易配置（视频+操作文档） -- 已完成

  - 程序配置
  - 流程配置
  - 数据库配置
  - （非新人培训）渠道定义和配置
  - （非新人培训）通讯程序编写

- 数据库基本尝试  -- 石宝琦

  - 常见数据库厂商 ORACLE（甲骨文），db2(IBM)，MySql
  - 数据SQL语句和常见SQL语句：select
  - （非新人）并表查询
  - oracle数据库的启停、监听的启停、服务实例的查看。 

#### 2. 基础基本点

- 一笔交易的详细流程图和说明（流转图、说明文档） -- 贺全阳

  - 前台填写数据
  - 组成报文（有格式的字符串）
  - 来源渠道主程序
    - 通讯服务程序接收、拆包（拆解字符串）
    - 配置的交易执行
      - 路由层
        - CALL
        - EVAL
        - COMM
    - 通讯服务程序组包（组成字符串）、返回

- 代缴费各业务场景和流程介绍（文档） -- 闫尚峰

  - 缴费前查询
  - 缴费
  - 缴费撤销
  - 流水查询
  - 对账+清算
  - 发票打印

- 看日志 （文档）  -- 

  - 日志文件位置、日志配置和日志格式说明

  - APPLOG查看

    - 服务开始
    - 头
    - 拆包
    - 流程 
    - 组包
    - 尾

  - 错误分析

    - 日志级别
    - 日志注意事项
    - 日志的格式 

  - XIPLOG查看

    - 服务开始
    - 头
    - 拆包
    - 流程
    - 系统传值
    - 组包
    - 尾

  - 日志编写规范

    必须：wherelist、不允许乱写、意义明确、简练汉字、不允许出现敏感信息（密码、余额）

    D: 调试信息(跟踪信息)

    I: 提示信息(不允许用)

    W: 警告信息(不允许用)

    E: 错误信息(错误)

    F: 致命错误(不允许用)

- 业务常识&常用术语（说明文档） -- 王长城

  - 流水号的作用和规则
  - 机构、法人、柜员
  - 授权复核手续费 
  - SIT、FAT、UAT    测试相关 黑盒、白盒

- socket常识（文档）  --  王长城

  - 客户端、服务端
  - 客户端通讯模型
  - 服务端通讯模型 
  - (非新人)tcp的三次握手和四次挥手 

- 项目基本流程 （说明文档）  -- 张书瑞

  - 开始、工作量评估
  - 项目立项
  - 谈需求、分析和确认
  - 设计、概要设计详细设计
  - 编码
  - 内测
  - 联调测试
  - 客户测试
  - 上线准备 （上线申请、更新包、回退方案）
  - 上线工作
  - 跟踪和业务验证
  - 项目验收
  - 公司结项

- 解决问题的办法 （文档和经验分享） -- 李鹏飞

  - 分配的任务要分析问题点，总结问题点。
  - 如报错问题看日志，并且有自己的初步分析结论。
  - 百度、公司论坛、将论坛地址发公司群里。 
  - 咨询地区负责人、咨询领导

#### 3. 配合文档学习点

- C语言程序的基本原理（文档）  -- 张大荣

  - .c程序
  - 编译器 gcc/xlc
  - 编译 -> 链接 -> 动态链接
  - 运行时 调用so

- makefile  （文档） -- 张大荣

  - 原理、依赖关系
  - 公司makefile介绍
  - 跟我一起写makefile

- PC程序原理  -- 张大荣

  - PROC, oracle/db2的支持
  - pc程序的初步原理
  - pc程序的常见封装写法

- 一个程序详细分析（说明文档） -- 张大荣

  - 注释头、必要的注释
  - 头文件
  - 函数名、xip结构体
  - 变量声明
  - 初始化
  - 取值
  - 查表
  - 错误判断
  - 返回

- 交易部署的shell分析（说明文档，例子分析） -- 张大荣

- 常用C语言函数（说明文档）  -- 张大荣

  ```
  变量声明
  memset
  sprintf
  strcpy
  atol
  strcmp
  get_zd_data/double/long
  set_zd_data/double/long
  表_Ins
  表_Sel
  表Dec/Fet/Upd_Upd
  表
  fopen
  fgets
  fprintf
  fclose
  ##自有函数:
  strtrim
  APPLOG
  SubSignString
  ```

- 基本账务基础 （说明文档） — 张强

  - 基本会计账原理
  - 个人理解和便于记忆的小技巧分享
  - 代缴费账户整体会计分录说明 

- 信息导出（视频+操作文档）  -- 张大荣

  - 渠道部署
  - 交易部署
  - 程序部署
  - 数据库部署

- 程序编写示例参考文档（文档） -- 张大荣

  - 插入程序编写
  - 更新程序编写
  - 批量查询程序编写
  - （非新人培训）解析文件程序编写

- 接口需求分析（文档、非新人）拿到一个接口文档和业务需求，如何开始 — 于帆

  - 通读文档
  - 列功能点



### DAS系统开发

- 整体讲解 各系统功能（图+文档）
- DSS 配置（视频）
- DAS 程序编写和配置（视频）
- DBO 程序编写和配置（视频）
- 日志初步查看（分析文档）
- 停启服务操作（文档）



### WEBUI开发

- WEB开发的基础介绍和学习资料（文档）
- 公司框架介绍、181、基本工具、业务管理端的功能（介绍）
- 流水查询：在一个项目中创建查询表的页面（视频+操作文档）
- 业务对账：创建一个有通讯的项目（视频+操作文档）