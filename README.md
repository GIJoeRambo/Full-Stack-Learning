# 第一部分：JavaScript 深度（语言基础 + 引擎底层原理）

## 1.1 JavaScript基础
- 1.1.1 JavaScript简介
- 1.1.2 Primitive Types（基本类型）
- 1.1.3 Reference Types（引用类型）
- 1.1.4 变量声明（var / let / const）
- 1.1.5 类型转换
- 1.1.6 Truthy / Falsy
- 1.1.7 运算符与比较规则
- 1.1.8 数组常用API
- 1.1.9 对象常用API
- 1.1.10 解构赋值
- 1.1.11 Spread / Rest Operator
- 1.1.12 Optional Chaining
- 1.1.13 Nullish Coalescing
- 1.1.14 Map / Set

## 1.2 数据类型与内存模型
- 1.2.1 Primitive Types与Reference Types的本质区别
- 1.2.2 Stack Memory（栈内存）
- 1.2.3 Heap Memory（堆内存）
- 1.2.4 JavaScript中的值传递
- 1.2.5 Shared Reference（共享引用）
- 1.2.6 浅拷贝的实现方式与局限
- 1.2.7 深拷贝的常见实现方式
- 1.2.8 structuredClone API
- 1.2.9 JSON序列化深拷贝的局限

## 1.3 函数
- 1.3.1 Function Declaration
- 1.3.2 Function Expression
- 1.3.3 Arrow Function
- 1.3.4 普通函数与箭头函数的区别
- 1.3.5 First-Class Function（一等函数）
- 1.3.6 Higher-Order Function（高阶函数）
- 1.3.7 Callback Function（回调函数）
- 1.3.8 Pure Function（纯函数）
- 1.3.9 IIFE（立即执行函数）
- 1.3.10 Rest Parameters
- 1.3.11 arguments对象
- 1.3.12 Default Parameters

## 1.4 对象
- 1.4.1 对象字面量
- 1.4.2 构造函数
- 1.4.3 Object.create
- 1.4.4 class语法
- 1.4.5 Property Descriptor
- 1.4.6 writable / enumerable / configurable
- 1.4.7 Getter / Setter
- 1.4.8 Object.keys / Object.values / Object.entries
- 1.4.9 Object.assign
- 1.4.10 Object.freeze
- 1.4.11 Object.seal

## 1.5 JavaScript执行机制
- 1.5.1 JavaScript Engine基本工作方式
- 1.5.2 V8引擎基础认识
- 1.5.3 Execution Context（执行上下文）
- 1.5.4 Global Execution Context
- 1.5.5 Function Execution Context
- 1.5.6 Execution Context Stack（执行栈）
- 1.5.7 Lexical Environment（词法环境）
- 1.5.8 Hoisting（变量提升与函数提升）
- 1.5.9 TDZ（暂时性死区）

## 1.6 作用域与闭包
- 1.6.1 Global Scope
- 1.6.2 Function Scope
- 1.6.3 Block Scope
- 1.6.4 Lexical Scope（词法作用域）
- 1.6.5 Scope Chain（作用域链）
- 1.6.6 Closure（闭包）的形成原理
- 1.6.7 闭包的常见应用场景
- 1.6.8 闭包与内存占用
- 1.6.9 React中的Stale Closure

## 1.7 this绑定
- 1.7.1 默认绑定
- 1.7.2 隐式绑定
- 1.7.3 显式绑定
- 1.7.4 new绑定
- 1.7.5 箭头函数的词法this
- 1.7.6 call / apply / bind
- 1.7.7 this绑定优先级
- 1.7.8 回调函数中的this丢失

## 1.8 原型与继承
- 1.8.1 prototype属性
- 1.8.2 __proto__与[[Prototype]]
- 1.8.3 constructor属性
- 1.8.4 Prototype Chain（原型链）
- 1.8.5 instanceof原理
- 1.8.6 new关键字执行过程
- 1.8.7 ES5继承方式
- 1.8.8 ES6 class
- 1.8.9 extends与super

## 1.9 异步编程
- 1.9.1 同步与异步
- 1.9.2 Callback模式
- 1.9.3 Callback Hell
- 1.9.4 Promise基本概念
- 1.9.5 Promise状态
- 1.9.6 resolve与reject
- 1.9.7 then / catch / finally
- 1.9.8 Promise.all
- 1.9.9 Promise.allSettled
- 1.9.10 Promise.race
- 1.9.11 Promise.any
- 1.9.12 async / await
- 1.9.13 异步错误处理

## 1.10 Event Loop
- 1.10.1 Call Stack
- 1.10.2 Web APIs
- 1.10.3 Task Queue（宏任务队列）
- 1.10.4 Microtask Queue（微任务队列）
- 1.10.5 Macro Task与Micro Task执行顺序
- 1.10.6 Promise Job
- 1.10.7 queueMicrotask
- 1.10.8 浏览器Event Loop
- 1.10.9 Node.js Event Loop基础
- 1.10.10 浏览器与Node.js Event Loop的区别

## 1.11 垃圾回收与内存泄漏
- 1.11.1 Garbage Collection基本概念
- 1.11.2 Mark and Sweep（标记清除）
- 1.11.3 WeakMap / WeakSet
- 1.11.4 Memory Leak的定义
- 1.11.5 定时器未清除
- 1.11.6 事件监听未移除
- 1.11.7 闭包持有大对象
- 1.11.8 全局变量意外挂载

## 1.12 模块化
- 1.12.1 CommonJS规范
- 1.12.2 ES Module规范
- 1.12.3 export / export default
- 1.12.4 import
- 1.12.5 Dynamic Import
- 1.12.6 Tree Shaking基础
- 1.12.7 Side Effects
- 1.12.8 Bundler与模块化的关系

# 第二部分：HTML、CSS与响应式网页

## 2.1 HTML基础
- 2.1.1 HTML文档结构
- 2.1.2 常用文本标签
- 2.1.3 链接与图片
- 2.1.4 列表与表格
- 2.1.5 表单元素
- 2.1.6 label与fieldset
- 2.1.7 语义化HTML
- 2.1.8 data-*属性

## 2.2 CSS基础
- 2.2.1 CSS引入方式
- 2.2.2 CSS选择器
- 2.2.3 Cascade（层叠）
- 2.2.4 Inheritance（继承）
- 2.2.5 Specificity（优先级）
- 2.2.6 常用尺寸单位
- 2.2.7 颜色与字体
- 2.2.8 Box Model
- 2.2.9 display
- 2.2.10 overflow
- 2.2.11 position
- 2.2.12 z-index与Stacking Context

## 2.3 页面布局
- 2.3.1 Flexbox基础
- 2.3.2 Flexbox常见布局
- 2.3.3 CSS Grid基础
- 2.3.4 CSS Grid常见布局
- 2.3.5 两栏与三栏布局
- 2.3.6 页面居中方案
- 2.3.7 固定头部与侧边栏

## 2.4 响应式设计
- 2.4.1 Media Query
- 2.4.2 Mobile First
- 2.4.3 响应式图片
- 2.4.4 自适应字体与间距
- 2.4.5 常见断点设计
- 2.4.6 响应式页面结构

## 2.5 CSS工程实践
- 2.5.1 CSS Variables
- 2.5.2 BEM命名基础
- 2.5.3 CSS Modules
- 2.5.4 Tailwind CSS
- 2.5.5 Tailwind与CSS Modules的选型
- 2.5.6 浏览器兼容性基础

## 2.6 Web可访问性
- 2.6.1 Accessibility基础
- 2.6.2 语义化HTML与可访问性
- 2.6.3 ARIA属性基础
- 2.6.4 键盘导航
- 2.6.5 焦点管理
- 2.6.6 表单可访问性
- 2.6.7 axe与Lighthouse检测

# 第三部分：TypeScript深度（类型系统 + 工程实践）

## 3.1 TypeScript基础
- 3.1.1 TypeScript解决的问题
- 3.1.2 基础类型标注
- 3.1.3 类型推断
- 3.1.4 类型断言
- 3.1.5 any
- 3.1.6 unknown
- 3.1.7 never
- 3.1.8 void
- 3.1.9 strict模式

## 3.2 Interface与Type Alias
- 3.2.1 Interface
- 3.2.2 Type Alias
- 3.2.3 Interface继承
- 3.2.4 Type交叉
- 3.2.5 Interface与Type Alias的区别
- 3.2.6 Declaration Merging
- 3.2.7 Enum与字符串联合类型的选型

## 3.3 高级类型
- 3.3.1 Union Types
- 3.3.2 Intersection Types
- 3.3.3 Literal Types
- 3.3.4 Discriminated Union
- 3.3.5 Type Guard
- 3.3.6 keyof
- 3.3.7 typeof
- 3.3.8 in操作符
- 3.3.9 Indexed Access Types
- 3.3.10 Mapped Types
- 3.3.11 Template Literal Types
- 3.3.12 Conditional Types
- 3.3.13 infer

## 3.4 泛型
- 3.4.1 Generic Function
- 3.4.2 Generic Interface
- 3.4.3 Generic Type Alias
- 3.4.4 Generic Class
- 3.4.5 Generic Constraints
- 3.4.6 默认泛型参数
- 3.4.7 泛型与类型推断
- 3.4.8 分布式条件类型

## 3.5 Utility Types
- 3.5.1 Partial
- 3.5.2 Required
- 3.5.3 Readonly
- 3.5.4 Pick
- 3.5.5 Omit
- 3.5.6 Record
- 3.5.7 Exclude
- 3.5.8 Extract
- 3.5.9 ReturnType
- 3.5.10 Parameters
- 3.5.11 NonNullable
- 3.5.12 Awaited

## 3.6 TypeScript工程实践
- 3.6.1 tsconfig.json
- 3.6.2 strict系列配置
- 3.6.3 module与moduleResolution
- 3.6.4 声明文件
- 3.6.5 第三方库类型
- 3.6.6 satisfies操作符
- 3.6.7 TypeScript与ESLint集成
- 3.6.8 环境变量类型设计
- 3.6.9 API请求与响应类型设计
- 3.6.10 前后端共享类型基础

# 第四部分：浏览器、HTTP与网络原理

## 4.1 浏览器架构
- 4.1.1 Browser Process
- 4.1.2 Render Process
- 4.1.3 多进程模型
- 4.1.4 浏览器主线程
- 4.1.5 Web APIs与浏览器能力

## 4.2 从URL到页面
- 4.2.1 URL结构
- 4.2.2 DNS解析
- 4.2.3 TCP三次握手
- 4.2.4 TLS握手
- 4.2.5 HTTP请求发送
- 4.2.6 HTTP响应接收
- 4.2.7 页面渲染整体流程

## 4.3 浏览器渲染原理
- 4.3.1 DOM树构建
- 4.3.2 CSSOM构建
- 4.3.3 Render Tree
- 4.3.4 Layout（重排）
- 4.3.5 Paint（重绘）
- 4.3.6 Composite（合成）
- 4.3.7 Stacking Context
- 4.3.8 渲染性能问题

## 4.4 HTTP基础
- 4.4.1 Request结构
- 4.4.2 Response结构
- 4.4.3 Headers
- 4.4.4 Body
- 4.4.5 Status Code
- 4.4.6 Content-Type
- 4.4.7 JSON数据格式

## 4.5 HTTP Methods与REST
- 4.5.1 GET
- 4.5.2 POST
- 4.5.3 PUT
- 4.5.4 PATCH
- 4.5.5 DELETE
- 4.5.6 幂等性
- 4.5.7 RESTful资源设计
- 4.5.8 路径参数与查询参数
- 4.5.9 REST API错误响应

## 4.6 HTTPS与现代HTTP
- 4.6.1 对称加密与非对称加密
- 4.6.2 Certificate（证书）
- 4.6.3 Certificate Chain（证书链）
- 4.6.4 TLS握手流程
- 4.6.5 HTTP/2多路复用
- 4.6.6 HTTP/2 Header Compression
- 4.6.7 HTTP/3与QUIC基础

## 4.7 浏览器缓存与CDN
- 4.7.1 强缓存
- 4.7.2 协商缓存
- 4.7.3 Cache-Control
- 4.7.4 ETag
- 4.7.5 Last-Modified
- 4.7.6 CDN基本原理
- 4.7.7 静态资源缓存策略
- 4.7.8 API缓存策略基础

## 4.8 浏览器存储
- 4.8.1 Cookie
- 4.8.2 LocalStorage
- 4.8.3 SessionStorage
- 4.8.4 IndexedDB基础
- 4.8.5 不同存储方式的选型

## 4.9 同源策略与CORS
- 4.9.1 Origin的组成
- 4.9.2 Same-Origin Policy
- 4.9.3 简单请求
- 4.9.4 Preflight Request
- 4.9.5 Access-Control-Allow-Origin
- 4.9.6 Credentials与Cookie
- 4.9.7 CORS常见配置错误

# 第五部分：React应用开发（基础 + 工程实践）

## 5.1 React基础
- 5.1.1 React解决的问题
- 5.1.2 创建React项目
- 5.1.3 JSX语法
- 5.1.4 JSX的本质
- 5.1.5 函数组件
- 5.1.6 Props
- 5.1.7 State
- 5.1.8 事件处理
- 5.1.9 条件渲染
- 5.1.10 列表渲染
- 5.1.11 Key的作用
- 5.1.12 组件组合

## 5.2 Hooks基础
- 5.2.1 useState
- 5.2.2 useEffect
- 5.2.3 依赖数组
- 5.2.4 Effect清理函数
- 5.2.5 useRef
- 5.2.6 useMemo
- 5.2.7 useCallback
- 5.2.8 useReducer
- 5.2.9 自定义Hook
- 5.2.10 Hook调用规则
- 5.2.11 Stale Closure

## 5.3 React与TypeScript
- 5.3.1 Props类型设计
- 5.3.2 children类型
- 5.3.3 事件类型
- 5.3.4 useState类型
- 5.3.5 useRef类型
- 5.3.6 useReducer类型
- 5.3.7 泛型组件
- 5.3.8 API数据类型
- 5.3.9 表单类型设计

## 5.4 表单处理
- 5.4.1 受控组件
- 5.4.2 非受控组件
- 5.4.3 表单提交
- 5.4.4 表单错误展示
- 5.4.5 React Hook Form
- 5.4.6 Zod表单校验
- 5.4.7 服务端校验错误映射
- 5.4.8 文件输入控件

## 5.5 React Router
- 5.5.1 路由配置
- 5.5.2 Link与Navigation
- 5.5.3 动态路由
- 5.5.4 嵌套路由
- 5.5.5 路由参数
- 5.5.6 Query String
- 5.5.7 路由懒加载
- 5.5.8 受保护路由
- 5.5.9 404页面

## 5.6 状态管理
- 5.6.1 Local State
- 5.6.2 Lifting State Up
- 5.6.3 Context API
- 5.6.4 Context性能问题
- 5.6.5 Zustand
- 5.6.6 Redux Toolkit基础
- 5.6.7 客户端状态与服务端状态的区别
- 5.6.8 状态管理方案选型

## 5.7 数据请求与服务端状态
- 5.7.1 Fetch API
- 5.7.2 Axios
- 5.7.3 请求状态管理
- 5.7.4 AbortController
- 5.7.5 TanStack Query
- 5.7.6 Query Key
- 5.7.7 缓存与失效
- 5.7.8 Mutation
- 5.7.9 乐观更新
- 5.7.10 分页查询
- 5.7.11 无限滚动基础
- 5.7.12 请求错误处理

## 5.8 React原理
- 5.8.1 Virtual DOM
- 5.8.2 Reconciliation
- 5.8.3 Diff基本策略
- 5.8.4 Key的底层作用
- 5.8.5 Render触发条件
- 5.8.6 Render Phase
- 5.8.7 Commit Phase
- 5.8.8 State批处理
- 5.8.9 Hook调用顺序
- 5.8.10 Concurrent Rendering基础
- 5.8.11 Suspense基础
- 5.8.12 useTransition
- 5.8.13 useDeferredValue

## 5.9 React性能优化
- 5.9.1 React DevTools Profiler
- 5.9.2 避免不必要的重新渲染
- 5.9.3 React.memo
- 5.9.4 useMemo的正确使用
- 5.9.5 useCallback的正确使用
- 5.9.6 组件拆分
- 5.9.7 列表虚拟化基础
- 5.9.8 Code Splitting
- 5.9.9 Lazy Loading

## 5.10 前端测试
- 5.10.1 测试金字塔
- 5.10.2 Vitest
- 5.10.3 React Testing Library
- 5.10.4 组件渲染测试
- 5.10.5 用户交互测试
- 5.10.6 表单测试
- 5.10.7 Mock模块
- 5.10.8 Mock网络请求
- 5.10.9 Playwright基础
- 5.10.10 端到端测试基础

# 第六部分：Next.js全栈框架（App Router）

## 6.1 Next.js基础
- 6.1.1 Next.js解决的问题
- 6.1.2 App Router
- 6.1.3 文件系统路由
- 6.1.4 Layout
- 6.1.5 Page
- 6.1.6 Link
- 6.1.7 useRouter
- 6.1.8 redirect
- 6.1.9 notFound
- 6.1.10 Loading UI
- 6.1.11 Error Boundary

## 6.2 Server Component与Client Component
- 6.2.1 React Server Components
- 6.2.2 Server Component的用途
- 6.2.3 Client Component
- 6.2.4 use client
- 6.2.5 Server与Client边界
- 6.2.6 数据序列化限制
- 6.2.7 组件边界设计
- 6.2.8 常见错误与最佳实践

## 6.3 渲染模型
- 6.3.1 CSR
- 6.3.2 SSR
- 6.3.3 SSG
- 6.3.4 ISR
- 6.3.5 Streaming SSR
- 6.3.6 Hydration
- 6.3.7 不同渲染模型的选型

## 6.4 数据获取
- 6.4.1 async Server Component
- 6.4.2 Next.js fetch
- 6.4.3 Parallel Fetch
- 6.4.4 Sequential Fetch
- 6.4.5 Request Waterfall
- 6.4.6 服务端数据获取
- 6.4.7 客户端数据获取
- 6.4.8 数据获取方案选型

## 6.5 Cache System
- 6.5.1 Request Memoization
- 6.5.2 Data Cache
- 6.5.3 Full Route Cache
- 6.5.4 Router Cache
- 6.5.5 动态路由与缓存
- 6.5.6 revalidate
- 6.5.7 revalidatePath
- 6.5.8 revalidateTag
- 6.5.9 缓存常见问题

## 6.6 服务端能力
- 6.6.1 Server Actions
- 6.6.2 Route Handlers
- 6.6.3 Middleware
- 6.6.4 Cookies API
- 6.6.5 Headers API
- 6.6.6 Server Actions与Route Handlers的选型
- 6.6.7 表单与Server Actions
- 6.6.8 服务端错误处理

## 6.7 Next.js工程实践
- 6.7.1 Metadata
- 6.7.2 SEO基础
- 6.7.3 next/image
- 6.7.4 next/font
- 6.7.5 环境变量
- 6.7.6 next.config.ts
- 6.7.7 项目目录结构
- 6.7.8 Core Web Vitals
- 6.7.9 Lighthouse
- 6.7.10 Bundle分析基础

## 6.8 Next.js身份认证
- 6.8.1 Auth.js基础
- 6.8.2 Credentials Provider
- 6.8.3 OAuth Provider
- 6.8.4 Session
- 6.8.5 JWT Session
- 6.8.6 Middleware权限控制
- 6.8.7 Server Component权限检查
- 6.8.8 Server Action权限检查

# 第七部分：工程化与团队协作

## 7.1 Git基础
- 7.1.1 Repository
- 7.1.2 Working Tree
- 7.1.3 Staging Area
- 7.1.4 Commit
- 7.1.5 Branch
- 7.1.6 Merge
- 7.1.7 Rebase
- 7.1.8 Cherry Pick
- 7.1.9 Reset
- 7.1.10 Revert
- 7.1.11 Conflict解决

## 7.2 Git团队协作
- 7.2.1 Feature Branch
- 7.2.2 Pull Request
- 7.2.3 Code Review
- 7.2.4 Commit Message
- 7.2.5 Squash Merge
- 7.2.6 Release Branch基础
- 7.2.7 Hotfix基础
- 7.2.8 Git Tag

## 7.3 包管理
- 7.3.1 npm
- 7.3.2 pnpm
- 7.3.3 package.json
- 7.3.4 package-lock与pnpm-lock
- 7.3.5 dependencies
- 7.3.6 devDependencies
- 7.3.7 peerDependencies
- 7.3.8 Semantic Versioning
- 7.3.9 npm scripts
- 7.3.10 依赖安全审计

## 7.4 构建工具
- 7.4.1 Vite
- 7.4.2 Development Server
- 7.4.3 Production Build
- 7.4.4 Source Map
- 7.4.5 Environment Variables
- 7.4.6 Webpack基础认识
- 7.4.7 Tree Shaking
- 7.4.8 Code Splitting
- 7.4.9 Bundle分析

## 7.5 代码规范
- 7.5.1 ESLint
- 7.5.2 Prettier
- 7.5.3 Type-Aware Linting
- 7.5.4 EditorConfig
- 7.5.5 Husky
- 7.5.6 lint-staged
- 7.5.7 Commitlint
- 7.5.8 Conventional Commits

## 7.6 Monorepo基础
- 7.6.1 Monorepo解决的问题
- 7.6.2 pnpm workspace
- 7.6.3 Turborepo基础
- 7.6.4 Shared Types
- 7.6.5 Shared UI Package
- 7.6.6 Shared Config
- 7.6.7 Monorepo适用场景

## 7.7 软件交付与协作能力
- 7.7.1 阅读陌生代码库
- 7.7.2 需求拆解
- 7.7.3 Acceptance Criteria
- 7.7.4 技术方案设计
- 7.7.5 工作量估算基础
- 7.7.6 Code Review反馈
- 7.7.7 Breaking Change
- 7.7.8 Feature Flag
- 7.7.9 Changelog
- 7.7.10 Rollback
- 7.7.11 README
- 7.7.12 Architecture Decision Record

# 第八部分：后端零基础入门

## 8.1 后端基本概念
- 8.1.1 什么是后端
- 8.1.2 客户端与服务器
- 8.1.3 一次完整请求的生命周期
- 8.1.4 业务逻辑
- 8.1.5 数据持久化
- 8.1.6 身份认证
- 8.1.7 权限控制
- 8.1.8 第三方服务集成

## 8.2 API基础
- 8.2.1 什么是API
- 8.2.2 前后端数据约定
- 8.2.3 REST API
- 8.2.4 GraphQL API
- 8.2.5 JSON请求与响应
- 8.2.6 Postman基础
- 8.2.7 API测试基础

## 8.3 开发环境
- 8.3.1 Node.js安装
- 8.3.2 nvm版本管理
- 8.3.3 终端基本命令
- 8.3.4 环境变量
- 8.3.5 开发环境与生产环境
- 8.3.6 调试基础

# 第九部分：Node.js基础（从底层服务器开始）

## 9.1 Node.js基础
- 9.1.1 Node.js是什么
- 9.1.2 Node.js与浏览器JavaScript的区别
- 9.1.3 Node.js能做什么
- 9.1.4 Node.js运行时
- 9.1.5 Node.js全局对象

## 9.2 Node.js异步模型
- 9.2.1 Node.js Event Loop
- 9.2.2 非阻塞I/O
- 9.2.3 libuv基础
- 9.2.4 异步回调
- 9.2.5 Promise与Node.js
- 9.2.6 async / await与Node.js
- 9.2.7 异步错误处理

## 9.3 原生HTTP服务器
- 9.3.1 http模块
- 9.3.2 createServer
- 9.3.3 IncomingMessage
- 9.3.4 ServerResponse
- 9.3.5 请求方法与URL
- 9.3.6 URL与Query解析
- 9.3.7 请求头处理
- 9.3.8 请求体读取
- 9.3.9 JSON响应
- 9.3.10 路由分发
- 9.3.11 404处理
- 9.3.12 原生服务器的局限

## 9.4 Node.js模块系统
- 9.4.1 CommonJS
- 9.4.2 require
- 9.4.3 module.exports
- 9.4.4 模块缓存
- 9.4.5 ES Module
- 9.4.6 package.json中的type字段
- 9.4.7 CommonJS与ES Module互操作

## 9.5 Node.js核心模块
- 9.5.1 process
- 9.5.2 process.env
- 9.5.3 process.argv
- 9.5.4 fs
- 9.5.5 fs/promises
- 9.5.6 path
- 9.5.7 url
- 9.5.8 crypto
- 9.5.9 events
- 9.5.10 Buffer
- 9.5.11 Stream基础

## 9.6 文件与数据处理
- 9.6.1 同步与异步文件操作
- 9.6.2 读取文本文件
- 9.6.3 写入文本文件
- 9.6.4 JSON文件读写
- 9.6.5 文件不存在时的处理
- 9.6.6 目录创建
- 9.6.7 文件删除
- 9.6.8 Path Traversal安全问题
- 9.6.9 Stream处理大文件

# 第十部分：Express Web框架

## 10.1 Express基础
- 10.1.1 为什么需要Web框架
- 10.1.2 Express项目创建
- 10.1.3 app实例
- 10.1.4 启动服务器
- 10.1.5 Express与原生HTTP的关系

## 10.2 路由
- 10.2.1 GET
- 10.2.2 POST
- 10.2.3 PUT
- 10.2.4 PATCH
- 10.2.5 DELETE
- 10.2.6 路由参数
- 10.2.7 查询参数
- 10.2.8 express.Router
- 10.2.9 路由模块拆分
- 10.2.10 路由匹配顺序

## 10.3 中间件
- 10.3.1 中间件的本质
- 10.3.2 req / res / next
- 10.3.3 中间件执行顺序
- 10.3.4 全局中间件
- 10.3.5 路由级中间件
- 10.3.6 express.json
- 10.3.7 express.urlencoded
- 10.3.8 静态文件中间件
- 10.3.9 第三方中间件
- 10.3.10 自定义中间件

## 10.4 请求处理
- 10.4.1 req.params
- 10.4.2 req.query
- 10.4.3 req.body
- 10.4.4 req.headers
- 10.4.5 Authorization Header
- 10.4.6 Content-Type
- 10.4.7 Cookie读取
- 10.4.8 请求数据校验

## 10.5 响应处理
- 10.5.1 res.status
- 10.5.2 res.json
- 10.5.3 res.send
- 10.5.4 res.set
- 10.5.5 res.cookie
- 10.5.6 res.clearCookie
- 10.5.7 Redirect
- 10.5.8 文件响应
- 10.5.9 统一响应格式

## 10.6 错误处理
- 10.6.1 同步错误
- 10.6.2 异步错误
- 10.6.3 try / catch
- 10.6.4 next(error)
- 10.6.5 404兜底
- 10.6.6 全局错误处理中间件
- 10.6.7 自定义错误类
- 10.6.8 操作型错误与程序错误
- 10.6.9 生产环境错误信息保护

## 10.7 Express项目结构
- 10.7.1 Routes
- 10.7.2 Controllers
- 10.7.3 Services
- 10.7.4 Repositories
- 10.7.5 Models
- 10.7.6 Middlewares
- 10.7.7 Validators
- 10.7.8 Config
- 10.7.9 Utils
- 10.7.10 依赖方向与职责边界

# 第十一部分：GraphQL基础与工程实践

## 11.1 GraphQL基础
- 11.1.1 GraphQL解决的问题
- 11.1.2 GraphQL与REST的区别
- 11.1.3 Schema
- 11.1.4 Object Type
- 11.1.5 Scalar Type
- 11.1.6 Non-Null
- 11.1.7 List
- 11.1.8 Enum
- 11.1.9 Input Type

## 11.2 Query与Mutation
- 11.2.1 Query
- 11.2.2 Mutation
- 11.2.3 Arguments
- 11.2.4 Variables
- 11.2.5 Aliases
- 11.2.6 Fragments
- 11.2.7 Operation Name
- 11.2.8 错误响应

## 11.3 Resolver
- 11.3.1 Resolver的职责
- 11.3.2 Parent
- 11.3.3 Args
- 11.3.4 Context
- 11.3.5 Info
- 11.3.6 Query Resolver
- 11.3.7 Mutation Resolver
- 11.3.8 Field Resolver
- 11.3.9 Resolver与Service层

## 11.4 Express集成GraphQL
- 11.4.1 Apollo Server
- 11.4.2 expressMiddleware
- 11.4.3 typeDefs
- 11.4.4 resolvers
- 11.4.5 Context注入
- 11.4.6 身份认证
- 11.4.7 权限控制
- 11.4.8 错误处理
- 11.4.9 项目目录结构

## 11.5 GraphQL性能与安全
- 11.5.1 N+1问题
- 11.5.2 DataLoader
- 11.5.3 Query Depth限制
- 11.5.4 Query Complexity基础
- 11.5.5 分页
- 11.5.6 Rate Limit
- 11.5.7 GraphQL错误信息保护

## 11.6 Shopify GraphQL基础
- 11.6.1 Shopify使用GraphQL的原因
- 11.6.2 Storefront API
- 11.6.3 Admin API
- 11.6.4 Connection
- 11.6.5 Edge与Node
- 11.6.6 Cursor Pagination
- 11.6.7 API Cost基础
- 11.6.8 Rate Limit处理

# 第十二部分：PostgreSQL、SQL与数据建模

## 12.1 数据库基础
- 12.1.1 数据持久化
- 12.1.2 关系型数据库
- 12.1.3 Table
- 12.1.4 Row
- 12.1.5 Column
- 12.1.6 Schema
- 12.1.7 Primary Key
- 12.1.8 Foreign Key
- 12.1.9 Constraint

## 12.2 PostgreSQL基础
- 12.2.1 PostgreSQL安装
- 12.2.2 创建数据库
- 12.2.3 创建用户
- 12.2.4 连接数据库
- 12.2.5 psql基础命令
- 12.2.6 数据库备份基础
- 12.2.7 数据库恢复基础

## 12.3 数据类型与约束
- 12.3.1 INTEGER
- 12.3.2 BIGINT
- 12.3.3 NUMERIC与DECIMAL
- 12.3.4 VARCHAR与TEXT
- 12.3.5 BOOLEAN
- 12.3.6 DATE与TIMESTAMP
- 12.3.7 UUID
- 12.3.8 JSONB
- 12.3.9 NOT NULL
- 12.3.10 UNIQUE
- 12.3.11 DEFAULT
- 12.3.12 CHECK
- 12.3.13 FOREIGN KEY

## 12.4 SQL CRUD
- 12.4.1 CREATE TABLE
- 12.4.2 INSERT
- 12.4.3 SELECT
- 12.4.4 UPDATE
- 12.4.5 DELETE
- 12.4.6 RETURNING
- 12.4.7 NULL处理

## 12.5 SQL查询
- 12.5.1 WHERE
- 12.5.2 AND / OR / NOT
- 12.5.3 IN
- 12.5.4 BETWEEN
- 12.5.5 LIKE与ILIKE
- 12.5.6 ORDER BY
- 12.5.7 LIMIT
- 12.5.8 OFFSET
- 12.5.9 DISTINCT
- 12.5.10 CASE

## 12.6 聚合与分组
- 12.6.1 COUNT
- 12.6.2 SUM
- 12.6.3 AVG
- 12.6.4 MIN与MAX
- 12.6.5 GROUP BY
- 12.6.6 HAVING
- 12.6.7 聚合查询执行顺序

## 12.7 JOIN与复杂查询
- 12.7.1 INNER JOIN
- 12.7.2 LEFT JOIN
- 12.7.3 RIGHT JOIN基础
- 12.7.4 多表JOIN
- 12.7.5 Self Join基础
- 12.7.6 Subquery
- 12.7.7 Common Table Expression
- 12.7.8 Window Function基础

## 12.8 数据建模
- 12.8.1 一对一关系
- 12.8.2 一对多关系
- 12.8.3 多对多关系
- 12.8.4 Junction Table
- 12.8.5 ER Diagram
- 12.8.6 Normalization基础
- 12.8.7 Denormalization基础
- 12.8.8 createdAt与updatedAt
- 12.8.9 Soft Delete
- 12.8.10 Audit Fields

## 12.9 索引与查询性能
- 12.9.1 索引解决的问题
- 12.9.2 B-Tree基础
- 12.9.3 单列索引
- 12.9.4 复合索引
- 12.9.5 唯一索引
- 12.9.6 索引列顺序
- 12.9.7 索引失效场景
- 12.9.8 EXPLAIN
- 12.9.9 EXPLAIN ANALYZE
- 12.9.10 全表扫描
- 12.9.11 慢查询基础

## 12.10 事务与并发控制
- 12.10.1 Transaction
- 12.10.2 ACID
- 12.10.3 BEGIN / COMMIT / ROLLBACK
- 12.10.4 事务使用场景
- 12.10.5 事务隔离级别基础
- 12.10.6 Dirty Read
- 12.10.7 Non-Repeatable Read
- 12.10.8 Phantom Read
- 12.10.9 悲观锁
- 12.10.10 乐观锁
- 12.10.11 Deadlock基础

## 12.11 分页与数据访问
- 12.11.1 Offset Pagination
- 12.11.2 Cursor Pagination
- 12.11.3 分页稳定性
- 12.11.4 数据库连接池
- 12.11.5 N+1查询问题
- 12.11.6 批量查询
- 12.11.7 批量写入

# 第十三部分：Prisma ORM与数据库工程

## 13.1 Prisma基础
- 13.1.1 ORM解决的问题
- 13.1.2 Prisma安装
- 13.1.3 schema.prisma
- 13.1.4 datasource
- 13.1.5 generator
- 13.1.6 Prisma Client
- 13.1.7 Prisma Studio

## 13.2 Prisma Schema
- 13.2.1 Model
- 13.2.2 Field
- 13.2.3 @id
- 13.2.4 @default
- 13.2.5 @unique
- 13.2.6 @relation
- 13.2.7 @@index
- 13.2.8 @@unique
- 13.2.9 @map与@@map
- 13.2.10 Enum

## 13.3 Migration工作流
- 13.3.1 prisma migrate dev
- 13.3.2 Migration文件
- 13.3.3 Schema变更
- 13.3.4 开发环境Migration
- 13.3.5 生产环境Migration
- 13.3.6 Migration回滚策略
- 13.3.7 数据迁移
- 13.3.8 破坏性变更风险

## 13.4 Prisma CRUD
- 13.4.1 create
- 13.4.2 createMany
- 13.4.3 findUnique
- 13.4.4 findFirst
- 13.4.5 findMany
- 13.4.6 update
- 13.4.7 updateMany
- 13.4.8 delete
- 13.4.9 deleteMany
- 13.4.10 upsert

## 13.5 Prisma查询
- 13.5.1 where
- 13.5.2 select
- 13.5.3 include
- 13.5.4 orderBy
- 13.5.5 skip与take
- 13.5.6 cursor
- 13.5.7 Relation Filter
- 13.5.8 Aggregate
- 13.5.9 Group By
- 13.5.10 Raw Query基础

## 13.6 Prisma事务
- 13.6.1 Batch Transaction
- 13.6.2 Interactive Transaction
- 13.6.3 事务超时
- 13.6.4 事务中的错误处理
- 13.6.5 下单与扣库存事务
- 13.6.6 乐观并发控制

## 13.7 Prisma工程实践
- 13.7.1 Prisma Client单例
- 13.7.2 Repository封装
- 13.7.3 查询性能
- 13.7.4 避免N+1
- 13.7.5 Seed数据
- 13.7.6 测试数据库
- 13.7.7 数据库连接管理
- 13.7.8 生产环境安全实践

# 第十四部分：认证、授权与Web安全

## 14.1 认证基础
- 14.1.1 Authentication
- 14.1.2 Authorization
- 14.1.3 HTTP无状态性
- 14.1.4 身份凭证
- 14.1.5 登录状态
- 14.1.6 前端与后端的职责

## 14.2 密码安全
- 14.2.1 明文密码风险
- 14.2.2 Hash
- 14.2.3 Salt
- 14.2.4 bcrypt
- 14.2.5 密码验证
- 14.2.6 密码强度策略
- 14.2.7 密码修改
- 14.2.8 密码重置

## 14.3 Session认证
- 14.3.1 Session认证原理
- 14.3.2 Session ID
- 14.3.3 Session Store
- 14.3.4 Cookie传输
- 14.3.5 登录
- 14.3.6 Session验证
- 14.3.7 注销
- 14.3.8 Session过期
- 14.3.9 Redis Session Store
- 14.3.10 多设备Session管理

## 14.4 JWT认证
- 14.4.1 JWT结构
- 14.4.2 Header
- 14.4.3 Payload
- 14.4.4 Signature
- 14.4.5 Access Token
- 14.4.6 Refresh Token
- 14.4.7 Token验证
- 14.4.8 Token过期
- 14.4.9 Refresh Token Rotation
- 14.4.10 Token撤销
- 14.4.11 注销处理
- 14.4.12 多设备Token管理

## 14.5 Cookie安全
- 14.5.1 HttpOnly
- 14.5.2 Secure
- 14.5.3 SameSite
- 14.5.4 Domain
- 14.5.5 Path
- 14.5.6 Max-Age与Expires
- 14.5.7 Cookie认证常见错误

## 14.6 OAuth 2.0与OpenID Connect
- 14.6.1 OAuth 2.0解决的问题
- 14.6.2 Authorization Code Flow
- 14.6.3 Access Token
- 14.6.4 Scope
- 14.6.5 OpenID Connect
- 14.6.6 ID Token
- 14.6.7 第三方登录
- 14.6.8 OAuth安全基础

## 14.7 权限控制
- 14.7.1 RBAC
- 14.7.2 Role
- 14.7.3 Permission
- 14.7.4 用户与角色关系
- 14.7.5 角色与权限关系
- 14.7.6 路由权限检查
- 14.7.7 资源所有权检查
- 14.7.8 前端权限展示
- 14.7.9 后端权限强制执行
- 14.7.10 ABAC基础

## 14.8 常见Web安全问题
- 14.8.1 XSS
- 14.8.2 Stored XSS
- 14.8.3 Reflected XSS
- 14.8.4 DOM-Based XSS
- 14.8.5 CSRF
- 14.8.6 SQL Injection
- 14.8.7 NoSQL Injection基础
- 14.8.8 Command Injection基础
- 14.8.9 Path Traversal
- 14.8.10 Open Redirect
- 14.8.11 SSRF基础

## 14.9 应用安全加固
- 14.9.1 Helmet
- 14.9.2 Content Security Policy
- 14.9.3 CORS安全配置
- 14.9.4 Rate Limit
- 14.9.5 登录失败限流
- 14.9.6 Brute Force防护
- 14.9.7 请求体大小限制
- 14.9.8 输入验证
- 14.9.9 输出编码
- 14.9.10 密钥与Secrets管理
- 14.9.11 依赖安全审计
- 14.9.12 安全日志

# 第十五部分：后端工程能力与API设计

## 15.1 分层架构
- 15.1.1 路由层职责
- 15.1.2 Controller层职责
- 15.1.3 Service层职责
- 15.1.4 Repository层职责
- 15.1.5 Model层职责
- 15.1.6 Dependency Direction
- 15.1.7 业务逻辑与HTTP解耦
- 15.1.8 可测试性设计

## 15.2 请求校验
- 15.2.1 为什么需要服务端校验
- 15.2.2 Zod Schema
- 15.2.3 Body校验
- 15.2.4 Params校验
- 15.2.5 Query校验
- 15.2.6 环境变量校验
- 15.2.7 校验错误格式化
- 15.2.8 类型推断

## 15.3 API设计规范
- 15.3.1 资源命名
- 15.3.2 URL设计
- 15.3.3 HTTP Method选择
- 15.3.4 Status Code选择
- 15.3.5 统一响应格式
- 15.3.6 统一错误格式
- 15.3.7 分页
- 15.3.8 过滤
- 15.3.9 排序
- 15.3.10 搜索
- 15.3.11 API版本管理
- 15.3.12 Idempotency Key

## 15.4 API文档
- 15.4.1 OpenAPI
- 15.4.2 Swagger UI
- 15.4.3 Request Schema
- 15.4.4 Response Schema
- 15.4.5 Error Schema
- 15.4.6 Authentication文档
- 15.4.7 API示例
- 15.4.8 文档与代码同步

## 15.5 文件上传
- 15.5.1 multipart/form-data
- 15.5.2 multer
- 15.5.3 文件类型校验
- 15.5.4 文件大小限制
- 15.5.5 文件名安全
- 15.5.6 本地存储
- 15.5.7 S3对象存储
- 15.5.8 Presigned URL
- 15.5.9 图片处理基础
- 15.5.10 文件删除与清理

## 15.6 Webhook
- 15.6.1 Webhook解决的问题
- 15.6.2 Webhook Endpoint
- 15.6.3 签名验证
- 15.6.4 Raw Body
- 15.6.5 Timestamp验证
- 15.6.6 Replay Attack防护
- 15.6.7 幂等性
- 15.6.8 重复事件处理
- 15.6.9 重试机制
- 15.6.10 Webhook日志

## 15.7 日志系统
- 15.7.1 日志的作用
- 15.7.2 Log Level
- 15.7.3 Structured Logging
- 15.7.4 pino
- 15.7.5 HTTP访问日志
- 15.7.6 错误日志
- 15.7.7 Request ID
- 15.7.8 Correlation ID
- 15.7.9 敏感信息脱敏
- 15.7.10 日志查询基础

## 15.8 后端测试
- 15.8.1 单元测试
- 15.8.2 集成测试
- 15.8.3 API测试
- 15.8.4 Vitest
- 15.8.5 Supertest
- 15.8.6 Service层测试
- 15.8.7 Controller层测试
- 15.8.8 数据库测试
- 15.8.9 Mock与Stub
- 15.8.10 Test Fixture
- 15.8.11 测试隔离
- 15.8.12 覆盖率认知

# 第十六部分：Redis、缓存与后台任务

## 16.1 Redis基础
- 16.1.1 Redis解决的问题
- 16.1.2 Key-Value模型
- 16.1.3 String
- 16.1.4 Hash
- 16.1.5 List
- 16.1.6 Set
- 16.1.7 Sorted Set
- 16.1.8 TTL
- 16.1.9 Redis持久化基础
- 16.1.10 Redis连接管理

## 16.2 缓存
- 16.2.1 缓存适用场景
- 16.2.2 Cache-Aside
- 16.2.3 Cache Key设计
- 16.2.4 TTL设计
- 16.2.5 缓存失效
- 16.2.6 缓存穿透
- 16.2.7 缓存击穿
- 16.2.8 缓存雪崩
- 16.2.9 数据一致性
- 16.2.10 缓存监控基础

## 16.3 Redis应用场景
- 16.3.1 Session Store
- 16.3.2 Rate Limit
- 16.3.3 验证码
- 16.3.4 临时Token
- 16.3.5 分布式锁基础
- 16.3.6 排行榜基础

## 16.4 后台任务
- 16.4.1 同步任务与异步任务
- 16.4.2 Queue
- 16.4.3 Job
- 16.4.4 Worker
- 16.4.5 BullMQ
- 16.4.6 Job Payload
- 16.4.7 Job Status
- 16.4.8 Job Retry
- 16.4.9 Exponential Backoff
- 16.4.10 Dead-Letter思想
- 16.4.11 Job Idempotency
- 16.4.12 并发控制

## 16.5 定时任务与通知
- 16.5.1 Cron表达式
- 16.5.2 定时任务
- 16.5.3 邮件发送任务
- 16.5.4 报表生成任务
- 16.5.5 Webhook重试任务
- 16.5.6 任务失败告警
- 16.5.7 定时任务重复执行问题

# 第十七部分：第三方服务与支付集成

## 17.1 第三方API集成
- 17.1.1 API Key
- 17.1.2 Bearer Token
- 17.1.3 OAuth Token
- 17.1.4 请求超时
- 17.1.5 Retry
- 17.1.6 Exponential Backoff
- 17.1.7 Rate Limit
- 17.1.8 Circuit Breaker基础
- 17.1.9 第三方错误映射
- 17.1.10 第三方API Mock

## 17.2 邮件服务
- 17.2.1 Transactional Email
- 17.2.2 邮件服务提供商
- 17.2.3 邮件模板
- 17.2.4 邮箱验证邮件
- 17.2.5 密码重置邮件
- 17.2.6 订单通知邮件
- 17.2.7 邮件发送队列
- 17.2.8 邮件发送状态

## 17.3 Stripe支付基础
- 17.3.1 Payment Intent
- 17.3.2 Checkout Session
- 17.3.3 客户端与服务端职责
- 17.3.4 支付状态
- 17.3.5 支付成功页面
- 17.3.6 Stripe Webhook
- 17.3.7 Webhook签名验证
- 17.3.8 支付幂等性
- 17.3.9 退款基础
- 17.3.10 支付安全边界

## 17.4 Shopify集成
- 17.4.1 Shopify OAuth安装流程
- 17.4.2 Admin GraphQL API
- 17.4.3 Product同步
- 17.4.4 Order同步
- 17.4.5 Inventory同步
- 17.4.6 Shopify Webhook
- 17.4.7 HMAC签名验证
- 17.4.8 API Rate Limit
- 17.4.9 Background Sync
- 17.4.10 数据一致性与幂等性

# 第十八部分：Docker、Linux与部署

## 18.1 Linux基础
- 18.1.1 Linux文件系统
- 18.1.2 常用目录
- 18.1.3 ls / cd / pwd
- 18.1.4 cp / mv / rm
- 18.1.5 mkdir / touch
- 18.1.6 cat / less / tail
- 18.1.7 grep
- 18.1.8 chmod
- 18.1.9 环境变量
- 18.1.10 进程与端口
- 18.1.11 SSH

## 18.2 Docker基础
- 18.2.1 Image
- 18.2.2 Container
- 18.2.3 Volume
- 18.2.4 Network
- 18.2.5 Dockerfile
- 18.2.6 Build
- 18.2.7 Run
- 18.2.8 Port Mapping
- 18.2.9 Environment Variable
- 18.2.10 Multi-Stage Build
- 18.2.11 .dockerignore
- 18.2.12 Docker安全基础

## 18.3 Docker Compose
- 18.3.1 Compose文件
- 18.3.2 Application Service
- 18.3.3 PostgreSQL Service
- 18.3.4 Redis Service
- 18.3.5 Volume配置
- 18.3.6 Network配置
- 18.3.7 Health Check
- 18.3.8 开发环境编排
- 18.3.9 生产环境注意事项

## 18.4 Nginx与进程管理
- 18.4.1 Reverse Proxy
- 18.4.2 Nginx基础配置
- 18.4.3 静态资源服务
- 18.4.4 HTTPS配置
- 18.4.5 Gzip基础
- 18.4.6 PM2
- 18.4.7 Process Restart
- 18.4.8 Zero-Downtime Reload基础

## 18.5 云平台基础
- 18.5.1 云计算基础概念
- 18.5.2 Region与Availability Zone
- 18.5.3 IAM基础
- 18.5.4 Object Storage
- 18.5.5 Managed Database
- 18.5.6 Compute Service
- 18.5.7 Secrets Management
- 18.5.8 Cloud Logging
- 18.5.9 环境隔离
- 18.5.10 成本意识

## 18.6 AWS基础
- 18.6.1 IAM
- 18.6.2 S3
- 18.6.3 RDS
- 18.6.4 EC2
- 18.6.5 Lambda基础
- 18.6.6 API Gateway基础
- 18.6.7 CloudWatch
- 18.6.8 Secrets Manager
- 18.6.9 Security Group
- 18.6.10 AWS部署方案选型

## 18.7 CI/CD
- 18.7.1 Continuous Integration
- 18.7.2 Continuous Delivery
- 18.7.3 GitHub Actions
- 18.7.4 Workflow
- 18.7.5 Job与Step
- 18.7.6 自动安装依赖
- 18.7.7 自动Lint
- 18.7.8 自动测试
- 18.7.9 自动Build
- 18.7.10 自动部署
- 18.7.11 Secrets配置
- 18.7.12 Rollback策略

# 第十九部分：可观测性与生产运维

## 19.1 可观测性基础
- 19.1.1 Logging
- 19.1.2 Metrics
- 19.1.3 Tracing
- 19.1.4 可观测性与监控的区别
- 19.1.5 生产问题排查流程

## 19.2 应用监控
- 19.2.1 Health Check
- 19.2.2 Liveness
- 19.2.3 Readiness
- 19.2.4 Uptime
- 19.2.5 Latency
- 19.2.6 Throughput
- 19.2.7 Error Rate
- 19.2.8 Resource Usage

## 19.3 错误追踪
- 19.3.1 Sentry
- 19.3.2 前端错误监控
- 19.3.3 后端错误监控
- 19.3.4 Source Map上传
- 19.3.5 Release Tracking
- 19.3.6 User Context
- 19.3.7 敏感数据保护
- 19.3.8 错误聚合与告警

## 19.4 日志与追踪
- 19.4.1 集中式日志
- 19.4.2 Request ID
- 19.4.3 Correlation ID
- 19.4.4 跨服务请求追踪
- 19.4.5 慢请求分析
- 19.4.6 数据库查询日志
- 19.4.7 第三方请求日志
- 19.4.8 Background Job日志

## 19.5 生产运维基础
- 19.5.1 Incident
- 19.5.2 Severity
- 19.5.3 Alert
- 19.5.4 On-Call基础
- 19.5.5 Rollback
- 19.5.6 Hotfix
- 19.5.7 Postmortem
- 19.5.8 Root Cause Analysis
- 19.5.9 容量与扩展基础

# 第二十部分：系统设计基础

## 20.1 系统设计方法
- 20.1.1 需求澄清
- 20.1.2 Functional Requirements
- 20.1.3 Non-Functional Requirements
- 20.1.4 数据模型设计
- 20.1.5 API设计
- 20.1.6 组件拆分
- 20.1.7 数据流设计
- 20.1.8 性能与扩展性
- 20.1.9 安全与可靠性
- 20.1.10 Trade-Off表达

## 20.2 常见系统设计能力
- 20.2.1 登录系统设计
- 20.2.2 权限系统设计
- 20.2.3 文件上传系统设计
- 20.2.4 通知系统设计
- 20.2.5 支付系统设计
- 20.2.6 Webhook系统设计
- 20.2.7 缓存系统设计
- 20.2.8 后台任务系统设计
- 20.2.9 电商订单系统设计
- 20.2.10 库存系统设计

## 20.3 扩展性与可靠性
- 20.3.1 Vertical Scaling
- 20.3.2 Horizontal Scaling
- 20.3.3 Load Balancer
- 20.3.4 Stateless Service
- 20.3.5 Database Bottleneck
- 20.3.6 Cache
- 20.3.7 Queue
- 20.3.8 Rate Limit
- 20.3.9 Timeout
- 20.3.10 Retry
- 20.3.11 Circuit Breaker
- 20.3.12 Graceful Degradation

## 20.4 数据一致性
- 20.4.1 Strong Consistency
- 20.4.2 Eventual Consistency
- 20.4.3 Transaction Boundary
- 20.4.4 Distributed Transaction基础
- 20.4.5 Idempotency
- 20.4.6 Duplicate Event
- 20.4.7 Outbox Pattern基础
- 20.4.8 Saga Pattern基础

# 第二十一部分：完整全栈项目（从零构建到生产部署）

## 21.1 项目定位与技术选型
- 21.1.1 项目目标
- 21.1.2 项目业务范围
- 21.1.3 用户角色
- 21.1.4 核心功能
- 21.1.5 非功能需求
- 21.1.6 技术栈选型
- 21.1.7 Monorepo结构
- 21.1.8 Git协作流程
- 21.1.9 Definition of Done
- 21.1.10 项目里程碑

## 21.2 需求分析
- 21.2.1 用户注册与登录
- 21.2.2 用户资料
- 21.2.3 商品管理
- 21.2.4 商品分类
- 21.2.5 商品图片
- 21.2.6 库存管理
- 21.2.7 购物车
- 21.2.8 订单管理
- 21.2.9 支付流程
- 21.2.10 权限管理
- 21.2.11 通知系统
- 21.2.12 Shopify数据同步
- 21.2.13 审计日志
- 21.2.14 管理后台

## 21.3 系统架构设计
- 21.3.1 系统上下文图
- 21.3.2 前端架构
- 21.3.3 后端架构
- 21.3.4 数据库架构
- 21.3.5 Redis架构
- 21.3.6 Background Worker
- 21.3.7 文件存储
- 21.3.8 支付服务
- 21.3.9 邮件服务
- 21.3.10 Shopify集成
- 21.3.11 部署架构
- 21.3.12 安全边界

## 21.4 项目初始化
- 21.4.1 创建Git仓库
- 21.4.2 创建Monorepo
- 21.4.3 初始化前端项目
- 21.4.4 初始化后端项目
- 21.4.5 配置TypeScript
- 21.4.6 配置ESLint
- 21.4.7 配置Prettier
- 21.4.8 配置Husky
- 21.4.9 配置环境变量
- 21.4.10 配置Docker Compose
- 21.4.11 配置PostgreSQL
- 21.4.12 配置Redis

## 21.5 数据库设计
- 21.5.1 User模型
- 21.5.2 Role模型
- 21.5.3 Permission模型
- 21.5.4 Product模型
- 21.5.5 Category模型
- 21.5.6 ProductImage模型
- 21.5.7 Inventory模型
- 21.5.8 Cart模型
- 21.5.9 CartItem模型
- 21.5.10 Order模型
- 21.5.11 OrderItem模型
- 21.5.12 Payment模型
- 21.5.13 RefreshToken或Session模型
- 21.5.14 WebhookEvent模型
- 21.5.15 AuditLog模型
- 21.5.16 索引设计
- 21.5.17 ER图
- 21.5.18 Prisma Schema
- 21.5.19 Migration
- 21.5.20 Seed数据

## 21.6 后端基础架构
- 21.6.1 Express应用启动
- 21.6.2 配置管理
- 21.6.3 Prisma Client
- 21.6.4 Redis Client
- 21.6.5 Router层
- 21.6.6 Controller层
- 21.6.7 Service层
- 21.6.8 Repository层
- 21.6.9 Zod校验
- 21.6.10 统一响应格式
- 21.6.11 自定义错误类
- 21.6.12 全局错误处理
- 21.6.13 Structured Logging
- 21.6.14 Request ID
- 21.6.15 Health Check
- 21.6.16 Graceful Shutdown

## 21.7 完整认证系统
- 21.7.1 用户注册
- 21.7.2 密码Hash
- 21.7.3 用户登录
- 21.7.4 Access Token生成
- 21.7.5 Refresh Token生成
- 21.7.6 Token Cookie设置
- 21.7.7 身份认证中间件
- 21.7.8 Token刷新
- 21.7.9 Refresh Token Rotation
- 21.7.10 用户注销
- 21.7.11 所有设备注销
- 21.7.12 邮箱验证
- 21.7.13 忘记密码
- 21.7.14 重置密码
- 21.7.15 登录失败限流
- 21.7.16 Session与Token清理任务
- 21.7.17 认证接口测试

## 21.8 权限系统
- 21.8.1 RBAC数据模型
- 21.8.2 角色初始化
- 21.8.3 权限初始化
- 21.8.4 权限检查中间件
- 21.8.5 资源所有权检查
- 21.8.6 管理员权限
- 21.8.7 普通用户权限
- 21.8.8 前端权限控制
- 21.8.9 权限接口测试

## 21.9 商品与分类模块
- 21.9.1 创建商品
- 21.9.2 查询商品列表
- 21.9.3 查询商品详情
- 21.9.4 更新商品
- 21.9.5 删除商品
- 21.9.6 创建分类
- 21.9.7 更新分类
- 21.9.8 删除分类
- 21.9.9 商品与分类关系
- 21.9.10 分页
- 21.9.11 搜索
- 21.9.12 过滤
- 21.9.13 排序
- 21.9.14 缓存商品详情
- 21.9.15 缓存失效
- 21.9.16 商品接口测试

## 21.10 文件与图片模块
- 21.10.1 文件上传接口
- 21.10.2 文件类型校验
- 21.10.3 文件大小校验
- 21.10.4 S3上传
- 21.10.5 Presigned URL
- 21.10.6 商品图片关联
- 21.10.7 图片删除
- 21.10.8 孤立文件清理
- 21.10.9 文件上传测试

## 21.11 库存模块
- 21.11.1 库存数据模型
- 21.11.2 增加库存
- 21.11.3 减少库存
- 21.11.4 库存查询
- 21.11.5 库存变更日志
- 21.11.6 乐观锁
- 21.11.7 超卖问题
- 21.11.8 库存接口测试

## 21.12 购物车模块
- 21.12.1 创建购物车
- 21.12.2 添加商品
- 21.12.3 修改商品数量
- 21.12.4 删除购物车商品
- 21.12.5 查询购物车
- 21.12.6 价格重新计算
- 21.12.7 库存校验
- 21.12.8 购物车接口测试

## 21.13 订单模块
- 21.13.1 创建订单
- 21.13.2 订单号生成
- 21.13.3 订单快照
- 21.13.4 订单金额计算
- 21.13.5 事务扣减库存
- 21.13.6 查询订单列表
- 21.13.7 查询订单详情
- 21.13.8 更新订单状态
- 21.13.9 取消订单
- 21.13.10 订单幂等性
- 21.13.11 订单接口测试

## 21.14 支付模块
- 21.14.1 创建Stripe Checkout Session
- 21.14.2 保存支付记录
- 21.14.3 支付成功返回
- 21.14.4 支付失败处理
- 21.14.5 Stripe Webhook
- 21.14.6 Webhook签名验证
- 21.14.7 支付事件幂等处理
- 21.14.8 更新订单支付状态
- 21.14.9 退款基础
- 21.14.10 支付模块测试

## 21.15 后台任务与通知
- 21.15.1 BullMQ配置
- 21.15.2 Worker配置
- 21.15.3 邮箱验证任务
- 21.15.4 密码重置邮件任务
- 21.15.5 订单确认邮件任务
- 21.15.6 支付结果通知任务
- 21.15.7 Webhook重试任务
- 21.15.8 失败重试
- 21.15.9 指数退避
- 21.15.10 任务幂等性
- 21.15.11 失败任务监控

## 21.16 Shopify集成
- 21.16.1 Shopify OAuth
- 21.16.2 店铺安装记录
- 21.16.3 Access Token安全存储
- 21.16.4 Product同步
- 21.16.5 Order同步
- 21.16.6 Inventory同步
- 21.16.7 Shopify Webhook
- 21.16.8 HMAC验证
- 21.16.9 Webhook幂等性
- 21.16.10 Rate Limit处理
- 21.16.11 Background Sync
- 21.16.12 同步状态与错误记录

## 21.17 前端基础架构
- 21.17.1 Next.js项目初始化
- 21.17.2 项目目录结构
- 21.17.3 全局Layout
- 21.17.4 UI基础样式
- 21.17.5 Tailwind配置
- 21.17.6 API Client
- 21.17.7 TanStack Query配置
- 21.17.8 全局错误处理
- 21.17.9 Loading状态
- 21.17.10 Toast通知
- 21.17.11 表单基础组件
- 21.17.12 可访问性基础

## 21.18 前端认证与权限
- 21.18.1 注册页面
- 21.18.2 登录页面
- 21.18.3 邮箱验证页面
- 21.18.4 忘记密码页面
- 21.18.5 重置密码页面
- 21.18.6 当前用户状态
- 21.18.7 自动刷新Token
- 21.18.8 注销
- 21.18.9 Middleware路由保护
- 21.18.10 权限菜单
- 21.18.11 无权限页面
- 21.18.12 认证端到端测试

## 21.19 商品与后台管理界面
- 21.19.1 商品列表页面
- 21.19.2 商品详情页面
- 21.19.3 商品搜索
- 21.19.4 商品过滤
- 21.19.5 商品排序
- 21.19.6 商品分页
- 21.19.7 创建商品表单
- 21.19.8 编辑商品表单
- 21.19.9 商品图片上传
- 21.19.10 商品删除确认
- 21.19.11 分类管理页面
- 21.19.12 库存管理页面
- 21.19.13 乐观更新
- 21.19.14 商品界面测试

## 21.20 购物车、订单与支付界面
- 21.20.1 购物车页面
- 21.20.2 商品数量修改
- 21.20.3 结账页面
- 21.20.4 创建订单
- 21.20.5 Stripe支付跳转
- 21.20.6 支付成功页面
- 21.20.7 支付失败页面
- 21.20.8 用户订单列表
- 21.20.9 用户订单详情
- 21.20.10 管理员订单页面
- 21.20.11 订单状态更新
- 21.20.12 订单端到端测试

## 21.21 安全加固
- 21.21.1 Helmet配置
- 21.21.2 CSP配置
- 21.21.3 CORS配置
- 21.21.4 Cookie安全配置
- 21.21.5 Rate Limit
- 21.21.6 请求体限制
- 21.21.7 输入校验
- 21.21.8 输出保护
- 21.21.9 敏感日志脱敏
- 21.21.10 依赖安全审计
- 21.21.11 权限绕过测试
- 21.21.12 常见攻击场景测试

## 21.22 测试体系
- 21.22.1 测试策略
- 21.22.2 后端单元测试
- 21.22.3 后端集成测试
- 21.22.4 API测试
- 21.22.5 前端组件测试
- 21.22.6 前端交互测试
- 21.22.7 端到端测试
- 21.22.8 测试数据库
- 21.22.9 测试Seed
- 21.22.10 Mock第三方服务
- 21.22.11 测试覆盖率
- 21.22.12 CI自动测试

## 21.23 性能优化
- 21.23.1 数据库索引分析
- 21.23.2 EXPLAIN ANALYZE
- 21.23.3 N+1检查
- 21.23.4 Redis缓存
- 21.23.5 API响应时间
- 21.23.6 前端Bundle分析
- 21.23.7 图片优化
- 21.23.8 路由懒加载
- 21.23.9 React渲染优化
- 21.23.10 Core Web Vitals
- 21.23.11 Lighthouse审计
- 21.23.12 性能优化记录

## 21.24 Docker与部署
- 21.24.1 前端Dockerfile
- 21.24.2 后端Dockerfile
- 21.24.3 Worker Dockerfile
- 21.24.4 Multi-Stage Build
- 21.24.5 Docker Compose生产配置
- 21.24.6 PostgreSQL生产配置
- 21.24.7 Redis生产配置
- 21.24.8 S3配置
- 21.24.9 Secrets配置
- 21.24.10 域名与HTTPS
- 21.24.11 数据库Migration部署
- 21.24.12 首次生产部署
- 21.24.13 Rollback演练

## 21.25 CI/CD
- 21.25.1 Pull Request检查
- 21.25.2 Lint Workflow
- 21.25.3 Test Workflow
- 21.25.4 Build Workflow
- 21.25.5 Docker Image Build
- 21.25.6 自动部署
- 21.25.7 Environment Secrets
- 21.25.8 Migration Step
- 21.25.9 Deployment Verification
- 21.25.10 Rollback Workflow

## 21.26 监控与可观测性
- 21.26.1 Sentry前端接入
- 21.26.2 Sentry后端接入
- 21.26.3 Structured Logging
- 21.26.4 Request ID
- 21.26.5 Health Check
- 21.26.6 Readiness Check
- 21.26.7 Uptime监控
- 21.26.8 错误率监控
- 21.26.9 延迟监控
- 21.26.10 Background Job监控
- 21.26.11 告警配置
- 21.26.12 生产故障演练

## 21.27 项目文档
- 21.27.1 README
- 21.27.2 本地开发文档
- 21.27.3 环境变量文档
- 21.27.4 API文档
- 21.27.5 数据库ER图
- 21.27.6 系统架构图
- 21.27.7 部署文档
- 21.27.8 测试文档
- 21.27.9 Security说明
- 21.27.10 Architecture Decision Record
- 21.27.11 已知限制
- 21.27.12 后续改进计划

## 21.28 项目复盘
- 21.28.1 需求完成情况
- 21.28.2 架构设计复盘
- 21.28.3 数据库设计复盘
- 21.28.4 安全设计复盘
- 21.28.5 测试体系复盘
- 21.28.6 性能优化复盘
- 21.28.7 部署流程复盘
- 21.28.8 生产问题复盘
- 21.28.9 技术债务
- 21.28.10 项目演示
- 21.28.11 简历项目描述
- 21.28.12 面试项目讲解

# 第二十二部分：面试与求职准备

## 22.1 JavaScript面试
- 22.1.1 数据类型与内存
- 22.1.2 作用域与闭包
- 22.1.3 this
- 22.1.4 原型与继承
- 22.1.5 Promise
- 22.1.6 Event Loop
- 22.1.7 常见代码题
- 22.1.8 调试题

## 22.2 TypeScript面试
- 22.2.1 Interface与Type
- 22.2.2 Union与Intersection
- 22.2.3 Generic
- 22.2.4 Utility Types
- 22.2.5 Type Guard
- 22.2.6 Conditional Types
- 22.2.7 工程配置
- 22.2.8 类型设计题

## 22.3 React与Next.js面试
- 22.3.1 React渲染机制
- 22.3.2 Hooks
- 22.3.3 State管理
- 22.3.4 性能优化
- 22.3.5 Server Component
- 22.3.6 Next.js缓存
- 22.3.7 SSR与CSR
- 22.3.8 前端系统设计基础

## 22.4 Node.js与后端面试
- 22.4.1 Node.js Event Loop
- 22.4.2 Express中间件
- 22.4.3 错误处理
- 22.4.4 分层架构
- 22.4.5 REST API设计
- 22.4.6 身份认证
- 22.4.7 权限控制
- 22.4.8 Redis与后台任务

## 22.5 数据库面试
- 22.5.1 SQL查询
- 22.5.2 JOIN
- 22.5.3 索引
- 22.5.4 事务
- 22.5.5 锁
- 22.5.6 数据建模
- 22.5.7 查询优化
- 22.5.8 ORM问题

## 22.6 系统设计面试
- 22.6.1 需求澄清
- 22.6.2 API设计
- 22.6.3 数据库设计
- 22.6.4 缓存
- 22.6.5 Queue
- 22.6.6 文件存储
- 22.6.7 支付系统
- 22.6.8 电商订单系统
- 22.6.9 Trade-Off表达

## 22.7 项目表达
- 22.7.1 项目背景
- 22.7.2 个人职责
- 22.7.3 技术选型
- 22.7.4 核心架构
- 22.7.5 技术难点
- 22.7.6 Bug与故障
- 22.7.7 性能优化
- 22.7.8 安全设计
- 22.7.9 测试与部署
- 22.7.10 项目成果

## 22.8 简历与作品集
- 22.8.1 Full Stack简历结构
- 22.8.2 Shopify经验与全栈能力结合
- 22.8.3 项目描述
- 22.8.4 技术成果量化
- 22.8.5 GitHub仓库整理
- 22.8.6 README优化
- 22.8.7 项目演示地址
- 22.8.8 LinkedIn资料
- 22.8.9 求职申请跟踪
- 22.8.10 模拟面试
