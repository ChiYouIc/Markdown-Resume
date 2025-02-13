 <center>
     <h1>池友 - Java 开发工程师</h1>
 </center>



 ## <img src="assets/info-circle-solid.svg" width="30px"> 个人信息 

 - 姓名：池友
 - 性别：男
 - 出生：1997 年 2 月
 - 现居住地：深圳 
 - 工作经验：2 年



## <img src="assets/graduation-cap-solid.svg" width="30px"> 教育经历

- 学士，贵州大学明德学院，网络工程专业，2016.9~2020.7
- 软考网络工程师认证



## <img src="assets/file-lines-solid.svg" width="30px"> 求职意向

- 职位：Java 开发工程师
- 工作类型：全职
- 到岗时间：本月
- 工作地点：深圳



## <img src="assets/briefcase-solid.svg" width="30px"> 工作经历

- **上海易立德信息技术股份有限公司，IT产品研发部，Java 开发工程师，2020.04 ~ 至今**

   为公司内部系统提供技术支持，应对各种特殊的业务场景，进行整理、分析，编写需求文档和说明文档，以及后期的开发文档，待开发文档成型后，进行实际开发实现。在职期间，为公司定制开发 OA 系统，向业务部门提供系统支撑，对人事、考勤、薪酬系统线上化。
   
   

## <img src="assets/project-diagram-solid.svg" width="30px"> 项目经历

- **Smart-OA 项目 2020.10 ~ 至今**

  **项目描述**：该项目主要为了应对 HR 领域特殊的业务场景而开发的 OA 系统，该项目旨在服务 HR 办公领域，简化以往繁琐的流程，提升沟通效率，更好的，更方便的管理员工的各项信息。该项目采取了前后端分离的思想，实现前端和后端的解耦。 

  **实现技术**：SpringBoot + Mybatis + MySQL + MongoDB + Vue + Element UI
  
  **职责描述**：
  
  - 通过自定义 MyBatis 拦截器，拦截提交的 SQL 语句，在 SQL 语句后添加条件语句，实现数据权限处理；执行的 SQL 是否需要添加该添加是通过在 xml 文件中使用 <![CDATA[ ]]> 来转义需要执行的条件语句标识，在拦截器中，通过正则匹配出标识，再与预先设定好的条件集合进行匹配，将结果语句连接到拦截的 SQL 语句中提交执行；
  
  - 通过自定义注解 + ResponseBodyAdvice 接口，对接口的响应数据进行封装返回，自定义注解是用于判别接口响应数据是否需要处理；
  
  - 工作流动态表单设计，通过前后端沟通协调，统一工作流表单的固定内容与自定义内容；前端的表单数据使用 json 格式，编译一个专门解析表单内容的解析引擎处理，将数据解析后渲染到浏览器页面；后端接受到上传的表单 json 数据，将原始的 json 存储一份，在将原始 json 中固定内容解析，存储到数据库，方便工作流审批时数据处理；
  
  - 定义工作流事件接口和行为模板，工作流的事件包括流程发起、流程结束，行为有审批、撤回、转交、抄送；工作流引擎自动识别事件进行行为调用；对于特殊工作流，通过实现接口注册到工作流引擎中，根据需要自行实现其定义好的行为；
  
  - 编写邮件发送工作，对邮件发送进行封装，提供一个调用方法；通过识别配置文件区分开发环境，进行邮箱切换和提示语，只会往开发人员邮箱推送邮件，避免开发环境测试时将邮件推送给真实用户；
  
  - 第三方接口封装，查阅第三方接口文档，将接口参数、返回值、异常等进行封装方便使用；
  
  - 编写考勤计算引擎，实现一个默认的计算规则，将工作流中的请假、出差、补卡等信息进行整合，计算迟到、早退、矿工、出勤时长；定义计算规则接口，对于特殊的考勤处理，可以通过实现接口注册到计算引擎中，计算引擎通过识别预先在考勤数据中打上的标识，选择计算规则。
  
    
  
- **在线考试项目 2021.05 ~ 至今** 

  **项目描述**：在线考试系统的开发主要目的是实现职能人员能力考核线上化，涉及到的考题包括了软考中高级题目、PMP项目管理，以及编程题目，其中编程题目包含语言 Java 、Python 、C、C++、JavaScript、Golang。该项目采取了前后端分离的思想，其中编程题目的校验，使用到了 Docker 虚拟机。

  **实现技术**：SpringBoot + Mybatis + MySQL + Docker + Vue + Element UI

  **职责描述**：

  - 参与该项目的数据库表设计，主要设计对象：试题表、试题分类表、试题答案表、试卷表、试卷权限表；
  - 参与上述表的前后端功能开发；
  - 参与编程题的前端页面开发，使用 codemirror-editor 开发代码编辑器，结合 highlight 实现代码高亮；
  - 参与编程题代码运行系统的搭建，运行代码的系统是一个开源的，使用 Golang 开发的系统，需要配合 Docker 虚拟机，因为实际的代码运行需要在虚拟环境中运行。
  - 参与系统对接，使用定时任务从 OA 系统中同步新入职人员以及人员的在离职情况，以及组织架构；

  

- **能力地图项目 2021.10 ~ 至今**

  **项目描述**：能力地图系统主要是收集并分析员工的技能分布情况，通过技能数、技能使用年限、技能掌握熟练度等指数进行综合评分，使用最后的评分测算出员工等级。该项目采取了前后端分离的思想，实现前端和后端的解耦。 

  **实现技术**：SpringBoot + Mybatis + MySQL + Vue + Element UI

  **职责描述**：

  - 参与数据库表设计，主要设计对象：技能表、技能分类表、技能等级表、技能申请表、技能审批表、待审核技能表；

  - 参与上述对应表的前后端功能开发；

  - 参与技能审批流程的开发，包括技能申请、技能审批任务分发、技能审批任务审批、员工技能生效功能；

  - 参与技能资源报表查询开发；

  - 参与系统对接，使用定时任务从 OA 系统中同步新入职人员以及人员的在离职情况，以及组织架构；

    

- **资产管理项目 2022.10 ~ 至今**

  **项目描述**：资产管理系统的目的是协助公司资产管理员对资产的管理，监控资产流向、资产使用情况；使用线上化管理，可以做好从资产入库、领用、归还、报废、维修等情况的记录；以及更便捷的资产盘点。该项目采取了前后端分离的思想，实现前端和后端的解耦。 

  **实现技术**：SpringBoot + Mybatis + MySQL + Vue3 + Ant Design Vue

  **职责描述**：

  - 参与数据库表设计，主要设计对象：资产批次表、资产表、资产价值表、资产盘点表；
  - 参与上述表的前后端功能开发；
  - 参与开发资产盘点功能，以月为单位对资产的使用人、所在部门、办公地区、座位号进行盘点确认；
  - 参与开发资产领用流程、资产归还流程、资产转移流程、资产报废流程、资产入库流程；
  - 参与开发资产价值开发，以月为单位，计算资产的当前折旧价值、折余价值并生成基线备份存档；
  - 参与开发资产价值与第三方系统用友的对接，提供本系统中资产原值、本期折旧、本期折余等信息。
  
  

## <img src="assets/tools-solid.svg" width="30px"> 技能清单

- 熟练使用 Idea 开发工具、Maven 依赖管理、Git 版本管理工具；
- 熟练使用 Java 基础；
- 熟练使用 Java 集合框架，并了解常用的 ArrayList、LinkedList、HashMap 的底层原理；
- 熟练使用 Java 多线程编程，了解 Java 线程池使用；
- 熟练使用 Spring、SpringMVC、SpringBoot、MyBatis 这些常用框架；
- 熟练使用 MySQL 数据库语法，SQL 优化操作；
- 熟练使用 HTML、CSS、JavaScript 前端技术；
- 熟练使用 Vue 和 Vue3 框架；
- 熟练使用 Element UI 和 Ant Design Vue 桌面端组件库；
- 了解常用的设计模式，并掌握其中部分设计模式，例如单例模式、工厂模式、责任链模式、模版方法模式、代理模式、适配器模式；
- 了解 SpringCloud 微服务架构以及其各个组件，例如：Eureka、Ribbon、Feign、Hystrix、Zuul；能做到独立搭建一个服务；
- 了解 Nacos，能做到整合 SpringCloud 和 SpringBoot，做注册中心、服务监控以及配置中心；
- 了解 Redis 缓存数据的基本使用；
- 了解 RabbitMQ 消息中间的基本使用；
- 了解 Electron 桌面应用程序框架使用；
- 了解 Docker 虚拟机的基本使用；
- 了解 Nginx 的基本使用；
- 了解 Golang 的基本语法和使用；



## <img src="assets/evaluate.svg" width="30px"> 自我评价

- **技术方面**：主攻后端开发，同时也会了解一下其它领域，例如前端开发、桌面应用开发、大数据等；因为学习技术不能只有深度没有宽度；
- **工作态度**：力争做到高效的完成本职工作，积极参与团队交流、相互学习与提升；
- **学习过程**：除了订阅浏览一些技术网站、博客以外，自己也有编写博客，记录自己的工作遇到的问题，用到的新技术栈；同时也拥有个人的开源项目，虽然没有人气，但这也是一个学习的过程。目前有三款个人开源项目，分别是单点登录系统和代码生成系统、还有一个前端模版。
- **开源项目**：
  - 代码仓库：https://gitee.com/coder-you
  - 代码生成系统：http://43.139.178.51/gen
  - 单点登录系统：http://43.139.178.51/sso
  - 前端模版：http://43.139.178.51/template/
  - 博客：http://43.139.178.51/blog/




## <img src="assets/flower.svg" width="30px"> 致谢

感谢您花时间阅读我的简历，期待能有机会和您共事。
