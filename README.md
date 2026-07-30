# 全栈开发学习大纲（整合版）

说明：本大纲将原始的22部分、数千个细碎知识点，压缩整合为"章.节.课"三级结构，
每"课"合并了若干原始知识点，作为一次完整讲解的粒度，避免过于碎片化。

---

## 第一章 JavaScript深度

1.1 基础语法与类型
- 1.1.1 变量与基本类型（primitive/reference类型、var/let/const、类型转换、truthy/falsy）
- 1.1.2 常用运算符与比较规则
- 1.1.3 数组与对象常用API
- 1.1.4 现代语法糖（解构赋值、展开/剩余运算符、可选链、空值合并）
- 1.1.5 Map与Set

1.2 内存模型与拷贝
- 1.2.1 栈内存与堆内存、值传递与共享引用
- 1.2.2 浅拷贝与深拷贝（含structuredClone、JSON方式的局限）

1.3 函数
- 1.3.1 函数的几种定义方式与箭头函数的区别
- 1.3.2 高阶函数、纯函数、回调函数、IIFE
- 1.3.3 参数处理（rest参数、arguments对象、默认参数）

1.4 对象与原型
- 1.4.1 对象创建方式（字面量/构造函数/Object.create/class）
- 1.4.2 属性描述符与getter/setter
- 1.4.3 Object常用静态方法（keys/values/entries/assign/freeze/seal）
- 1.4.4 原型链与继承（prototype、\_\_proto\_\_、instanceof原理、new执行过程、ES5与ES6继承）

1.5 执行机制与作用域闭包
- 1.5.1 执行上下文与执行栈（含V8引擎基础认识）
- 1.5.2 词法环境、变量提升与TDZ
- 1.5.3 作用域与作用域链
- 1.5.4 闭包原理、应用场景与内存影响（含React中的Stale Closure）

1.6 this绑定
- 1.6.1 四种绑定规则与优先级
- 1.6.2 call/apply/bind与箭头函数的词法this
- 1.6.3 常见this丢失场景

1.7 异步编程
- 1.7.1 同步与异步、回调地狱
- 1.7.2 Promise基础（状态、resolve/reject、then/catch/finally）
- 1.7.3 Promise组合方法（all/allSettled/race/any）
- 1.7.4 async/await与异步错误处理

1.8 Event Loop与内存管理
- 1.8.1 调用栈、Web APIs、宏任务队列与微任务队列
- 1.8.2 浏览器与Node.js Event Loop的区别
- 1.8.3 垃圾回收机制（标记清除、WeakMap/WeakSet）
- 1.8.4 常见内存泄漏场景

1.9 模块化
- 1.9.1 CommonJS与ES Module对比
- 1.9.2 动态导入、Tree Shaking与副作用

---

## 第二章 HTML与CSS

2.1 HTML基础
- 2.1.1 文档结构与常用标签（文本/链接/图片/列表/表格）
- 2.1.2 表单元素、语义化HTML与data-\*属性

2.2 CSS基础
- 2.2.1 引入方式、选择器、层叠与继承、优先级
- 2.2.2 盒模型、display、overflow
- 2.2.3 定位与层叠上下文（position/z-index/Stacking Context）

2.3 页面布局
- 2.3.1 Flexbox
- 2.3.2 CSS Grid
- 2.3.3 常见布局模式（两栏三栏、居中方案、固定头部与侧边栏）

2.4 响应式设计
- 2.4.1 Media Query与Mobile First
- 2.4.2 响应式图片、自适应字体间距与断点设计

2.5 CSS工程实践
- 2.5.1 CSS Variables与BEM命名
- 2.5.2 CSS Modules与Tailwind CSS（含选型对比）
- 2.5.3 浏览器兼容性基础

2.6 Web可访问性
- 2.6.1 可访问性基础与语义化HTML
- 2.6.2 ARIA属性、键盘导航与焦点管理
- 2.6.3 表单可访问性与检测工具（axe/Lighthouse）

---

## 第三章 TypeScript深度

3.1 TS基础
- 3.1.1 TS解决的问题、基础类型标注与类型推断
- 3.1.2 any/unknown/never/void与类型断言
- 3.1.3 strict模式

3.2 Interface与Type Alias
- 3.2.1 Interface与Type Alias的定义、继承与区别
- 3.2.2 Declaration Merging与Enum选型

3.3 高级类型
- 3.3.1 联合类型、交叉类型、字面量类型与判别联合
- 3.3.2 类型守卫、keyof、typeof、in操作符
- 3.3.3 索引访问类型、映射类型、模板字面量类型
- 3.3.4 条件类型与infer

3.4 泛型
- 3.4.1 泛型函数、接口、类型别名与类
- 3.4.2 泛型约束、默认参数与类型推断
- 3.4.3 分布式条件类型

3.5 Utility Types
- 3.5.1 对象操作类（Partial/Required/Readonly/Pick/Omit/Record）
- 3.5.2 联合与函数类（Exclude/Extract/ReturnType/Parameters/NonNullable/Awaited）

3.6 TS工程实践
- 3.6.1 tsconfig.json与strict系列配置
- 3.6.2 声明文件与第三方库类型
- 3.6.3 satisfies操作符与ESLint集成
- 3.6.4 环境变量类型设计与API请求响应类型设计（含前后端共享类型）

---

## 第四章 浏览器、HTTP与网络原理

4.1 浏览器架构与渲染
- 4.1.1 浏览器多进程架构与主线程
- 4.1.2 从URL到页面的完整流程（DNS/TCP三次握手/TLS握手/请求响应）
- 4.1.3 渲染流程（DOM/CSSOM/Render Tree/Layout/Paint/Composite）

4.2 HTTP基础与REST
- 4.2.1 请求响应结构、Headers、Body、Status Code、Content-Type
- 4.2.2 HTTP方法与幂等性
- 4.2.3 RESTful资源设计（路径参数、查询参数、错误响应）

4.3 HTTPS与现代HTTP
- 4.3.1 加密与证书（对称/非对称加密、证书链、TLS握手流程）
- 4.3.2 HTTP/2多路复用与HTTP/3基础

4.4 缓存与存储
- 4.4.1 浏览器缓存机制（强缓存/协商缓存/Cache-Control/ETag/CDN原理）
- 4.4.2 浏览器存储方案（Cookie/LocalStorage/SessionStorage/IndexedDB选型）

4.5 同源策略与CORS
- 4.5.1 同源策略与简单请求
- 4.5.2 预检请求、CORS配置与常见错误

---

## 第五章 React应用开发

5.1 React基础
- 5.1.1 React解决的问题、项目创建与JSX本质
- 5.1.2 函数组件、Props、State与事件处理
- 5.1.3 条件渲染、列表渲染与key的作用、组件组合

5.2 Hooks
- 5.2.1 useState与useEffect（依赖数组、清理函数）
- 5.2.2 useRef、useMemo、useCallback
- 5.2.3 useReducer与自定义Hook
- 5.2.4 Hook调用规则与Stale Closure

5.3 React与TypeScript
- 5.3.1 Props/children/事件类型设计
- 5.3.2 useState/useRef/useReducer的类型写法
- 5.3.3 泛型组件与API数据类型设计、表单类型设计

5.4 表单处理
- 5.4.1 受控与非受控组件、表单提交与错误展示
- 5.4.2 React Hook Form与Zod校验（含服务端校验错误映射、文件输入控件）

5.5 React Router
- 5.5.1 路由配置、Link、动态路由与嵌套路由
- 5.5.2 路由参数、Query String、懒加载、受保护路由与404页面

5.6 状态管理
- 5.6.1 Local State、Lifting State Up与Context API（含性能问题）
- 5.6.2 Zustand与Redux Toolkit基础
- 5.6.3 客户端状态与服务端状态的区别及方案选型

5.7 数据请求与服务端状态
- 5.7.1 Fetch/Axios与请求状态管理（含AbortController）
- 5.7.2 TanStack Query基础（Query Key、缓存与失效）
- 5.7.3 Mutation、乐观更新、分页查询与无限滚动、请求错误处理

5.8 React原理
- 5.8.1 Virtual DOM、Reconciliation与Diff基本策略、key的底层作用
- 5.8.2 Render触发条件、Render Phase与Commit Phase、State批处理、Hook调用顺序
- 5.8.3 Concurrent Rendering、Suspense、useTransition、useDeferredValue

5.9 React性能优化
- 5.9.1 React DevTools Profiler与避免不必要的重新渲染
- 5.9.2 React.memo、useMemo/useCallback的正确使用与组件拆分
- 5.9.3 列表虚拟化基础、Code Splitting与Lazy Loading

5.10 前端测试
- 5.10.1 测试金字塔与Vitest
- 5.10.2 React Testing Library（组件渲染测试、用户交互测试、表单测试、Mock模块与网络请求）
- 5.10.3 Playwright基础与端到端测试基础

---

## 第六章 Next.js全栈框架（App Router）

6.1 Next.js基础
- 6.1.1 App Router与文件系统路由
- 6.1.2 Layout、Page、Link、useRouter、redirect、notFound
- 6.1.3 Loading UI与Error Boundary

6.2 Server Component与Client Component
- 6.2.1 React Server Components的用途与Client Component（use client）
- 6.2.2 Server与Client边界、数据序列化限制、组件边界设计与常见错误

6.3 渲染模型
- 6.3.1 CSR/SSR/SSG/ISR/Streaming SSR
- 6.3.2 Hydration与不同渲染模型的选型

6.4 数据获取
- 6.4.1 async Server Component与Next.js fetch
- 6.4.2 Parallel Fetch、Sequential Fetch与Request Waterfall
- 6.4.3 服务端与客户端数据获取方案选型

6.5 缓存系统
- 6.5.1 四层缓存机制（Request Memoization/Data Cache/Full Route Cache/Router Cache）
- 6.5.2 revalidate/revalidatePath/revalidateTag与常见缓存问题

6.6 服务端能力
- 6.6.1 Server Actions与表单集成
- 6.6.2 Route Handlers、Middleware与Server Actions的选型
- 6.6.3 Cookies API与Headers API

6.7 Next.js工程实践
- 6.7.1 Metadata与SEO基础
- 6.7.2 next/image、next/font、环境变量与next.config.ts
- 6.7.3 项目目录结构、Core Web Vitals、Lighthouse与Bundle分析基础

6.8 Next.js身份认证
- 6.8.1 Auth.js基础（Credentials Provider、OAuth Provider、Session、JWT Session）
- 6.8.2 Middleware权限控制、Server Component与Server Action权限检查

---

## 第七章 工程化与团队协作

7.1 Git基础
- 7.1.1 仓库结构（Working Tree/Staging Area/Commit）与分支合并
- 7.1.2 Rebase、Cherry Pick、Reset、Revert与冲突解决

7.2 Git团队协作
- 7.2.1 Feature Branch、Pull Request与Code Review
- 7.2.2 Commit Message规范、Squash Merge、Release/Hotfix基础与Git Tag

7.3 包管理
- 7.3.1 npm/pnpm与package.json（dependencies/devDependencies/peerDependencies、lock文件）
- 7.3.2 语义化版本、npm scripts与依赖安全审计

7.4 构建工具
- 7.4.1 Vite开发服务器与生产构建（Source Map、环境变量）
- 7.4.2 Webpack基础认识、Tree Shaking、Code Splitting与Bundle分析

7.5 代码规范
- 7.5.1 ESLint、Prettier与Type-Aware Linting、EditorConfig
- 7.5.2 Husky、lint-staged、Commitlint与Conventional Commits

7.6 Monorepo基础
- 7.6.1 Monorepo解决的问题与pnpm workspace
- 7.6.2 Turborepo基础、共享类型/UI/配置包与适用场景

7.7 软件交付与协作能力
- 7.7.1 阅读陌生代码库、需求拆解与Acceptance Criteria
- 7.7.2 技术方案设计与工作量估算基础
- 7.7.3 Code Review反馈、Breaking Change与Feature Flag
- 7.7.4 Changelog、Rollback、README与Architecture Decision Record

---

## 第八章 后端零基础入门

8.1 后端基本概念
- 8.1.1 什么是后端、客户端与服务器、一次完整请求的生命周期
- 8.1.2 业务逻辑、数据持久化、身份认证与权限控制、第三方服务集成

8.2 API基础
- 8.2.1 什么是API、前后端数据约定（REST API、GraphQL API、JSON格式）
- 8.2.2 Postman基础与API测试基础

8.3 开发环境
- 8.3.1 Node.js安装与nvm版本管理
- 8.3.2 终端基本命令、环境变量、开发/生产环境区别与调试基础

---

## 第九章 Node.js基础（从底层服务器开始）

9.1 Node.js是什么
- 9.1.1 和浏览器JS的区别
- 9.1.2 Node能做什么、Node.js运行时与全局对象

9.2 事件循环与异步编程模型
- 9.2.1 Node.js Event Loop与非阻塞I/O（含libuv基础）
- 9.2.2 异步回调、Promise与async/await在Node中的使用、异步错误处理

9.3 手写第一个服务器
- 9.3.1 http模块与createServer、IncomingMessage/ServerResponse
- 9.3.2 请求方法、URL与Query解析、请求头与请求体读取
- 9.3.3 JSON响应、简单路由分发与404处理、原生服务器的局限

9.4 CommonJS模块系统
- 9.4.1 require与module.exports、模块缓存
- 9.4.2 ES Module与package.json中的type字段、二者互操作

9.5 npm基础
- 9.5.1 npm包管理基础（承接第七章包管理内容，聚焦Node项目场景）

9.6 process对象与环境变量
- 9.6.1 process、process.env、process.argv

9.7 fs与path模块
- 9.7.1 同步与异步文件操作、fs/promises、path模块
- 9.7.2 常见文件操作场景（读写文本/JSON、文件不存在处理、目录创建删除、Path Traversal安全问题、Stream处理大文件）

---

## 第十章 Express Web框架

10.1 为什么需要框架
- 10.1.1 对比手写http模块的痛点、Express项目创建与app实例

10.2 路由基础
- 10.2.1 GET/POST/PUT/PATCH/DELETE
- 10.2.2 路由参数与查询参数
- 10.2.3 用express.Router()拆分路由模块、路由匹配顺序

10.3 中间件
- 10.3.1 中间件是什么（req/res/next）
- 10.3.2 执行顺序、全局中间件与路由级中间件
- 10.3.3 内置中间件（express.json/express.urlencoded/静态文件）与第三方、自定义中间件

10.4 请求处理
- 10.4.1 req.params/req.query/req.body
- 10.4.2 req.headers、Authorization Header、Content-Type与Cookie读取、请求数据校验

10.5 响应处理
- 10.5.1 res.status/res.json/res.send/res.set
- 10.5.2 res.cookie/res.clearCookie、Redirect、文件响应与统一响应格式

10.6 错误处理
- 10.6.1 404兜底处理
- 10.6.2 全局错误处理中间件（含同步/异步错误、try/catch、next(error)、自定义错误类、操作型与程序错误、生产环境错误信息保护）

10.7 🎯里程碑项目：纯内存版Todo List API
- 10.7.1 需求拆解与路由设计
- 10.7.2 CRUD接口实现
- 10.7.3 联调测试（Postman）

10.8 Express项目结构
- 10.8.1 分层结构总览（Routes/Controllers/Services/Repositories/Models/Middlewares/Validators/Config/Utils与依赖方向）

---

## 第十一章 GraphQL基础与工程实践

11.1 为什么Shopify等电商平台转向GraphQL
- 11.1.1 REST的局限与GraphQL解决的问题（REST逐步废弃的背景）

11.2 GraphQL核心概念
- 11.2.1 Schema、Object Type、Scalar Type、Non-Null、List、Enum、Input Type
- 11.2.2 Query与基本语法（Arguments、Variables、Aliases、Fragments）
- 11.2.3 Mutation

11.3 Resolver
- 11.3.1 Resolver职责（Parent/Args/Context/Info）与Query/Mutation/Field Resolver
- 11.3.2 Resolver与Service层的关系

11.4 GraphQL vs REST：对比实战
- 11.4.1 对照第十章学过的REST设计做对比

11.5 在Express中集成GraphQL
- 11.5.1 Apollo Server基础、typeDefs与resolvers
- 11.5.2 Context注入、身份认证与权限控制、错误处理、项目目录结构

11.6 GraphQL性能与安全
- 11.6.1 N+1问题与DataLoader
- 11.6.2 Query Depth/Complexity限制、分页与Rate Limit、错误信息保护

11.7 Shopify GraphQL基础
- 11.7.1 Shopify使用GraphQL的原因、Storefront API与Admin API
- 11.7.2 Connection、Edge与Node、Cursor Pagination、API Cost与Rate Limit处理

---

## 第十二章 PostgreSQL、SQL与数据建模

12.1 数据库基础概念
- 12.1.1 关系型数据库核心概念（Table/Row/Column/Schema/主外键/约束）

12.2 PostgreSQL基础操作
- 12.2.1 安装、创建数据库与用户、连接与psql基础命令
- 12.2.2 备份与恢复基础

12.3 数据类型与约束
- 12.3.1 常用数据类型（INTEGER/BIGINT/NUMERIC/VARCHAR/TEXT/BOOLEAN/DATE/TIMESTAMP/UUID/JSONB）
- 12.3.2 常用约束（NOT NULL/UNIQUE/DEFAULT/CHECK/FOREIGN KEY）

12.4 SQL增删改查
- 12.4.1 CREATE TABLE与INSERT/SELECT/UPDATE/DELETE
- 12.4.2 RETURNING与NULL处理

12.5 SQL查询进阶
- 12.5.1 WHERE条件（AND/OR/NOT/IN/BETWEEN/LIKE与ILIKE）
- 12.5.2 ORDER BY/LIMIT/OFFSET/DISTINCT/CASE

12.6 聚合与分组
- 12.6.1 聚合函数（COUNT/SUM/AVG/MIN/MAX）
- 12.6.2 GROUP BY与HAVING、聚合查询执行顺序

12.7 JOIN与复杂查询
- 12.7.1 INNER/LEFT/RIGHT JOIN与多表JOIN、Self Join基础
- 12.7.2 Subquery与Common Table Expression
- 12.7.3 Window Function基础

12.8 数据建模
- 12.8.1 一对一/一对多/多对多关系与Junction Table
- 12.8.2 ER图、范式化基础与反范式化基础
- 12.8.3 createdAt/updatedAt、软删除与审计字段

12.9 索引与查询性能
- 12.9.1 索引原理（B-Tree、单列/复合/唯一索引、索引列顺序）
- 12.9.2 索引失效场景与EXPLAIN/EXPLAIN ANALYZE
- 12.9.3 全表扫描与慢查询基础

12.10 事务与并发控制
- 12.10.1 事务与ACID、BEGIN/COMMIT/ROLLBACK、事务使用场景
- 12.10.2 隔离级别基础与并发问题（脏读/不可重复读/幻读）
- 12.10.3 悲观锁、乐观锁与死锁基础

12.11 分页与数据访问
- 12.11.1 Offset分页与Cursor分页（含分页稳定性）
- 12.11.2 数据库连接池、N+1查询问题与批量查询/写入

---

## 第十三章 Prisma ORM与数据库工程

13.1 Prisma基础
- 13.1.1 ORM解决的问题、Prisma安装（schema.prisma/datasource/generator）
- 13.1.2 Prisma Client与Prisma Studio

13.2 Prisma Schema设计
- 13.2.1 Model与Field定义、常用装饰器（@id/@default/@unique/@relation）
- 13.2.2 索引装饰器（@@index/@@unique）、@map/@@map与Enum

13.3 Migration工作流
- 13.3.1 prisma migrate dev与Migration文件、Schema变更
- 13.3.2 开发与生产环境Migration、回滚策略、数据迁移与破坏性变更风险

13.4 Prisma CRUD
- 13.4.1 create/createMany、findUnique/findFirst/findMany
- 13.4.2 update/updateMany、delete/deleteMany、upsert

13.5 Prisma查询进阶
- 13.5.1 where/select/include/orderBy/skip与take/cursor
- 13.5.2 Relation Filter、Aggregate、Group By与Raw Query基础

13.6 Prisma事务
- 13.6.1 Batch Transaction与Interactive Transaction、事务超时
- 13.6.2 事务中的错误处理（下单扣库存场景）与乐观并发控制

13.7 Prisma工程实践
- 13.7.1 Prisma Client单例与Repository封装
- 13.7.2 查询性能优化、避免N+1
- 13.7.3 Seed数据、测试数据库、数据库连接管理与生产环境安全实践

---

## 第十四章 认证、授权与Web安全

14.1 认证基础概念
- 14.1.1 Authentication与Authorization的区别、HTTP无状态性、身份凭证与登录状态、前后端职责划分

14.2 密码安全
- 14.2.1 明文密码风险、Hash、Salt与bcrypt
- 14.2.2 密码验证、强度策略、修改与重置

14.3 Session认证
- 14.3.1 Session认证原理（Session ID、Session Store、Cookie传输）
- 14.3.2 登录、验证、注销流程与Session过期处理
- 14.3.3 Redis Session Store与多设备Session管理

14.4 JWT认证
- 14.4.1 JWT结构（Header/Payload/Signature）
- 14.4.2 Access Token与Refresh Token机制
- 14.4.3 Token验证、过期、Refresh Token Rotation、撤销、注销处理与多设备管理

14.5 Cookie安全
- 14.5.1 HttpOnly/Secure/SameSite/Domain/Path、Max-Age与Expires
- 14.5.2 常见Cookie认证错误

14.6 OAuth 2.0与OpenID Connect
- 14.6.1 OAuth 2.0解决的问题、Authorization Code Flow、Access Token与Scope
- 14.6.2 OpenID Connect、ID Token、第三方登录与OAuth安全基础

14.7 权限控制
- 14.7.1 RBAC模型（Role/Permission及其关系）
- 14.7.2 路由权限检查与资源所有权检查
- 14.7.3 前端权限展示、后端权限强制执行与ABAC基础

14.8 常见Web安全问题
- 14.8.1 XSS（存储型/反射型/DOM型）
- 14.8.2 CSRF与SQL Injection
- 14.8.3 NoSQL Injection、Command Injection、Path Traversal、Open Redirect、SSRF基础

14.9 应用安全加固
- 14.9.1 Helmet、Content Security Policy与CORS安全配置
- 14.9.2 Rate Limit、登录失败限流与Brute Force防护
- 14.9.3 请求体大小限制、输入验证与输出编码
- 14.9.4 密钥与Secrets管理、依赖安全审计、安全日志

---

## 第十五章 后端工程能力与API设计

15.1 分层架构
- 15.1.1 路由/Controller/Service/Repository/Model各层职责与Dependency Direction
- 15.1.2 业务逻辑与HTTP解耦、可测试性设计

15.2 请求校验
- 15.2.1 为什么需要服务端校验、Zod Schema校验（Body/Params/Query/环境变量）
- 15.2.2 校验错误格式化与类型推断

15.3 API设计规范
- 15.3.1 资源命名、URL设计、HTTP Method与Status Code选择
- 15.3.2 统一响应格式与统一错误格式
- 15.3.3 分页、过滤、排序、搜索
- 15.3.4 API版本管理与Idempotency Key

15.4 API文档
- 15.4.1 OpenAPI与Swagger UI
- 15.4.2 Request/Response/Error Schema、Authentication文档、API示例与文档同步

15.5 文件上传
- 15.5.1 multipart/form-data与multer、文件类型/大小校验、文件名安全
- 15.5.2 本地存储、S3对象存储、Presigned URL、图片处理基础与文件清理

15.6 Webhook
- 15.6.1 Webhook解决的问题、Webhook Endpoint、签名验证、Raw Body与Timestamp验证
- 15.6.2 Replay Attack防护、幂等性、重复事件处理与重试机制、Webhook日志

15.7 日志系统
- 15.7.1 日志的作用、Log Level与Structured Logging（pino）
- 15.7.2 HTTP访问日志、错误日志、Request ID/Correlation ID、敏感信息脱敏、日志查询基础

15.8 后端测试
- 15.8.1 单元测试与集成测试、API测试（Vitest/Supertest）
- 15.8.2 Service层测试、Controller层测试与数据库测试
- 15.8.3 Mock与Stub、Test Fixture、测试隔离与覆盖率认知

---

## 第十六章 Redis、缓存与后台任务

16.1 Redis基础
- 16.1.1 Redis解决的问题、Key-Value模型与数据结构（String/Hash/List/Set/Sorted Set）
- 16.1.2 TTL、Redis持久化基础与连接管理

16.2 缓存策略
- 16.2.1 缓存适用场景、Cache-Aside模式与Cache Key/TTL设计
- 16.2.2 缓存失效、缓存穿透、击穿、雪崩、数据一致性与缓存监控基础

16.3 Redis应用场景
- 16.3.1 Session Store、Rate Limit、验证码与临时Token
- 16.3.2 分布式锁基础与排行榜基础

16.4 后台任务
- 16.4.1 同步任务与异步任务、Queue、Job、Worker概念与BullMQ基础
- 16.4.2 Job Payload/Status、Job Retry、指数退避、Dead-Letter思想、幂等性与并发控制

16.5 定时任务与通知
- 16.5.1 Cron表达式与常见定时任务场景（邮件发送、报表生成、Webhook重试）
- 16.5.2 任务失败告警与定时任务重复执行问题

---

## 第十七章 第三方服务与支付集成

17.1 第三方API集成
- 17.1.1 认证方式（API Key/Bearer Token/OAuth Token）
- 17.1.2 请求超时、Retry、指数退避、Rate Limit、Circuit Breaker基础、第三方错误映射与Mock

17.2 邮件服务
- 17.2.1 Transactional Email、邮件服务提供商与邮件模板
- 17.2.2 常见邮件场景（验证/密码重置/订单通知）、发送队列与发送状态

17.3 Stripe支付基础
- 17.3.1 Payment Intent与Checkout Session、客户端与服务端职责、支付状态与支付成功页面
- 17.3.2 Stripe Webhook与签名验证、支付幂等性
- 17.3.3 退款基础与支付安全边界

17.4 Shopify集成
- 17.4.1 OAuth安装流程与Admin GraphQL API
- 17.4.2 Product/Order/Inventory同步
- 17.4.3 Shopify Webhook、HMAC签名验证、API Rate Limit、Background Sync与数据一致性/幂等性

---

## 第十八章 Docker、Linux与部署

18.1 Linux基础
- 18.1.1 文件系统与常用目录、常用命令（ls/cd/pwd/cp/mv/rm/mkdir/touch/cat/less/tail/grep/chmod）
- 18.1.2 环境变量、进程与端口、SSH

18.2 Docker基础
- 18.2.1 Image/Container/Volume/Network核心概念
- 18.2.2 Dockerfile编写、Build、Run、Port Mapping、Environment Variable
- 18.2.3 Multi-Stage Build、.dockerignore与Docker安全基础

18.3 Docker Compose
- 18.3.1 Compose文件结构与服务编排（App Service/PostgreSQL Service/Redis Service）
- 18.3.2 Volume/Network配置、Health Check、开发环境编排与生产环境注意事项

18.4 Nginx与进程管理
- 18.4.1 反向代理与Nginx基础配置（静态资源服务、HTTPS配置、Gzip基础）
- 18.4.2 PM2、Process Restart与Zero-Downtime Reload基础

18.5 云平台与AWS基础
- 18.5.1 云计算基础概念（Region/AZ/IAM/Object Storage/Managed Database/Compute Service/Secrets Management/Cloud Logging/环境隔离/成本意识）
- 18.5.2 AWS核心服务（IAM/S3/RDS/EC2/Lambda基础/API Gateway基础/CloudWatch/Secrets Manager/Security Group）与部署方案选型

18.6 CI/CD
- 18.6.1 CI/CD概念与GitHub Actions基础（Workflow/Job与Step）
- 18.6.2 自动安装依赖、Lint、测试、Build、部署、Secrets配置与Rollback策略

---

## 第十九章 可观测性与生产运维

19.1 可观测性基础
- 19.1.1 Logging/Metrics/Tracing三大支柱、可观测性与监控的区别、生产问题排查流程

19.2 应用监控
- 19.2.1 Health Check（Liveness/Readiness）
- 19.2.2 核心指标（Uptime/Latency/Throughput/Error Rate/Resource Usage）

19.3 错误追踪
- 19.3.1 Sentry前端与后端错误监控接入、Source Map上传、Release Tracking
- 19.3.2 User Context、敏感数据保护与错误聚合告警

19.4 日志与追踪
- 19.4.1 集中式日志、Request ID与Correlation ID、跨服务请求追踪
- 19.4.2 慢请求分析、数据库查询日志、第三方请求日志与Background Job日志

19.5 生产运维基础
- 19.5.1 Incident、Severity、Alert与On-Call基础
- 19.5.2 Rollback、Hotfix、Postmortem、Root Cause Analysis与容量扩展基础

---

## 第二十章 系统设计基础

20.1 系统设计方法
- 20.1.1 需求澄清（Functional/Non-Functional Requirements）
- 20.1.2 数据模型设计、API设计、组件拆分、数据流设计、性能扩展性、安全可靠性与Trade-Off表达

20.2 常见系统设计场景
- 20.2.1 登录系统、权限系统、文件上传系统、通知系统设计
- 20.2.2 支付系统、Webhook系统、缓存系统、后台任务系统设计
- 20.2.3 电商订单系统与库存系统设计

20.3 扩展性与可靠性
- 20.3.1 垂直/水平扩展、负载均衡与无状态服务
- 20.3.2 数据库瓶颈、缓存、队列
- 20.3.3 Rate Limit、Timeout、Retry、Circuit Breaker与优雅降级

20.4 数据一致性
- 20.4.1 强一致性与最终一致性、事务边界
- 20.4.2 分布式事务基础、幂等性与重复事件处理
- 20.4.3 Outbox Pattern与Saga Pattern基础

---

## 第二十一章 完整全栈项目（从零构建到生产部署）

21.1 项目规划
- 21.1.1 项目定位与技术选型（目标/业务范围/用户角色/核心功能/非功能需求/技术栈/Monorepo结构/Git协作流程/Definition of Done/项目里程碑）
- 21.1.2 需求分析（注册登录、用户资料、商品管理与分类、库存、购物车、订单、支付流程、权限管理、通知系统、Shopify数据同步、审计日志、管理后台）
- 21.1.3 系统架构设计（系统上下文图、前后端架构、数据库架构、Redis架构、Background Worker、文件存储、支付/邮件服务、Shopify集成、部署架构、安全边界）

21.2 项目初始化与数据库设计
- 21.2.1 项目初始化（Git仓库、Monorepo、前后端项目、TypeScript/ESLint/Prettier/Husky配置、环境变量、Docker Compose、PostgreSQL/Redis配置）
- 21.2.2 数据库设计（User/Role/Permission/Product/Category/ProductImage/Inventory/Cart/CartItem/Order/OrderItem/Payment/RefreshToken/WebhookEvent/AuditLog等模型、索引设计、ER图、Prisma Schema、Migration与Seed数据）

21.3 后端基础架构
- 21.3.1 Express应用启动与配置管理、Prisma Client与Redis Client、Router/Controller/Service/Repository层搭建
- 21.3.2 Zod校验、统一响应格式、自定义错误类与全局错误处理、Structured Logging、Request ID、Health Check与Graceful Shutdown

21.4 认证与权限系统
- 21.4.1 完整认证流程（用户注册、密码Hash、登录、Access/Refresh Token生成、Token Cookie设置、身份认证中间件、Token刷新与Rotation、注销、所有设备注销）
- 21.4.2 邮箱验证、忘记密码与重置密码、登录失败限流、Session与Token清理任务、认证接口测试
- 21.4.3 RBAC权限系统（数据模型、角色与权限初始化、权限检查中间件、资源所有权检查、管理员与普通用户权限、前端权限控制、权限接口测试）

21.5 商品、库存与购物车模块
- 21.5.1 商品与分类模块（创建/查询/更新/删除、分页、搜索、过滤、排序、缓存商品详情与缓存失效、接口测试）
- 21.5.2 文件与图片模块（上传接口、类型/大小校验、S3上传、Presigned URL、商品图片关联、图片删除与孤立文件清理、测试）
- 21.5.3 库存模块（数据模型、增加/减少库存、库存查询、变更日志、乐观锁、超卖问题、接口测试）
- 21.5.4 购物车模块（创建购物车、添加/修改/删除商品、查询购物车、价格重新计算、库存校验、接口测试）

21.6 订单与支付模块
- 21.6.1 订单模块（创建订单、订单号生成、订单快照、金额计算、事务扣减库存、查询列表与详情、更新状态、取消订单、幂等性、接口测试）
- 21.6.2 支付模块（创建Stripe Checkout Session、保存支付记录、支付成功/失败处理、Stripe Webhook与签名验证、支付事件幂等处理、更新订单支付状态、退款基础、测试）

21.7 后台任务与Shopify集成
- 21.7.1 BullMQ任务队列（配置、Worker配置、邮箱验证/密码重置/订单确认/支付通知等邮件任务、Webhook重试任务、失败重试与指数退避、任务幂等性、失败任务监控）
- 21.7.2 Shopify集成（OAuth、店铺安装记录、Access Token安全存储、Product/Order/Inventory同步、Shopify Webhook与HMAC验证、Webhook幂等性、Rate Limit处理、Background Sync、同步状态与错误记录）

21.8 前端开发
- 21.8.1 前端基础架构（Next.js项目初始化、目录结构、全局Layout、Tailwind配置、API Client、TanStack Query配置、全局错误处理、Loading状态、Toast通知、表单基础组件、可访问性基础）
- 21.8.2 认证与权限界面（注册/登录/邮箱验证/忘记密码/重置密码页面、当前用户状态、自动刷新Token、注销、Middleware路由保护、权限菜单、无权限页面、认证端到端测试）
- 21.8.3 商品与后台管理界面（列表页、详情页、搜索/过滤/排序/分页、创建/编辑商品表单、图片上传、删除确认、分类管理、库存管理、乐观更新、界面测试）
- 21.8.4 购物车、订单与支付界面（购物车页面、数量修改、结账页面、创建订单、Stripe支付跳转、支付成功/失败页面、用户订单列表/详情、管理员订单页面、订单状态更新、端到端测试）

21.9 安全加固与测试
- 21.9.1 安全加固（Helmet配置、CSP配置、CORS配置、Cookie安全配置、Rate Limit、请求体限制、输入校验、输出保护、敏感日志脱敏、依赖安全审计、权限绕过测试、常见攻击场景测试）
- 21.9.2 测试体系（测试策略、后端单元/集成测试、API测试、前端组件/交互测试、端到端测试、测试数据库与Seed、Mock第三方服务、测试覆盖率、CI自动测试）

21.10 性能优化
- 21.10.1 后端性能（数据库索引分析、EXPLAIN ANALYZE、N+1检查、Redis缓存、API响应时间）
- 21.10.2 前端性能（Bundle分析、图片优化、路由懒加载、React渲染优化、Core Web Vitals、Lighthouse审计、性能优化记录）

21.11 部署与CI/CD
- 21.11.1 Docker化（前端/后端/Worker Dockerfile、Multi-Stage Build、Docker Compose生产配置、PostgreSQL/Redis生产配置、S3配置、Secrets配置）
- 21.11.2 首次生产部署（域名与HTTPS、数据库Migration部署、首次上线、Rollback演练）
- 21.11.3 CI/CD流水线（Pull Request检查、Lint/Test/Build Workflow、Docker Image Build、自动部署、Environment Secrets、Migration Step、Deployment Verification、Rollback Workflow）

21.12 监控与项目收尾
- 21.12.1 监控接入（Sentry前后端接入、Structured Logging、Request ID、Health/Readiness Check、Uptime监控、错误率与延迟监控、Background Job监控、告警配置、生产故障演练）
- 21.12.2 项目文档（README、本地开发文档、环境变量文档、API文档、数据库ER图、系统架构图、部署文档、测试文档、Security说明、ADR、已知限制、后续改进计划）
- 21.12.3 项目复盘（需求完成情况、架构/数据库/安全/测试/性能/部署/生产问题各环节复盘、技术债务、项目演示、简历项目描述、面试项目讲解）

---

## 第二十二章 面试与求职准备

22.1 技术面试核心
- 22.1.1 JavaScript高频考点（数据类型与内存、作用域与闭包、this、原型继承、Promise、Event Loop、常见代码题与调试题）
- 22.1.2 TypeScript高频考点（Interface与Type、联合与交叉类型、Generic、Utility Types、Type Guard、Conditional Types、工程配置与类型设计题）
- 22.1.3 React与Next.js高频考点（渲染机制、Hooks、State管理、性能优化、Server Component、Next.js缓存、SSR与CSR、前端系统设计基础）
- 22.1.4 Node.js与后端高频考点（Event Loop、Express中间件、错误处理、分层架构、REST API设计、身份认证、权限控制、Redis与后台任务）
- 22.1.5 数据库高频考点（SQL查询、JOIN、索引、事务、锁、数据建模、查询优化、ORM问题）

22.2 系统设计面试
- 22.2.1 系统设计答题框架（需求澄清、API设计、数据库设计、缓存、Queue、文件存储、Trade-Off表达）
- 22.2.2 常见场景实战（支付系统、电商订单系统）

22.3 项目表达与求职材料
- 22.3.1 项目表达技巧（项目背景、个人职责、技术选型、核心架构、技术难点、Bug与故障、性能优化、安全设计、测试与部署、项目成果）
- 22.3.2 简历与作品集打磨（Full Stack简历结构、Shopify经验与全栈能力结合、项目描述、技术成果量化、GitHub仓库整理、README优化、项目演示地址）
- 22.3.3 求职流程管理（LinkedIn资料、求职申请跟踪、模拟面试）
