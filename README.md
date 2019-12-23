# Reviewed-material-
拼多多【电话一面】

如何在 React 项目中使用 Echarts，在哪个生命周期实例化图表（componentDidMount），什么场景下使用了 Echarts 的高级特性
项目 i18n 的方案，在可视化图表中如何引入 i18n
React Hooks 解决了什么问题，如何用 Hooks 的方法去模拟 Class Components 的功能
Function Component 多次执行，useRef() 会不会每次都执行生成新对象
React16 对比 15 有什么更新（Fiber 历史背景和原理）
什么是受控组件和非受控组件
React项目的技术栈是怎样的？讲一下 redux-saga 的概念、API 和用法
Redux 的三大特点

单一数据源、State 是只读的、使用纯函数来修改状态


项目中是否使用了 TypeScript，TS 中的枚举是怎样写的，如果用原生 JS 怎样实现
webpack 配置可以怎样优化，有哪些策略，如果项目要使用 TS 在 webpack 中需要配置什么
项目使用了 ES6 吗，是如何使用 ES6 的（Babel 使用 @babel/preset-env）
举例子 window 对象下的一些属性
讲一下对闭包的理解
如何用原生 JS 实现 Promise 的 polyfill，需要注意哪些点
HTML 的字符实体是什么，都有哪些（❌一开始没反应过来字符实体是什么）
前端模块化是为了解决什么问题，简单介绍目前有哪些模块化规范，CommonJS 和 ES6 的区别
常见的前端涉及到的安全问题，以及如何防范
是否用 LESS/SASS，LESS 中如何写函数
编程题：有一个长度为 32 的数组，如何将它转换为长度为4*8的二维数组


拼多多【视频三面】

React 和 Vue 的分别的优点，你觉得现在这些 MV* 框架以后会往哪个方向/趋势发展
有没有做过项目的性能优化，从业务和工具链两个方面讲
最近遇到的技术难题
有没有参加过开源社区给开源项目贡献代码；介绍一下自己业余时间做的开发工作
在团队内是否有维护公共组件或工具，你觉得维护公共逻辑跟个人开发上有什么区别，如何去协调不同开发者的需求
团队的组成情况，在团队协作上遇见什么困难，是如何解决的；
将来的职业规划是怎样的，带领团队/下属最重要的是什么
最近读了什么书有什么感想，有没有写技术文章



字节跳动【视频一面】

WebGL 了解到什么程度，都有哪些基本功能；项目中是如何使用 WebGL 的
讲一下 GLSL Shader 实现亮度(Brightness)、对比度(Contrast) 和边缘检测(Edge Detection) 是如何实现的

回答的时候忘记了对比度的算法实现没答上来，讲了下明度 Luminance 的调节；亮度Brightness是RGB+亮度系数；边缘检测和图像锐化是使用 Convolution Kernel 卷积核加深中心像素与周围像素的色彩差值梯度，使边缘更加突出


亮度、对比度与原像素的 RGB 通道分别是什么关系

这题其实我没理解题意，其实现在想想应该答案是 亮度是在原RGB上直接添加亮度系数(color+brightness)，而对比度是 在原色彩与中间值的差 上与对比度系数相乘 (color-0.5)*contrast+0.5


是否有进行过 node 开发；简单介绍一下你开发的这一个 webpack 插件的功能和原理
Vue 响应式原理；响应式原理中的 Deps 数组订阅发布中心是在什么时机去收集依赖的？
介绍这三个步骤的流程 Vue Template -> VDOM -> 真实 DOM；
Vue Template 生成的 render 函数里面都有什么内容（主要要提到 createElement 函数的递归调用）
编程题：Promise 调度相关，JS 实现一个带并发限制的异步调度器 Scheduler，保证同时运行的任务最多有两个

字节跳动【视频一面】

WebGL 了解到什么程度，都有哪些基本功能；项目中是如何使用 WebGL 的
讲一下 GLSL Shader 实现亮度(Brightness)、对比度(Contrast) 和边缘检测(Edge Detection) 是如何实现的

回答的时候忘记了对比度的算法实现没答上来，讲了下明度 Luminance 的调节；亮度Brightness是RGB+亮度系数；边缘检测和图像锐化是使用 Convolution Kernel 卷积核加深中心像素与周围像素的色彩差值梯度，使边缘更加突出


亮度、对比度与原像素的 RGB 通道分别是什么关系

这题其实我没理解题意，其实现在想想应该答案是 亮度是在原RGB上直接添加亮度系数(color+brightness)，而对比度是 在原色彩与中间值的差 上与对比度系数相乘 (color-0.5)*contrast+0.5


是否有进行过 node 开发；简单介绍一下你开发的这一个 webpack 插件的功能和原理
Vue 响应式原理；响应式原理中的 Deps 数组订阅发布中心是在什么时机去收集依赖的？
介绍这三个步骤的流程 Vue Template -> VDOM -> 真实 DOM；
Vue Template 生成的 render 函数里面都有什么内容（主要要提到 createElement 函数的递归调用）
编程题：Promise 调度相关，JS 实现一个带并发限制的异步调度器 Scheduler，保证同时运行的任务最多有两个

字节跳动【视频二面】

如何预防/减少 Node.js 程序的崩溃，有没有实际操作的案例
如何判断一个点在正多边形内部
Web Worker 的局限性；如何使用动态的 JS 代码生成动态的 Web Worker 实例（ArrayBuffer + URL.createObjectURL）
iframe 中脚本的执行是否会阻塞主页面的渲染线程和 JS 线程，从不同浏览器内核去分析
websocket 和 TCP Socket的区别，websocket 的握手过程，为什么要基于 HTTP 请求来握手
CSS 选择器的权重，使用什么机制来计算的
CSS 后处理器和预处理器分别是什么，有什么区别
什么情况下会发生 Ajax 的跨域请求，浏览器是如何处理 Ajax 跨域的
ES6 箭头函数与 ES5 普通函数的区别
Promise 的 then 方法可以 chaining 调用，它是如何保存这个过程中的值的；then 中回调函数如果返回 Promise/带有 then 属性的对象（then属性值是function 或者非 function 的情况下）/非上述两种 这些情况下，then() 方法是如何处理的
Vue 中为何不使用 Object.defineProperty 去转换数组为响应式数据，对数组是如何处理的

字节跳动【视频三面】

介绍觉得最有挑战的项目，做了什么工作
Vue 虚拟化列表的思路和实现原理
优化树形图表渲染的其他方法
简述思路：在不使用 Promise 或 async/await 等其他 JS 异步控制的情况下，设计一个网络请求 Scheduler 类，确保每个 ajax 请求的回调函数按发起请求的顺序执行
项目开发流程，异地协作流程保证
有没有特别想做的业务方向；以后的工作和技术规划

快手【视频一面】

六道笔试题和几道简单的编程题
手写 bind 和 apply
水平垂直居中的几种方法
扩展 flex:1
请用 React Hooks 实现无状态组件的 componentDidMount、componentDidUpdate 生命周期效果
setState 的第二个参数的作用
useCallback 的使用
React 受控和非受控组件的区别
HTTPS 和 HTTP 的区别
CSRF 如何防御
Promise all/race/finally 的原理
节流和防抖的区别和应用场景
解释 0.3-0.2=0.99999999...
原生 DOM API 相关：创建节点、插入/移除节点、选择节点
element.style 和 getComputedStyle() 的区别
下面代码的输出结果是// counter.js
let counter = 10;
export default counter;
// index.js
import myCounter from "./counter";
myCounter += 1;
console.log(myCounter);
复制代码
请用JavaScript实现一个函数求解整数N，N满足 %2==1，%3==2，%5==4，%6==5，%7==0

快手【视频二面】

输出代码结果：函数提升问题、JS 异步事件循环问题
React Hooks 优点、解决什么问题、useEffect 的调用时机
webpack 优化的方法和配置
webpack 开发插件的原理，简单介绍你的插件
webpack watch 本身的 cache 机制
讲觉得最有挑战的项目，做了什么工作，做了什么优化
如何判断模块的循环引用（DFS 拓扑排序）

快手【现场技术终面】

这轮面试我临时订机票从珠海坐飞机飞北京到快手总部，11月里从24摄氏度到零下一度的落差真的要把我这个广东人冻僵了QAQ 不禁感叹祖国幅员辽阔啊~


项目技术选型，为什么又有 Vue 又有 React
项目的研发管理流程
前端项目自动化发布方式
团队情况，团队沟通中遇到最大的困难，个人在团队中的角色

OPPO-商业化
一面电话沟通，都是前端非常基础的问题，例如闭包、跨域、Vue响应式、HTTP 基础等等；二面现场面、HR电话面
滴滴-两轮车业务
技术面都是电话沟通，HR视频面，后面题目没有记录了

webpack 打包的整个流程，简述 webpack 插件的开发和功能
Commonjs 原理
Koa/Express 中的中间件是什么
如何提高Node.js 程序的稳健性
如何理解 HTTP 协议
RESTful API
HR面：项目异地协作是如何保证流程，对流程推进做了什么工作；从0开始带项目的思路是什么

Promise.reject()😿
平安人寿【电话一面挂】

数据看板开发流程，数据看板是静态数据的还是实时渲染的？

静态数据数据量多大，数据量大的时候是如何优化性能的
可视化看板实时渲染的技术方案


Echarts 除了普通的柱状图折线图，还用过什么高级功能
Canvas 与 SVG 的区别，和它们在 Echarts 中使用的区别

Canvas 适合绘制图形元素数量巨大的场景，如热力图、地理坐标系或平行坐标系上的大规模散点图和线图，SVG 本质上生成了 DOM 节点，会对浏览器渲染造成很大的负担；SVG 的优势是占用的内存更低（对移动端尤其重要），渲染性能略高，并且用户使用浏览器内置的缩放功能时不会模糊；而且因为是生成了 DOM 节点，在开发上直接使用 DOM API 进行用户的交互会更方便



企业微信【视频一面挂】

项目中的权限系统是怎样实现的
Vue 虚拟化列表的实现原理
webpack 优化打包的策略、内部的机制和插件开发的原理
假设现在有一个微信公众号文章的页面，可以展示文章、图片、视频和读者留言，从安全和交互性能的角度去讲一下如何优化

安全：用户输入的时候编辑页面防止 XSS 攻击、敏感字符过滤、外链资源白名单过滤、图片资源脱敏处理转换为本地资源；优化：关键请求路径优化、事件监听节流、非首屏资源懒加载、代码压缩、服务端渲染、利用好缓存策略、开启 HTTP2


HTTP2 相对于 HTTP1.1 有哪些优点，解决了什么问题

首部压缩、数据分帧、多路复用，服务端推送


Webpack 实现热更新的流程（webpack-dev-server 和 HotModuleReplacementPlugin 的实现）
Vue 生成 VDOM 的流程和 Vue 响应式原理
看过哪些项目的源代码，为什么要去看源代码
有没有开发过小程序，是否有 TypeScript 开发经验
介绍一下现在团队的基本情况，在团队内部的贡献（技术分享、维护工具）

欢聚YY【现场面挂】

如何优化网页上需要展示的超大图片，从请求和性能来解释
实现 Adblock 的策略
WebGL 渲染的流程；GLSL Shader 是什么，有什么作用
Shader 实现一个滤光滤镜的思路
WebGL FrameBufferObject 的概念
是否有对动画有了解、FLIP 的概念和应用；Vue Transition 源码底层原理
Vuex 的单向数据流模型；对比直接在 window 下用变量储存数据，使用状态管理库的优点在哪里

微众银行【现场一面 没有下文】

可视化大屏是怎样使用 websocket 中遇到什么问题
如何管理 redux 之间不同模块的数据
讲一下使用 redux-saga 控制数据流的具体需求的实现
一个监听了 input 事件的输入框，每次触发input都会发送请求，这个输入框的优化方案
防抖的作用和手写实现
看了 Vue 代码有哪些自己的心得
vue-router 的原理，history 模式和 hash 模式的区别，为什么 history 模式是先进行 app 内模块的切换再去手动更新路由
介绍一下项目中单元测试的情况，用例有多少，如何运行
编程题：将一个对象中所有值为字符串的提出取出来，拼接成大的字符串
开放题：一共有103位参赛者的1v1赛事，设计一个比赛淘汰机制

未走完的流程👨‍💻‍
有赞-监控平台【视频+电话+在线coding 过】

CSS 选择器有哪些，优先级是怎样的，!important 的表现
display 有哪些值，inline 和 inline-block 的区别
float: left/right 的表现是什么，什么是 BFC，能解决什么问题
websocket 在项目中的用途，握手过程
Babel 的原理、运行过程、如何做 Polyfill
=== 和 == 的区别
JS 基本类型
webpack 优化和配置策略
Service Worker的作用；如何划分缓存策略，对同源/非同源的资源是如何处理缓存的
SSR 的好处，主要解决什么问题
coding: 二叉树的遍历和镜像；实现 EventEmitter

百度-基础架构部 【电话三轮技术面 过】

项目技术选型，不同场景为何使用 Vue/React
HTTPS 原理，CA、数字证书、数字证书的信任链；
对优化业务开发流程做了什么推动工作；项目开发规范：API 规范、仓库和分支规范、需求/开发/提测规范
从输入 URL 到网页渲染，发生了什么事情
coding: 查找根节点到目标节点的路径
