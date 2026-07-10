👋 你好，我是马继强 | Java 后端开发工程师
🎓 教育背景：广州大学 · 软件工程（本科，2027 届应届生）
📍 坐标：广州 | 💰 期望薪资：4-6K | 🔧 技术领域：Java 后端开发
⏳ 到岗时间：在校，可月内到岗
🛠 技术栈 & 擅长方向
后端框架：Spring Boot / Spring Cloud Alibaba / Spring Cloud Gateway
微服务组件：Nacos / OpenFeign / Seata / RabbitMQ
数据存储：MySQL 8.0 / Redis / Elasticsearch 7.12
工具链：Maven / MyBatis-Plus / Knife4j / JWT
架构设计：多模块工程化、微服务解耦、分布式事务、异步通信
🚀 项目实践
1. 微服务电商平台（后端开发工程师）| 2025.10 - 2026.01
基于 Spring Cloud Alibaba构建的微服务电商系统，覆盖商品、购物车、订单、支付等核心模块，采用多模块分层架构（公共组件 hm-common、API 接口 hm-api、业务服务解耦）。
工程化架构：Maven 多模块拆分，实现「公共组件 + API 契约 + 业务服务」分层解耦，支持团队并行开发与独立部署；
网关与安全：Spring Cloud Gateway 做全局 JWT 鉴权，自定义 GlobalFilter拦截请求、校验 Token，白名单路径放行，未登录返回 401；
上下文传递：ThreadLocal + Feign RequestInterceptor实现用户上下文在微服务链路透明传递（网关解析 Token 后写请求头，下游服务提取存 ThreadLocal，Feign 调用自动携带）；
动态路由：Nacos 配置中心监听路由变更，热更新 Gateway 路由表（无需重启服务）；
服务调用：OpenFeign 声明式远程调用 + FallbackFactory降级（非关键查询兜底、关键写操作快速失败）；
异步解耦：RabbitMQ 延迟消息（TTL + Dead Letter Exchange）实现「订单超时取消 + 支付二次确认」，防止边界情况；支付成功后异步通知订单状态，避免同步级联故障；
数据一致性：Seata 分布式事务解决「下单时订单、商品、购物车」多服务数据一致性；乐观锁（状态条件判断）防止并发支付重复扣款；
搜索能力：Elasticsearch + IK 中文分词，实现商品多字段（名/品牌/分类/规格）+ 价格范围毫秒级检索；
工程提效：封装通用分页组件 PageQuery / PageDTO（泛型工厂适配 MyBatis-Plus / ES 分页）；@RestControllerAdvice全局异常统一处理（分层捕获 DB/业务/参数校验异常，HTTP 状态码区分类型）；
文档 & ORM：MyBatis-Plus 操作数据库，Knife4j 生成 API 接口文档。
2. SkyCloudTakeout 外卖平台后端服务（后端开发人员）| 2025.03 - 2025.06
基于 Spring Boot 2.7.3的企业级外卖平台，多模块架构（sky-common / sky-pojo / sky-server），前后端分离。
核心模块：订单生命周期（下单/支付/接单/派送/完成）、数据报表（营业额/订单量/销量排行）、菜品管理（CRUD/分类/套餐组合）；
技术亮点：
AOP 切面：公共字段（如创建时间、更新人）自动填充，减少重复代码 ~30%；
JWT 认证：管理员 + 用户双重认证体系，保障系统安全；
WebSocket：订单状态实时推送，提升商家接单效率；
定时任务：自动处理「超时订单」，保证数据一致性；
全局异常处理：统一响应格式，优化用户体验；
技术栈：Spring Boot + MyBatis + Redis + JWT + WebSocket + 阿里云 OSS。
🎯 求职意向
岗位：Java 后端开发工程师
城市：广州
行业：不限
✨ 补充说明
应届生身份（2027 届），可快速到岗；
专注 Java 后端 + 微服务架构，对「高可用、高性能、工程化」有实践积累；
欢迎交流技术/合作机会，可通过邮箱482592641@@qq.com联系

