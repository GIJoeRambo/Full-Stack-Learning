# JavaScript全栈开发 —— 完整知识点目录（最终合并版，层级编号）

> 编号规则：部.章.知识点，例如 5.7.3 表示第五部分第7章第3个知识点

---

# 第一部分：JavaScript 深度（含引擎底层原理，面试重点）

## 1.1 JS基础快速复习
- 1.1.1 Primitive Types / Reference Types
- 1.1.2 数组常用API：map / filter / find / some / every / reduce / sort
- 1.1.3 对象常用操作
- 1.1.4 解构赋值
- 1.1.5 Spread Operator
- 1.1.6 Optional Chaining
- 1.1.7 Nullish Coalescing
- 1.1.8 Map / Set

## 1.2 数据类型与内存模型【重点·面试高频】
- 1.2.1 Primitive vs Reference本质区别
- 1.2.2 Stack Memory（栈内存）
- 1.2.3 Heap Memory（堆内存）
- 1.2.4 值传递 vs 引用传递（JS里的准确说法：共享传递）
- 1.2.5 浅拷贝的实现方式与局限
- 1.2.6 深拷贝的实现方式（手写 + 库方案）
- 1.2.7 structuredClone API

## 1.3 函数【重点】
- 1.3.1 Function Declaration vs Function Expression
- 1.3.2 Arrow Function与普通函数的本质差异
- 1.3.3 First-Class Function（一等公民）
- 1.3.4 Higher Order Function
- 1.3.5 Callback Function
- 1.3.6 IIFE（立即执行函数）及其应用场景
- 1.3.7 Rest Parameters vs arguments对象
- 1.3.8 call / apply / bind 底层实现原理（手写实现）

## 1.4 对象【重点】
- 1.4.1 对象创建的几种方式（字面量/构造函数/Object.create/class）
- 1.4.2 Property Descriptor：writable / enumerable / configurable
- 1.4.3 Getter / Setter
- 1.4.4 Object.keys / Object.values / Object.entries
- 1.4.5 Object.freeze vs Object.seal 区别
- 1.4.6 this与对象的绑定关系

## 1.5 JS执行机制【重点·面试高频】
- 1.5.1 JavaScript Engine工作原理（V8简介）
- 1.5.2 Execution Context（执行上下文）概念
- 1.5.3 Global Execution Context
- 1.5.4 Function Execution Context
- 1.5.5 Execution Context Stack（执行栈）
- 1.5.6 Lexical Environment（词法环境）
- 1.5.7 Variable Environment
- 1.5.8 Hoisting（变量提升与函数提升）底层机制
- 1.5.9 TDZ（暂时性死区）原理

## 1.6 作用域与闭包【重点·面试高频】
- 1.6.1 Scope（作用域）分类
- 1.6.2 Global Scope / Function Scope / Block Scope
- 1.6.3 Scope Chain（作用域链）
- 1.6.4 Closure（闭包）形成原理
- 1.6.5 闭包应用场景（模块模式、防抖节流、计数器）
- 1.6.6 闭包与内存泄漏的关系
- 1.6.7 React中的闭包陷阱（Stale Closure）

## 1.7 垃圾回收【重点·面试高频】
- 1.7.1 Garbage Collection基本概念
- 1.7.2 Reference Counting（引用计数）算法与循环引用问题
- 1.7.3 Mark and Sweep（标记清除）算法
- 1.7.4 WeakMap / WeakSet 的作用与原理
- 1.7.5 Memory Leak的定义
- 1.7.6 常见内存泄漏场景（定时器未清除、事件监听未移除、闭包持有大对象、全局变量意外挂载）

## 1.8 this绑定【重点·面试高频】
- 1.8.1 默认绑定
- 1.8.2 隐式绑定
- 1.8.3 显式绑定（call/apply/bind）
- 1.8.4 new绑定
- 1.8.5 箭头函数的this（词法this）
- 1.8.6 绑定优先级规则
- 1.8.7 面试高频题实战解析（多层嵌套/回调丢失this等场景）

## 1.9 原型与继承【重点·面试高频】
- 1.9.1 prototype 属性
- 1.9.2 __proto__ 与 [[Prototype]]
- 1.9.3 constructor
- 1.9.4 Prototype Chain（原型链）查找机制
- 1.9.5 instanceof 底层原理（手写实现）
- 1.9.6 new关键字执行过程（手写实现new）
- 1.9.7 ES5原型继承的几种方式
- 1.9.8 ES6 class 语法糖本质
- 1.9.9 extends 与 super 底层实现

## 1.10 异步编程【重点·面试高频】
- 1.10.1 同步与异步的本质区别
- 1.10.2 Callback模式与Callback Hell
- 1.10.3 Promise规范（Promise/A+简介）
- 1.10.4 Promise State（pending/fulfilled/rejected）
- 1.10.5 then / catch / finally 链式调用原理
- 1.10.6 Promise.all / allSettled / race / any 区别与实现原理
- 1.10.7 async / await 底层原理（基于Generator+Promise的语法糖本质）
- 1.10.8 手写实现一个简易Promise（面试高频手写题）

## 1.11 Event Loop【重点·面试高频】
- 1.11.1 Call Stack
- 1.11.2 Web APIs（浏览器提供的异步能力）
- 1.11.3 Task Queue（宏任务队列）
- 1.11.4 Microtask Queue（微任务队列）
- 1.11.5 Macro Task vs Micro Task 优先级机制
- 1.11.6 Promise Job / queueMicrotask
- 1.11.7 浏览器Event Loop完整流程
- 1.11.8 Node.js Event Loop（timers/pending callbacks/poll/check/close callbacks六阶段）
- 1.11.9 浏览器与Node Event Loop的差异
- 1.11.10 高频面试题解析（多道经典执行顺序题）

## 1.12 模块化
- 1.12.1 CommonJS规范（require/module.exports原理）
- 1.12.2 ES Module规范
- 1.12.3 export / export default
- 1.12.4 import / Dynamic Import
- 1.12.5 Tree Shaking原理
- 1.12.6 Side Effects对Tree Shaking的影响
- 1.12.7 Bundler与模块化的关系

---

# 第二部分：TypeScript 深度

## 2.1 TS基础
- 2.1.1 基础类型标注
- 2.1.2 类型推断机制
- 2.1.3 类型断言（as / 尖括号语法）及其风险

## 2.2 类型系统
- 2.2.1 Interface详解
- 2.2.2 Type Alias详解
- 2.2.3 Interface vs Type Alias的本质区别与选型
- 2.2.4 Enum（数字枚举/字符串枚举/const enum）
- 2.2.5 Declaration Merging（声明合并）

## 2.3 高级类型【重点】
- 2.3.1 Union Types（联合类型）
- 2.3.2 Intersection Types（交叉类型）
- 2.3.3 Discriminated Union（可辨识联合）实战模式
- 2.3.4 Type Guard（类型守卫）的几种实现方式
- 2.3.5 keyof操作符
- 2.3.6 typeof操作符（类型层面）
- 2.3.7 in操作符（类型层面 / 映射类型中的in）
- 2.3.8 infer关键字与类型推断提取
- 2.3.9 Mapped Types（映射类型）
- 2.3.10 Template Literal Types（模板字面量类型）

## 2.4 泛型【重点】
- 2.4.1 Generic Function（泛型函数）
- 2.4.2 Generic Interface / Generic Class
- 2.4.3 Generic Constraints（泛型约束，extends）
- 2.4.4 默认泛型参数
- 2.4.5 Conditional Types（条件类型）
- 2.4.6 分布式条件类型（Distributive Conditional Types）

## 2.5 Utility Types【重点】
- 2.5.1 Partial / Required
- 2.5.2 Pick / Omit
- 2.5.3 Record
- 2.5.4 Exclude / Extract
- 2.5.5 ReturnType / Parameters
- 2.5.6 NonNullable
- 2.5.7 手写实现常见工具类型（面试常考：手写Partial/Pick等）

## 2.6 TS工程实践
- 2.6.1 tsconfig.json关键配置（strict系列）
- 2.6.2 声明文件（.d.ts）与第三方库类型
- 2.6.3 与ESLint集成（type-aware linting）
- 2.6.4 satisfies操作符

## 2.7 React + TS
- 2.7.1 组件Props类型设计（含children、事件类型）
- 2.7.2 Hook类型设计（useState/useReducer泛型用法）
- 2.7.3 API请求/响应类型设计
- 2.7.4 泛型组件写法
- 2.7.5 前后端共享类型的工程方案（monorepo + shared types）

---

# 第三部分：浏览器与网络原理

## 3.1 浏览器架构
- 3.1.1 Browser Process与Render Process
- 3.1.2 多进程模型的意义（安全性、稳定性）

## 3.2 从URL到页面【重点】
- 3.2.1 DNS解析过程
- 3.2.2 TCP三次握手
- 3.2.3 TLS握手过程
- 3.2.4 HTTP请求发送与响应接收
- 3.2.5 页面渲染整体流程串联

## 3.3 浏览器渲染原理【重点】
- 3.3.1 DOM树构建
- 3.3.2 CSSOM构建
- 3.3.3 Render Tree合并
- 3.3.4 Layout（重排）
- 3.3.5 Paint（重绘）
- 3.3.6 Composite（合成层）

## 3.4 浏览器缓存【重点】
- 3.4.1 强缓存机制
- 3.4.2 协商缓存机制
- 3.4.3 Cache-Control详解
- 3.4.4 ETag
- 3.4.5 Last-Modified

## 3.5 浏览器存储
- 3.5.1 Cookie（属性、作用域、安全标记）
- 3.5.2 LocalStorage
- 3.5.3 SessionStorage
- 3.5.4 IndexedDB基础

## 3.6 前端性能优化（浏览器层面）
- 3.6.1 Reflow（重排）触发场景与规避
- 3.6.2 Repaint（重绘）
- 3.6.3 Lazy Load
- 3.6.4 资源优化（压缩、预加载、懒加载策略）

## 3.7 Web Worker基础

## 3.8 Web安全基础
- 3.8.1 XSS原理与防护
- 3.8.2 CSRF原理与防护
- 3.8.3 CSP（内容安全策略）

---

# 第四部分：HTTP与网络协议

## 4.1 HTTP基础
- 4.1.1 Request结构
- 4.1.2 Response结构
- 4.1.3 Status Code分类详解

## 4.2 HTTP Methods
- 4.2.1 GET
- 4.2.2 POST
- 4.2.3 PUT
- 4.2.4 PATCH
- 4.2.5 DELETE
- 4.2.6 幂等性概念

## 4.3 HTTPS
- 4.3.1 TLS
- 4.3.2 Certificate（证书链）
- 4.3.3 Handshake完整流程

## 4.4 Cookie与Session机制

## 4.5 JWT【重点】
- 4.5.1 JWT结构（Header.Payload.Signature）
- 4.5.2 Access Token
- 4.5.3 Refresh Token
- 4.5.4 Token续期与失效策略

## 4.6 CORS【重点】
- 4.6.1 同源策略
- 4.6.2 简单请求 vs 预检请求（Preflight）
- 4.6.3 CORS响应头详解

## 4.7 HTTP2
- 4.7.1 Multiplexing（多路复用）
- 4.7.2 Header Compression
- 4.7.3 Server Push

## 4.8 HTTP3（了解）
- 4.8.1 QUIC协议基础

## 4.9 CDN原理

## 4.10 RESTful API设计规范

---

# 第五部分：React（基础 + 原理深度）

## 5.1 React基础
- 5.1.1 JSX语法与本质（React.createElement）
- 5.1.2 Component（函数组件）
- 5.1.3 Props
- 5.1.4 State

## 5.2 Hooks基础
- 5.2.1 useState
- 5.2.2 useEffect（依赖数组、清理函数）
- 5.2.3 useRef
- 5.2.4 useMemo
- 5.2.5 useCallback
- 5.2.6 自定义Hook设计原则

## 5.3 表单处理
- 5.3.1 受控 vs 非受控组件
- 5.3.2 React Hook Form
- 5.3.3 Zod表单校验

## 5.4 状态管理
- 5.4.1 Context API
- 5.4.2 Zustand
- 5.4.3 Redux Toolkit（了解对比）
- 5.4.4 TanStack Query（服务端状态）

## 5.5 React Router
- 5.5.1 路由配置
- 5.5.2 嵌套路由与动态路由
- 5.5.3 路由懒加载

## 5.6 Data Fetching
- 5.6.1 Fetch API
- 5.6.2 Axios
- 5.6.3 TanStack Query深入（缓存、失效、乐观更新）

## 5.7 React原理【重点·面试高频】
- 5.7.1 Virtual DOM是什么、为什么需要
- 5.7.2 Diff Algorithm：同层比较策略
- 5.7.3 Diff Algorithm：Key的作用与原理
- 5.7.4 Diff策略详解（tree diff / component diff / element diff）
- 5.7.5 Fiber架构诞生的背景（解决什么问题）
- 5.7.6 Fiber Node数据结构
- 5.7.7 Fiber Tree（current树与workInProgress树）
- 5.7.8 Scheduler调度器与优先级机制
- 5.7.9 Render Phase（协调阶段）
- 5.7.10 Commit Phase（提交阶段）
- 5.7.11 Hooks底层原理：Hook链表结构
- 5.7.12 Hooks调用顺序为什么不能放在条件语句中
- 5.7.13 Hooks更新机制（如何找到对应的Hook）
- 5.7.14 Batch Update（批处理更新机制）
- 5.7.15 Concurrent Update（并发更新）
- 5.7.16 Suspense
- 5.7.17 useTransition / useDeferredValue
- 5.7.18 React性能优化实战（结合以上原理）

---

# 第六部分：Next.js（App Router）

## 6.1 Next.js基础
- 6.1.1 为什么需要 Next.js
- 6.1.2 App Router
- 6.1.3 Layout
- 6.1.4 Navigation（Link、Router、Redirect）
- 6.1.5 Loading / Error处理机制

## 6.2 React Server Components【重点】
- 6.2.1 为什么需要 Server Component
- 6.2.2 Server Component原理
- 6.2.3 Client Component
- 6.2.4 Server / Client边界与最佳实践

## 6.3 渲染模型【重点】
- 6.3.1 CSR
- 6.3.2 SSR
- 6.3.3 SSG
- 6.3.4 ISR
- 6.3.5 Streaming SSR
- 6.3.6 CSR / SSR / SSG / ISR 对比与选型

## 6.4 数据获取
- 6.4.1 async Page
- 6.4.2 Next.js fetch
- 6.4.3 Parallel Fetch
- 6.4.4 Sequential Fetch
- 6.4.5 数据获取最佳实践

## 6.5 Cache System【重点】
- 6.5.1 为什么需要 Cache
- 6.5.2 Request Memoization
- 6.5.3 Data Cache
- 6.5.4 Full Route Cache
- 6.5.5 Router Cache
- 6.5.6 revalidate / revalidatePath / revalidateTag

## 6.6 服务端能力【重点】
- 6.6.1 Server Actions
- 6.6.2 Route Handlers
- 6.6.3 Middleware
- 6.6.4 Server Actions 与 Route Handlers 如何选择

## 6.7 工程化开发
- 6.7.1 Metadata（SEO）
- 6.7.2 next/image
- 6.7.3 next/font
- 6.7.4 环境变量（.env、NEXT_PUBLIC）
- 6.7.5 next.config.ts
- 6.7.6 项目目录结构最佳实践

## 6.8 身份认证
- 6.8.1 Auth.js简介
- 6.8.2 Provider（Google、GitHub、Credentials）
- 6.8.3 Session 与 JWT
- 6.8.4 权限控制（Middleware + Server Component）

## 6.9 综合项目实践【重点】
- 6.9.1 创建Next.js项目
- 6.9.2 商品列表（Server Component）
- 6.9.3 商品详情（Dynamic Route）
- 6.9.4 CRUD（Server Actions）
- 6.9.5 登录系统（Auth.js）
- 6.9.6 项目部署（Vercel）

---

# 第七部分：工程化基础（新增）

> 建议穿插在学习过程中用，不必单独占用整块时间——Git和npm可以很早用起来，Vite/ESLint可以在搭第一个React项目时顺带学，Monorepo和Bundle优化放到项目实战阶段结合实际项目讲效果最好。

## 7.1 Git
- 7.1.1 分支管理（Branch）
- 7.1.2 Merge vs Rebase
- 7.1.3 Cherry Pick
- 7.1.4 常见协作流程（Feature Branch / PR流程）

## 7.2 包管理
- 7.2.1 npm基础
- 7.2.2 pnpm与npm的区别
- 7.2.3 package.json结构详解
- 7.2.4 依赖版本管理（semver规则）

## 7.3 构建工具
- 7.3.1 Vite基础配置
- 7.3.2 Webpack（了解即可）

## 7.4 代码规范
- 7.4.1 ESLint配置
- 7.4.2 Prettier配置
- 7.4.3 ESLint与Prettier协同

## 7.5 Git Hooks
- 7.5.1 Husky配置
- 7.5.2 Commitlint提交规范

## 7.6 Monorepo
- 7.6.1 Turborepo基础
- 7.6.2 pnpm workspace
- 7.6.3 前后端共享类型实战（与2.7.5配套）

## 7.7 环境变量管理
- 7.7.1 dev/test/prod多环境配置
- 7.7.2 .env文件与安全实践

## 7.8 Bundle优化
- 7.8.1 Tree Shaking实战
- 7.8.2 Code Splitting

---

# 第八部分：后端零基础入门

## 8.1 什么是后端
- 8.1.1 客户端-服务器模型
- 8.1.2 一次完整网络请求发生了什么
- 8.1.3 后端到底在"处理"什么（业务逻辑/鉴权/数据读写角色定位）

## 8.2 HTTP基础（零基础视角）
- 8.2.1 URL结构拆解
- 8.2.2 常见请求方法初步认识（GET/POST等）
- 8.2.3 状态码分类初步认识
- 8.2.4 Request/Response长什么样

## 8.3 什么是API
- 8.3.1 为什么需要API
- 8.3.2 RESTful是什么（感性认识）
- 8.3.3 前后端如何"约定"数据格式

## 8.4 什么是数据库
- 8.4.1 为什么要有数据库
- 8.4.2 数据怎么"持久化"

## 8.5 环境搭建
- 8.5.1 Node安装与版本管理（nvm）
- 8.5.2 终端基本操作
- 8.5.3 Postman用法

---

# 第九部分：Node.js基础——从最原始的服务器写起

## 9.1 Node.js是什么
- 9.1.1 和浏览器JS的区别
- 9.1.2 Node能做什么

## 9.2 手写第一个服务器
- 9.2.1 http模块基础
- 9.2.2 处理请求与响应
- 9.2.3 手写一个最简单的服务器（不用框架，理解本质）

## 9.3 CommonJS模块系统
- 9.3.1 require / module.exports原理
- 9.3.2 模块加载机制

## 9.4 npm基础
- 9.4.1 package.json结构
- 9.4.2 依赖安装与管理

## 9.5 fs模块
- 9.5.1 同步 vs 异步读写
- 9.5.2 常见文件操作场景

---

# 第十部分：Express——你的第一个真正Web框架

## 10.1 为什么需要框架
- 10.1.1 对比手写http模块的痛点

## 10.2 路由基础
- 10.2.1 GET / POST / PUT / DELETE
- 10.2.2 路由参数

## 10.3 中间件
- 10.3.1 中间件是什么（本质是函数管道）
- 10.3.2 执行顺序与next()

## 10.4 请求处理
- 10.4.1 params
- 10.4.2 query
- 10.4.3 body

## 10.5 响应处理
- 10.5.1 status
- 10.5.2 json / send

## 10.6 🎯里程碑项目：纯内存版Todo List API
- 10.6.1 需求拆解与路由设计
- 10.6.2 CRUD接口实现
- 10.6.3 联调测试（Postman）

---

# 第十一部分：数据库入门

## 11.1 为什么内存不够用
- 11.1.1 持久化的必要性

## 11.2 PostgreSQL安装与基本操作
- 11.2.1 安装与连接
- 11.2.2 基本命令

## 11.3 SQL基础CRUD
- 11.3.1 INSERT
- 11.3.2 SELECT
- 11.3.3 UPDATE
- 11.3.4 DELETE

## 11.4 SQL进阶
- 11.4.1 WHERE条件
- 11.4.2 JOIN（INNER / LEFT）
- 11.4.3 GROUP BY

## 11.5 数据建模基础
- 11.5.1 一对多关系
- 11.5.2 多对多关系
- 11.5.3 画ER图

## 11.6 Prisma ORM
- 11.6.1 Schema定义
- 11.6.2 Migration工作流
- 11.6.3 Client查询API

## 11.7 🎯里程碑项目：把Todo List改造成真正连数据库
- 11.7.1 Schema设计
- 11.7.2 替换内存存储为数据库操作
- 11.7.3 联调测试

---

# 第十二部分：认证与安全基础

## 12.1 为什么需要认证
- 12.1.1 无状态HTTP的问题

## 12.2 密码存储
- 12.2.1 为什么不能明文存
- 12.2.2 bcrypt加密实践

## 12.3 Session认证
- 12.3.1 原理
- 12.3.2 实现

## 12.4 JWT认证
- 12.4.1 原理
- 12.4.2 实现

## 12.5 权限控制基础
- 12.5.1 简化版RBAC

## 12.6 常见安全问题
- 12.6.1 XSS
- 12.6.2 CSRF
- 12.6.3 SQL注入基础

---

# 第十三部分：进阶后端工程能力

## 13.1 错误处理与统一响应格式

## 13.2 请求校验
- 13.2.1 Zod

## 13.3 日志系统
- 13.3.1 winston / pino

## 13.4 环境变量与配置管理

## 13.5 API设计规范
- 13.5.1 分页 / 过滤 / 排序
- 13.5.2 API版本管理
- 13.5.3 GraphQL基础（Schema/Query/Mutation/Resolver）
- 13.5.4 OpenAPI / Swagger文档生成

## 13.6 NestJS
- 13.6.1 为什么用它（对比Express的痛点）
- 13.6.2 Controller / Service / Module
- 13.6.3 Dependency Injection（依赖注入）原理
- 13.6.4 装饰器（Decorator）基础概念

## 13.7 Redis基础
- 13.7.1 缓存场景实战（Cache-aside）
- 13.7.2 Session存储

## 13.8 MongoDB（选学）
- 13.8.1 与关系型数据库的区别
- 13.8.2 适用场景

## 13.9 测试基础
- 13.9.1 Vitest单元测试
- 13.9.2 Supertest接口测试

---

# 第十四部分：部署与上线

## 14.1 Docker基础概念
- 14.1.1 Image / Container / Volume / Network
- 14.1.2 Dockerfile编写

## 14.2 Linux基础
- 14.2.1 SSH连接与基本命令

## 14.3 Nginx与PM2
- 14.3.1 Nginx反向代理配置
- 14.3.2 PM2进程管理

## 14.4 云平台部署实战
- 14.4.1 VPS部署完整流程
- 14.4.2 Vercel部署

## 14.5 CI/CD基础
- 14.5.1 GitHub Actions workflow语法
- 14.5.2 自动化测试与部署流水线

---

# 第十五部分：系统设计基础

## 15.1 常见系统设计场景
- 15.1.1 登录系统设计
- 15.1.2 权限系统设计
- 15.1.3 文件上传系统设计
- 15.1.4 支付系统设计（Stripe集成思路）
- 15.1.5 消息通知系统设计
- 15.1.6 电商订单系统设计（结合Shopify背景重点练）
- 15.1.7 缓存设计实战
- 15.1.8 高并发基础概念（限流/降级/熔断）

---

# 第十六部分：项目实战

## 16.1 项目1：博客系统（练手，巩固CRUD+认证）

## 16.2 项目2：迷你电商后台管理系统（核心简历项目）
- 16.2.1 需求与数据库设计
- 16.2.2 后端API开发（商品/订单/库存/权限）
- 16.2.3 前端管理界面开发
- 16.2.4 支付集成
- 16.2.5 测试与部署
- 16.2.6 架构文档撰写

## 16.3 项目3：SaaS系统（可选，加深多用户/订阅计费）

## 16.4 项目4：AI SaaS项目（可选，见第十七部分AI章节后再做）

## 16.5 项目复盘与文档整理

---

# 第十七部分：AI应用开发（可选，求职加分项）

## 17.1 LLM基础概念
## 17.2 Prompt Engineering基础
## 17.3 OpenAI API使用
## 17.4 Streaming响应处理
## 17.5 Function Calling
## 17.6 Embedding基础
## 17.7 Vector Database基础
## 17.8 RAG（检索增强生成）基础
## 17.9 MCP基础概念
## 17.10 Agent基础概念
## 17.11 AI SaaS开发实战（把前面全栈技能与AI结合）

---

# 第十八部分：面试专项

## 18.1 分模块面试题库
- 18.1.1 JavaScript面试高频题
- 18.1.2 TypeScript面试高频题
- 18.1.3 浏览器面试高频题
- 18.1.4 HTTP面试高频题
- 18.1.5 React面试高频题
- 18.1.6 Next.js面试高频题
- 18.1.7 Node.js面试高频题
- 18.1.8 数据库面试高频题
- 18.1.9 系统设计面试实战

## 18.2 项目讲解训练
- 18.2.1 项目介绍的结构化表达方法
- 18.2.2 技术难点提炼与表达

## 18.3 简历优化
- 18.3.1 简历撰写（Shopify经验与全栈结合叙事）
- 18.3.2 GitHub/作品集整理

---

## 说明

- 标【重点】【面试高频】的章节是深挖优先级最高的部分，其余偏"知道即可"或"用到再查"
- 与旧版最主要的变化：①新增第七部分"工程化基础"；②后端（原第七至十三部分）整体重新设计为第八至十四部分，路径更循序渐进、加了两个里程碑项目；③原"系统设计基础"独立保留为第十五部分
- 建议顺序：第一部分JS深度 → 第三/四部分浏览器/HTTP → 第二部分TS → 第五/六部分React/Next.js → 第七部分工程化（穿插进行）→ 第八至十四部分后端 → 第十五部分系统设计 → 第十六部分项目实战穿插 → 第十七部分AI(可选) → 第十八部分面试专项冲刺
- 当前进度：正在讲第六部分6.1.1（App Router）
