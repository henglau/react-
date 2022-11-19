# React 面试问答

> 如果您喜欢该项目请点击:star:. 极力推荐你拉取仓库. 关注我[@SudheerJonna](https://twitter.com/SudheerJonna)以获取技术更新.

---
<div>
<a href="https://zerotomastery.io/?utm_source=github&utm_medium=sponsor&utm_campaign=reactjs-interview-questions">从零到精通</a>学习编码并获得录用。 
<ol>
<li>如果您正在努力学习 React 超出基础知识，那么这个<a href="https://links.zerotomastery.io/react_sudheer">React 课程</a>很好</li>
<li>如果您认真考虑被聘为开发人员，这个<a href="http://links.zerotomastery.io/mci_sudheer">编码面试训练营</a>会很有帮助。</li>
</ol>
</div>

---

**注意:** 这个项目仓库仅针对ReactJS。 请查看 [Javascript 面试问题](https://github.com/sudheerj/javascript-interview-questions) 以了解核心 javascript 问题。


### 目录 {#table-of-contents}

| 序号 | 问题 |
| --- | --------- |
|   | **React 核心** |
|1  | [什么是React？](#1) |
|2  | [React 的主要特点是什么？](#2) |
|3  | [什么是 JSX？](#3) |
|4  | [Element 和 Component 之间有什么区别？](#4) |
|5  | [如何在 React 中创建 Component？](#5) |
|6  | [什么时候用类组件而不是函数组件？](#6) |
|7  | [什么是纯组件？](#7) |
|8  | [React 中的 state 是什么？](#8) |
|9  | [React 中的 props 是什么？](#9) |
|10 | [state and props 之间有什么区别？](#10) |
|11 | [为什么我们不应该直接更新 state？](#11) |
|12 | [回调函数作为 setState() 的参数的目的是什么？](#12)
|13 | [HTML 和 React 事件处理有什么区别？](#13) |
|14 | [如何在 JSX 回调中绑定方法或事件处理程序？](#14) |
|15 | [如何将参数传递给事件处理程序或回调？](#15) |
|16 | [React 中的合成事件是什么？](#16) |
|17 | [什么是内联条件表达式？](#17) |
|18 | [什么是“key”属性，在元素数组中使用它有什么好处？](#18) |
|19 | [refs有什么用？](#19) |
|20 | [如何创建 refs？](#20)
|21 | [什么是 ref转发？](#21) |
|22 | [在 回调refs 和 findDOMNode() 中，选哪个更佳？](#22) |
|23 | [为什么 字符串引用 被删除？](#23) |
|24 | [什么是 虚拟DOM？](#24) |
|25 | [虚拟 DOM 是如何工作的？](#25) |
|26 | [Shadow DOM 和 Virtual DOM 有什么区别？](#26) |
|27 | [什么是 React Fiber？](#27) |
|28 | [React Fiber 的主要目标是什么？](#28) |
|29 | [什么是受控组件？](#29) |
|30 | [什么是不受控组件？](#30) |
|31 | [createElement 和 cloneElement 有什么区别？](#31) |
|32 | [React 中的状态提升是什么？](#32) |
|33 | [组件生命周期的不同阶段是什么？](#33) |
|34 | [React 的生命周期方法有哪些？](#34) |
|35 | [什么是高阶组件？](#35) |
|36 | [如何为 HOC 组件创建 props 代理？](#36) |
|37 | [什么是 context？](#37) |
|38 | [什么是子属性？](#38) |
|39 | [如何在 React 中写注释？](#39) |
|40 | [使用 super(props) 的目的是什么？](#40) |
|41 | [什么是协调？](#41) |
|42 | [如何使用动态 key 设置 state？](#42) |
|43 | [每次渲染组件时调用函数的常见错误是什么？](#43) |
|44 | [惰性函数是否支持命名导出？](#44) |
|45 | [为什么 React 使用 className 而不是 class 属性？](#45) |
|46 | [什么是 fragments？](#46) |
|47 | [为什么 fragments 比容器 div 更好？](#47) |
|48 | [React 中的Portal是什么？](#48) |
|49 | [什么是无状态组件？](#49) |
|50 | [什么是有状态组件？](#50) |
|51 | [如何在 React 中验证 props？](#51) |
|52 | [React 的优点是什么？](#52) |
|53 | [React 的局限性是什么？](#53) |
|54 | [React v16 中的错误边界是什么？](#54) |
|55 | [React v15 中如何处理错误边界？](#55) |
|56 | [静态类型检查的推荐方法是什么？](#56) |
|57 | [react-dom 包有什么用？](#57) |
|58 | [react-dom的render方法的目的是什么？](#58) |
|59 | [ReactDOMServer 是什么？](#59) |
|60 | [如何在 React 中使用 InnerHtml？](#60) |
|61 | [如何在 React 中使用样式？](#61) |
|62 | [React 中的事件有何不同？](#62) |
|63 | [如果在构造函数中使用 setState() 会发生什么？](#63) |
|64 | [索引作为键有什么影响？](#64) |
|65 | [在 componentWillMount() 方法中使用 setState() 好吗？](#65) |
|66 | [如果你在初始化状态时使用 props 会发生什么？](#66) |
|67 | [如何条件渲染组件？](#67)
|68 | [为什么我们在 DOM 元素上传播 props 时需要小心？](#68) |
|69 | [你如何在 React 中使用装饰器？](#69) |
|70 | [你如何记忆一个组件？](#70) |
|71 | [您如何实现服务器端渲染或 SSR？](#71) |
|72 | [如何在 React 中启用生产模式？](#72) |
|73 | [什么是 CRA 及其好处？](#73) |
|74 | [Mounting 中的生命周期方法顺序是什么？](#74) |
|75 | [React v16 将弃用哪些生命周期方法？](#75) |
|76 | [getDerivedStateFromProps() 生命周期方法的目的是什么？](#76) |
|77 | [getSnapshotBeforeUpdate() 生命周期方法的目的是什么？](#77) |
|78 | [Hooks 会取代 render props 和 高阶组件吗？](#78) |
|79 | [命名组件的推荐用法是什么？](#79) |
|80 | [组件类中方法的推荐顺序是什么？](#80) |
|81 | [什么是开关组件？](#81) |
|82 | [为什么我们需要给 setState() 传递函数？](#82) |
|83 | [React 中的严格模式是什么？](#83) |
|84 | [React Mixins是什么？](#84) |
|85 | [为什么 isMounted() 是反模式，正确的解决方案是什么？](#85) |
|86 | [React 支持哪些指针事件？](#86) |
|87 | [为什么组件名称要以大写字母开头？](#87) |
|88 | [React v16 是否支持自定义 DOM 属性？](#88) |
|89 | [构造函数和getInitialState有什么区别？](#89) |
|90 | [你能在不调用 setState 的情况下强制组件重新渲染吗？](#90) |
|91 | [使用 ES6 类的 React 中的 super() 和 super(props) 有什么区别？](#91) |
|92 | [如何在 JSX 中循环？](#92) |
|93 | [如何在属性引号中访问 props？](#93) |
|94 | [什么是带形状的 React PropType 数组？](#94) |
|95 | [如何有条件地应用 class 属性？](#95) |
|96 | [React 和 ReactDOM 有什么区别？](#96) |
|97 | [为什么 ReactDOM 与 React 分离？](#97) |
|98 | [如何使用 React 标签元素？](#98) |
|99 | [如何组合多个内联样式对象？](#99) |
|100| [调整浏览器大小时如何重新渲染视图？](#100)
|101| [setState 和 replaceState 方法有什么区别？](#101) |
|102| [如何监听 state 变化？](#102) |
|103| [在 react state 中删除数组元素的推荐方法是什么？](#103) |
|104| [是否可以在不渲染 HTML 的情况下使用 React？](#104) |
|105| [如何使用 React 格式化打印 JSON？](#105) |
|106| [为什么你不能在 React 中更新 props？](#106) |
|107| [如何在页面加载时让输入元素获取焦点？](#107) |
|108| [更新 state 中的对象的方式有哪些？](#108) |
|109| [我们如何在浏览器中找到当前运行的 React 版本？](#109) |
|110| [在你的 create-react-app 中包含 polyfill 的方法有哪些？](#101) |
|111| [如何在 create-react-app 中使用 https 而不是 http？](#111) |
|112| [如何避免在 create-react-app 中使用相对路径导入？](#112) |
|113| [如何为 react-router 添加 Google Analytics？](#113) |
|114| [如何每秒更新组件？](#114) |
|115| [如何将供应商前缀应用于 React 中的内联样式？](#115) |
|116| [如何使用 react 和 ES6 导入和导出组件？](#116) |
|117| [React 组件命名有哪些例外？](#117) |
|118| [为什么组件 constructor 函数只调用一次？](#118) |
|119| [如何在 React 中定义常量？](#119) |
|120| [如何以编程方式触发 React 中的点击事件？](#120) |
|121| [是否可以在普通 React 中使用 async/await？](#121) |
|122| [React 的常见文件夹结构是什么？](#122) |
|123| [流行的动画包有哪些？](#123) |
|124| [样式模块化有什么好处？](#124) |
|125| [什么是流行的特定于 React 的 linter？](#125) |
|126| [如何进行 AJAX 调用以及我应该在哪些组件生命周期方法中进行 AJAX 调用？](#126) |
|127| [什么是 render props?](#127) |
|   | **React Router** |
|128| [什么是 React Router?](#128) |
|129| [React Router 与 history 库有何不同？](#129) |
|130| [React Router v4 中的 <Router\> 组件是什么？](#131) |
|131| [history 中的 push 和 replace 方法的作用是什么？](#131) |
|132| [React Router v4 中如何以编程方式导航？](#132) |
|133| [React Router v4 中如何获取 query 参数](#133) |
|134| [为什么会收到 "Router may have only one child element" 警告信息？](#134) |
|135| [React Router v4 中 history.push 方法如何传递参数？](#135) |
|136| [如何实现默认或 NotFound 页面？](#136) |
|137| [React Router v4 中如何获取历史记录？](#137) |
|138| [登录后如何执行自动重定向？](#138) |
|   | **React 国际化** |
|139| [什么是 React-Intl？](#139) |
|140| [React Intl 的主要特点是什么？](#140) |
|141| [React Intl 中的两种格式化方式是什么？](#141) |
|142| [React Intl 中如何使用 FormattedMessage 作为占位符？](#142) |
|143| [React Intl 中如何获取当前语言环境](#143) |
|144| [React Intl 中如何格式化日期？](#144) |
|   | **React 测试** |
|145| [React 测试中的 Shallow Renderer 是什么？](#145) |
|146| [React 中的 TestRenderer 包是什么？](#146) |
|147| [ReactTestUtils 包的作用是什么？](#147) |
|148| [Jest 是什么？](#148) |
|149| [Jest 比 Jasmine 有什么优势？](#149) |
|150| [举一个Jest测试用例的简单例子？](#150) |
|   | **React Redux** |
|151| [Flux 是什么](#151) |
|152| [Redux 是什么？](#152) |
|153| [Redux 的核心原则是什么？](#153) |
|154| [与 Flux 相比，Redux 的缺点是什么？](#154) |
|155| [mapStateToProps() 和 mapDispatchToProps() 有什么区别？](#155) |
|156| [可以在 reducer 中 dispatch 一个 action 吗？](#156) |
|157| [如何访问组件外部的 Redux 存储？](#157) |
|158| [MVW模式有什么缺点？](#158) |
|159| [Redux 和 RxJS 之间有什么相似之处？](#159) |
|160| [如何在加载时 dispatch 一个 action？](#160) |
|161| [如何使用 React Redux 的连接？](#161) |
|162| [如何在 Redux 中重置 state？](#162) |
|163| [redux 连接装饰器中 at 符号的作用是什么？](#163) |
|164| [React context 和 React Redux 有什么区别？](#164) |
|165| [为什么 Redux 操作 state 的函数称为 reducer？](#165) |
|166| [如何在 Redux 中发送 AJAX 请求？](#166) |
|167| [我应该将所有组件的 state 保留在 Redux store中吗？](#167) |
|168| [访问 Redux store 的正确方法是什么？](#168) |
|169| [React Redux 中的组件和容器有什么区别？](#169) |
|170| [Redux 中常量的用途是什么？](#170) |
|171| [编写 mapDispatchToProps() 有哪些不同的方法？](#171) |
|172| [mapStateToProps() 和 mapDispatchToProps() 中的 ownProps 参数有什么用？](#172) |
|173| [如何构建 Redux 顶级目录？](#173) |
|174| [redux-saga 是什么？](#174) |
|175| [redux-saga 的思维模型是什么？](#175) |
|176| [redux-saga 中 call 和 put 有什么区别？](#176) |
|177| [Redux Thunk 是什么？](#177) |
|178| [redux-saga 和 redux-thunk 有什么区别？](#178) |
|179| [Redux DevTools 是什么?](#179) |
|180| [Redux DevTools 有哪些特点？](#180) |
|181| [什么是 Redux 选择器以及为什么要使用它们？](#181) |
|182| [Redux Form 是什么？](#182) |
|183| [Redux Form 的主要特点是什么？](#183) |
|184| [如何向 Redux 添加多个中间件？](#184) |
|185| [如何在 Redux 中设置初始状态？](#185) |
|186| [Relay 与 Redux 有何不同？](#186) |
|187| [Redux 中的 action 是什么？](#187) |
|   | **React Native** |
|188| [React Native 和 React 有什么区别？](#188) |
|189| [如何测试 React Native 应用程序？](#189) |
|190| [如何登录 React Native？](#190) |
|191| [如何调试你的 React Native？](#191) |
|   | **React 支持的库和集成** |
|192| [什么是重新选择以及它是如何工作的？](#192) |
|193| [Flow 是什么?](#193) |
|194| [Flow 和 PropTypes 有什么区别？](#194) |
|195| [如何在 React 中使用 font-awesome 图标？](#195) |
|196| [React Dev Tools 是什么？](#196) |
|197| [为什么在 Chrome 中加载本地文件时  DevTools 没有 加载？](#197) |
|198| [如何在 React 中使用 Polymer？](#198) |
|199| [与 Vue.js 相比，React 有哪些优势？](#199) |
|200| [React 和 Angular 有什么区别？](#200) |
|201| [为什么在 DevTools 中没有出现 React 选项卡？](#201) |
|202| [样式化组件是什么？](#202) |
|203| [举一个样式化组件的例子？](#203) |
|204| [Relay 是什么？](#204) |
|205| [如何在 create-react-app 应用程序中使用 TypeScript？](#205) |
|   | **各种各样的** |
|206| [重新选择库有哪些要点？](#206) |
|207| [举个重新选择库的例子？](#207) |
|208| [React 中，ES6 类的静态属性是否生效？](#208) |
|209| [Redux 只能与 React 一起使用吗？](#209) |
|210| [使用 Redux 时，您是否需要特定的构建工具？](#210) |
|211| [Redux Form initialValues 如何从 state 中更新？](#211) |
|212| [React PropTypes 如何配置一个 prop 可以使用不同的类型？](#212) |
|213| [可以导入 SVG 文件作为 React 组件吗？](#213) |
|214| [为什么不推荐 ref 使用内联回调或函数？](#214)|
|215| [React 中的渲染劫持是什么？](#215)|
|216| [HOC 工厂实现是什么？](#216)|
|217| [如何给 React 组件传递数字？](#217)|
|218| [我需要将我的所有状态都保存到 Redux 中吗？我应该使用 React 内部状态吗？](#218)|
|229| [React 中 registerServiceWorker 的作用是什么？](#219)|
|220| [React 记忆功能是什么？](#220)|
|221| [React 惰性函数是什么？](#221)|
|222| [如何使用 setState 防止不必要的更新？](#222)|
|223| [在 React 16 版本中如何渲染数组、字符串和数字？](#223)|
|224| [React 类中，如何使用类字段声明语法？](#224)|
|225| [什么是 hooks?](#225)|
|226| [hooks 需要遵循哪些规则？](#226)|
|227| [项目中如何确保 hook 遵循规则？](#227)|
|228| [Flux 和 Redux 有什么区别？](#228)|
|229| [React Router V4 有什么优点？](#229)|
|230| [你能描述一下 componentDidCatch 生命周期方法吗？](#230)|
|231| [在哪些情况下错误边界不会捕获错误？](#231)|
|232| [为什么事件处理程序不需要错误边界？](#232)|
|233| [try catch 块和错误边界有什么区别？](#233)|
|234| [react 16 中未捕获的错误的行为是什么？](#234)|
|235| [错误边界在什么位置比较合适？](#235)|
|236| [从错误边界跟踪组件堆栈有什么好处？](#236)|
|237| [类组件必需定义的方法是什么？](#237)|
|238| [渲染方法可以返回哪些类型？](#238)|
|239| [构造函数的主要作用是什么？](#239)|
|240| [React 组件是否必须定义构造函数？](#240)|
|241| [什么是默认 props？](#241)|
|242| [为什么不应该在 componentWillUnmount 中调用 setState？](#242)|
|243| [getDerivedStateFromError 的作用是什么？](#243)|
|244| [组件重新渲染时依次调用了哪些方法？](#244)|
|245| [捕获错误时依次调用了哪些方法？](#245)|
|246| [类属性 displayName 的用途是什么？](#246)|
|247| [React 应用程序支持哪些浏览器？](#247)|
|248| [unmountComponentAtNode 方法的作用是什么？](#248)|
|249| [什么是代码拆分？](#249)|
|250| [严格模式有什么好处？](#250)|
|251| [带 key 的 Fragments 是什么？](#251)|
|252| [React 是否支持所有 HTML 属性？](#252)|
|253| [HOC 有什么限制？](#253)|
|254| [DevTools 中如何调试 forwardRefs？](#254)|
|255| [组件 props 什么时候默认为 true？](#255)|
|256| [NextJS 是什么？它的主要特点是什么？](#256)|
|257| [如何给组件传递事件处理程序？](#257)|
|258| [在渲染方法中使用箭头函数好吗？](#258)|
|259| [如何防止函数被多次调用？](#259)|
|260| [JSX 如何防止注入攻击？](#260)|
|261| [你如何更新被渲染过的元素？](#261)|
|262| [你怎么理解 props 是只读的？](#262)|
|263| [你怎么理解状态更新是合并的？](#263)|
|264| [如何给事件处理程序传递参数？](#264)|
|265| [如何防止组件渲染？](#265)|
|266| [什么条件下使用索引作为 key 是安全的？](#266)|
|267| [key 是否应该是全局唯一的？](#267)|
|268| [流行的表单处理方案有哪些？](#268)|
|269| [formik 相对于 redux 表单库有什么优势？](#269)|
|270| [为什么不需要使用继承？](#270)|
|271| [我可以在 React 应用程序中使用 Web 组件吗？](#271)|
|272| [什么是动态导入？](#272)|
|273| [什么是可加载组件？](#273)|
|274| [什么是 suspense 组件？](#274)|
|275| [基于路由的代码拆分是什么？](#275)|
|276| [举例说明如何使用 context？](#276)|
|277| [context 中默认值的目的是什么？](#277)|
|278| [你如何使用上下文类型？](#278)|
|279| [什么是消费者？](#279)|
|280| [在使用 context 时如何解决性能问题？](#280)|
|281| [HOC中 forward ref 的目的是什么？](#281)|
|282| [是否所有函数或类组件都可用 ref 参数？](#282)|
|283| [为什么在使用 forward ref 时需要额外注意组件库？](#283)|
|284| [如何在没有 ES6 的情况下创建 react 类组件？](#284)|
|285| [可以在没有 JSX 的情况下使用 react 吗？](#285)|
|286| [什么是差异算法？](#286)|
|287| [diffing 算法涵盖哪些规则？](#287)|
|288| [什么时候需要使用 refs？](#288)|
|289| [prop 是否必须与渲染函数中的 props 命名一致？](#289)|
|290| [纯组件使用 render props 有什么问题？](#290)|
|291| [如何使用 render props 创建 HOC？](#291)|
|292| [什么是开窗技术？](#292)|
|293| [如何在 JSX 中打印 falsy 值？](#293)|
|294| [门户的典型用例是什么？](#294)|
|295| [如何为不受控组件设置默认值？](#295)|
|296| [你最喜欢的 React 技术栈是什么？](#296)|
|297| [真实 DOM 和虚拟 DOM 有什么区别？](#297)|
|298| [如何将 Bootstrap 添加到 React 应用程序？](#298)|
|299| [你能列出使用 react 作为前端框架的顶级网站或应用程序吗？](#299)|
|300| [是否推荐在 React 中使用 CSS In JS 技术？](#300)|
|301| [我需要用钩子重写我的所有类组件吗？](#301)|
|302| [如何使用 React Hooks 获取数据？](#302)|
|303| [Hooks 是否涵盖了类的所有用例？](#303)|
|304| [hooks 支持的稳定版本是什么？](#304)|
|305| [为什么我们在 useState 中使用数组解构（方括号表示法）？](#305)|
|306| [为什么引入 hooks？](#306)|
|307| [你如何看待 Web 组件的命令式 API？](#307)|
|308| [formik 是什么？](#308)|
|309| [在 Redux 中处理异步调用的典型中间件，选择用什么？](#309)|
|310| [浏览器能理解 JSX 代码吗？](#310)|
|311| [描述 React 中的数据流？](#311)|
|312| [react scripts 是什么？](#312)|
|313| [create react app 有什么特点？](#313)|
|314| [renderToNodeStream 方法的作用是什么？](#314)|
|315| [MobX 是什么？](#315)|
|316| [Redux 和 MobX 有什么区别？](#316)|
|317| [我应该在学习 ReactJS 之前学习 ES6 吗？](#317)|
|318| [什么是并发渲染？](#318)|
|319| [异步模式和并发模式有什么区别？](#319)|
|320| [我可以在 react16.9 中使用 javascript urls 吗？](#320)|
|321| [用于钩子的 eslint 插件的作用是什么？](#321)|
|322| [React 中的命令式和声明式有什么区别？](#322)|
|323| [将 typescript 与 reactjs 一起使用有什么好处？](#323)|
|324| [在使用 context API 状态管理时，如何确保用户在页面刷新时保持身份验证？](#324)|
|325| [新的 JSX 转换有什么好处？](#325)|
|326| [新的 JSX 转换与旧的转换有何不同？](#326)|
|327| [如何使用 create-react-app 获得 redux 脚手架？](#327)|
|328| [什么是 React 服务端组件？](#328)|
|329| [什么是 prop drilling?](#329)|
|330| [什么是 state 突变以及如何预防？](#330)|
|331| [useState 和 useRef 钩子有什么区别？](#331)|
|332| [React 中函数式组件和类组件有什么区别](#332)

## React 核心


    
1. ### 什么是React？ {#1}

    React 是一个**开源的前端 JavaScript 库**，用于构建用户界面，尤其适用于单页应用程序。它用于处理 Web 和移动应用程序的视图层。React 是由为 Facebook 工作的软件工程师JordanWalke创建的。 (https://github.com/jordwalke)React 于 2011 年首次部署在 Facebook 的 NewsFeed 上，并于 2012 年部署在 Instagram 上。


   **[⬆ 返回顶部](#table-of-contents)**
    
2. ### React 的主要特点是什么？ {#2}

    React 的主要特点是：

    * 考虑到 RealDOM 操作成本高昂，它使用 **VirtualDOM** 而不是 RealDOM。
    * 支持 **服务器端渲染**。
    * 遵循 **单向** 数据流或数据绑定。
    * 使用 **可重用/可组合** 的 UI 组件来开发视图。


   **[⬆ 返回顶部](#table-of-contents)**
    
3. ### 什么是 JSX？ {#3}

    *JSX* 是 ECMAScript 的类似 XML 的语法扩展（首字母缩写词代表 *JavaScript XML*）。基本上，它只是为`React.createElement()`函数提供语法糖，为我们提供 JavaScript 的表现力以及类似HTML 的模板语法。

    在下面的示例中，`<h1>`标签内的文本作为 JavaScript 函数返回给渲染函数。

    ```jsx
    class App extends React.Component {
      render() {
        return(
          <div>
            <h1>{'Welcome to React world!'}</h1>
          </div>
        )
      }
    }
    ```


   **[⬆ 返回顶部](#table-of-contents)**
    
4. ### Element 和 Component 之间有什么区别？ {#4}

    *Element* 是一个简单的对象，它根据 DOM 节点或其他组件描述您希望在屏幕上显示的内容。*Elements*可以在其 props 中包含其他*Elements*。创建一个 React 元素很容易。一旦创建了一个元素，它就永远不会发生变异。

    React Element 的对象表示如下：

    ```javascript
    const element = React.createElement(
      'div',
      {id: 'login-btn'},
      'Login'
    )
    ```

    上面的`React.createElement()`函数返回一个对象：

    ```javascript
    {
      type: 'div',
      props: {
        children: 'Login',
        id: 'login-btn'
      }
    }
    ```

    最后它使用`ReactDOM.render()`方法渲染到 DOM：

    ```html
    <div id='login-btn'>Login</div>
    ```

    而一个 **component** 可以用几种不同的方式声明。它可以是具有`render()`方法的类，也可以定义为函数。无论哪种情况，它都将 props 作为输入，并返回一个 JSX 树作为输出：

    ```javascript
    const Button = ({ onLogin }) =>
      <div id={'login-btn'} onClick={onLogin}>Login</div>
    ```

    然后 JSX 被转译成`React.createElement()`函数：

    ```javascript
    const Button = ({ onLogin }) => React.createElement(
      'div',
      { id: 'login-btn', onClick: onLogin },
      'Login'
    )
    ```


   **[⬆ 返回顶部](#table-of-contents)**
    
5. ### 如何在 React 中创建 Component？ {#5}

    有两种方法来创建组件。

    1. **函数组件：** 这是创建组件的最简单方法。这些是纯 JavaScript 函数，它们接受 props 对象作为第一个参数并返回 React 元素：
        ```jsx
        function Greeting({ message }) {
          return <h1>{`Hello, ${message}`}</h1>

        }
        ```

    2. **类组件：** 你也可以使用 ES6 类来定义一个组件。上面的函数组件可以写成：
        ```jsx
        class Greeting extends React.Component {
          render() {
            return <h1>{`Hello, ${this.props.message}`}</h1>
          }
        }
        ```


   **[⬆ 返回顶部](#table-of-contents)**
    
6. ### 什么时候用类组件而不是函数组件？ {#6}

    如果组件需要*状态或生命周期方法*，则使用类组件，否则使用 函数组件。
    *但是，从 React 16.8开始，添加了 Hooks，您可以在函数组件中使用状态、生命周期方法和其他仅在类组件中可用的功能。*
    *因此，始终建议使用 函数组件，除非您需要一个 React 功能，但它的 Function组件等效项尚不存在，例如错误边界。*


   **[⬆ 返回顶部](#table-of-contents)**
    
7. ### 什么是纯组件？ {#7}

    *`React.PureComponent`* 与 *`React.Component`*完全相同，只是它帮我们处理了`shouldComponentUpdate()`方法。当 props 或 state 发生变化时，*PureComponent* 将对 props 和 state 进行浅比较。 *Component* 不会将当前的 props 和 state 与下一次更新的进行比较。因此，`shouldComponentUpdate`方法默认返回`true`，该组件都会重新渲染。


   **[⬆ 返回顶部](#table-of-contents)**
    
8. ### React 中的 state 是什么？ {#8}

    组件的*State*是一个对象，它包含一些可能在组件的生命周期内发生变化的信息。 我们应该始终使我们的 state 尽可能简单，并尽量减少有状态组件的数量。

    让我们创建一个带有 message state 的用户组件，


    ```jsx
    class User extends React.Component {
      constructor(props) {
        super(props)

        this.state = {
          message: 'Welcome to React world'
        }
      }

      render() {
        return (
          <div>
            <h1>{this.state.message}</h1>
          </div>
        )
      }
    }
    ```

    ![state](images/state.jpg)

    state 类似于 props，但它是私有的并且完全由组件控制，如果该该组件不向其他组件传递，任何其他组件都无法访问它。


   **[⬆ 返回顶部](#table-of-contents)**
    
9. ### React 中的 props 是什么？ {#9}

    *Props* 是组件的入参。它们是单个值或包含一组值的对象，这些值在创建时使用类似于 HTML 标记属性的命名约定传递给组件。它们是从父组件传递到子组件的数据。

    React 中 props 的主要目的是提供以下组件功能：

    1. 将自定义数据传递给您的组件。
    2. 触发 state 变化。
    3. 在组件内的 `render()` 方法中，通过 `this.props.reactProp` 使用。

    例如，让我们创建一个具有 `reactProp` 属性的元素：

    ```jsx
    <Element reactProp={'1'} />
    ```

    把这个 `reactProp` (或任何你想出的) 属性名附加你使用 React 库创建的所有组件上，那么所有这些组件就有了这么一个 props 对象.

    ```jsx
    props.reactProp
    ```
    

    **示例：基于类的组件中的 props**

    ```jsx
    import React from 'react'
    import ReactDOM from 'react-dom'

    class ChildComponent extends React.Component {
        render() {
            return (
                <div>
                    <p>{this.props.name}</p>
                    <p>{this.props.age}</p>
                </div>
            )
        }
    }

    class ParentComponent extends React.Component {
        render() {
            return (
                <div>
                    <ChildComponent name='John' age='30' />
                    <ChildComponent name='Mary' age='25' />
                </div>
            )
        }
    }
    ```

    **示例：函数组件中的 props**

    ```jsx
    import React from 'react'
    import ReactDOM from 'react-dom'

    const ChildComponent = (props) => {
        return (
            <div>
                <p>{props.name}</p>
                <p>{props.age}</p>
            </div>
        )
    }

    const ParentComponent = () => {
        return (
            <div>
                <ChildComponent name='John' age='30' />
                <ChildComponent name='Mary' age='25' />
            </div>
        )
    }
    ```



   **[⬆ 返回顶部](#table-of-contents)**
    
10. ### state and props 之间有什么区别？ {#10}

    *props* and *state* 都是纯 JavaScript 对象。虽然它们都影响渲染输出的信息，但它们在组件方面的功能不同。`props` 类似于函数参数传递给组件，而 `state` 是在组件内管理的，类似于在函数中声明的变量。


   **[⬆ 返回顶部](#table-of-contents)**
    
11. ### 为什么我们不应该直接更新 state？ {#11}

    如果您尝试直接更新 `state`，那么它不会重新渲染组件。

    ```javascript
    //Wrong
    this.state.message = 'Hello world'
    ```

    而是使用 `setState()` 方法. 它用来更新组件中的 state 对象。当 state 改变时，组件会重新渲染。

    ```javascript
    //Correct
    this.setState({ message: 'Hello World' })
    ```

    **注意：**您可以使用最新的 javascript 的类声明语法，并直接在`constructor`中给 state 对象赋值。


   **[⬆ 返回顶部](#table-of-contents)**
    
12. ### 回调函数作为 `setState()` 的参数的目的是什么？ {#12}

    当 setState 完成并渲染组件时调用回调函数。由于`setState()`是**异步的**，回调函数可以用于任何发布操作。

    **注意：** 建议使用生命周期方法而不是这个回调函数。

    ```javascript
    setState({ name: 'John' }, () => console.log('The name has updated and component re-rendered'))
    ```


   **[⬆ 返回顶部](#table-of-contents)**
    
13. ### HTML 和 React 事件处理有什么区别？ {#13}
    以下是 HTML 和 React 事件处理之间的一些主要区别：

    1. 在 HTML 中，事件名称通常以*小写*形式表示：
        ```html
        <button onclick='activateLasers()'>
        ```

       而在 React 中，它遵循*camelCase*约定：
        ```jsx
        <button onClick={activateLasers}>
        ```

    2. 在 HTML 中，您可以返回`false`以阻止默认行为：
        ```html
        <a href='#' onclick='console.log("The link was clicked."); return false;' />
        ```

       而在 React 中你必须显式调用`preventDefault()`：
        ```javascript
        function handleClick(event) {
          event.preventDefault()
          console.log('The link was clicked.')
        }
        ```

    3. 在 HTML 中，您需要通过附加`()`来调用函数，而在 react 中，您不应该函数名称后附加`()`。（例如，参考第一点中的“activateLasers”功能）


   **[⬆ 返回顶部](#table-of-contents)**
    
14. ### 如何在 JSX 回调中绑定方法或事件处理程序？ {#14}

    有 3 种方法来实现这一点：

    1.	**构造函数中的绑定：** 在 JavaScript 类中，默认情况下不绑定方法。同样的事情也适用于定义为类方法的 React 事件处理程序。通常我们在构造函数中绑定它们。
        ```javascript
        class Foo extends Component {
          constructor(props) {
            super(props);
            this.handleClick = this.handleClick.bind(this);
          }
          handleClick() {
            console.log('Click happened');
          }
          render() {
            return <button onClick={this.handleClick}>Click Me</button>;
          }
        }

        ```

    2. **公共类字段语法：** 如果您不喜欢使用绑定方法，则可以使用*公共类字段语法*正确绑定回调。
        ```jsx
        handleClick = () => {
          console.log('this is:', this)
        }
        ```
        ```jsx
        <button onClick={this.handleClick}>
          {'Click me'}
        </button>
        ```

    3. **回调中的箭头函数：** 您可以直接在回调中使用*箭头函数*。
        ```jsx
        handleClick() {
            console.log('Click happened');
        }
        render() {
            return <button onClick={() => this.handleClick()}>Click Me</button>;
        }
        ```

    **注意：** 如果回调作为 prop 传递给子组件，这些组件可能会进行额外的重新渲染。在这些情况下，考虑到性能，最好使用`.bind()`*公共类字段语法*方法。


   **[⬆ 返回顶部](#table-of-contents)**
    
15. ### 如何将参数传递给事件处理程序或回调？ {#15}

    您可以使用*箭头函数*环绕*事件处理程序*并传递参数：

    ```jsx
    <button onClick={() => this.handleClick(id)} />
    ```

    这是一个等价的 `.bind` 写法:

    ```jsx
    <button onClick={this.handleClick.bind(this, id)} />
    ```
    除了这两种方法，您还可以将参数传递给返回值为箭头函数的函数
    ```jsx
    <button onClick={this.handleClick(id)} />
    handleClick = (id) => () => {
        console.log("Hello, your ticket number is", id)
    };
    ```


   **[⬆ 返回顶部](#table-of-contents)**
    
16. ### React 中的合成事件是什么？ {#16}

    `合成事件` 是围绕浏览器的本机事件的跨浏览器包装器。它的 API 与浏览器的原生事件相同，包括`stopPropagation()`和`preventDefault()`，除了事件在所有浏览器中的工作方式相同。


   **[⬆ 返回顶部](#table-of-contents)**
    
17. ### 什么是内联条件表达式？ {#17}

    您可以使用JS 提供的*if 语句*或*三元表达式*来有条件地呈现表达式。除了这些方法之外，您还可以通过将任何表达式包裹在花括号中，然后在 JS 逻辑运算符`&&`后面来嵌入任何 JSX 表达式。

    ```jsx
    <h1>Hello!</h1>
    {
        messages.length > 0 && !isLogin?
          <h2>
              You have {messages.length} unread messages.
          </h2>
          :
          <h2>
              You don't have unread messages.
          </h2>
    }
    ```


   **[⬆ 返回顶部](#table-of-contents)**
    
18. ### 什么是“key”属性，在元素数组中使用它有什么好处？ {#18}

    `key` 是一个特殊的字符属性，你应该 **should** 在创建元素数组时，为每一个元素添加一个 `key` 属性。 *Key* 属性帮助 React 识别哪些项目已更改、添加或删除。

    大多数情况下，我们使用数据中的 ID 作为 *key*:

    ```jsx
    const todoItems = todos.map((todo) =>
      <li key={todo.id}>
        {todo.text}
      </li>
    )
    ```

    当你的列表项没有固定 ID 时，你可以使用项目 *index* 作为 *key* 作为最后的选择：

    ```jsx
    const todoItems = todos.map((todo, index) =>
      <li key={index}>
        {todo.text}
      </li>
    )
    ```

    **笔记：**

    1. 如果列表顺序可能发生变化，**不建议**使用*索引*作为*key*。这会对性能产生负面影响，并可能导致组件状态出现问题。
    2. 如果列表项上不存在*key*属性，控制台中将显示一条警告消息。


   **[⬆ 返回顶部](#table-of-contents)**
    
19. ### refs有什么用？ {#19}

    *ref*用于返回对元素的引用。在大多数情况下应该*避免使用*它们，但是，当您需要直接访问 DOM元素或组件实例时，它们会很有用。


   **[⬆ 返回顶部](#table-of-contents)**
    
20. ### 如何创建 refs？ {#20}

    有两种方法
    1. 这是最近新增的方法。通过 `React.createRef()` 方法创建*Refs*。 然后将创建的 *Refs* 作为 React 元素的 `ref`属性。为了在整个组件中使用*refs*，只需将 *ref* 分配给构造函数中的实例属性。
        ```jsx
        class MyComponent extends React.Component {
          constructor(props) {
            super(props)
            this.myRef = React.createRef()
          }
          render() {
            return <div ref={this.myRef} />
          }
        }
        ```
    2. 你也可以在任何版本 React 中使用 ref 回调方法。例如，搜索栏组件的输入元素访问如下：
        ```jsx
        class SearchBar extends Component {
           constructor(props) {
              super(props);
              this.txtSearch = null;
              this.state = { term: '' };
              this.setInputSearchRef = e => {
                 this.txtSearch = e;
              }
           }
           onInputChange(event) {
              this.setState({ term: this.txtSearch.value });
           }
           render() {
              return (
                 <input
                    value={this.state.term}
                    onChange={this.onInputChange.bind(this)}
                    ref={this.setInputSearchRef} />
              );
           }
        }
        ```

    你也可以在函数组件中通过 **闭包** 使用 *refs* .
    **注意**: 即使不推荐使用内联 ref 回调，您也可以使用它。

   **[⬆ 返回顶部](#table-of-contents)**
    
21. ### 什么是 ref转发? {#21}

    *Ref 转发* 是一项功能，它允许某些组件获取它们接收到的 *ref*，并将其进一步传递给子组件。

    ```jsx
    const ButtonElement = React.forwardRef((props, ref) => (
      <button ref={ref} className="CustomButton">
        {props.children}
      </button>
    ));

    // 创建 DOM 按钮的引用:
    const ref = React.createRef();
    <ButtonElement ref={ref}>{'Forward Ref'}</ButtonElement>
    ```


   **[⬆ 返回顶部](#table-of-contents)**
    
22. ### 在 回调refs 和 findDOMNode() 中，选哪个更佳？ {#22}

    相对`findDOMNode()` API，最好使用*回调refs*。因为 `findDOMNode()` 阻碍了React未来的某些改进。

    使用 `findDOMNode` 的 **传统方法**:

    ```javascript
    class MyComponent extends Component {
      componentDidMount() {
        findDOMNode(this).scrollIntoView()
      }

      render() {
        return <div />
      }
    }
    ```

    推荐的方法：

    ```javascript
    class MyComponent extends Component {
      constructor(props){
        super(props);
        this.node = createRef();
      }
      componentDidMount() {
        this.node.current.scrollIntoView();
      }

      render() {
        return <div ref={this.node} />
      }
    }
    ```


   **[⬆ 返回顶部](#table-of-contents)**
    
23. ### 为什么 字符串引用 被删除？ {#23}

    如果您之前使用过 React，您可能会熟悉一个较旧的 API，其中 `ref` 属性是字符串，例如 `ref={'textInput'}`，并且 DOM 以 `this.refs.textInput` 方式来访问. 我们建议不要这样做，因为 *字符串引用有以下问题*, 并被认为是遗留问题。在 **React v16** 删除了字符串引用.

    1. 它们 *强制 React 跟踪当前正在执行的组件*。这是有问题的，因为它使 React 模块有状态，因此当 React 模块在包中复制时会导致奇怪的错误。
    2. 它们是*不可组合*的 — 如果一个组件在它的子组件上放置了一个 ref，用户就不能在它上面放置另一个 ref。而回调 ref 是完全可以组合的。
    3. 它们不能像 Flow 那样*做静态分析*。回调引用对静态分析更友好。
    4. 它不像大多数人所期望的那样使用 "render回调" 模式 (例如 <DataGrid renderRow={this.renderRow} />)
       ```jsx
       class MyComponent extends Component {
         renderRow = (index) => {
           // 这不起作用。 Ref 将会附加到 DataTable 而不是 MyComponent:
           return <input ref={'input-' + index} />;

           // 这会起作用! 回调 refs 很棒.
           return <input ref={input => this['input-' + index] = input} />;
         }

         render() {
           return <DataTable data={this.props.data} renderRow={this.renderRow} />
         }
       }
       ```

   **[⬆ 返回顶部](#table-of-contents)**
    
24. ### 什么是 虚拟DOM？ {#24}

    *虚拟 DOM* (VDOM) *真实 DOM* 的内存表示. UI 表示是保持内存的对象与"真实"DOM保持同步。这是在调用渲染函数和在屏幕上显示元素之间发生的一个步骤。这整个过程称为*和解*。


   **[⬆ 返回顶部](#table-of-contents)**
    
25. ### 虚拟 DOM 是如何工作的？ {#25}

    虚拟 DOM 通过三个简单的步骤工作。

    1. 每当任何底层数据发生变化时，整个 UI 都会以 虚拟 DOM 表示形式重新渲染。

        ![vdom](images/vdom1.png)

    2. 然后计算前一个 DOM 表示和新的表示之间的差异。

        ![vdom2](images/vdom2.png)

    3. 一旦计算完成，真实的 DOM 将只更新实际发生变化的内容。

        ![vdom3](images/vdom3.png)


   **[⬆ 返回顶部](#table-of-contents)**
    
26. ### Shadow DOM 和 Virtual DOM 有什么区别？ {#26}

    *Shadow DOM*是一种浏览器技术，主要设计用于*Web 组件*中的范围变量和 CSS。*虚拟 DOM*是一个由 JavaScript 库在浏览器 API 之上实现的概念。


   **[⬆ 返回顶部](#table-of-contents)**
    
27. ### 什么是 React Fiber？ {#27}

    Fiber 是 React v16 中新的*协调引擎*（或核心算法）的重新实现。React Fiber 的目标是提高其对动画、布局、手势等领域的适用性，以及暂停、中止或重用工作的能力，并为不同类型的更新分配优先级；和新的并发原语。


   **[⬆ 返回顶部](#table-of-contents)**
    
28. ### React Fiber 的主要目标是什么？ {#28}

    *React Fiber*的目标是提高其在动画、布局和手势等领域的适用性。它的主要功能是 **增量渲染** ：能够将渲染工作分成块并将其分散到多个帧上。
    
    *来源于文档说明*

    它的主要目标是:
      1. 能够将可中断的工作分成块。
      2. 对正在进行的工作进行优先级排序、变基和重用的能力。
      3. 能够在父组件和子组件之间来回让步以支持React中的布局。
      4. 能够从 render() 返回多个元素。
      5. 更好地支持错误边界。

   **[⬆ 返回顶部](#table-of-contents)**
    
29. ### 什么是受控组件？ {#29}

    控制后续用户输入时表单中的输入元素的组件称为**受控组件**，即每个 state 变化都有一个关联的处理函数。例如，要将所有名称都写成大写字母，我们使用 handleChange 如下，

    ```javascript
    handleChange(event) {
      this.setState({value: event.target.value.toUpperCase()})
    }
    ```


   **[⬆ 返回顶部](#table-of-contents)**
    
30. ### 什么是不受控组件？ {#30}

    **不受控制的组件**是在内部存储自己状态的组件，您可以在需要时使用 ref 查询 DOM 以找到其当前值。这有点像传统的 HTML。

    在下面的 UserProfile 组件中，`name`输入框使用 ref 访问输入。

    ```jsx
    class UserProfile extends React.Component {
      constructor(props) {
        super(props)
        this.handleSubmit = this.handleSubmit.bind(this)
        this.input = React.createRef()
      }

      handleSubmit(event) {
        alert('A name was submitted: ' + this.input.current.value)
        event.preventDefault()
      }

      render() {
        return (
          <form onSubmit={this.handleSubmit}>
            <label>
              {'Name:'}
              <input type="text" ref={this.input} />
            </label>
            <input type="submit" value="Submit" />
          </form>
        );
      }
    }
    ```

    在大多数情况下，建议使用受控组件来实现表单。在受控组件中，表单数据由 React 组件处理。另一种方法是不受控制的组件，其中表单数据由 DOM 本身处理。


   **[⬆ 返回顶部](#table-of-contents)**
    
31. ### createElement 和 cloneElement 有什么区别？ {#31}

    JSX 元素将被转换为`React.createElement()`函数以创建 React 元素，这些元素将用于 UI 的对象表示。而`cloneElement`用于克隆元素并传递新的 props。


   **[⬆ 返回顶部](#table-of-contents)**
    
32. ### React 中的状态提升是什么？ {#32}

    当多个组件需要共享相同的变化数据时，建议*将共享状态提升*到它们最近的共同祖先。这意味着如果两个子组件从其父组件共享相同的数据，则将状态移动到父组件，而不是在两个子组件中保持各自的状态。


   **[⬆ 返回顶部](#table-of-contents)**
    
33. ### 组件生命周期的不同阶段是什么？ {#33}

    组件具有三个不同的生命周期阶段：

    1. **挂载:** 组件已准备好挂载到浏览器 DOM 中。此阶段涵盖从 `constructor()`, `getDerivedStateFromProps()`, `render()`, 和 `componentDidMount()` 生命周期方法初始化.

    2. **更新:** 在这个阶段，组件以两种方式更新，发送新的 props，从setState()或forceUpdate()更新状态。 此阶段涵盖 `getDerivedStateFromProps()`, `shouldComponentUpdate()`, `render()`, `getSnapshotBeforeUpdate()` 和 `componentDidUpdate()` 生命周期方法

    3. **卸载:** 在最后一个阶段，不需要组件并从浏览器 DOM 中卸载。此阶段包括 `componentWillUnmount()` 生命周期方法。

    值得一提的是，React 内部在将更改应用于 DOM 时有一个阶段的概念。它们分别如下：

    1. **渲染** 该组件将渲染而没有任何副作用。这适用于 Pure 组件，在此阶段，React 可以暂停、中止或重新启动渲染。

    2. **预提交** 在组件实际将更改应用到 DOM 之前，有一段时间允许 React 通过 `getSnapshotBeforeUpdate()` 读取DOM。

    3. **提交** React 与 DOM 一起工作，并分别执行`componentDidMount()`安装、`componentDidUpdate()`更新和`componentWillUnmount()`卸载的最终生命周期。

    React 16.3+ 版本 ((http://projects.wojtekmaj.pl/react-lifecycle-methods-diagram/))

    ![phases 16.4+](images/phases16.4.png)

    React 16.3 之前版本

    ![phases 16.2](images/phases.png)



   **[⬆ 返回顶部](#table-of-contents)**
    
34. ### React 的生命周期方法有哪些？ {#34}

    在 React 16.3 之前

    - **componentWillMount:** 在渲染之前执行，用于根组件中的 App 级别配置。
    - **componentDidMount:** 在第一次渲染后执行，这里应该发生所有 AJAX 请求、DOM 或状态更新，并设置事件侦听器。
    - **componentWillReceiveProps:** 当特定的 prop 更新触发状态转换时执行。
    - **shouldComponentUpdate:** 确定是否更新组件。默认情况下它返回 `true` 。如果您确定组件在 state 或 props 更新后不需要渲染，则可以返回 false 值。这是提高性能的好地方，因为它允许您在组件收到新道具时防止重新渲染。
    - **componentWillUpdate:** 在重新渲染组件之前执行，当有 props 和 state 更改确认时 `shouldComponentUpdate()` 返回 true。
    - **componentDidUpdate:** 主要用于更新 DOM 以响应 prop 或 state 的变化。
    - **componentWillUnmount:** 它将用于取消任何传出的网络请求，或删除与该组件关联的所有事件侦听器。

    React 16.3+

    - **getDerivedStateFromProps:** 在调用 `render()` 之前调用，并在*每次* `render()` 时调用。这适用于需要派生状态的罕见用例。如果您需要派生状态](https://reactjs.org/blog/2018/06/07/you-probably-dont-need-derived-state.html).
    - **componentDidMount:** 在第一次渲染后执行，所有 AJAX 请求、DOM 或状态更新以及设置事件侦听器都应该发生。
    - **shouldComponentUpdate:** 确定是否更新组件。默认情况下，它返回 `true` 。如果您确定组件在 state 或 props 更新后不需要渲染，则可以返回 false 值。这是提高性能的好地方，因为它允许您在组件收到新props时防止重新渲染。
    - **getSnapshotBeforeUpdate:** 在渲染更新 DOM 之前执行。此返回的任何值都将传递到 `componentDidUpdate()` 。这对于从 DOM 捕获信息（即滚动位置）很有用。
    - **componentDidUpdate:** 主要用于更新 DOM 以响应 prop 或 state 的变化。如果 `shouldComponentUpdate()` 返回 `false`，该生命周期方法将不会触发。
    - **componentWillUnmount** 它将用于取消任何传出的网络请求，或删除与该组件关联的所有事件侦听器。


   **[⬆ 返回顶部](#table-of-contents)**
    
35. ### 什么是高阶组件？ {#35}

    *高阶组件* (*HOC*) 是一个函数，它接受一个组件作为参数并返回一个新组件。基本上，它是一种源自React 组合特性的模式。

    我们称它们为**纯组件**，因为它们可以接受任何动态提供的子组件，但它们不会修改或复制其输入组件的任何行为。

    ```javascript
    const EnhancedComponent = higherOrderComponent(WrappedComponent)
    ```

    HOC 可用于许多用例：

    1. 代码重用、逻辑和引导抽象。
    2. 渲染劫持。
    3. State 抽象和操作。
    4. Props 操作。


   **[⬆ 返回顶部](#table-of-contents)**
    
36. ### 如何为 HOC 组件创建 props 代理？ {#36}

    您可以使用*props 代理*模式添加/编辑传递给组件的props，如下所示：

    ```jsx
    function HOC(WrappedComponent) {
      return class Test extends Component {
        render() {
          const newProps = {
            title: 'New Header',
            footer: false,
            showFeatureX: false,
            showFeatureY: true
          }

          return <WrappedComponent {...this.props} {...newProps} />
        }
      }
    }
    ```


   **[⬆ 返回顶部](#table-of-contents)**
    
37. ### 什么是 context？ {#37}

    *Context*提供了一种通过组件树传递数据的方法，而无需在每个级别手动传递 props。
    例如，经过身份验证的用户、区域设置偏好、UI 主题需要在应用程序中由许多组件访问。

    ```javascript
    const {Provider, Consumer} = React.createContext(defaultValue)
    ```


   **[⬆ 返回顶部](#table-of-contents)**
    
38. ### 什么是子属性？ {#38}

    *Children* 是一个属性 (`this.props.children`) 它允许您将组件作为数据传递给其他组件，就像您使用的任何其他 prop 一样。放在组件的开始标签和结束标签之间的组件树将作为`children` prop 传递给该组件。

    React API 中有几种方法可以使用这个 prop。这些包括 `React.Children.map`, `React.Children.forEach`, `React.Children.count`, `React.Children.only`, `React.Children.toArray`.

    children prop 的简单用法如下所示，

    ```jsx
    const MyDiv = React.createClass({
      render: function() {
        return <div>{this.props.children}</div>
      }
    })

    ReactDOM.render(
      <MyDiv>
        <span>{'Hello'}</span>
        <span>{'World'}</span>
      </MyDiv>,
      node
    )
    ```


   **[⬆ 返回顶部](#table-of-contents)**
    
39. ### 如何在 React 中写评论？ {#39}

    React/JSX 中的注释类似于 JavaScript 多行注释，但用花括号括起来。

    **单行注释:**

    ```jsx
    <div>
      {/* Single-line comments(In vanilla JavaScript, the single-line comments are represented by double slash(//)) */}
      {`Welcome ${user}, let's play React`}
    </div>
    ```

    **多行注释:**

    ```jsx
    <div>
      {/* Multi-line comments for more than
       one line */}
      {`Welcome ${user}, let's play React`}
    </div>
    ```


   **[⬆ 返回顶部](#table-of-contents)**
    
40. ### 使用 super(props) 的目的是什么？ {#40}

    在调用`super(props)`方法之前，子类构造函数不能使用`this`引用。 `super()`同样适用于 ES6 子类。调用 `super(props)` 的主要原因就是在你的子构造函数中访问 `this.props` 。

    **super() 传 props:**

    ```javascript
    class MyComponent extends React.Component {
      constructor(props) {
        super(props)

        console.log(this.props) // prints { name: 'John', age: 42 }
      }
    }
    ```

    **super() 不传 props:**

    ```javascript
    class MyComponent extends React.Component {
      constructor(props) {
        super()

        console.log(this.props) // prints undefined

        // but props parameter is still available
        console.log(props) // prints { name: 'John', age: 42 }
      }

      render() {
        // no difference outside constructor
        console.log(this.props) // prints { name: 'John', age: 42 }
      }
    }
    ```

    上面的代码片段表明，`this.props` 仅在构造函数中有所不同。在构造函数之外也是一样的。


   **[⬆ 返回顶部](#table-of-contents)**
    
41. ### 什么是协调？ {#41}

    当组件的 props 或 state 发生变化时，React 通过将新返回的元素与之前渲染的元素进行比较来决定是否需要进行实际的 DOM 更新。当它们不相等时，React 将更新 DOM。这个过程称为*协调*。


   **[⬆ 返回顶部](#table-of-contents)**
    
42. ### 如何使用动态 key 设置 state？ {#42}

    如果您使用 ES6 或 Babel 转译器来转换您的 JSX 代码，那么您可以使用*计算的属性名*来完成此操作。

    ```javascript
    handleInputChange(event) {
      this.setState({ [event.target.id]: event.target.value })
    }
    ```


   **[⬆ 返回顶部](#table-of-contents)**
    
43. ### 每次渲染组件时调用函数的常见错误是什么？ {#43}

    您需要确保在将函数作为参数传递时没有调用该函数。

    ```jsx
    render() {
      // Wrong: handleClick is called instead of passed as a reference!
      return <button onClick={this.handleClick()}>{'Click Me'}</button>
    }
    ```

    相反，不带括号传递函数本身：

    ```jsx
    render() {
      // Correct: handleClick is passed as a reference!
      return <button onClick={this.handleClick}>{'Click Me'}</button>
    }
    ```


   **[⬆ 返回顶部](#table-of-contents)**
    
44. ### 惰性函数是否支持命名导出？ {#44}
    不支持，当前`React.lazy`功能仅支持默认导出。如果您想导入名为导出的模块，您可以创建一个中间模块，将其重新导出为默认模块。它还确保 tree shaking 继续工作并且不会拉动未使用的组件。让我们看一个导出多个命名组件的组件文件，
    ```javascript
    // MoreComponents.js
    export const SomeComponent = /* ... */;
    export const UnusedComponent = /* ... */;
    ```
    并在 `IntermediateComponent.js` 这个中间文件中重新导出 `MoreComponents.js` 组件。
    ```javascript
    // IntermediateComponent.js
    export { SomeComponent as default } from "./MoreComponents.js";
    ```
    现在您可以使用以下惰性函数导入模块，
    ```javascript
    import React, { lazy } from 'react';
    const SomeComponent = lazy(() => import("./IntermediateComponent.js"));
    ```

   **[⬆ 返回顶部](#table-of-contents)**
    
45. ### 为什么 React 使用 `className` 而不是 `class` 属性？ {#45}

    `class` 是 JavaScript 中的关键字，而 JSX 是 JavaScript 的扩展。这就是 React 使用 `className` 而不是 `class`，传递一个字符串作为 `className` 属性的原因。

    ```jsx
    render() {
      return <span className={'menu navigation-menu'}>{'Menu'}</span>
    }
    ```


   **[⬆ 返回顶部](#table-of-contents)**
    
46. ### 什么是 fragments？ {#46}

    这是 React 中的一种常见模式，用于组件返回多个元素。*Fragments* 让您可以对子列表进行分组，而无需向 DOM 添加额外的节点。

    ```jsx
    render() {
      return (
        <React.Fragment>
          <ChildA />
          <ChildB />
          <ChildC />
        </React.Fragment>
      )
    }
    ```

    还有一个*简短的语法*，但许多工具不支持它：

    ```jsx
    render() {
      return (
        <>
          <ChildA />
          <ChildB />
          <ChildC />
        </>
      )
    }
    ```


   **[⬆ 返回顶部](#table-of-contents)**
    
47. ### 为什么 fragments 比容器 div 更好？ {#47}
    有以下原因，

    1. 通过不创建额外的 DOM 节点，Fragments速度更快并且使用更少的内存。这只对非常大和深的树有真正的好处。
    2. 一些 CSS 机制如 `Flexbox` 和 `CSS Grid` 有特殊的父子关系，中间添加 div 很难保持想要的布局。
    3. DOM Inspector 不那么杂乱。


   **[⬆ 返回顶部](#table-of-contents)**
    
48. ### React 中的`Portal`是什么？ {#48}

    *Portal* 将子级渲染到存在于父组件的 DOM 层次结构之外的 DOM 节点中的推荐方式。

    ```javascript
    ReactDOM.createPortal(child, container)
    ```

    第一个参数是任何可渲染的 React 子节点，例如元素、字符串或片段。第二个参数是一个 DOM元素。


   **[⬆ 返回顶部](#table-of-contents)**
    
49. ### 什么是无状态组件？ {#49}

    如果组件的行为独立于其状态，则它可以是无状态组件。您可以使用函数或类来创建无状态组件。但除非您需要在组件中使用生命周期挂钩，否则您应该选择功能组件。如果你决定在这里使用函数组件，会有很多好处；它们易于编写、理解和测试，速度稍快，您可以完全避免使用关键字`this`。


   **[⬆ 返回顶部](#table-of-contents)**
    
50. ### 什么是有状态组件？ {#50}

    如果组件的行为依赖于组件的*state*，那么它可以称为有状态组件。这些*有状态组件*总是*类组件*，并且在`constructor`进行初始化`state`。

    ```javascript
    class App extends Component {
      constructor(props) {
        super(props)
        this.state = { count: 0 }
      }

      render() {
        // ...
      }
    }
    ```
    **React 16.8 更新:**

     Hooks 让你无需编写类即可使用状态和其他 React 特性。

     *等价的函数组件*

       ```javascript
        import React, {useState} from 'react';

        const App = (props) => {
          const [count, setCount] = useState(0);

          return (
            // JSX
          )
        }
       ```



   **[⬆ 返回顶部](#table-of-contents)**
    
51. ### 如何在 React 中验证 props？ {#51}

    当应用在*开发模式*下运行时，React 自动检查我们在组件上设置的所有prop，以确保它们具有正确的类型。如果类型不正确，React 将在控制台中生成警告消息。由于性能影响，它在*生产模式*下被禁用。强制性 `prop` 用`isRequired`。

    一组预定义的`prop`类型：

    1. `PropTypes.number`
    2. `PropTypes.string`
    3. `PropTypes.array`
    4. `PropTypes.object`
    5. `PropTypes.func`
    6. `PropTypes.node`
    7. `PropTypes.element`
    8. `PropTypes.bool`
    9. `PropTypes.symbol`
    10. `PropTypes.any`

    我们可以为`User`组件定义如下`PropTypes`：

    ```jsx
    import React from 'react'
    import PropTypes from 'prop-types'

    class User extends React.Component {
      static propTypes = {
        name: PropTypes.string.isRequired,
        age: PropTypes.number.isRequired
      }

      render() {
        return (
          <>
            <h1>{`Welcome, ${this.props.name}`}</h1>
            <h2>{`Age, ${this.props.age}`}</h2>
          </>
        )
      }
    }
    ```

    **注意:** 在 React v15.5 中 *PropTypes* 已从 `React.PropTypes` to `prop-types` 库.

    *等价的函数组件*

    ```jsx
    import React from 'react'
    import PropTypes from 'prop-types'
   
    function User({name, age}) {
      return (
        <>
          <h1>{`Welcome, ${name}`}</h1>
          <h2>{`Age, ${age}`}</h2>
        </>
      )
    }

    User.propTypes = {
      name: PropTypes.string.isRequired,
      age: PropTypes.number.isRequired
    }
    ```

   **[⬆ 返回顶部](#table-of-contents)**
    
52. ### React 的优点是什么？ {#52}
    以下是 React 的主要优点，

    1. 使用*Virtual DOM*提高应用程序的性能。
    2. JSX 使代码易于阅读和编写。
    3. 它在客户端和服务器端（*SSR*）呈现。
    4. 易于与框架（Angular、Backbone）集成，因为它只是一个视图库。
    5. 易于与其他测试工具，如 Jest 等工具配合使用时，轻松编写单元和集成测试。


   **[⬆ 返回顶部](#table-of-contents)**
    
53. ### React 的局限性是什么？ {#53}
    除了优点之外，React 的限制也不少,

    1. React 只是一个视图库，而不是一个完整的框架。
    2. 对于刚接触 Web 开发的初学者来说，有一个学习曲线。
    3. 将 React 集成到传统的 MVC 框架中需要一些额外的配置。
    4. 内联模板和 JSX 会增加代码复杂性。
    5. 太多较小的组件导致过度工程化或样板化。


   **[⬆ 返回顶部](#table-of-contents)**
    
54. ### React v16 中的错误边界是什么？ {#54}

    *错误边界*是在其子组件树的任何位置捕获 JavaScript 错误、记录这些错误并显示后备 UI 而不是崩溃的组件树。

    如果一个类组件定义了一个名为 `componentDidCatch(error, info)` 或 `static getDerivedStateFromError() `的新生命周期方法，它就会成为错误边界:

    ```jsx
    class ErrorBoundary extends React.Component {
      constructor(props) {
        super(props)
        this.state = { hasError: false }
      }

      componentDidCatch(error, info) {
        // You can also log the error to an error reporting service
        logErrorToMyService(error, info)
      }

      static getDerivedStateFromError(error) {
         // Update state so the next render will show the fallback UI.
         return { hasError: true };
       }

      render() {
        if (this.state.hasError) {
          // You can render any custom fallback UI
          return <h1>{'Something went wrong.'}</h1>
        }
        return this.props.children
      }
    }
    ```

    之后将其作为常规组件使用:

    ```jsx
    <ErrorBoundary>
      <MyWidget />
    </ErrorBoundary>
    ```


   **[⬆ 返回顶部](#table-of-contents)**
    
55. ### React v15 中如何处理错误边界？ {#55}

    React v15 使用 `unstable_handleError` 方法，为*错误边界*提供了非常基本的支持. 它在 React v16 被重命名为 `componentDidCatch` 。


   **[⬆ 返回顶部](#table-of-contents)**
    
56. ### 静态类型检查的推荐方法是什么？ {#56}

    通常我们使用 *PropTypes 库* (从 React v15.5 开始 `React.PropTypes` 被移到 `prop-types` 包) 在 React 应用程序中做 *类型检查* 。对于大型代码库，建议使用*静态类型检查器*，例如Flow 或 TypeScript，它们在编译时执行类型检查并提供自动完成功能。


   **[⬆ 返回顶部](#table-of-contents)**
    
57. ### `react-dom` 包有什么用？ {#57}

    `react-dom` 包提供了可以在应用程序的顶层使用的*特定于DOM的方法*。大多数组件都不需要使用此模块。这个包的一些方法是：

    1. `render()`
    2. `hydrate()`
    3. `unmountComponentAtNode()`
    4. `findDOMNode()`
    5. `createPortal()`


   **[⬆ 返回顶部](#table-of-contents)**
    
58. ### `react-dom`的render方法的目的是什么？ {#58}

    此方法用于将 React 元素渲染到所提供容器中的 DOM 中，并返回对该组件的引用。如果React 元素之前已渲染到容器中，它将对其执行更新，并且仅根据需要更改 DOM 以反映最新更改。

    ```
    ReactDOM.render(element, container, [callback])
    ```

    如果提供了可选的 callback 参数，它将在组件渲染或更新后执行。


   **[⬆ 返回顶部](#table-of-contents)**
    
59. ### ReactDOMServer 是什么？ {#59}

    ReactDOMServer对象使您能够将组件呈现为静态标签（通常在node服务器上使用）。该对象主要用于*服务端渲染（SSR）。*在服务器和浏览器环境中都可以使用以下方法：

    1. `renderToString()`
    2. `renderToStaticMarkup()`

    例如，您通常运行基于 node 的 Web 服务器，如 Express、Hapi 或 Koa，然后调用`renderToString`以将根组件呈现为字符串，然后将其作为响应发送。

    ```javascript
    // using Express
    import { renderToString } from 'react-dom/server'
    import MyPage from './MyPage'

    app.get('/', (req, res) => {
      res.write('<!DOCTYPE html><html><head><title>My Page</title></head><body>')
      res.write('<div id="content">')
      res.write(renderToString(<MyPage/>))
      res.write('</div></body></html>')
      res.end()
    })
    ```


   **[⬆ 返回顶部](#table-of-contents)**
    
60. ### 如何在 React 中使用 InnerHtml？ {#60}

     React 中的 `dangerouslySetInnerHTML` 属性，与浏览器 DOM 中 `innerHTML`等价。就像 `innerHTML` 一样，考虑到跨站点脚本 (XSS) 攻击，使用此属性是有风险的。您只需将`__html`对象作为键和 HTML 文本作为值传递。

    在这个例子中 MyComponent 使用`dangerouslySetInnerHTML`属性来设置 HTML 标记：

    ```jsx
    function createMarkup() {
      return { __html: 'First &middot; Second' }
    }

    function MyComponent() {
      return <div dangerouslySetInnerHTML={createMarkup()} />
    }
    ```


   **[⬆ 返回顶部](#table-of-contents)**
    
61. ### 如何在 React 中使用样式？ {#61}

    该`style`属性接受带有驼峰式属性的 JavaScript 对象，而不是 CSS 字符串。这与 DOM 样式的JavaScript 属性一致，效率更高，并且可以防止 XSS 安全漏洞。

    ```jsx
    const divStyle = {
      color: 'blue',
      backgroundImage: 'url(' + imgUrl + ')'
    };

    function HelloWorldComponent() {
      return <div style={divStyle}>Hello World!</div>
    }
    ```

    样式键是驼峰式的，以便与在 JavaScript 中访问 DOM 节点上的属性保持一致（例如`node.style.backgroundImage`）。


   **[⬆ 返回顶部](#table-of-contents)**
    
62. ### React 中的事件有何不同？ {#62}

    在 React 元素中处理事件有一些语法差异：

    1. React 事件处理程序使用驼峰命名，而不是小写。
    2. 使用 JSX，您将函数作为事件处理程序传递，而不是字符串。


   **[⬆ 返回顶部](#table-of-contents)**
    
63. ### 如果在构造函数中使用 setState() 会发生什么？ {#63}

    当您使用`setState()`时，除了分配给对象状态之外，React 还会重新渲染组件及其所有子组件。你会得到这样的错误：*只能更新一个挂载或挂载的组件*。所以我们需要在构造函数内部，使用`this.state`来初始化 state 变量。


   **[⬆ 返回顶部](#table-of-contents)**
    
64. ### 索引作为键有什么影响？ {#64}

    键应该是稳定的、可预测的和唯一的，以便 React 可以跟踪元素。

    在下面的代码片段中，每个元素的键都将基于排序，而不是与所表示的数据相关联。这限制了React 可以做的优化。

    ```jsx
    {todos.map((todo, index) =>
      <Todo
        {...todo}
        key={index}
      />
    )}
    ```

    如果你使用元素数据作为唯一键，假设 `todo.id` 对这个列表是唯一的并且是稳定的，React 将能够重新排序元素而无需重新计算它们。

    ```jsx
    {todos.map((todo) =>
      <Todo {...todo}
        key={todo.id} />
    )}
    ```


   **[⬆ 返回顶部](#table-of-contents)**
    
65. ### 在 `componentWillMount()` 方法中使用 `setState()` 好吗？ {#65}

    是的, 在 `componentWillMount()` 方法中使用 `setState()` 是安全的。 但同时建议在 `componentWillMount()` 生命周期方法中避免异步初始化。`componentWillMount()` 在挂载发生之前立即调用。它在 `render()` 方法之前调用，因此在此方法中设置状态不会触发重新渲染。避免在此方法中引入任何副作用或订阅。我们需要确保组件初始化的异步调用发生在 `componentDidMount()` 而不是 `componentWillMount()` 中。

    ```jsx
    componentDidMount() {
      axios.get(`api/todos`)
        .then((result) => {
          this.setState({
            messages: [...result.data]
          })
        })
    }
    ```


   **[⬆ 返回顶部](#table-of-contents)**
    
66. ### 如果你在初始化状态时使用 props 会发生什么？ {#66}

    如果组件上的 props 在组件没有被刷新的情况下发生了变化，那么新的 props 值将永远不会显示，因为构造函数永远不会更新组件的当前状态。来自 props 的状态初始化仅在组件首次创建时运行。

    以下组件不会显示更新的输入值：

    ```jsx
    class MyComponent extends React.Component {
      constructor(props) {
        super(props)

        this.state = {
          records: [],
          inputValue: this.props.inputValue
        };
      }

      render() {
        return <div>{this.state.inputValue}</div>
      }
    }
    ```

    在 render 方法中使用 props 会更新值：

    ```jsx
    class MyComponent extends React.Component {
      constructor(props) {
        super(props)

        this.state = {
          record: []
        }
      }

      render() {
        return <div>{this.props.inputValue}</div>
      }
    }
    ```


   **[⬆ 返回顶部](#table-of-contents)**
    
67. ### 如何条件渲染组件？ {#67}

   在某些情况下，您希望根据某些状态呈现不同的组件。 JSX 不渲染 `false` 、 `undefined`，因此只有在某个条件为真时，您才能使用条件`短路`来渲染组件的给定部分。

    ```jsx
    const MyComponent = ({ name, address }) => (
      <div>
        <h2>{name}</h2>
        {address &&
          <p>{address}</p>
        }
      </div>
    )
    ```

    如果您需要 `if-else` 条件，请使用 *三元运算符*。

    ```jsx
    const MyComponent = ({ name, address }) => (
      <div>
        <h2>{name}</h2>
        {address
          ? <p>{address}</p>
          : <p>{'Address is not available'}</p>
        }
      </div>
    )
    ```


   **[⬆ 返回顶部](#table-of-contents)**
    
68. ### 为什么我们在 DOM 元素上传递 props 时需要小心？ {#68}

    当我们*传递 props*时，我们会遇到添加未知 HTML 属性的风险，这是一种不好的做法。相反，我们可以使用带有运算符的属性解构`...rest`，那么它只会添加所需的属性。

    例如，

    ```jsx
    const ComponentA = () =>
      <ComponentB isDisplay={true} className={'componentStyle'} />

    const ComponentB = ({ isDisplay, ...domProps }) =>
      <div {...domProps}>{'ComponentB'}</div>
    ```


   **[⬆ 返回顶部](#table-of-contents)**
    
69. ### 如何在 React 中使用装饰器？ {#69}

    您可以*装饰*您的*类*组件，这与将组件传递给函数相同。**装饰器** 是修改组件功能的很灵活且可读的方式。

    ```jsx
    @setTitle('Profile')
    class Profile extends React.Component {
        //....
    }

    /*
      title 是一个字符串，将被设置为文档标题，就像上面的例子中，WrappedComponent 就是我们的装饰器在类组件上接收到的内容
    */
    const setTitle = (title) => (WrappedComponent) => {
      return class extends React.Component {
        componentDidMount() {
          document.title = title
        }

        render() {
          return <WrappedComponent {...this.props} />
        }
      }
    }
    ```

    **注意：** 装饰器是一个没有进入 ES7 的特性，但目前是第 2 阶段的提案。


   **[⬆ 返回顶部](#table-of-contents)**
    
70. ### 你如何记忆一个组件？ {#70}

    有可用的 memoize 库可用于函数组件。

    例如`moize`库可以在另一个组件中记住该组件。

    ```jsx
    import moize from 'moize'
    import Component from './components/Component' // 这个模块导出一个非记忆的组件

    const MemoizedFoo = moize.react(Component)

    const Consumer = () => {
      <div>
        {'I will memoize the following entry:'}
        <MemoizedFoo/>
      </div>
    }
    ```

    **更新：** 从 React v16.6.0 开始，我们有了一个 `React.memo`。它提供了一个更高阶的组件，它可以记忆组件，除非 props 发生变化。要使用它，只需在使用之前使用 `React.memo` 包装组件即可。

    ```js
      const MemoComponent = React.memo(function MemoComponent(props) {
        /* 使用 props 渲染 */
      });
      OR
      export default React.memo(MyFunctionComponent);
    ```

   **[⬆ 返回顶部](#table-of-contents)**
    
71. ### 您如何实现服务器端渲染或 SSR？ {#71}

    React 已经具备在 Node 服务器上处理渲染的能力。有一个特殊版本的 DOM 渲染器可用，它遵循与客户端相同的模式。

    ```jsx
    import ReactDOMServer from 'react-dom/server'
    import App from './App'

    ReactDOMServer.renderToString(<App />)
    ```

    此方法会将常规 HTML 输出为字符串，然后可以将其作为服务器响应的一部分放置在页面正文中。在客户端，React 检测到预渲染的内容并无缝地从中断的地方继续。


   **[⬆ 返回顶部](#table-of-contents)**
    
72. ### 如何在 React 中启用生产模式？ {#72}

    您应该使用 Webpack 的 `DefinePlugin` 方法设置 `NODE_ENV` 为 `production` ，通过它去除诸如 propType 验证和额外警告之类的东西。除此之外，如果你压缩代码，例如，Uglify 的废代码消除，以及仅开发时用到的调试代码和注释，它将大大减少你的包的大小。


   **[⬆ 返回顶部](#table-of-contents)**
    
73. ### 什么是 CRA 及其好处？ {#73}

    `create-react-app` CLI 工具使您无需配置步骤即可快速创建和运行 React 应用程序。

    让我们使用*CRA*创建 Todo App：

    ```console
    # 安装
    $ npm install -g create-react-app

    # 创建新项目
    $ create-react-app todo-app
    $ cd todo-app

    # 构建、测试和运行
    $ npm run build
    $ npm run test
    $ npm start
    ```
    它包含了我们构建 React 应用程序所需的一切：

    1. React、JSX、ES6 和 Flow 语法支持。
    2. ES6 之外的语言附加功能，例如对象扩展运算符。
    3. 自动添加 CSS 前缀，因此您不需要添加 -webkit- 或其他前缀。
    4. 一个快速的交互式单元测试运行器，内置对覆盖率报告的支持。
    5. 对常见错误发出警告的实时开发服务器。
    6. 一个构建脚本，用于生产的 JS、CSS 和图像的打包，以及散列和源映射。


   **[⬆ 返回顶部](#table-of-contents)**
    
74. ### Mounting 中的生命周期方法顺序是什么？ {#74}

    在创建组件实例并将其插入 DOM 时，将按以下顺序调用生命周期方法。

    1. `constructor()`
    2. `static getDerivedStateFromProps()`
    3. `render()`
    4. `componentDidMount()`


   **[⬆ 返回顶部](#table-of-contents)**
    
75. ### React v16 将弃用哪些生命周期方法？ {#75}

    以下生命周期方法将是不安全的编码实践，并且在异步渲染时会出现更多问题。

    1. `componentWillMount()`
    2. `componentWillReceiveProps()`
    3. `componentWillUpdate()`

    从 React v16.3 开始，这些方法使用 `UNSAFE_` 前缀作为别名，并且在 React v17 中将删除无前缀版本。


   **[⬆ 返回顶部](#table-of-contents)**
    
76. ### `getDerivedStateFromProps()` 生命周期方法的目的是什么？ {#76}

    新的静态 `getDerivedStateFromProps()` 生命周期方法在组件被实例化之后以及在重新渲染之前被调用。它可以返回一个对象来更新状态，或者返回 `null` 表明不需要任何状态更新。

    ```javascript
    class MyComponent extends React.Component {
      static getDerivedStateFromProps(props, state) {
        // ...
      }
    }
    ```

    这个生命周期方法与 `componentDidUpdate()` 涵盖了 `componentWillReceiveProps()` 的所有使用场景。


   **[⬆ 返回顶部](#table-of-contents)**
    
77. ### `getSnapshotBeforeUpdate()` 生命周期方法的目的是什么？ {#77}

    新的 `getSnapshotBeforeUpdate()` 生命周期方法在 DOM 更新之前被调用。此方法的返回值将作为第三个参数传递给 `componentDidUpdate()`。

    ```javascript
    class MyComponent extends React.Component {
      getSnapshotBeforeUpdate(prevProps, prevState) {
        // ...
      }
    }
    ```

    这个生命周期方法与 `componentDidUpdate()` 涵盖了 `componentWillUpdate()` 的所有使用场景。


   **[⬆ 返回顶部](#table-of-contents)**
    
78. ### Hooks 会取代 render props 和 高阶组件吗？ {#78}

    渲染道具和高阶组件都只渲染一个子节点，但在大多数情况下，Hooks 是一种通过减少树中的嵌套来提供此服务的更简单方法。


   **[⬆ 返回顶部](#table-of-contents)**
    
79. ### 命名组件的推荐用法是什么？ {#79}

    建议通过引用来命名组件，而不是使用 `displayName`.

    使用 `displayName` 命名组件：

    ```javascript
    export default React.createClass({
      displayName: 'TodoApp',
      // ...
    })
    ```

    **推荐** 的方法

    ```javascript
    export default class TodoApp extends React.Component {
      // ...
    }
    ```
    也可以这样 
    ```javascript 
    const TodoApp = () => {
     //...
    }
    export default TodoApp;
    ```

   **[⬆ 返回顶部](#table-of-contents)**
    
80. ### 组件类中方法的推荐顺序是什么？ {#80}

    *Recommended* ordering of methods from *mounting* to *render stage*:
    从*挂载*到*渲染*阶段的*推荐*方法顺序：

    1. `static` 方法
    2. `constructor()`
    3. `getChildContext()`
    4. `componentWillMount()`
    5. `componentDidMount()`
    6. `componentWillReceiveProps()`
    7. `shouldComponentUpdate()`
    8. `componentWillUpdate()`
    9. `componentDidUpdate()`
    10. `componentWillUnmount()`
    11. 单击处理程序或事件处理程序，例如 `onClickSubmit()` 或 `onChangeDescription()`
    12. 用于渲染的 getter 方法如 `getSelectReason()` 或 `getFooterContent()`
    13. 可选的渲染方法，如 `renderNavigation()` 或 `renderProfilePicture()`
    14. `render()`


   **[⬆ 返回顶部](#table-of-contents)**
    
81. ### 什么是开关组件？ {#81}

    *开关组件* 是呈现多个组件之一的组件。我们需要使用 object 将 prop 值映射到组件。

    比如一个开关组件，根据 `page` 属性显示不同的页面：

    ```jsx
    import HomePage from './HomePage'
    import AboutPage from './AboutPage'
    import ServicesPage from './ServicesPage'
    import ContactPage from './ContactPage'

    const PAGES = {
      home: HomePage,
      about: AboutPage,
      services: ServicesPage,
      contact: ContactPage
    }

    const Page = (props) => {
      const Handler = PAGES[props.page] || ContactPage

      return <Handler {...props} />
    }

    // PAGES 对象的键可用于page属性类型中以捕获开发时错误。
    Page.propTypes = {
      page: PropTypes.oneOf(Object.keys(PAGES)).isRequired
    }
    ```


   **[⬆ 返回顶部](#table-of-contents)**
    
82. ### 为什么我们需要给 setState() 传递函数？ {#82}

    这背后的原因是这 `setState()` 是一个异步操作。出于性能原因，React 批处理状态更改，因此在调用`setState()`后状态可能不会立即更改。这意味着您在调用 `setState()` 时不应依赖当前状态，因为您无法确定该状态将是什么。解决方案是将函数传递给 `setState()` ，将先前的状态作为参数。通过这样做，您可以避免由于`setState()`的异步特性而导致用户在访问时获取旧状态值的问题。

    假设初始计数值为零。在三个连续的递增操作之后，该值将仅递增 1。

    ```javascript
    // 假设 this.state.count === 0
    this.setState({ count: this.state.count + 1 })
    this.setState({ count: this.state.count + 1 })
    this.setState({ count: this.state.count + 1 })
    // this.state.count === 1, 而不是 3
    ```

    如果我们将函数传递给 `setState()`，则计数会正确递增。

    ```javascript
    this.setState((prevState, props) => ({
      count: prevState.count + props.increment
    }))
    // this.state.count === 3 符合预期
    ```

    **（或者）**

    ### 为什么 `setState()` 方法中函数优先于对象？

     React 可以将多个`setState()`调用批处理到单个更新中以提高性能。因为`this.props`和`this.state`可能会异步更新，所以您不应该依赖它们的值来计算下一个状态。

     此计数器示例将无法按预期更新：

     ```javascript
     // 错误的
     this.setState({
       counter: this.state.counter + this.props.increment,
     })
     ```

     首选方法是调用 `setState()` 方法，并传递函数而不是对象。该函数将接收先前的状态作为第一个参数，并将应用更新时的属性作为第二个参数。

     ```javascript
     // 正确的
     this.setState((prevState, props) => ({
       counter: prevState.counter + props.increment
     }))
     ```


   **[⬆ 返回顶部](#table-of-contents)**

    
83. ### React 中的严格模式是什么？ {#83}

    `React.StrictMode` 是一个有用的组件，用于暴露应用程序中的潜在问题。它像 `<Fragment>`, `<StrictMode>` 组件一样，不会渲染任何额外的 DOM 元素。它为其后代激活额外的检查和警告。这些检查仅适用于*开发模式*。

    ```jsx
    import React from 'react'

    function ExampleApplication() {
      return (
        <div>
          <Header />
          <React.StrictMode>
            <div>
              <ComponentOne />
              <ComponentTwo />
            </div>
          </React.StrictMode>
          <Header />
        </div>
      )
    }
    ```

    在上面的示例中，*严格模式*检查仅适用于`<ComponentOne>`和`<ComponentTwo>`组件。


   **[⬆ 返回顶部](#table-of-contents)**
    
84. ### React Mixins是什么？ {#84}

    *Mixins*是一种完全分离组件以具有通用功能的方法。**不应该使用**Mixins，可以用*高阶组件*或*装饰器*替换。

    最常用的 mixin 之一是`PureRenderMixin`。当 props 和 state 与先前的 props 和 state 浅相等时，您可能会在某些组件中使用它来防止不必要的重新渲染：

    ```javascript
    const PureRenderMixin = require('react-addons-pure-render-mixin')

    const Button = React.createClass({
      mixins: [PureRenderMixin],
      // ...
    })
    ```
    <!-- TODO: mixins 已被弃用 -->


   **[⬆ 返回顶部](#table-of-contents)**
    
85. ### Why is `isMounted()` an anti-pattern and what is the proper solution?

    The primary use case for `isMounted()` is to avoid calling `setState()` after a component has been unmounted, because it will emit a warning.

    ```javascript
    if (this.isMounted()) {
      this.setState({...})
    }
    ```

    Checking `isMounted()` before calling `setState()` does eliminate the warning, but it also defeats the purpose of the warning. Using `isMounted()` is a code smell because the only reason you would check is because you think you might be holding a reference after the component has unmounted.

    An optimal solution would be to find places where `setState()` might be called after a component has unmounted, and fix them. Such situations most commonly occur due to callbacks, when a component is waiting for some data and gets unmounted before the data arrives. Ideally, any callbacks should be canceled in `componentWillUnmount()`, prior to unmounting.


   **[⬆ 返回顶部](#table-of-contents)**
    
86. ### React 支持哪些指针事件？ {#86}

    *指针事件*提供了处理所有输入事件的统一方式。在过去，我们有一个鼠标和相应的事件监听器来处理它们，但现在我们有许多与鼠标无关的设备，比如带有触摸表面或笔的手机。我们需要记住，这些事件只会在支持*指针事件*规范的浏览器中起作用。

    *React DOM*现在可以使用以下事件类型：

    1. `onPointerDown`
    2. `onPointerMove`
    3. `onPointerUp`
    4. `onPointerCancel`
    5. `onGotPointerCapture`
    6. `onLostPointerCapture`
    7. `onPointerEnter`
    8. `onPointerLeave`
    9. `onPointerOver`
    10. `onPointerOut`


   **[⬆ 返回顶部](#table-of-contents)**
    
87. ### 为什么组件名称要以大写字母开头？ {#87}

    如果您使用 JSX 渲染组件，则该组件的名称必须以大写字母开头，否则 React 将作为无法识别的标记抛出错误。这个约定是因为只有 HTML 元素和 SVG 标签可以以小写字母开头。
    ```jsx
    class SomeComponent extends Component {
     // Code goes here
    }
    ```
    您可以定义名称以小写字母开头的组件类，但是当它被导入时，它应该是大写字母。这里小写没问题：

    ```jsx
    class myComponent extends Component {
      render() {
        return <div />
      }
    }

    export default myComponent
    ```

    而在另一个文件中导入时，它应该以大写字母开头：

    ```jsx
    import MyComponent from './myComponent'
    ```

    #### React 组件命名有哪些例外？

    组件名称应以大写字母开头，但此约定很少有例外。带有点的小写标记名称（属性访问器）仍被视为有效的组件名称。
    例如，下面的标签可以编译成一个有效的组件，

    ```jsx
         render() {
              return (
                <obj.component/> // `React.createElement(obj.component)`
              )
        }
    ```

   **[⬆ 返回顶部](#table-of-contents)**
    
88. ### React v16 是否支持自定义 DOM 属性？ {#88}

    是的。过去，React 过去常常忽略未知的 DOM 属性。如果你用 React 无法识别的属性编写JSX，React 会跳过它。

    例如，让我们看一下下面的属性：

    ```jsx
    <div mycustomattribute={'something'} />
    ```

    使用 React v15 将向 DOM 渲染一个空 div：

    ```html
    <div />
    ```

    在 React v16 中，任何未知的 DOM 属性最终都会出现在 DOM 中：

    ```html
    <div mycustomattribute='something' />
    ```

    这对于提供特定于浏览器的非标准属性、尝试新的 DOM API 以及与个性化的第三方库集成很有用。


   **[⬆ 返回顶部](#table-of-contents)**
    
89. ### 构造函数和getInitialState有什么区别？ {#89}

    使用 ES6 类时应在构造函数中初始化状态，使用`React.createClass()` 时使用 `getInitialState()` 方法初始化状态。

    **使用 ES6 类：**

    ```javascript
    class MyComponent extends React.Component {
      constructor(props) {
        super(props)
        this.state = { /* 初始状态 */ }
      }
    }
    ```

    **使用 `React.createClass()`：**

    ```javascript
    const MyComponent = React.createClass({
      getInitialState() {
        return { /* 初始状态 */ }
      }
    })
    ```

    **注意：** `React.createClass()` 在 React v16 中已弃用和删除。请改用纯 JavaScript 类。


   **[⬆ 返回顶部](#table-of-contents)**
    
90. ### 你能在不调用 setState 的情况下强制组件重新渲染吗？ {#90}

    默认情况下，当您的组件的 `state` 或 `props` 发生变化时，您的组件将重新渲染。如果你的`render()`方法依赖于其他一些数据，你可以通过调用`forceUpdate()`告诉 React 组件需要重新渲染。

    ```javascript
    component.forceUpdate(callback)
    ```

    建议避免使用`forceUpdate()`，并且在`render()`方法中只读取`this.props`和`this.state`。


   **[⬆ 返回顶部](#table-of-contents)**
    
91. ### 使用 ES6 类的 React 中的 `super()` 和 `super(props)` 有什么区别？ {#91}

    当您想在`constructor()`方法中访问`this.props`时，您应该将`props`传递给`super()`方法。

    **使用`super(props)`：**

    ```javascript
    class MyComponent extends React.Component {
      constructor(props) {
        super(props)
        console.log(this.props) // { name: 'John', ... }
      }
    }
    ```

    **使用`super()`：**

    ```javascript
    class MyComponent extends React.Component {
      constructor(props) {
        super()
        console.log(this.props) // undefined
      }
    }
    ```

    在`constructor()`方法之外，`this.props`都将显示相同的值。


   **[⬆ 返回顶部](#table-of-contents)**
    
92. ### 如何在 JSX 中循环？ {#92}

    您可以简单地使用`Array.prototype.map`和*ES6箭头函数*语法。

    例如，`items`对象数组被映射为组件数组：

    ```jsx
    <tbody>
      {items.map(item => <SomeComponent key={item.id} name={item.name} />)}
    </tbody>
    ```

    但是您不能使用 `for` 循环进行迭代：

    ```jsx
    <tbody>
      for (let i = 0; i < items.length; i++) {
        <SomeComponent key={items[i].id} name={items[i].name} />
      }
    </tbody>
    ```

    这是因为 JSX 标签被转译为*函数调用*，你不能在表达式中使用语句。


   **[⬆ 返回顶部](#table-of-contents)**
    
93. ### 如何在属性引号中访问 props？ {#93}

    React（或 JSX）不支持属性值内的变量插值。以下表示将不起作用：

    ```jsx
    <img className='image' src='images/{this.props.image}' />
    ```

    但是您可以将任何 JS 表达式放在大括号内作为整个属性值。所以下面的表达式有效：

    ```jsx
    <img className='image' src={'images/' + this.props.image} />
    ```

    使用*模板字符串*也可以：

    ```jsx
    <img className='image' src={`images/${this.props.image}`} />
    ```


   **[⬆ 返回顶部](#table-of-contents)**
    
94. ### 什么是带形状的 React PropType 数组？ {#94}

    如果要将对象数组传递给具有特定形状的组件，那么使用 `React.PropTypes.shape()` 作为参数传递给 `React.PropTypes.arrayOf()`。

    ```javascript
    ReactComponent.propTypes = {
      arrayWithShape: React.PropTypes.arrayOf(React.PropTypes.shape({
        color: React.PropTypes.string.isRequired,
        fontSize: React.PropTypes.number.isRequired
      })).isRequired
    }
    ```


   **[⬆ 返回顶部](#table-of-contents)**
    
95. ### 如何有条件地应用 class 属性？ {#95}

    您不应该在引号内使用大括号，因为它将被当作字符串。

    ```jsx
    <div className="btn-panel {this.props.visible ? 'show' : 'hidden'}">
    ```

    相反，您需要将花括号移到外面（不要忘记在类名之间包含空格）：

    ```jsx
    <div className={'btn-panel ' + (this.props.visible ? 'show' : 'hidden')}>
    ```

    *模板字符串*也可以：

    ```jsx
    <div className={`btn-panel ${this.props.visible ? 'show' : 'hidden'}`}>
    ```


   **[⬆ 返回顶部](#table-of-contents)**
    
96. ### React 和 ReactDOM 有什么区别？ {#96}

    `react` 包包含 `React.createElement()`, `React.Component`, `React.Children`，和其他与元素、组件类相关的帮助程序。您可以将这些视为构建组件所需的同构或通用助手。`react-dom` 包包含 `ReactDOM.render()`，并且在 `react-dom/server` 中有 `ReactDOMServer.renderToString()` 和 `ReactDOMServer.renderToStaticMarkup()`方法来支持*服务端渲染*。


   **[⬆ 返回顶部](#table-of-contents)**
    
97. ### 为什么 ReactDOM 与 React 分离？ {#97}

    React 团队致力于将所有与 DOM 相关的特性提取到一个名为*ReactDOM*的单独库中。React v0.14 是第一个拆分库的版本。通过查看一些包，`react-native`、`react-art`、`react-canvas`与`react-three`，很明显 React 的妙处和本质与浏览器或 DOM 无关。

    为了构建更多 React 可以渲染的环境，React 团队计划将主要的 React 包分成两个：`react`和`react-dom`。这为编写可以在 Web 版本的 React 和 React Native 之间共享的组件铺平了道路。


   **[⬆ 返回顶部](#table-of-contents)**
    
98. ### 如何使用 React 标签元素？ {#98}

    如果你尝试渲染一个 `<label>` 元素，并且使用标准的 `for` 属性绑定到一个文本输入框，那么生成HTML标签将会丢失该属性，并向控制台打印警告。

    ```jsx
    <label for={'user'}>{'User'}</label>
    <input type={'text'} id={'user'} />
    ```

    由于 `for` 是 JavaScript 中的保留关键字，请改用 `htmlFor`。

    ```jsx
    <label htmlFor={'user'}>{'User'}</label>
    <input type={'text'} id={'user'} />
    ```


   **[⬆ 返回顶部](#table-of-contents)**
    
99. ### 如何组合多个内联样式对象？ {#99}

    您可以在React中使用*扩展运算符*：

    ```jsx
     <button style={{...styles.panel.button, ...styles.panel.submitButton}}>{'Submit'}</button>
    ```

    如果您使用的是 React Native，那么您可以使用数组表示法：

    ```jsx
    <button style={[styles.panel.button, styles.panel.submitButton]}>{'Submit'}</button>
    ```


   **[⬆ 返回顶部](#table-of-contents)**
    
100. ### 调整浏览器大小时如何重新渲染视图？

     您可以在`componentDidMount()`中监听`resize`事件，然后更新维度（`width`和`height`）。你应该在 `componentWillUnmount()` 方法中删除监听事件。

     ```javascript
     class WindowDimensions extends React.Component {
       constructor(props){
         super(props);
         this.updateDimensions = this.updateDimensions.bind(this);
       }
        
       componentWillMount() {
         this.updateDimensions()
       }

       componentDidMount() {
         window.addEventListener('resize', this.updateDimensions)
       }

       componentWillUnmount() {
         window.removeEventListener('resize', this.updateDimensions)
       }

       updateDimensions() {
         this.setState({width: window.innerWidth, height: window.innerHeight})
       }

       render() {
         return <span>{this.state.width} x {this.state.height}</span>
       }
     }
     ```


   **[⬆ 返回顶部](#table-of-contents)**
    
101. ### `setState()` 和 `replaceState()` 方法有什么区别？ {#101}

     当您使用`setState()`，当前和以前的状态会合并。 `replaceState()` 舍弃当前状态，并仅用您提供的内容替换它。通常使用 `setState()`，除非您出于某种原因确实需要删除所有以前的`key`。你也可以在`setState()`中，将状态设置为`false`/`null`，而不是使用`replaceState()`。


   **[⬆ 返回顶部](#table-of-contents)**
    
102. ### 如何监听 state 变化？ {#102}

     状态改变时会调用`componentDidUpdate`生命周期方法。您可以将新的 state 和 props 值与当前state 和 props 进行比较，以确定是否有变化。

     ```javascript
     componentDidUpdate(object prevProps, object prevState)
     ```

     **注意：** ReactJS 的早期版本也使用 `componentWillUpdate(object nextProps, object nextState)` 来监听 state 变化。它已在最新版本中被弃用。

   **[⬆ 返回顶部](#table-of-contents)**
    
103. ### 在 react state 中删除数组元素的推荐方法是什么？ {#103}

     较好的方法是使用 `Array.prototype.filter()` 方法。

     例如，让我们创建一个 `removeItem()` 更新状态的方法。

     ```javascript
     removeItem(index) {
       this.setState({
         data: this.state.data.filter((item, i) => i !== index)
       })
     }
     ```


   **[⬆ 返回顶部](#table-of-contents)**
    
104. ### 是否可以在不渲染 HTML 的情况下使用 React？ {#104}

     最新版本（> = 16.2）是可以的。以下是可以的选项：

     ```jsx
     render() {
       return false
     }
     ```

     ```jsx
     render() {
       return null
     }
     ```

     ```jsx
     render() {
       return []
     }
     ```

     ```jsx
     render() {
       return <React.Fragment></React.Fragment>
     }
     ```

     ```jsx
     render() {
       return <></>
     }
     ```

     返回 `undefined` 就不行。


   **[⬆ 返回顶部](#table-of-contents)**
    
105. ### 如何使用 React 格式化打印 JSON？ {#105}

     我们可以使用 `<pre>` 标签来格式化显示`JSON.stringify()`的输出内容：

     ```jsx
     const data = { name: 'John', age: 42 }

     class User extends React.Component {
       render() {
         return (
           <pre>
             {JSON.stringify(data, null, 2)}
           </pre>
         )
       }
     }

     React.render(<User />, document.getElementById('container'))
     ```


   **[⬆ 返回顶部](#table-of-contents)**
    
106. ### 为什么你不能在 React 中更新 props？ {#106}

     React 的哲学是 props 应该是*不可变*的和*自上向下*的。这意味着父组件可以向子组件发送任何`props`值，但子组件不能修改收到的`props`。


   **[⬆ 返回顶部](#table-of-contents)**
    
107. ### 如何在页面加载时让输入元素获取焦点？

     您可以为`输入元素`创建*ref*，在`componentDidMount()`方法中使元素获取焦点：

     ```jsx
     class App extends React.Component{
       componentDidMount() {
         this.nameInput.focus()
       }

       render() {
         return (
           <div>
             <input
               defaultValue={'Won\'t focus'}
             />
             <input
               ref={(input) => this.nameInput = input}
               defaultValue={'Will focus'}
             />
           </div>
         )
       }
     }

     ReactDOM.render(<App />, document.getElementById('app'))
     ```

     在函数组件中可以这样（react 16.08 及更高版本）
     
      ```jsx
      import React, {useEffect, useRef} from 'react';

      const App = () => {
        const inputElRef = useRef(null)
        
        useEffect(()=>{
          inputElRef.current.focus()
        }, [])
        
        return(
          <div>
            <input
              defaultValue={'Won\'t focus'}
            />
            <input
              ref={inputElRef}
              defaultValue={'Will focus'}
            />
          </div>
        )
      }

      ReactDOM.render(<App />, document.getElementById('app'))
      ```
   **[⬆ 返回顶部](#table-of-contents)**
    
108. ### 更新 state 中的对象的方式有哪些？ {#108}

     1. **调用 `setState()` 以合并state的对象**

         * 使用 `Object.assign()` 创建对象的副本：

             ```javascript
             const user = Object.assign({}, this.state.user, { age: 42 })
             this.setState({ user })
             ```

         * 使用*扩展运算符*：

             ```javascript
             const user = { ...this.state.user, age: 42 }
             this.setState({ user })
             ```

     2. **调用 `setState()` 并传递一个函数**

         ```javascript
         this.setState(prevState => ({
           user: {
             ...prevState.user,
             age: 42
           }
         }))
         ```


   **[⬆ 返回顶部](#table-of-contents)**
    

109. ### 我们如何在浏览器中找到当前运行的 React 版本？ {#109}

     可以使用 `React.version` 来获取版本。

     ```jsx
     const REACT_VERSION = React.version

     ReactDOM.render(
       <div>{`React version: ${REACT_VERSION}`}</div>,
       document.getElementById('app')
     )
     ```


   **[⬆ 返回顶部](#table-of-contents)**
    
110. ### 在你的 `create-react-app` 中包含 polyfill 的方法有哪些？ {#110}

     有这些方法可以让 create-react-app 中包含 polyfill，

     1. **手动导入 `core-js`：**

         创建一个名为（类似）`polyfills.js`的文件，并将其导入根文件`index.js`。运行`npm install core-js`或`yarn add core-js`导入您的特定所需功能。

         ```javascript
         import 'core-js/fn/array/find'
         import 'core-js/fn/array/includes'
         import 'core-js/fn/number/is-nan'
         ```

     2. **使用 Polyfill 服务：**

         使用 polyfill.io CDN 检索自定义的、特定于浏览器的 polyfill，方法是将此行添加到`index.html`：

         ```html
         <script src='https://cdn.polyfill.io/v2/polyfill.min.js?features=default,Array.prototype.includes'></script>
         ```

         在上面的脚本中，我们明确请求`Array.prototype.includes`功能，因为它不包含在默认功能集中。


   **[⬆ 返回顶部](#table-of-contents)**
    
111. ### 如何在 create-react-app 中使用 https 而不是 http？ {#111}

     你只需要使用 `HTTPS=true` 配置。您可以编辑 `package.json` scripts 部分:

     ```json
     "scripts": {
       "start": "set HTTPS=true && react-scripts start"
     }
     ```

     或者运行 `set HTTPS=true && npm start`


   **[⬆ 返回顶部](#table-of-contents)**
    
112. ### 如何避免在 create-react-app 中使用相对路径导入？ {#112}

     在项目根目录创建 `.env` 文件，并写入导入路径：

     ```
     NODE_PATH=src/app
     ```

     之后重新启动开发服务器。现在您应该能够在`src/app`内没有相对路径的情况下导入任何内容。


   **[⬆ 返回顶部](#table-of-contents)**
    
113. ### 如何为 react-router 添加 Google Analytics？ {#113}

     在`history`对象上添加一个监听器来记录每个页面视图：

     ```javascript
     history.listen(function (location) {
       window.ga('set', 'page', location.pathname + location.search)
       window.ga('send', 'pageview', location.pathname + location.search)
     })
     ```


   **[⬆ 返回顶部](#table-of-contents)**
    
114. ### 如何每秒更新组件？ {#114}

     您需要使用`setInterval()`来触发更新，但您还需要在组件卸载时清除计时器以防止错误和内存泄漏。

     ```javascript
     componentDidMount() {
       this.interval = setInterval(() => this.setState({ time: Date.now() }), 1000)
     }

     componentWillUnmount() {
       clearInterval(this.interval)
     }
     ```


   **[⬆ 返回顶部](#table-of-contents)**
    
115. ### 如何将供应商前缀应用于 React 中的内联样式？ {#115}

     React*不会*自动应用*供应商前缀*。您需要手动添加供应商前缀。

     ```jsx
     <div style={{
       transform: 'rotate(90deg)',
       WebkitTransform: 'rotate(90deg)', // note the capital 'W' here
       msTransform: 'rotate(90deg)' // 'ms' is the only lowercase vendor prefix
     }} />
     ```


   **[⬆ 返回顶部](#table-of-contents)**
    
116. ### 如何使用 react 和 ES6 导入和导出组件？ {#116}

     您应该使用默认值来导出组件

     ```jsx
     import React from 'react'
     import User from 'user'

     export default class MyProfile extends React.Component {
       render(){
         return (
           <User type="customer">
             //...
           </User>
         )
       }
     }
     ```

     使用导出标识符，MyProfile 表示该模块并被导出，在可以其他组件中可以在不使用该名称的情况下导入该组件。


   **[⬆ 返回顶部](#table-of-contents)**

117. ### React 组件命名有哪些例外？ {#117}

     正在收集中。。。

   **[⬆ 返回顶部](#table-of-contents)**
    
118. ### 为什么组件 constructor 函数只调用一次？ {#118}

     React 的*协调*算法假设在没有任何相反信息的情况下，如果自定义组件在后续渲染中出现在同一位置，则它与之前的组件相同，因此重用之前的实例而不是创建新实例。


   **[⬆ 返回顶部](#table-of-contents)**
    
119. ### 如何在 React 中定义常量？ {#119}

     您可以使用 ES7 `static` 修饰符来定义常量。

     ```javascript
     class MyComponent extends React.Component {
       static DEFAULT_PAGINATION = 10
     }
     ```
     

   **[⬆ 返回顶部](#table-of-contents)**
    
120. ### 如何以编程方式触发 React 中的点击事件？ {#120}

     您可以使用 ref 属性通过回调获取对底层`HTMLInputElement`对象进行引用，将该引用存储为类属性，然后使用该引用稍后使用该`HTMLElement.click`方法触发来自事件处理程序的单击。

     这可以分两步完成：

     1. 在 render 方法中创建 ref：

         ```jsx
         <input ref={input => this.inputElement = input} />
         ```

     2. 在事件处理程序中执行点击事件：

         ```javascript
         this.inputElement.click()
         ```


   **[⬆ 返回顶部](#table-of-contents)**
    
121. ### 是否可以在普通 React 中使用 async/await？ {#121}

     如果你想在 React 中使用 `async`/`await` ，你需要使用 *Babel* 和 [transform-async-to-generator](https://babeljs.io/docs/en/babel-plugin-transform-async-to-generator) 插件。React Native 附带Babel和各种转换的功能。


   **[⬆ 返回顶部](#table-of-contents)**
    
122. ### React 的常见文件夹结构是什么？ {#122}

     React 项目文件结构有两种常见的做法。

     1. **按功能或路由分组：**

         构建项目的一种常见方法是将 CSS、JS 和测试用例放在一起，按功能或路由分组。

         ```
         common/
         ├─ Avatar.js
         ├─ Avatar.css
         ├─ APIUtils.js
         └─ APIUtils.test.js
         feed/
         ├─ index.js
         ├─ Feed.js
         ├─ Feed.css
         ├─ FeedStory.js
         ├─ FeedStory.test.js
         └─ FeedAPI.js
         profile/
         ├─ index.js
         ├─ Profile.js
         ├─ ProfileHeader.js
         ├─ ProfileHeader.css
         └─ ProfileAPI.js
         ```

     2. **按文件类型分组：**

         构建项目的另一种流行方法是将相似的文件组合在一起。

         ```
         api/
         ├─ APIUtils.js
         ├─ APIUtils.test.js
         ├─ ProfileAPI.js
         └─ UserAPI.js
         components/
         ├─ Avatar.js
         ├─ Avatar.css
         ├─ Feed.js
         ├─ Feed.css
         ├─ FeedStory.js
         ├─ FeedStory.test.js
         ├─ Profile.js
         ├─ ProfileHeader.js
         └─ ProfileHeader.css
         ```


   **[⬆ 返回顶部](#table-of-contents)**
    
123. ### 流行的动画包有哪些？ {#123}

     *React Transition Group* 和 *React Motion* 是 React 生态系统中流行的动画包。


   **[⬆ 返回顶部](#table-of-contents)**
    
124. ### 样式模块化有什么好处？ {#124}

     建议避免在组件中使用硬编码样式值。任何可能跨不同 UI 组件使用的样式值都应提取到它们自己的模块中。

     例如，可以将这些样式提取到单独的组件中：

     ```javascript
     export const colors = {
       white,
       black,
       blue
     }

     export const space = [
       0,
       8,
       16,
       32,
       64
     ]
     ```

     然后在其他组件中单独导入：

     ```javascript
     import { space, colors } from './styles'
     ```


   **[⬆ 返回顶部](#table-of-contents)**
    
125. ### 什么是流行的特定于 React 的 linter？ {#125}

     ESLint 是一种流行的 JavaScript linter。有一些插件可以分析特定的代码风格。`eslint-plugin-ract`npm包是React最常用的一个 lint 包。 默认情况下，它将检查许多最佳实践，包括迭代器中的 key、prop types等。

     另一个流行的插件是 `eslint-plugin-jsx-a11y`，它帮助解决可访问性的常见问题。由于JSX 提供的语法与常规 HTML 略有不同，因此常规插件不会发现`alt文本`和`tabindex`的问题。


   **[⬆ 返回顶部](#table-of-contents)**
    
126. ### 如何进行 AJAX 调用以及我应该在哪些组件生命周期方法中进行 AJAX 调用？ {#126}

     您可以使用 AJAX 库，例如 Axios、jQuery AJAX 和浏览器内置的`fetch`。您应该在`componentDidMount()`生命周期方法中获取数据。这样您就可以在检索数据时使用`setState()`来更新组件。

     例如，从 API 中获取员工列表并设置本地状态：

     ```jsx
     class MyComponent extends React.Component {
       constructor(props) {
         super(props)
         this.state = {
           employees: [],
           error: null
         }
       }

       componentDidMount() {
         fetch('https://api.example.com/items')
           .then(res => res.json())
           .then(
             (result) => {
               this.setState({
                 employees: result.employees
               })
             },
             (error) => {
               this.setState({ error })
             }
           )
       }

       render() {
         const { error, employees } = this.state
         if (error) {
           return <div>Error: {error.message}</div>;
         } else {
           return (
             <ul>
               {employees.map(employee => (
                 <li key={employee.name}>
                   {employee.name}-{employee.experience}
                 </li>
               ))}
             </ul>
           )
         }
       }
     }
     ```


   **[⬆ 返回顶部](#table-of-contents)**
    
127. ### 什么是 render props? {#127}

     **Render Props** 是一种在组件之间共享代码的技术，它使用函数作为prop值。下面的组件使用了render prop，在render prop 中返回一个 React 元素。

     ```jsx
     <DataProvider render={data => (
       <h1>{`Hello ${data.target}`}</h1>
     )}/>
     ```

     React Router 和 DownShift 等库正在使用这种模式。

## React Router


   **[⬆ 返回顶部](#table-of-contents)**
    
128. ### 什么是 React Router? {#128}

     React Router 是一个建立在 React 之上的强大的路由库，它可以帮助你非常快速地向应用程序添加新的页面和流程，同时保持页面上显示的内容与 URL 同步。


   **[⬆ 返回顶部](#table-of-contents)**
    
129. ### React Router 与 history 库有何不同？ {#129}

     React Router 是`history`库的包装器，它处理浏览器`window.history` hash 与浏览器的交互。它还提供了内存历史记录，这对于没有全局历史记录的环境很有用，例如移动应用程序开发（React Native）和Node的单元测试。


   **[⬆ 返回顶部](#table-of-contents)**
    
130. ### React Router v4 中的 `<Router>` 组件是什么？ {#130}

     React Router v4 提供了以下 3个 `<Router>` 组件:

     1. `<BrowserRouter>`
     2. `<HashRouter>`
     3. `<MemoryRouter>`

     上述组件将创建*browser*、*hash*和*memory* history实例。 React Router v4 使`history`与您的路由器关联的实例的属性和方法可通过`router`对象中的上下文使用。


   **[⬆ 返回顶部](#table-of-contents)**
    
132. ### What is the purpose of `push()` and `replace()` methods of `history`?

     A history instance has two methods for navigation purpose.

     1. `push()`
     2. `replace()`

     If you think of the history as an array of visited locations, `push()` will add a new location to the array and `replace()` will replace the current location in the array with the new one.


   **[⬆ 返回顶部](#table-of-contents)**
    
133. ### How do you programmatically navigate using React Router v4?

     There are three different ways to achieve programmatic routing/navigation within components.

     1. **Using the `withRouter()` higher-order function:**

         The `withRouter()` higher-order function will inject the history object as a prop of the component. This object provides `push()` and `replace()` methods to avoid the usage of context.

         ```jsx harmony
         import { withRouter } from 'react-router-dom' // this also works with 'react-router-native'

         const Button = withRouter(({ history }) => (
           <button
             type='button'
             onClick={() => { history.push('/new-location') }}
           >
             {'Click Me!'}
           </button>
         ))
         ```

     2. **Using `<Route>` component and render props pattern:**

         The `<Route>` component passes the same props as `withRouter()`, so you will be able to access the history methods through the history prop.

         ```jsx harmony
         import { Route } from 'react-router-dom'

         const Button = () => (
           <Route render={({ history }) => (
             <button
               type='button'
               onClick={() => { history.push('/new-location') }}
             >
               {'Click Me!'}
             </button>
           )} />
         )
         ```

     3. **Using context:**

         This option is not recommended and treated as unstable API.

         ```jsx harmony
         const Button = (props, context) => (
           <button
             type='button'
             onClick={() => {
               context.history.push('/new-location')
             }}
           >
             {'Click Me!'}
           </button>
         )

         Button.contextTypes = {
           history: React.PropTypes.shape({
             push: React.PropTypes.func.isRequired
           })
         }
         ```


   **[⬆ 返回顶部](#table-of-contents)**
    
134. ### How to get query parameters in React Router v4?

     The ability to parse query strings was taken out of React Router v4 because there have been user requests over the years to support different implementation. So the decision has been given to users to choose the implementation they like. The recommended approach is to use query strings library.

     ```javascript
     const queryString = require('query-string');
     const parsed = queryString.parse(props.location.search);
     ```

     You can also use `URLSearchParams` if you want something native:

     ```javascript
     const params = new URLSearchParams(props.location.search)
     const foo = params.get('name')
     ```

     You should use a *polyfill* for IE11.


   **[⬆ 返回顶部](#table-of-contents)**
    
135. ### Why you get "Router may have only one child element" warning?

     You have to wrap your Route's in a `<Switch>` block because `<Switch>` is unique in that it renders a route exclusively.

     At first you need to add `Switch` to your imports:

     ```javascript
     import { Switch, Router, Route } from 'react-router'
     ```

     Then define the routes within `<Switch>` block:

     ```jsx harmony
     <Router>
       <Switch>
         <Route {/* ... */} />
         <Route {/* ... */} />
       </Switch>
     </Router>
     ```


   **[⬆ 返回顶部](#table-of-contents)**
    
136. ### How to pass params to `history.push` method in React Router v4?

     While navigating you can pass props to the `history` object:

     ```javascript
     this.props.history.push({
       pathname: '/template',
       search: '?name=sudheer',
       state: { detail: response.data }
     })
     ```

     The `search` property is used to pass query params in `push()` method.


   **[⬆ 返回顶部](#table-of-contents)**
    
137. ### How to implement *default* or *NotFound* page?

     A `<Switch>` renders the first child `<Route>` that matches. A `<Route>` with no path always matches. So you just need to simply drop path attribute as below

     ```jsx harmony
     <Switch>
       <Route exact path="/" component={Home}/>
       <Route path="/user" component={User}/>
       <Route component={NotFound} />
     </Switch>
     ```


   **[⬆ 返回顶部](#table-of-contents)**
    
138. ### How to get history on React Router v4?
     Below are the list of steps to get history object on React Router v4,

     1. Create a module that exports a `history` object and import this module across the project.

         For example, create `history.js` file:

         ```javascript
         import { createBrowserHistory } from 'history'

         export default createBrowserHistory({
           /* pass a configuration object here if needed */
         })
         ```

     2. You should use the `<Router>` component instead of built-in routers. Import the above `history.js` inside `index.js` file:

         ```jsx harmony
         import { Router } from 'react-router-dom'
         import history from './history'
         import App from './App'

         ReactDOM.render((
           <Router history={history}>
             <App />
           </Router>
         ), holder)
         ```

     3. You can also use push method of `history` object similar to built-in history object:

         ```javascript
         // some-other-file.js
         import history from './history'

         history.push('/go-here')
         ```


   **[⬆ 返回顶部](#table-of-contents)**
    
139. ### How to perform automatic redirect after login?

     The `react-router` package provides `<Redirect>` component in React Router. Rendering a `<Redirect>` will navigate to a new location. Like server-side redirects, the new location will override the current location in the history stack.

     ```javascript
     import React, { Component } from 'react'
     import { Redirect } from 'react-router'

     export default class LoginComponent extends Component {
       render() {
         if (this.state.isLoggedIn === true) {
           return <Redirect to="/your/redirect/page" />
         } else {
           return <div>{'Login Please'}</div>
         }
       }
     }
     ```

## React 国际化


   **[⬆ 返回顶部](#table-of-contents)**
    
140. ### What is React Intl?

     The *React Intl* library makes internationalization in React straightforward, with off-the-shelf components and an API that can handle everything from formatting strings, dates, and numbers, to pluralization. React Intl is part of *FormatJS* which provides bindings to React via its components and API.


   **[⬆ 返回顶部](#table-of-contents)**
    
141. ### What are the main features of React Intl?
     Below are the main features of React Intl,

        1. Display numbers with separators.
        2. Display dates and times correctly.
        3. Display dates relative to "now".
        4. Pluralize labels in strings.
        5. Support for 150+ languages.
        6. Runs in the browser and Node.
        7. Built on standards.


   **[⬆ 返回顶部](#table-of-contents)**
    
142. ### What are the two ways of formatting in React Intl?

     The library provides two ways to format strings, numbers, and dates:

     1. **Using react components:**

         ```jsx harmony
         <FormattedMessage
           id={'account'}
           defaultMessage={'The amount is less than minimum balance.'}
         />
         ```

     2. **Using an API:**

         ```javascript
         const messages = defineMessages({
           accountMessage: {
             id: 'account',
             defaultMessage: 'The amount is less than minimum balance.',
           }
         })

         formatMessage(messages.accountMessage)
         ```


   **[⬆ 返回顶部](#table-of-contents)**
    
143. ### How to use `<FormattedMessage>` as placeholder using React Intl?

     The `<Formatted... />` components from `react-intl` return elements, not plain text, so they can't be used for placeholders, alt text, etc. In that case, you should use lower level API `formatMessage()`. You can inject the `intl` object into your component using `injectIntl()` higher-order component and then format the message using `formatMessage()` available on that object.

     ```jsx harmony
     import React from 'react'
     import { injectIntl, intlShape } from 'react-intl'

     const MyComponent = ({ intl }) => {
       const placeholder = intl.formatMessage({id: 'messageId'})
       return <input placeholder={placeholder} />
     }

     MyComponent.propTypes = {
       intl: intlShape.isRequired
     }

     export default injectIntl(MyComponent)
     ```


   **[⬆ 返回顶部](#table-of-contents)**
    
144. ### How to access current locale with React Intl?

     You can get the current locale in any component of your application using `injectIntl()`:

     ```jsx harmony
     import { injectIntl, intlShape } from 'react-intl'

     const MyComponent = ({ intl }) => (
       <div>{`The current locale is ${intl.locale}`}</div>
     )

     MyComponent.propTypes = {
       intl: intlShape.isRequired
     }

     export default injectIntl(MyComponent)
     ```


   **[⬆ 返回顶部](#table-of-contents)**
    
145. ### How to format date using React Intl?

     The `injectIntl()` higher-order component will give you access to the `formatDate()` method via the props in your component. The method is used internally by instances of `FormattedDate` and it returns the string representation of the formatted date.

     ```jsx harmony
     import { injectIntl, intlShape } from 'react-intl'

     const stringDate = this.props.intl.formatDate(date, {
       year: 'numeric',
       month: 'numeric',
       day: 'numeric'
     })

     const MyComponent = ({intl}) => (
       <div>{`The formatted date is ${stringDate}`}</div>
     )

     MyComponent.propTypes = {
       intl: intlShape.isRequired
     }

     export default injectIntl(MyComponent)
     ```

## React Testing


   **[⬆ 返回顶部](#table-of-contents)**
    
146. ### What is Shallow Renderer in React testing?

     *Shallow rendering* is useful for writing unit test cases in React. It lets you render a component *one level deep* and assert facts about what its render method returns, without worrying about the behavior of child components, which are not instantiated or rendered.

     For example, if you have the following component:

     ```javascript
     function MyComponent() {
       return (
         <div>
           <span className={'heading'}>{'Title'}</span>
           <span className={'description'}>{'Description'}</span>
         </div>
       )
     }
     ```

     Then you can assert as follows:

     ```jsx harmony
     import ShallowRenderer from 'react-test-renderer/shallow'

     // in your test
     const renderer = new ShallowRenderer()
     renderer.render(<MyComponent />)

     const result = renderer.getRenderOutput()

     expect(result.type).toBe('div')
     expect(result.props.children).toEqual([
       <span className={'heading'}>{'Title'}</span>,
       <span className={'description'}>{'Description'}</span>
     ])
     ```


   **[⬆ 返回顶部](#table-of-contents)**
    
147. ### What is `TestRenderer` package in React?

     This package provides a renderer that can be used to render components to pure JavaScript objects, without depending on the DOM or a native mobile environment. This package makes it easy to grab a snapshot of the platform view hierarchy (similar to a DOM tree) rendered by a ReactDOM or React Native without using a browser or `jsdom`.

     ```jsx harmony
     import TestRenderer from 'react-test-renderer'

     const Link = ({page, children}) => <a href={page}>{children}</a>

     const testRenderer = TestRenderer.create(
       <Link page={'https://www.facebook.com/'}>{'Facebook'}</Link>
     )

     console.log(testRenderer.toJSON())
     // {
     //   type: 'a',
     //   props: { href: 'https://www.facebook.com/' },
     //   children: [ 'Facebook' ]
     // }
     ```


   **[⬆ 返回顶部](#table-of-contents)**
    
148. ### What is the purpose of ReactTestUtils package?

     *ReactTestUtils* are provided in the `with-addons` package and allow you to perform actions against a simulated DOM for the purpose of unit testing.


   **[⬆ 返回顶部](#table-of-contents)**
    
149. ### What is Jest?

     *Jest* is a JavaScript unit testing framework created by Facebook based on Jasmine and provides automated mock creation and a `jsdom` environment. It's often used for testing components.


   **[⬆ 返回顶部](#table-of-contents)**
    
150. ### What are the advantages of Jest over Jasmine?

     There are couple of advantages compared to Jasmine:

     - Automatically finds tests to execute in your source code.
     - Automatically mocks dependencies when running your tests.
     - Allows you to test asynchronous code synchronously.
     - Runs your tests with a fake DOM implementation (via `jsdom`) so that your tests can be run on the command line.
     - Runs tests in parallel processes so that they finish sooner.


   **[⬆ 返回顶部](#table-of-contents)**
    
151. ### Give a simple example of Jest test case

     Let's write a test for a function that adds two numbers in `sum.js` file:

     ```javascript
     const sum = (a, b) => a + b

     export default sum
     ```

     Create a file named `sum.test.js` which contains actual test:

     ```javascript
     import sum from './sum'

     test('adds 1 + 2 to equal 3', () => {
       expect(sum(1, 2)).toBe(3)
     })
     ```

     And then add the following section to your `package.json`:

     ```json
     {
       "scripts": {
         "test": "jest"
       }
     }
     ```

     Finally, run `yarn test` or `npm test` and Jest will print a result:

     ```console
     $ yarn test
     PASS ./sum.test.js
     ✓ adds 1 + 2 to equal 3 (2ms)
     ```

## React Redux


   **[⬆ 返回顶部](#table-of-contents)**
    
152. ### What is flux?

     *Flux* is an *application design paradigm* used as a replacement for the more traditional MVC pattern. It is not a framework or a library but a new kind of architecture that complements React and the concept of Unidirectional Data Flow. Facebook uses this pattern internally when working with React.

     The workflow between dispatcher, stores and views components with distinct inputs and outputs as follows:

     ![flux](images/flux.png)


   **[⬆ 返回顶部](#table-of-contents)**
    
153. ### What is Redux?

     *Redux* is a predictable state container for JavaScript apps based on the *Flux design pattern*. Redux can be used together with React, or with any other view library. It is tiny (about 2kB) and has no dependencies.


   **[⬆ 返回顶部](#table-of-contents)**
    
154. ### What are the core principles of Redux?

     Redux follows three fundamental principles:

     1. **Single source of truth:** The state of your whole application is stored in an object tree within a single store. The single state tree makes it easier to keep track of changes over time and debug or inspect the application.
     2. **State is read-only:** The only way to change the state is to emit an action, an object describing what happened. This ensures that neither the views nor the network callbacks will ever write directly to the state.
     3. **Changes are made with pure functions:** To specify how the state tree is transformed by actions, you write reducers. Reducers are just pure functions that take the previous state and an action as parameters, and return the next state.


   **[⬆ 返回顶部](#table-of-contents)**
    
155. ### What are the downsides of Redux compared to Flux?

     Instead of saying downsides we can say that there are few compromises of using Redux over Flux. Those are as follows:

     1. **You will need to learn to avoid mutations:** Flux is un-opinionated about mutating data, but Redux doesn't like mutations and many packages complementary to Redux assume you never mutate the state. You can enforce this with dev-only packages like `redux-immutable-state-invariant`, Immutable.js, or instructing your team to write non-mutating code.
     2. **You're going to have to carefully pick your packages:** While Flux explicitly doesn't try to solve problems such as undo/redo, persistence, or forms, Redux has extension points such as middleware and store enhancers, and it has spawned a rich ecosystem.
     3. **There is no nice Flow integration yet:** Flux currently lets you do very impressive static type checks which Redux doesn't support yet.


   **[⬆ 返回顶部](#table-of-contents)**
    
156. ### What is the difference between `mapStateToProps()` and `mapDispatchToProps()`?

     `mapStateToProps()` is a utility which helps your component get updated state (which is updated by some other components):

     ```javascript
     const mapStateToProps = (state) => {
       return {
         todos: getVisibleTodos(state.todos, state.visibilityFilter)
       }
     }
     ```

     `mapDispatchToProps()` is a utility which will help your component to fire an action event (dispatching action which may cause change of application state):

     ```javascript
     const mapDispatchToProps = (dispatch) => {
       return {
         onTodoClick: (id) => {
           dispatch(toggleTodo(id))
         }
       }
     }
     ```
     
     It is recommended to always use the “object shorthand” form for the `mapDispatchToProps`.
        
     Redux wraps it in another function that looks like (…args) => dispatch(onTodoClick(…args)), and pass that wrapper function as a prop to your component.
      
      ```javascript
       const mapDispatchToProps = ({
         onTodoClick
       })
      ```


   **[⬆ 返回顶部](#table-of-contents)**
    
157. ### Can I dispatch an action in reducer?

     Dispatching an action within a reducer is an **anti-pattern**. Your reducer should be *without side effects*, simply digesting the action payload and returning a new state object. Adding listeners and dispatching actions within the reducer can lead to chained actions and other side effects.


   **[⬆ 返回顶部](#table-of-contents)**
    
158. ### How to access Redux store outside a component?

     You just need to export the store from the module where it created with `createStore()`. Also, it shouldn't pollute the global window object.

     ```javascript
     store = createStore(myReducer)

     export default store
     ```


   **[⬆ 返回顶部](#table-of-contents)**
    
159. ### What are the drawbacks of MVW pattern?

     1. DOM manipulation is very expensive which causes applications to behave slow and inefficient.
     3. Due to circular dependencies, a complicated model was created around models and views.
     3. Lot of data changes happens for collaborative applications(like Google Docs).
     4. No way to do undo (travel back in time) easily without adding so much extra code.


   **[⬆ 返回顶部](#table-of-contents)**
    
160. ### Are there any similarities between Redux and RxJS?

     These libraries are very different for very different purposes, but there are some vague similarities.

     Redux is a tool for managing state throughout the application. It is usually used as an architecture for UIs. Think of it as an alternative to (half of) Angular. RxJS is a reactive programming library. It is usually used as a tool to accomplish asynchronous tasks in JavaScript. Think of it as an alternative to Promises. Redux uses the Reactive paradigm because the Store is reactive. The Store observes actions from a distance, and changes itself. RxJS also uses the Reactive paradigm, but instead of being an architecture, it gives you basic building blocks, Observables, to accomplish this pattern.


   **[⬆ 返回顶部](#table-of-contents)**
    
161. ### How to dispatch an action on load?

     You can dispatch an action in `componentDidMount()` method and in `render()` method you can verify the data.

     ```javascript
     class App extends Component {
       componentDidMount() {
         this.props.fetchData()
       }

       render() {
         return this.props.isLoaded
           ? <div>{'Loaded'}</div>
           : <div>{'Not Loaded'}</div>
       }
     }

     const mapStateToProps = (state) => ({
       isLoaded: state.isLoaded
     })

     const mapDispatchToProps = { fetchData }

     export default connect(mapStateToProps, mapDispatchToProps)(App)
     ```


   **[⬆ 返回顶部](#table-of-contents)**
    
162. ### How to use `connect()` from React Redux?

     You need to follow two steps to use your store in your container:

     1. **Use `mapStateToProps()`:** It maps the state variables from your store to the props that you specify.
     2. **Connect the above props to your container:** The object returned by the `mapStateToProps` function is connected to the container. You can import `connect()` from `react-redux`.

         ```jsx harmony
         import React from 'react'
         import { connect } from 'react-redux'

         class App extends React.Component {
           render() {
             return <div>{this.props.containerData}</div>
           }
         }

         function mapStateToProps(state) {
           return { containerData: state.data }
         }

         export default connect(mapStateToProps)(App)
         ```


   **[⬆ 返回顶部](#table-of-contents)**
    
163. ### How to reset state in Redux?

     You need to write a *root reducer* in your application which delegate handling the action to the reducer generated by `combineReducers()`.

     For example, let us take `rootReducer()` to return the initial state after `USER_LOGOUT` action. As we know, reducers are supposed to return the initial state when they are called with `undefined` as the first argument, no matter the action.

     ```javascript
     const appReducer = combineReducers({
       /* your app's top-level reducers */
     })

     const rootReducer = (state, action) => {
       if (action.type === 'USER_LOGOUT') {
         state = undefined
       }

       return appReducer(state, action)
     }
     ```

     In case of using `redux-persist`, you may also need to clean your storage. `redux-persist` keeps a copy of your state in a storage engine. First, you need to import the appropriate storage engine and then, to parse the state before setting it to undefined and clean each storage state key.

     ```javascript
     const appReducer = combineReducers({
       /* your app's top-level reducers */
     })

     const rootReducer = (state, action) => {
       if (action.type === 'USER_LOGOUT') {
         Object.keys(state).forEach(key => {
           storage.removeItem(`persist:${key}`)
         })

         state = undefined
       }

       return appReducer(state, action)
     }
     ```


   **[⬆ 返回顶部](#table-of-contents)**
    
164. ### Whats the purpose of `at` symbol in the Redux connect decorator?

     The **@** symbol is in fact a JavaScript expression used to signify decorators. *Decorators* make it possible to annotate and modify classes and properties at design time.

     Let's take an example setting up Redux without and with a decorator.

     * **Without decorator:**

         ```javascript
         import React from 'react'
         import * as actionCreators from './actionCreators'
         import { bindActionCreators } from 'redux'
         import { connect } from 'react-redux'

         function mapStateToProps(state) {
           return { todos: state.todos }
         }

         function mapDispatchToProps(dispatch) {
           return { actions: bindActionCreators(actionCreators, dispatch) }
         }

         class MyApp extends React.Component {
           // ...define your main app here
         }

         export default connect(mapStateToProps, mapDispatchToProps)(MyApp)
         ```

     * **With decorator:**

         ```javascript
         import React from 'react'
         import * as actionCreators from './actionCreators'
         import { bindActionCreators } from 'redux'
         import { connect } from 'react-redux'

         function mapStateToProps(state) {
           return { todos: state.todos }
         }

         function mapDispatchToProps(dispatch) {
           return { actions: bindActionCreators(actionCreators, dispatch) }
         }

         @connect(mapStateToProps, mapDispatchToProps)
         export default class MyApp extends React.Component {
           // ...define your main app here
         }
         ```

     The above examples are almost similar except the usage of decorator. The decorator syntax isn't built into any JavaScript runtimes yet, and is still experimental and subject to change. You can use babel for the decorators support.


   **[⬆ 返回顶部](#table-of-contents)**
    
165. ### What is the difference between React context and React Redux?

     You can use **Context** in your application directly and is going to be great for passing down data to deeply nested components which what it was designed for.

     Whereas **Redux** is much more powerful and provides a large number of features that the Context API doesn't provide. Also, React Redux uses context internally but it doesn't expose this fact in the public API.


   **[⬆ 返回顶部](#table-of-contents)**
    
166. ### Why are Redux state functions called reducers?

     Reducers always return the accumulation of the state (based on all previous and current actions). Therefore, they act as a reducer of state. Each time a Redux reducer is called, the state and action are passed as parameters. This state is then reduced (or accumulated) based on the action, and then the next state is returned. You could *reduce* a collection of actions and an initial state (of the store) on which to perform these actions to get the resulting final state.


   **[⬆ 返回顶部](#table-of-contents)**
    
167. ### How to make AJAX request in Redux?

     You can use `redux-thunk` middleware which allows you to define async actions.

     Let's take an example of fetching specific account as an AJAX call using *fetch API*:

     ```javascript
     export function fetchAccount(id) {
       return dispatch => {
         dispatch(setLoadingAccountState()) // Show a loading spinner
         fetch(`/account/${id}`, (response) => {
           dispatch(doneFetchingAccount()) // Hide loading spinner
           if (response.status === 200) {
             dispatch(setAccount(response.json)) // Use a normal function to set the received state
           } else {
             dispatch(someError)
           }
         })
       }
     }

     function setAccount(data) {
      return { type: 'SET_Account', data: data }
     }
     ```


   **[⬆ 返回顶部](#table-of-contents)**
    
168. ### Should I keep all component's state in Redux store?

      Keep your data in the Redux store, and the UI related state internally in the component.


   **[⬆ 返回顶部](#table-of-contents)**
    
169. ### What is the proper way to access Redux store?

     The best way to access your store in a component is to use the `connect()` function, that creates a new component that wraps around your existing one. This pattern is called *Higher-Order Components*, and is generally the preferred way of extending a component's functionality in React. This allows you to map state and action creators to your component, and have them passed in automatically as your store updates.

     Let's take an example of `<FilterLink>` component using connect:

     ```javascript
     import { connect } from 'react-redux'
     import { setVisibilityFilter } from '../actions'
     import Link from '../components/Link'

     const mapStateToProps = (state, ownProps) => ({
       active: ownProps.filter === state.visibilityFilter
     })

     const mapDispatchToProps = (dispatch, ownProps) => ({
       onClick: () => dispatch(setVisibilityFilter(ownProps.filter))
     })

     const FilterLink = connect(
       mapStateToProps,
       mapDispatchToProps
     )(Link)

     export default FilterLink
     ```

     Due to it having quite a few performance optimizations and generally being less likely to cause bugs, the Redux developers almost always recommend using `connect()` over accessing the store directly (using context API).

     ```javascript
     class MyComponent {
       someMethod() {
         doSomethingWith(this.context.store)
       }
     }
     ```


   **[⬆ 返回顶部](#table-of-contents)**
    
170. ### What is the difference between component and container in React Redux?

     **Component** is a class or function component that describes the presentational part of your application.

     **Container** is an informal term for a component that is connected to a Redux store. Containers *subscribe* to Redux state updates and *dispatch* actions, and they usually don't render DOM elements; they delegate rendering to presentational child components.


   **[⬆ 返回顶部](#table-of-contents)**
    
171. ### What is the purpose of the constants in Redux?

     Constants allows you to easily find all usages of that specific functionality across the project when you use an IDE. It also prevents you from introducing silly bugs caused by typos – in which case, you will get a `ReferenceError` immediately.

     Normally we will save them in a single file (`constants.js` or `actionTypes.js`).

     ```javascript
     export const ADD_TODO = 'ADD_TODO'
     export const DELETE_TODO = 'DELETE_TODO'
     export const EDIT_TODO = 'EDIT_TODO'
     export const COMPLETE_TODO = 'COMPLETE_TODO'
     export const COMPLETE_ALL = 'COMPLETE_ALL'
     export const CLEAR_COMPLETED = 'CLEAR_COMPLETED'
     ```

     In Redux, you use them in two places:

     1. **During action creation:**

         Let's take `actions.js`:

         ```javascript
         import { ADD_TODO } from './actionTypes';

         export function addTodo(text) {
           return { type: ADD_TODO, text }
         }
         ```

     2. **In reducers:**

         Let's create `reducer.js`:

         ```javascript
         import { ADD_TODO } from './actionTypes'

         export default (state = [], action) => {
           switch (action.type) {
             case ADD_TODO:
               return [
                 ...state,
                 {
                   text: action.text,
                   completed: false
                 }
               ];
             default:
               return state
           }
         }
         ```


   **[⬆ 返回顶部](#table-of-contents)**
    
172. ### What are the different ways to write `mapDispatchToProps()`?

     There are a few ways of binding *action creators* to `dispatch()` in `mapDispatchToProps()`.

     Below are the possible options:

     ```javascript
     const mapDispatchToProps = (dispatch) => ({
      action: () => dispatch(action())
     })
     ```

     ```javascript
     const mapDispatchToProps = (dispatch) => ({
      action: bindActionCreators(action, dispatch)
     })
     ```

     ```javascript
     const mapDispatchToProps = { action }
     ```

     The third option is just a shorthand for the first one.


   **[⬆ 返回顶部](#table-of-contents)**
    
173. ### What is the use of the `ownProps` parameter in `mapStateToProps()` and `mapDispatchToProps()`?

     If the `ownProps` parameter is specified, React Redux will pass the props that were passed to the component into your *connect* functions. So, if you use a connected component:

     ```jsx harmony
     import ConnectedComponent from './containers/ConnectedComponent';

     <ConnectedComponent user={'john'} />
     ```

     The `ownProps` inside your `mapStateToProps()` and `mapDispatchToProps()` functions will be an object:

     ```javascript
     { user: 'john' }
     ```

     You can use this object to decide what to return from those functions.


   **[⬆ 返回顶部](#table-of-contents)**
    
174. ### How to structure Redux top level directories?

     Most of the applications has several top-level directories as below:

     1. **Components**: Used for *dumb* components unaware of Redux.
     2. **Containers**: Used for *smart* components connected to Redux.
     3. **Actions**: Used for all action creators, where file names correspond to part of the app.
     4. **Reducers**: Used for all reducers, where files name correspond to state key.
     5. **Store**: Used for store initialization.

     This structure works well for small and medium size apps.


   **[⬆ 返回顶部](#table-of-contents)**
    
175. ### What is redux-saga?

     `redux-saga` is a library that aims to make side effects (asynchronous things like data fetching and impure things like accessing the browser cache) in React/Redux applications easier and better.

     It is available in NPM:

     ```console
     $ npm install --save redux-saga
     ```


   **[⬆ 返回顶部](#table-of-contents)**
    
176. ### What is the mental model of redux-saga?

     *Saga* is like a separate thread in your application, that's solely responsible for side effects. `redux-saga` is a redux *middleware*, which means this thread can be started, paused and cancelled from the main application with normal Redux actions, it has access to the full Redux application state and it can dispatch Redux actions as well.


   **[⬆ 返回顶部](#table-of-contents)**
    
177. ### What are the differences between `call()` and `put()` in redux-saga?

     Both `call()` and `put()` are effect creator functions. `call()` function is used to create effect description, which instructs middleware to call the promise. `put()` function creates an effect, which instructs middleware to dispatch an action to the store.

     Let's take example of how these effects work for fetching particular user data.

     ```javascript
     function* fetchUserSaga(action) {
       // `call` function accepts rest arguments, which will be passed to `api.fetchUser` function.
       // Instructing middleware to call promise, it resolved value will be assigned to `userData` variable
       const userData = yield call(api.fetchUser, action.userId)

       // Instructing middleware to dispatch corresponding action.
       yield put({
         type: 'FETCH_USER_SUCCESS',
         userData
       })
     }
     ```


   **[⬆ 返回顶部](#table-of-contents)**
    
178. ### What is Redux Thunk?

     *Redux Thunk* middleware allows you to write action creators that return a function instead of an action. The thunk can be used to delay the dispatch of an action, or to dispatch only if a certain condition is met. The inner function receives the store methods `dispatch()` and `getState()` as parameters.


   **[⬆ 返回顶部](#table-of-contents)**
    
179. ### What are the differences between `redux-saga` and `redux-thunk`?

     Both *Redux Thunk* and *Redux Saga* take care of dealing with side effects. In most of the scenarios, Thunk uses *Promises* to deal with them, whereas Saga uses *Generators*. Thunk is simple to use and Promises are familiar to many developers, Sagas/Generators are more powerful but you will need to learn them. But both middleware can coexist, so you can start with Thunks and introduce Sagas when/if you need them.


   **[⬆ 返回顶部](#table-of-contents)**
    
180. ### What is Redux DevTools?

     *Redux DevTools* is a live-editing time travel environment for Redux with hot reloading, action replay, and customizable UI. If you don't want to bother with installing Redux DevTools and integrating it into your project, consider using Redux DevTools Extension for Chrome and Firefox.


   **[⬆ 返回顶部](#table-of-contents)**
    
181. ### What are the features of Redux DevTools?
     Some of the main features of Redux DevTools are below,

        1. Lets you inspect every state and action payload.
        2. Lets you go back in time by *cancelling* actions.
        3. If you change the reducer code, each *staged* action will be re-evaluated.
        4. If the reducers throw, you will see during which action this happened, and what the error was.
        5. With `persistState()` store enhancer, you can persist debug sessions across page reloads.


   **[⬆ 返回顶部](#table-of-contents)**
    
182. ### What are Redux selectors and why to use them?

     *Selectors* are functions that take Redux state as an argument and return some data to pass to the component.

     For example, to get user details from the state:

     ```javascript
     const getUserData = state => state.user.data
     ```

     These selectors have two main benefits,

     1. The selector can compute derived data, allowing Redux to store the minimal possible state
     2. The selector is not recomputed unless one of its arguments changes


   **[⬆ 返回顶部](#table-of-contents)**
    
183. ### What is Redux Form?

     *Redux Form* works with React and Redux to enable a form in React to use Redux to store all of its state. Redux Form can be used with raw HTML5 inputs, but it also works very well with common UI frameworks like Material UI, React Widgets and React Bootstrap.


   **[⬆ 返回顶部](#table-of-contents)**
    
184. ### What are the main features of Redux Form?
     Some of the main features of Redux Form are:

       1. Field values persistence via Redux store.
       2. Validation (sync/async) and submission.
       3. Formatting, parsing and normalization of field values.


   **[⬆ 返回顶部](#table-of-contents)**
    
185. ### How to add multiple middlewares to Redux?

     You can use `applyMiddleware()`.

     For example, you can add `redux-thunk` and `logger` passing them as arguments to `applyMiddleware()`:

     ```javascript
     import { createStore, applyMiddleware } from 'redux'
     const createStoreWithMiddleware = applyMiddleware(ReduxThunk, logger)(createStore)
     ```


   **[⬆ 返回顶部](#table-of-contents)**
    
186. ### How to set initial state in Redux?

     You need to pass initial state as second argument to createStore:

     ```javascript
     const rootReducer = combineReducers({
       todos: todos,
       visibilityFilter: visibilityFilter
     })

     const initialState = {
       todos: [{ id: 123, name: 'example', completed: false }]
     }

     const store = createStore(
       rootReducer,
       initialState
     )
     ```


   **[⬆ 返回顶部](#table-of-contents)**
    
187. ### How Relay is different from Redux?

     Relay is similar to Redux in that they both use a single store. The main difference is that relay only manages state originated from the server, and all access to the state is used via *GraphQL* queries (for reading data) and mutations (for changing data). Relay caches the data for you and optimizes data fetching for you, by fetching only changed data and nothing more.

188. ### What is an action in Redux?

     *Actions* are plain JavaScript objects or payloads of information that send data from your application to your store. They are the only source of information for the store. Actions must have a type property that indicates the type of action being performed.

     For example, let's take an action which represents adding a new todo item:

     ```
     {
       type: ADD_TODO,
       text: 'Add todo item'
     }
     ```


   **[⬆ 返回顶部](#table-of-contents)**

## React Native


   **[⬆ 返回顶部](#table-of-contents)**
    
188. ### What is the difference between React Native and React?

     **React** is a JavaScript library, supporting both front end web and being run on the server, for building user interfaces and web applications.

     **React Native** is a mobile framework that compiles to native app components, allowing you to build native mobile applications (iOS, Android, and Windows) in JavaScript that allows you to use React to build your components, and implements React under the hood.


   **[⬆ 返回顶部](#table-of-contents)**
    
189. ### How to test React Native apps?

     React Native can be tested only in mobile simulators like iOS and Android. You can run the app in your mobile using expo app (https://expo.io) Where it syncs using QR code, your mobile and computer should be in same wireless network.


   **[⬆ 返回顶部](#table-of-contents)**
    
190. ### How to do logging in React Native?

     You can use `console.log`, `console.warn`, etc. As of React Native v0.29 you can simply run the following to see logs in the console:

     ```
     $ react-native log-ios
     $ react-native log-android
     ```


   **[⬆ 返回顶部](#table-of-contents)**
    
191. ### How to debug your React Native?

     Follow the below steps to debug React Native app:

     1. Run your application in the iOS simulator.
     2. Press `Command + D` and a webpage should open up at `http://localhost:8081/debugger-ui`.
     3. Enable *Pause On Caught Exceptions* for a better debugging experience.
     4. Press `Command + Option + I` to open the Chrome Developer tools, or open it via `View` -> `Developer` -> `Developer Tools`.
     5. You should now be able to debug as you normally would.

## React supported libraries & Integration


   **[⬆ 返回顶部](#table-of-contents)**
    
192. ### What is reselect and how it works?

     *Reselect* is a **selector library** (for Redux) which uses *memoization* concept. It was originally written to compute derived data from Redux-like applications state, but it can't be tied to any architecture or library.

     Reselect keeps a copy of the last inputs/outputs of the last call, and recomputes the result only if one of the inputs changes. If the the same inputs are provided twice in a row, Reselect returns the cached output. It's memoization and cache are fully customizable.


   **[⬆ 返回顶部](#table-of-contents)**
    
193. ### What is Flow?

     *Flow* is a *static type checker* designed to find type errors in JavaScript. Flow types can express much more fine-grained distinctions than traditional type systems. For example, Flow helps you catch errors involving `null`, unlike most type systems.


   **[⬆ 返回顶部](#table-of-contents)**
    
194. ### What is the difference between Flow and PropTypes?

     Flow is a *static analysis tool* (static checker) which uses a superset of the language, allowing you to add type annotations to all of your code and catch an entire class of bugs at compile time.

     PropTypes is a *basic type checker* (runtime checker) which has been patched onto React. It can't check anything other than the types of the props being passed to a given component. If you want more flexible typechecking for your entire project Flow/TypeScript are appropriate choices.


   **[⬆ 返回顶部](#table-of-contents)**
    
195. ### How to use Font Awesome icons in React?

     The below steps followed to include Font Awesome in React:

     1. Install `font-awesome`:

         ```console
         $ npm install --save font-awesome
         ```

     2. Import `font-awesome` in your `index.js` file:

         ```javascript
         import 'font-awesome/css/font-awesome.min.css'
         ```

     3. Add Font Awesome classes in `className`:

         ```javascript
         render() {
           return <div><i className={'fa fa-spinner'} /></div>
         }
         ```


   **[⬆ 返回顶部](#table-of-contents)**
    
196. ### What is React Dev Tools?

     *React Developer Tools* let you inspect the component hierarchy, including component props and state. It exists both as a browser extension (for Chrome and Firefox), and as a standalone app (works with other environments including Safari, IE, and React Native).

     The official extensions available for different browsers or environments.
     1. **Chrome extension**
     2. **Firefox extension**
     3. **Standalone app** (Safari, React Native, etc)


   **[⬆ 返回顶部](#table-of-contents)**
    
197. ### Why is DevTools not loading in Chrome for local files?

     If you opened a local HTML file in your browser (`file://...`) then you must first open *Chrome Extensions* and check `Allow access to file URLs`.


   **[⬆ 返回顶部](#table-of-contents)**
    
198. ### How to use Polymer in React?
     You need to follow below steps to use Polymer in React,

     1. Create a Polymer element:

         ```jsx harmony
         <link rel='import' href='../../bower_components/polymer/polymer.html' />
         Polymer({
           is: 'calender-element',
           ready: function() {
             this.textContent = 'I am a calender'
           }
         })
         ```

     2. Create the Polymer component HTML tag by importing it in a HTML document, e.g. import it in the `index.html` of your React application:

         ```html
         <link rel='import' href='./src/polymer-components/calender-element.html'>
         ```

     3. Use that element in the JSX file:

         ```javascript
         import React from 'react'

         class MyComponent extends React.Component {
           render() {
             return (
               <calender-element />
             )
           }
         }

         export default MyComponent
         ```


   **[⬆ 返回顶部](#table-of-contents)**
    
199. ### What are the advantages of React over Vue.js?

     React has the following advantages over Vue.js:

     1. Gives more flexibility in large apps developing.
     2. Easier to test.
     3. Suitable for mobile apps creating.
     4. More information and solutions available.

   **Note:** The above list of advantages are purely opinionated and it vary based on the professional experience. But they are helpful as base parameters.

   **[⬆ 返回顶部](#table-of-contents)**
    
200. ### What is the difference between React and Angular?
     Let's see the difference between React and Angular in a table format.

     | React | Angular |
     | ----- | ------- |
     | React is a library and has only the View layer | Angular is a framework and has complete MVC functionality |
     | React handles rendering on the server side | AngularJS renders only on the client side but Angular 2 and above renders on the server side |
     | React uses JSX that looks like HTML in JS which can be confusing | Angular follows the template approach for HTML, which makes code shorter and easy to understand |
     | React Native, which is a React type to build mobile applications are faster and more stable | Ionic, Angular's mobile native app is relatively less stable and slower |
     | In React, data flows only in one way and hence debugging is easy | In Angular, data flows both way i.e it has two-way data binding between children and parent and hence debugging is often difficult |

   **Note:** The above list of differences are purely opinionated and it vary based on the professional experience. But they are helpful as base parameters.

   **[⬆ 返回顶部](#table-of-contents)**
    
201. ### Why React tab is not showing up in DevTools?

     When the page loads, *React DevTools* sets a global named `__REACT_DEVTOOLS_GLOBAL_HOOK__`, then React communicates with that hook during initialization. If the website is not using React or if React fails to communicate with DevTools then it won't show up the tab.


   **[⬆ 返回顶部](#table-of-contents)**
    
202. ### What are Styled Components?

     `styled-components` is a JavaScript library for styling React applications. It removes the mapping between styles and components, and lets you write actual CSS augmented with JavaScript.


   **[⬆ 返回顶部](#table-of-contents)**
    
203. ### Give an example of Styled Components?

     Lets create `<Title>` and `<Wrapper>` components with specific styles for each.

     ```javascript
     import React from 'react'
     import styled from 'styled-components'

     // Create a <Title> component that renders an <h1> which is centered, red and sized at 1.5em
     const Title = styled.h1`
       font-size: 1.5em;
       text-align: center;
       color: palevioletred;
     `

     // Create a <Wrapper> component that renders a <section> with some padding and a papayawhip background
     const Wrapper = styled.section`
       padding: 4em;
       background: papayawhip;
     `
     ```

     These two variables, `Title` and `Wrapper`, are now components that you can render just like any other react component.

     ```jsx harmony
     <Wrapper>
       <Title>{'Lets start first styled component!'}</Title>
     </Wrapper>
     ```


   **[⬆ 返回顶部](#table-of-contents)**
    
204. ### What is Relay?

     Relay is a JavaScript framework for providing a data layer and client-server communication to web applications using the React view layer.


   **[⬆ 返回顶部](#table-of-contents)**
    
205. ### How to use TypeScript in `create-react-app` application?
     Starting from react-scripts@2.1.0 or higher, there is a built-in support for typescript. i.e, `create-react-app` now supports typescript natively. You can just pass `--typescript` option as below
     ```bash
     npx create-react-app my-app --typescript

     # or

     yarn create react-app my-app --typescript
     ```
     But for lower versions of react scripts, just supply `--scripts-version` option as `react-scripts-ts` while you create a new project. `react-scripts-ts` is a set of adjustments to take the standard `create-react-app` project pipeline and bring TypeScript into the mix.

     Now the project layout should look like the following:

     ```
     my-app/
     ├─ .gitignore
     ├─ images.d.ts
     ├─ node_modules/
     ├─ public/
     ├─ src/
     │  └─ ...
     ├─ package.json
     ├─ tsconfig.json
     ├─ tsconfig.prod.json
     ├─ tsconfig.test.json
     └─ tslint.json
     ```

## Miscellaneous


   **[⬆ 返回顶部](#table-of-contents)**
    
206. ### What are the main features of Reselect library?

     Let's see the main features of Reselect library,

       1. Selectors can compute derived data, allowing Redux to store the minimal possible state.
       2. Selectors are efficient. A selector is not recomputed unless one of its arguments changes.
       3. Selectors are composable. They can be used as input to other selectors.

207. #### Give an example of Reselect usage?

     Let's take calculations and different amounts of a shipment order with the simplified usage of Reselect:

     ```javascript
     import { createSelector } from 'reselect'

     const shopItemsSelector = state => state.shop.items
     const taxPercentSelector = state => state.shop.taxPercent

     const subtotalSelector = createSelector(
       shopItemsSelector,
       items => items.reduce((acc, item) => acc + item.value, 0)
     )

     const taxSelector = createSelector(
       subtotalSelector,
       taxPercentSelector,
       (subtotal, taxPercent) => subtotal * (taxPercent / 100)
     )

     export const totalSelector = createSelector(
       subtotalSelector,
       taxSelector,
       (subtotal, tax) => ({ total: subtotal + tax })
     )

     let exampleState = {
       shop: {
         taxPercent: 8,
         items: [
           { name: 'apple', value: 1.20 },
           { name: 'orange', value: 0.95 },
         ]
       }
     }

     console.log(subtotalSelector(exampleState)) // 2.15
     console.log(taxSelector(exampleState))      // 0.172
     console.log(totalSelector(exampleState))    // { total: 2.322 }
     ```


   **[⬆ 返回顶部](#table-of-contents)**
    
209. ### Does the statics object work with ES6 classes in React?

     No, `statics` only works with `React.createClass()`:

     ```javascript
     someComponent= React.createClass({
       statics: {
         someMethod: function() {
           // ..
         }
       }
     })
     ```

     But you can write statics inside ES6+ classes as below,

     ```javascript
     class Component extends React.Component {
       static propTypes = {
         // ...
       }

       static someMethod() {
         // ...
       }
     }
     ```

     or writing them outside class as below,

     ```javascript
     class Component extends React.Component {
        ....
     }

     Component.propTypes = {...}
     Component.someMethod = function(){....}
     ```


   **[⬆ 返回顶部](#table-of-contents)**
    
210. ### Can Redux only be used with React?

     Redux can be used as a data store for any UI layer. The most common usage is with React and React Native, but there are bindings available for Angular, Angular 2, Vue, Mithril, and more. Redux simply provides a subscription mechanism which can be used by any other code.


   **[⬆ 返回顶部](#table-of-contents)**
    
211. ### Do you need to have a particular build tool to use Redux?

     Redux is originally written in ES6 and transpiled for production into ES5 with Webpack and Babel. You should be able to use it regardless of your JavaScript build process. Redux also offers a UMD build that can be used directly without any build process at all.


   **[⬆ 返回顶部](#table-of-contents)**
    
212. ### How Redux Form `initialValues` get updated from state?

     You need to add `enableReinitialize : true` setting.

     ```javascript
     const InitializeFromStateForm = reduxForm({
       form: 'initializeFromState',
       enableReinitialize : true
     })(UserEdit)
     ```

     If your `initialValues` prop gets updated, your form will update too.


   **[⬆ 返回顶部](#table-of-contents)**
    
213. ### How React PropTypes allow different types for one prop?

     You can use `oneOfType()` method of `PropTypes`.

     For example, the height property can be defined with either `string` or `number` type as below:

     ```javascript
     Component.propTypes = {
       size: PropTypes.oneOfType([
         PropTypes.string,
         PropTypes.number
       ])
     }
     ```


   **[⬆ 返回顶部](#table-of-contents)**
    
214. ### Can I import an SVG file as react component?

     You can import SVG directly as component instead of loading it as a file. This feature is available with `react-scripts@2.0.0` and higher.

     ```jsx harmony
     import { ReactComponent as Logo } from './logo.svg'

     const App = () => (
       <div>
         {/* Logo is an actual react component */}
         <Logo />
       </div>
     )
     ```

     **Note**: Don't forget about the curly braces in the import.


   **[⬆ 返回顶部](#table-of-contents)**
    
215. ### Why are inline ref callbacks or functions not recommended?

     If the ref callback is defined as an inline function, it will get called twice during updates, first with null and then again with the DOM element. This is because a new instance of the function is created with each render, so React needs to clear the old ref and set up the new one.

     ```jsx
     class UserForm extends Component {
       handleSubmit = () => {
         console.log("Input Value is: ", this.input.value)
       }


       render () {
        return (
          <form onSubmit={this.handleSubmit}>
            <input
              type='text'
              ref={(input) => this.input = input} /> // Access DOM input in handle submit
            <button type='submit'>Submit</button>
          </form>
        )
      }
     }
     ```

     But our expectation is for the ref callback to get called once, when the component mounts. One quick fix is to use the ES7 class property syntax to define the function

     ```jsx
     class UserForm extends Component {
      handleSubmit = () => {
        console.log("Input Value is: ", this.input.value)
      }

      setSearchInput = (input) => {
        this.input = input
      }

      render () {
        return (
          <form onSubmit={this.handleSubmit}>
            <input
              type='text'
              ref={this.setSearchInput} /> // Access DOM input in handle submit
            <button type='submit'>Submit</button>
          </form>
        )
      }
     }
     ```

    **Note:** In React v16.3,
   **[⬆ 返回顶部](#table-of-contents)**
    
216. ### What is render hijacking in react?

     The concept of render hijacking is the ability to control what a component will output from another component. It  means that you decorate your component by wrapping it into a Higher-Order component. By wrapping, you can inject additional props or make other changes, which can cause changing logic of rendering. It does not actually enable hijacking, but by using HOC you make your component behave differently.


   **[⬆ 返回顶部](#table-of-contents)**
    
217. ### What are HOC factory implementations?
     There are two main ways of implementing HOCs in React.

     1. Props Proxy (PP) and
     2. Inheritance Inversion (II).

     But they follow different approaches for manipulating the *WrappedComponent*.

     **Props Proxy**

     In this approach, the render method of the HOC returns a React Element of the type of the WrappedComponent. We also pass through the props that the HOC receives, hence the name **Props Proxy**.

     ```jsx

     function ppHOC(WrappedComponent) {
      return class PP extends React.Component {
        render() {
          return <WrappedComponent {...this.props}/>
        }
      }
     }
     ```
     **Inheritance Inversion**

     In this approach, the returned HOC class (Enhancer) extends the WrappedComponent. It is called Inheritance Inversion because instead of the WrappedComponent extending some Enhancer class, it is passively extended by the Enhancer. In this way the relationship between them seems **inverse**.

     ```jsx
     function iiHOC(WrappedComponent) {
      return class Enhancer extends WrappedComponent {
        render() {
          return super.render()
        }
      }
     }
     ```

   **[⬆ 返回顶部](#table-of-contents)**
    
218. ### How to pass numbers to React component?

     You should be passing the numbers via curly braces({}) where as strings in quotes

     ```jsx
        React.render(<User age={30} department={"IT"} />, document.getElementById('container'));
     ```

   **[⬆ 返回顶部](#table-of-contents)**
    
219. ### Do I need to keep all my state into Redux? Should I ever use react internal state?
     It is up to the developer's decision, i.e., it is developer's job to determine what kinds of state make up your application, and where each piece of state should live. Some users prefer to keep every single piece of data in Redux, to maintain a fully serializable and controlled version of their application at all times. Others prefer to keep non-critical or UI state, such as “is this dropdown currently open”, inside a component's internal state.

     Below are the thumb rules to determine what kind of data should be put into Redux
     1. Do other parts of the application care about this data?
     2. Do you need to be able to create further derived data based on this original data?
     3. Is the same data being used to drive multiple components?
     4. Is there value to you in being able to restore this state to a given point in time (ie, time travel debugging)?
     5. Do you want to cache the data (i.e, use what's in state if it's already there instead of re-requesting it)?


   **[⬆ 返回顶部](#table-of-contents)**
    
220. ### What is the purpose of registerServiceWorker in React?

     React creates a service worker for you without any configuration by default. The service worker is a web API that helps you cache your assets and other files so that when the user is offline or on a slow network, he/she can still see results on the screen, as such, it helps you build a better user experience, that's what you should know about service worker for now. It's all about adding offline capabilities to your site.

     ```jsx
        import React from 'react';
        import ReactDOM from 'react-dom';
        import App from './App';
        import registerServiceWorker from './registerServiceWorker';

        ReactDOM.render(<App />, document.getElementById('root'));
        registerServiceWorker();
     ```

   **[⬆ 返回顶部](#table-of-contents)**
    
221. ### What is React memo function?

     Class components can be restricted from re-rendering when their input props are the same using **PureComponent or shouldComponentUpdate**. Now you can do the same with function components by wrapping them in **React.memo**.
     ```jsx
     const MyComponent = React.memo(function MyComponent(props) {
      /* only rerenders if props change */
     });
     ```

   **[⬆ 返回顶部](#table-of-contents)**
    
222. ### What is React lazy function?
     The `React.lazy` function lets you render a dynamic import as a regular component. It will automatically load the bundle containing the `OtherComponent` when the component gets rendered. This must return a Promise which resolves to a module with a default export containing a React component.
     ```jsx
     const OtherComponent = React.lazy(() => import('./OtherComponent'));

     function MyComponent() {
      return (
        <div>
          <OtherComponent />
        </div>
      );
     }
     ```
     **Note:**
     `React.lazy` and `Suspense` is not yet available for server-side rendering. If you want to do code-splitting in a server rendered app, we still recommend React Loadable.

   **[⬆ 返回顶部](#table-of-contents)**
    
223. ### How to prevent unnecessary updates using setState?
     You can compare the current value of the state with an existing state value and decide whether to rerender the page or not. If the values are the same then you need to return **null** to stop re-rendering otherwise return the latest state value.

     For example, the user profile information is conditionally rendered as follows,
     ```jsx
     getUserProfile = user => {
       const latestAddress = user.address;
       this.setState(state => {
         if (state.address === latestAddress) {
           return null;
         } else {
           return { title: latestAddress };
         }
       });
     };
     ```

   **[⬆ 返回顶部](#table-of-contents)**
    
224. ### How do you render Array, Strings and Numbers in React 16 Version?
     **Arrays**: Unlike older releases, you don't need to make sure **render** method return a single element in React16. You are able to return multiple sibling elements without a wrapping element by returning an array.

     For example, let us take the below list of developers,

     ```jsx
     const ReactJSDevs = () => {
       return [
         <li key="1">John</li>,
         <li key="2">Jackie</li>,
         <li key="3">Jordan</li>
       ];
     }
     ```
     You can also merge this array of items in another array component.
     ```jsx
     const JSDevs = () => {
       return (
         <ul>
           <li>Brad</li>
           <li>Brodge</li>
           <ReactJSDevs/>
           <li>Brandon</li>
         </ul>
       );
     }
     ```
     **Strings and Numbers:** You can also return string and number type from the render method.

     ```jsx
     render() {
      return 'Welcome to ReactJS questions';
     }
     // Number
     render() {
      return 2018;
     }
     ```

   **[⬆ 返回顶部](#table-of-contents)**
    
225. ### How to use class field declarations syntax in React classes?
     React Class Components can be made much more concise using the class field declarations. You can initialize the local state without using the constructor and declare class methods by using arrow functions without the extra need to bind them.

     Let's take a counter example to demonstrate class field declarations for state without using constructor and methods without binding,
     ```jsx
     class Counter extends Component {
       state = { value: 0 };

       handleIncrement = () => {
         this.setState(prevState => ({
           value: prevState.value + 1
         }));
       };

       handleDecrement = () => {
         this.setState(prevState => ({
           value: prevState.value - 1
         }));
       };

       render() {
         return (
           <div>
             {this.state.value}

             <button onClick={this.handleIncrement}>+</button>
             <button onClick={this.handleDecrement}>-</button>
           </div>
         )
       }
     }
     ```

   **[⬆ 返回顶部](#table-of-contents)**
    
226. ### What are hooks?
     Hooks is a special function (introduced as a new feature in React 16.8) that lets you use state and other React features without writing a class.

     Let's see an example of useState hook:
     ```jsx
     import { useState } from 'react';

     function Example() {
       // Declare a new state variable, which we'll call "count"
       const [count, setCount] = useState(0);

       return (
         <div>
           <p>You clicked {count} times</p>
           <button onClick={() => setCount(count + 1)}>
             Click me
           </button>
         </div>
       );
     }
     ```
     **Note:** Hooks can be used inside an existing function component.

   **[⬆ 返回顶部](#table-of-contents)**
    
227. ### What rules need to be followed for hooks?

     You need to follow two rules in order to use hooks,

     1. Call Hooks only at the top level of your react functions. i.e, You shouldn’t call Hooks inside loops, conditions, or nested functions. This will ensure that Hooks are called in the same order each time a component renders and it preserves the state of Hooks between multiple useState and useEffect calls.
     2. Call Hooks from React Functions only. i.e, You shouldn’t call Hooks from regular JavaScript functions.


   **[⬆ 返回顶部](#table-of-contents)**
    
228. ### How to ensure hooks followed the rules in your project?
     React team released an ESLint plugin called **eslint-plugin-react-hooks** that enforces these two rules. You can add this plugin to your project using the below command,
     ```javascript
     npm install eslint-plugin-react-hooks@next
     ```
     And apply the below config in your ESLint config file,
     ```javascript
     // Your ESLint configuration
     {
       "plugins": [
         // ...
         "react-hooks"
       ],
       "rules": {
         // ...
         "react-hooks/rules-of-hooks": "error"
       }
     }
     ```
     **Note:** This plugin is intended to use in Create React App by default.


   **[⬆ 返回顶部](#table-of-contents)**
    
229. ### What are the differences between Flux and Redux?
     Below are the major differences between Flux and Redux

     | Flux | Redux |
     | ----- | ------- |
     | State is mutable | State is immutable |
     | The Store contains both state and change logic | The Store and change logic are separate |
     | There are multiple stores exist | There is only one store exist |
     | All the stores are disconnected and flat | Single store with hierarchical reducers|
     | It has a singleton dispatcher | There is no concept of dispatcher |
     | React components subscribe to the store | Container components uses connect function|

   **[⬆ 返回顶部](#table-of-contents)**
    
230. ### What are the benefits of React Router V4?
     Below are the main benefits of React Router V4 module,

     1. In React Router v4(version 4), the API is completely about components. A router can be visualized as a single component(`<BrowserRouter>`) which wraps specific child router components(`<Route>`).
     2. You don't need to manually set history. The router module will take care history by wrapping routes with  `<BrowserRouter>` component.
     3. The application size is reduced by adding only the specific router module(Web, core, or native)

   **[⬆ 返回顶部](#table-of-contents)**
    
231. ### Can you describe about componentDidCatch lifecycle method signature?
     The **componentDidCatch** lifecycle method is invoked after an error has been thrown by a descendant component. The method receives two parameters,
     1. error: - The error object which was thrown
     2. info: - An object with a componentStack key contains the information about which component threw the error.

     The method structure would be as follows
     ```javascript
     componentDidCatch(error, info)
     ```

   **[⬆ 返回顶部](#table-of-contents)**
    
232. ### In which scenarios error boundaries do not catch errors?
     Below are the cases in which error boundaries doesn't work,

     1. Inside Event handlers
     2. Asynchronous code using **setTimeout or requestAnimationFrame** callbacks
     3. During Server side rendering
     4. When errors thrown in the error boundary code itself

   **[⬆ 返回顶部](#table-of-contents)**
    
233. ### Why do you not need error boundaries for event handlers?
     Error boundaries do not catch errors inside event handlers.
     
     React doesn’t need error boundaries to recover from errors in event handlers. Unlike the render method and lifecycle methods, the event handlers don’t happen during rendering. So if they throw, React still knows what to display on the screen.

     If you need to catch an error inside an event handler, use the regular JavaScript try / catch statement:

     ```javascript
     class MyComponent extends React.Component {
       constructor(props) {
         super(props);
         this.state = { error: null };
         this.handleClick = this.handleClick.bind(this);
       }

       handleClick() {
         try {
           // Do something that could throw
         } catch (error) {
           this.setState({ error });
         }
       }

       render() {
         if (this.state.error) {
           return <h1>Caught an error.</h1>
         }
         return <button onClick={this.handleClick}>Click Me</button>
       }
     }
     ```
     Note that the above example is demonstrating regular JavaScript behavior and doesn’t use error boundaries.

   **[⬆ 返回顶部](#table-of-contents)**
    
234. ### What is the difference between try catch block and error boundaries?
     Try catch block works with imperative code whereas error boundaries are meant for declarative code to render on the screen.

     For example, the try catch block used for below imperative code
     ```javascript
     try {
       showButton();
     } catch (error) {
       // ...
     }
     ```
     Whereas error boundaries wrap declarative code as below,
     ```javascript
     <ErrorBoundary>
       <MyComponent />
     </ErrorBoundary>
     ```
     So if an error occurs in a **componentDidUpdate** method caused by a **setState** somewhere deep in the tree, it will still correctly propagate to the closest error boundary.


   **[⬆ 返回顶部](#table-of-contents)**
    
235. ### What is the behavior of uncaught errors in react 16?
     In React 16, errors that were not caught by any error boundary will result in unmounting of the whole React component tree. The reason behind this decision is that it is worse to leave corrupted UI in place than to completely remove it. For example, it is worse for a payments app to display a wrong amount than to render nothing.

   **[⬆ 返回顶部](#table-of-contents)**
    
236. ### What is the proper placement for error boundaries?
     The granularity of error boundaries usage is up to the developer based on project needs. You can follow either of these approaches,
     1. You can wrap top-level route components to display a generic error message for the entire application.
     2. You can also wrap individual components in an error boundary to protect them from crashing the rest of the application.

   **[⬆ 返回顶部](#table-of-contents)**
    
237. ### What is the benefit of component stack trace from error boundary?
     Apart from error messages and javascript stack, React16 will display the component stack trace with file names and line numbers using error boundary concept.

     For example, BuggyCounter component displays the component stack trace as below,

     ![stacktrace](images/error_boundary.png)


   **[⬆ 返回顶部](#table-of-contents)**
    
238. ### What is the required method to be defined for a class component?
     The `render()` method is the only required method in a class component. i.e, All methods other than render method are optional for a class component.

   **[⬆ 返回顶部](#table-of-contents)**
    
239. ### What are the possible return types of render method?
     Below are the list of following types used and return from render method,

     1. **React elements:** Elements that instruct React to render a DOM node. It includes html elements such as `<div/>` and user defined elements.
     2. **Arrays and fragments:** Return multiple elements to render as Arrays and Fragments to wrap multiple elements
     3. **Portals:** Render children into a different DOM subtree.
     4. **String and numbers:** Render both Strings and Numbers as text nodes in the DOM
     5. **Booleans or null:** Doesn't render anything but these types are used to conditionally render content.


   **[⬆ 返回顶部](#table-of-contents)**
    
240. ### What is the main purpose of constructor?
     The constructor is mainly used for two purposes,

     1. To initialize local state by assigning object to this.state
     2. For binding event handler methods to the instance
     For example, the below code covers both the above cases,
     ```javascript
     constructor(props) {
       super(props);
       // Don't call this.setState() here!
       this.state = { counter: 0 };
       this.handleClick = this.handleClick.bind(this);
     }
     ```

   **[⬆ 返回顶部](#table-of-contents)**
    
241. ### Is it mandatory to define constructor for React component?
     No, it is not mandatory. i.e, If you don’t initialize state and you don’t bind methods, you don’t need to implement a constructor for your React component.

   **[⬆ 返回顶部](#table-of-contents)**
    
242. ### What are default props?
     The defaultProps are defined as a property on the component class to set the default props for the class. This is used for undefined props, but not for null props.

     For example, let us create color default prop for the button component,

     ```javascript
     class MyButton extends React.Component {
       // ...
     }

     MyButton.defaultProps = {
       color: 'red'
     };

     ```

     If `props.color` is not provided then it will set the default value to 'red'. i.e, Whenever you try to access the color prop it uses default value
     ```javascript
     render() {
        return <MyButton /> ; // props.color will be set to red
      }
     ```
     **Note:** If you provide null value then it remains null value.

   **[⬆ 返回顶部](#table-of-contents)**
    
243. ### Why should not call setState in componentWillUnmount?
     You should not call `setState()` in `componentWillUnmount()` because once a component instance is unmounted, it will never be mounted again.

   **[⬆ 返回顶部](#table-of-contents)**
    
244. ### What is the purpose of getDerivedStateFromError?
     This lifecycle method is invoked after an error has been thrown by a descendant component. It receives the error that was thrown as a parameter and should return a value to update state.

     The signature of the lifecycle method is as follows,
     ```javascript
     static getDerivedStateFromError(error)
     ```
     Let us take error boundary use case with the above lifecycle method for demonstration purpose,
     ```javascript
     class ErrorBoundary extends React.Component {
       constructor(props) {
         super(props);
         this.state = { hasError: false };
       }

       static getDerivedStateFromError(error) {
         // Update state so the next render will show the fallback UI.
         return { hasError: true };
       }

       render() {
         if (this.state.hasError) {
           // You can render any custom fallback UI
           return <h1>Something went wrong.</h1>;
         }

         return this.props.children;
       }
     }
     ```

   **[⬆ 返回顶部](#table-of-contents)**
    
245. ### What is the methods order when component re-rendered?
     An update can be caused by changes to props or state. The below methods are called in the following order when a component is being re-rendered.

     1. static getDerivedStateFromProps()
     2. shouldComponentUpdate()
     3. render()
     4. getSnapshotBeforeUpdate()
     5. componentDidUpdate()


   **[⬆ 返回顶部](#table-of-contents)**
    
246. ### What are the methods invoked during error handling?
     Below methods are called when there is an error during rendering, in a lifecycle method, or in the constructor of any child component.

     1. static getDerivedStateFromError()
     2. componentDidCatch()

   **[⬆ 返回顶部](#table-of-contents)**
    
247. ### What is the purpose of displayName class property?
     The displayName string is used in debugging messages. Usually, you don’t need to set it explicitly because it’s inferred from the name of the function or class that defines the component. You might want to set it explicitly if you want to display a different name for debugging purposes or when you create a higher-order component.

     For example, To ease debugging, choose a display name that communicates that it’s the result of a withSubscription HOC.

     ```javascript
     function withSubscription(WrappedComponent) {
       class WithSubscription extends React.Component {/* ... */}
       WithSubscription.displayName = `WithSubscription(${getDisplayName(WrappedComponent)})`;
       return WithSubscription;
     }
     function getDisplayName(WrappedComponent) {
       return WrappedComponent.displayName || WrappedComponent.name || 'Component';
     }
     ```

   **[⬆ 返回顶部](#table-of-contents)**
    
248. ### What is the browser support for react applications?
     React supports all popular browsers, including Internet Explorer 9 and above, although some polyfills are required for older browsers such as IE 9 and IE 10. If you use  **es5-shim and es5-sham** polyfill then it even support old browsers that doesn't support ES5 methods.

   **[⬆ 返回顶部](#table-of-contents)**
    
249. ### What is the purpose of unmountComponentAtNode method?
     This method is available from react-dom package and it removes a mounted React component from the DOM and clean up its event handlers and state. If no component was mounted in the container, calling this function does nothing. Returns true if a component was unmounted and false if there was no component to unmount.

     The method signature would be as follows,
     ```javascript
     ReactDOM.unmountComponentAtNode(container)
     ```

   **[⬆ 返回顶部](#table-of-contents)**
    
250. ### What is code-splitting?
     Code-Splitting is a feature supported by bundlers like Webpack and Browserify which can create multiple bundles that can be dynamically loaded at runtime. The react project supports code splitting via dynamic import() feature.

     For example, in the below code snippets, it will make moduleA.js and all its unique dependencies as a separate chunk that only loads after the user clicks the 'Load' button.
     **moduleA.js**
     ```javascript
     const moduleA = 'Hello';

     export { moduleA };
     ```
     **App.js**
     ```javascript
     import React, { Component } from 'react';

     class App extends Component {
       handleClick = () => {
         import('./moduleA')
           .then(({ moduleA }) => {
             // Use moduleA
           })
           .catch(err => {
             // Handle failure
           });
       };

       render() {
         return (
           <div>
             <button onClick={this.handleClick}>Load</button>
           </div>
         );
       }
     }

     export default App;

     ```

   **[⬆ 返回顶部](#table-of-contents)**
    
251. ### What is the benefit of strict mode?
     The <StrictMode> will be  helpful in the below cases

     1. Identifying components with **unsafe lifecycle methods**.
     2. Warning about **legacy string ref** API usage.
     3. Detecting unexpected **side effects**.
     4. Detecting **legacy context** API.
     5. Warning about deprecated findDOMNode usage

   **[⬆ 返回顶部](#table-of-contents)**
    
252. ### What are Keyed Fragments?
     The Fragments declared with the explicit <React.Fragment> syntax may have keys. The general use case is mapping a collection to an array of fragments as below,

     ```javascript
     function Glossary(props) {
       return (
         <dl>
           {props.items.map(item => (
             // Without the `key`, React will fire a key warning
             <React.Fragment key={item.id}>
               <dt>{item.term}</dt>
               <dd>{item.description}</dd>
             </React.Fragment>
           ))}
         </dl>
       );
     }
     ```

     **Note:** key is the only attribute that can be passed to Fragment. In the future, there might be a support for additional attributes, such as event handlers.

   **[⬆ 返回顶部](#table-of-contents)**
    
253. ### Does React support all HTML attributes?
     As of React 16, both standard or custom DOM attributes are fully supported. Since React components often take both custom and DOM-related props, React uses the camelCase convention just like the DOM APIs.

     Let us take few props with respect to standard HTML attributes,

     ```javascript
     <div tabIndex="-1" />      // Just like node.tabIndex DOM API
     <div className="Button" /> // Just like node.className DOM API
     <input readOnly={true} />  // Just like node.readOnly DOM API
     ```
     These props work similarly to the corresponding HTML attributes, with the exception of the special cases. It also support all SVG attributes.

   **[⬆ 返回顶部](#table-of-contents)**
    
254. ### What are the limitations with HOCs?

     Higher-order components come with a few caveats apart from its benefits. Below are the few listed in an order,
     1. **Don’t use HOCs inside the render method:**
        It is not recommended to apply a HOC to a component within the render method of a component.
        ```javascript
        render() {
          // A new version of EnhancedComponent is created on every render
          // EnhancedComponent1 !== EnhancedComponent2
          const EnhancedComponent = enhance(MyComponent);
          // That causes the entire subtree to unmount/remount each time!
          return <EnhancedComponent />;
        }
        ```
        The above code impacts on performance by remounting a component that causes the state of that component and all of its children to be lost. Instead, apply HOCs outside the component definition so that the resulting component is created only once.

     2. **Static methods must be copied over:**
        When you apply a HOC to a component the new component does not have any of the static methods of the original component
        ```javascript
        // Define a static method
        WrappedComponent.staticMethod = function() {/*...*/}
        // Now apply a HOC
        const EnhancedComponent = enhance(WrappedComponent);

        // The enhanced component has no static method
        typeof EnhancedComponent.staticMethod === 'undefined' // true
        ```
        You can overcome this by copying the methods onto the container before returning it,

        ```javascript
        function enhance(WrappedComponent) {
          class Enhance extends React.Component {/*...*/}
          // Must know exactly which method(s) to copy :(
          Enhance.staticMethod = WrappedComponent.staticMethod;
          return Enhance;
        }
        ```
     3. **Refs aren’t passed through:**
        For HOCs you need to pass through all props to the wrapped component but this does not work for refs. This is because ref is not really a prop similar to key. In this case you need to use the React.forwardRef API

   **[⬆ 返回顶部](#table-of-contents)**
    
255. ### How to debug forwardRefs in DevTools?

     **React.forwardRef** accepts a render function as parameter and DevTools uses this function to determine what to display for the ref forwarding component.

     For example, If you don't name the render function or not using displayName property then it will appear as ”ForwardRef” in the DevTools,

     ```javascript
     const WrappedComponent = React.forwardRef((props, ref) => {
       return <LogProps {...props} forwardedRef={ref} />;
     });
     ```

     But If you name the render function then it will appear as **”ForwardRef(myFunction)”**

     ```javascript
     const WrappedComponent = React.forwardRef(
       function myFunction(props, ref) {
         return <LogProps {...props} forwardedRef={ref} />;
       }
     );
     ```

     As an alternative, You can also set displayName property for forwardRef function,

     ```javascript
     function logProps(Component) {
       class LogProps extends React.Component {
         // ...
       }

       function forwardRef(props, ref) {
         return <LogProps {...props} forwardedRef={ref} />;
       }

       // Give this component a more helpful display name in DevTools.
       // e.g. "ForwardRef(logProps(MyComponent))"
       const name = Component.displayName || Component.name;
       forwardRef.displayName = `logProps(${name})`;

       return React.forwardRef(forwardRef);
     }
     ```

   **[⬆ 返回顶部](#table-of-contents)**
    
256. ### When component props defaults to true?
     If you pass no value for a prop, it defaults to true. This behavior is available so that it matches the behavior of HTML.

     For example, below expressions are equivalent,

     ```javascript
     <MyInput autocomplete />

     <MyInput autocomplete={true} />
     ```
     **Note:** It is not recommended to use this approach because it can be confused with the ES6 object shorthand (example, `{name}` which is short for `{name: name}`)

   **[⬆ 返回顶部](#table-of-contents)**
    
257. ### What is NextJS and major features of it?
     Next.js is a popular and lightweight framework for static and server‑rendered applications built with React. It also provides styling and routing solutions. Below are the major features provided by NextJS,

     1. Server-rendered by default
     2. Automatic code splitting for faster page loads
     3. Simple client-side routing (page based)
     4. Webpack-based dev environment which supports (HMR)
     5. Able to implement with Express or any other Node.js HTTP server
     6. Customizable with your own Babel and Webpack configurations

   **[⬆ 返回顶部](#table-of-contents)**
    
258. ### How do you pass an event handler to a component?
     You can pass event handlers and other functions as props to child components. It can be used in child component as  below,

     ```html
     <button onClick={this.handleClick}>
     ```

   **[⬆ 返回顶部](#table-of-contents)**
    
259. ### Is it good to use arrow functions in render methods?
     Yes, You can use. It is often the easiest way to pass parameters to callback functions. But you need to optimize the performance while using it.

     ```javascript
     class Foo extends Component {
       handleClick() {
         console.log('Click happened');
       }
       render() {
         return <button onClick={() => this.handleClick()}>Click Me</button>;
       }
     }
     ```

     **Note:** Using an arrow function in render method creates a new function each time the component renders, which may have performance implications

   **[⬆ 返回顶部](#table-of-contents)**
    
260. ### How to prevent a function from being called multiple times?
     If you use an event handler such as **onClick or onScroll** and want to prevent the callback from being fired too quickly, then you can limit the rate at which callback is executed. This can be achieved in the below possible ways,

     1. **Throttling:** Changes based on a time based frequency. For example, it can be used using _.throttle lodash function
     2. **Debouncing:** Publish changes after a period of inactivity. For example, it can be used using _.debounce lodash function
     3. **RequestAnimationFrame throttling:** Changes based on requestAnimationFrame. For example, it can be used using raf-schd lodash function

   **[⬆ 返回顶部](#table-of-contents)**
    
261. ### How JSX prevents Injection Attacks?
     React DOM escapes any values embedded in JSX before rendering them. Thus it ensures that you can never inject anything that’s not explicitly written in your application. Everything is converted to a string before being rendered.

     For example, you can embed user input as below,

     ```javascript
     const name = response.potentiallyMaliciousInput;
     const element = <h1>{name}</h1>;
     ```
     This way you can prevent XSS(Cross-site-scripting) attacks in the application.

   **[⬆ 返回顶部](#table-of-contents)**
    
262. ### How do you update rendered elements?
     You can update UI(represented by rendered element) by passing the newly created element to ReactDOM's render method.

     For example, lets take a ticking clock example, where it updates the time by calling render method multiple times,

     ```javascript
     function tick() {
       const element = (
         <div>
           <h1>Hello, world!</h1>
           <h2>It is {new Date().toLocaleTimeString()}.</h2>
         </div>
       );
       ReactDOM.render(element, document.getElementById('root'));
     }

     setInterval(tick, 1000);
     ```

   **[⬆ 返回顶部](#table-of-contents)**
    
263. ### How do you say that props are readonly?
     When you declare a component as a function or a class, it must never modify its own props.

     Let us take a below capital function,

     ```javascript
     function capital(amount, interest) {
        return amount + interest;
     }
     ```
     The above function is called “pure” because it does not attempt to change their inputs, and always return the same result for the same inputs. Hence, React has a single rule saying "All React components must act like pure functions with respect to their props."

   **[⬆ 返回顶部](#table-of-contents)**
    
264. ### How do you say that state updates are merged?
     When you call setState() in the component, React merges the object you provide into the current state.

     For example, let us take a facebook user with posts and comments details as state variables,

     ```javascript
       constructor(props) {
         super(props);
         this.state = {
           posts: [],
           comments: []
         };
       }
     ```

     Now you can update them independently with separate `setState()` calls as below,

     ```javascript
      componentDidMount() {
         fetchPosts().then(response => {
           this.setState({
             posts: response.posts
           });
         });

         fetchComments().then(response => {
           this.setState({
             comments: response.comments
           });
         });
       }
     ```
     As mentioned in the above code snippets, `this.setState({comments})` updates only comments variable without modifying or replacing `posts` variable.

   **[⬆ 返回顶部](#table-of-contents)**
    
265. ### How do you pass arguments to an event handler?
     During iterations or loops, it is common to pass an extra parameter to an event handler. This can be achieved through arrow functions or bind method.

     Let us take an example of user details updated in a grid,

     ```javascript
     <button onClick={(e) => this.updateUser(userId, e)}>Update User details</button>
     <button onClick={this.updateUser.bind(this, userId)}>Update User details</button>
     ```
     In the both approaches, the synthetic argument `e` is passed as a second argument. You need to pass it explicitly for arrow functions and it will be passed automatically for `bind` method.

   **[⬆ 返回顶部](#table-of-contents)**
    
266. ### How to prevent component from rendering?
     You can prevent component from rendering by returning null based on specific condition. This way it can conditionally render component.

     ```javascript
     function Greeting(props) {
       if (!props.loggedIn) {
         return null;
       }

       return (
         <div className="greeting">
           welcome, {props.name}
         </div>
       );
     }
     ```
     ```javascript
     class User extends React.Component {
       constructor(props) {
         super(props);
         this.state = {loggedIn: false, name: 'John'};
       }

       render() {
        return (
            <div>
              //Prevent component render if it is not loggedIn
              <Greeting loggedIn={this.state.loggedIn} />
              <UserDetails name={this.state.name}>
            </div>
        );
       }
     ```
     In the above example, the `greeting` component skips its rendering section by applying condition and returning null value.

   **[⬆ 返回顶部](#table-of-contents)**
    
267. ### What are the conditions to safely use the index as a key?
     There are three conditions to make sure, it is safe use the index as a key.

     1. The list and items are static– they are not computed and do not change
     2. The items in the list have no ids
     3. The list is never reordered or filtered.


   **[⬆ 返回顶部](#table-of-contents)**
    
268. ### Should keys be globally unique?
     The keys used within arrays should be unique among their siblings but they don’t need to be globally unique. i.e, You can use the same keys with two different arrays.

     For example, the below `Book` component uses two arrays with different arrays,

     ```javascript
     function Book(props) {
       const index = (
         <ul>
           {props.pages.map((page) =>
             <li key={page.id}>
               {page.title}
             </li>
           )}
         </ul>
       );
       const content = props.pages.map((page) =>
         <div key={page.id}>
           <h3>{page.title}</h3>
           <p>{page.content}</p>
           <p>{page.pageNumber}</p>
         </div>
       );
       return (
         <div>
           {index}
           <hr />
           {content}
         </div>
       );
     }
     ```

   **[⬆ 返回顶部](#table-of-contents)**
    
269. ### What is the popular choice for form handling?
     `Formik` is a form library for react which provides solutions such as validation, keeping track of the visited fields, and handling form submission.

     In detail, You can categorize them as follows,

     1. Getting values in and out of form state
     2. Validation and error messages
     3. Handling form submission

     It is used to create a scalable, performant, form helper with a minimal API to solve annoying stuff.

   **[⬆ 返回顶部](#table-of-contents)**
    
270. ### What are the advantages of formik over redux form library?
     Below are the main reasons to recommend formik over redux form library,

     1. The form state is inherently short-term and local, so tracking it in Redux (or any kind of Flux library) is unnecessary.
     2. Redux-Form calls your entire top-level Redux reducer multiple times ON EVERY SINGLE KEYSTROKE. This way it increases input latency for large apps.
     3. Redux-Form is 22.5 kB minified gzipped whereas Formik is 12.7 kB


   **[⬆ 返回顶部](#table-of-contents)**
    
271. ### Why are you not required to use inheritance?
     In React, it is recommended to use composition over inheritance to reuse code between components. Both Props and composition give you all the flexibility you need to customize a component’s look and behavior explicitly and safely.
     Whereas, If you want to reuse non-UI functionality between components, it is suggested to extract it into a separate JavaScript module. Later components import it and use that function, object, or class, without extending it.

   **[⬆ 返回顶部](#table-of-contents)**
    
272. ### Can I use web components in react application?
     Yes, you can use web components in a react application. Even though many developers won't use this combination, it may require especially if you are using third-party UI components that are written using Web Components.

     For example, let us use `Vaadin` date picker web component as below,

     ```javascript
     import React, { Component } from 'react';
     import './App.css';
     import '@vaadin/vaadin-date-picker';
     class App extends Component {
       render() {
         return (
           <div className="App">
             <vaadin-date-picker label="When were you born?"></vaadin-date-picker>
           </div>
         );
       }
     }
     export default App;
     ```

   **[⬆ 返回顶部](#table-of-contents)**
    
273. ### What is dynamic import?
     You can achieve code-splitting in your app using dynamic import.

     Let's take an example of addition,

     1. **Normal Import**
     ```javascript
     import { add } from './math';
     console.log(add(10, 20));
     ```
     2. **Dynamic Import**
     ```javascript
     import("./math").then(math => {
       console.log(math.add(10, 20));
     });
     ```

   **[⬆ 返回顶部](#table-of-contents)**
    
274. ### What are loadable components?
     If you want to do code-splitting in a server rendered app, it is recommend to use Loadable Components because React.lazy and Suspense is not yet available for server-side rendering. Loadable lets you render a dynamic import as a regular component.

     Lets take an example,

     ```javascript
     import loadable from '@loadable/component'

     const OtherComponent = loadable(() => import('./OtherComponent'))

     function MyComponent() {
       return (
         <div>
           <OtherComponent />
         </div>
       )
     }
     ```
     Now OtherComponent will be loaded in a separated bundle

   **[⬆ 返回顶部](#table-of-contents)**
    
275. ### What is suspense component?
     If the module containing the dynamic import is not yet loaded by the time parent component renders, you must show some fallback content while you’re waiting for it to load using a loading indicator. This can be done using **Suspense** component.

     For example, the below code uses suspense component,

     ```javascript
     const OtherComponent = React.lazy(() => import('./OtherComponent'));

     function MyComponent() {
       return (
         <div>
           <Suspense fallback={<div>Loading...</div>}>
             <OtherComponent />
           </Suspense>
         </div>
       );
     }
     ```
     As mentioned in the above code, Suspense is wrapped above the lazy component.

   **[⬆ 返回顶部](#table-of-contents)**
    
276. ### What is route based code splitting?
     One of the best place to do code splitting is with routes. The entire page is going to re-render at once so users are unlikely to interact with other elements in the page at the same time. Due to this, the user experience won't be disturbed.

     Let us take an example of route based website using libraries like React Router with React.lazy,

     ```javascript
     import { BrowserRouter as Router, Route, Switch } from 'react-router-dom';
     import React, { Suspense, lazy } from 'react';

     const Home = lazy(() => import('./routes/Home'));
     const About = lazy(() => import('./routes/About'));

     const App = () => (
       <Router>
         <Suspense fallback={<div>Loading...</div>}>
           <Switch>
             <Route exact path="/" component={Home}/>
             <Route path="/about" component={About}/>
           </Switch>
         </Suspense>
       </Router>
     );
     ```
     In the above code, the code splitting will happen at each route level.

   **[⬆ 返回顶部](#table-of-contents)**
    
277. ### Give an example on How to use context?
     **Context** is designed to share data that can be considered **global** for a tree of React components.

     For example, in the code below lets manually thread through a “theme” prop in order to style the Button component.

     ```javascript
     //Lets create a context with a default theme value "luna"
     const ThemeContext = React.createContext('luna');
     // Create App component where it uses provider to pass theme value in the tree
     class App extends React.Component {
       render() {
         return (
           <ThemeContext.Provider value="nova">
             <Toolbar />
           </ThemeContext.Provider>
         );
       }
     }
     // A middle component where you don't need to pass theme prop anymore
     function Toolbar(props) {
       return (
         <div>
           <ThemedButton />
         </div>
       );
     }
     // Lets read theme value in the button component to use
     class ThemedButton extends React.Component {
       static contextType = ThemeContext;
       render() {
         return <Button theme={this.context} />;
       }
     }
     ```

   **[⬆ 返回顶部](#table-of-contents)**
    
278. ### What is the purpose of default value in context?
     The defaultValue argument is only used when a component does not have a matching Provider above it in the tree. This can be helpful for testing components in isolation without wrapping them.

     Below code snippet provides default theme value as Luna.

     ```javascript
     const MyContext = React.createContext(defaultValue);
     ```

   **[⬆ 返回顶部](#table-of-contents)**
    
279. ### How do you use contextType?
     ContextType is used to consume the context object. The contextType property can be used in two ways,

     1. **contextType as property of class:**
         The contextType property on a class can be assigned a Context object created by React.createContext(). After that, you can consume the nearest current value of that Context type using this.context in any of the lifecycle methods and render function.

         Lets assign contextType property on MyClass as below,

         ```javascript
         class MyClass extends React.Component {
           componentDidMount() {
             let value = this.context;
             /* perform a side-effect at mount using the value of MyContext */
           }
           componentDidUpdate() {
             let value = this.context;
             /* ... */
           }
           componentWillUnmount() {
             let value = this.context;
             /* ... */
           }
           render() {
             let value = this.context;
             /* render something based on the value of MyContext */
           }
         }
         MyClass.contextType = MyContext;
         ```

     2. **Static field**
         You can use a static class field to initialize your contextType using public class field syntax.

         ```javascript
         class MyClass extends React.Component {
           static contextType = MyContext;
           render() {
             let value = this.context;
             /* render something based on the value */
           }
         }
         ```

   **[⬆ 返回顶部](#table-of-contents)**
    
280. ### What is a consumer?
     A Consumer is a React component that subscribes to context changes. It requires a function as a child which receives current context value as argument and returns a react node. The value argument passed to the function will be equal to the value prop of the closest Provider for this context above in the tree.

     Lets take a simple example,

     ```javascript
     <MyContext.Consumer>
       {value => /* render something based on the context value */}
     </MyContext.Consumer>
     ```

   **[⬆ 返回顶部](#table-of-contents)**
    
281. ### How do you solve performance corner cases while using context?
     The context uses reference identity to determine when to re-render, there are some gotchas that could trigger unintentional renders in consumers when a provider’s parent re-renders.

     For example, the code below will re-render all consumers every time the Provider re-renders because a new object is always created for value.

     ```javascript
     class App extends React.Component {
       render() {
         return (
           <Provider value={{something: 'something'}}>
             <Toolbar />
           </Provider>
         );
       }
     }
     ```

     This can be solved by lifting up the value to parent state,

     ```javascript
     class App extends React.Component {
       constructor(props) {
         super(props);
         this.state = {
           value: {something: 'something'},
         };
       }

       render() {
         return (
           <Provider value={this.state.value}>
             <Toolbar />
           </Provider>
         );
       }
     }
     ```

   **[⬆ 返回顶部](#table-of-contents)**
    
282. ### What is the purpose of forward ref in HOCs?
     Refs will not get passed through because ref is not a prop. It is handled differently by React just like **key**. If you add a ref to a HOC, the ref will refer to the outermost container component, not the wrapped component. In this case, you can use Forward Ref API. For example, we can explicitly forward refs to the inner FancyButton component using the React.forwardRef API.

     The below HOC logs all props,
     
     ```javascript
         function logProps(Component) {
           class LogProps extends React.Component {
             componentDidUpdate(prevProps) {
               console.log('old props:', prevProps);
               console.log('new props:', this.props);
             }

             render() {
               const {forwardedRef, ...rest} = this.props;

               // Assign the custom prop "forwardedRef" as a ref
               return <Component ref={forwardedRef} {...rest} />;
             }
           }

           return React.forwardRef((props, ref) => {
             return <LogProps {...props} forwardedRef={ref} />;
           });
         }
     ```

     Let's use this HOC to log all props that get passed to our “fancy button” component,

     ```javascript
         class FancyButton extends React.Component {
           focus() {
             // ...
           }

           // ...
         }
         export default logProps(FancyButton);
     ```

     Now let's create a ref and pass it to FancyButton component. In this case, you can set focus to button element.

     ```javascript
         import FancyButton from './FancyButton';

         const ref = React.createRef();
         ref.current.focus();
         <FancyButton
           label="Click Me"
           handleClick={handleClick}
           ref={ref}
         />;
     ```

   **[⬆ 返回顶部](#table-of-contents)**
    
283. ### Is ref argument available for all functions or class components?
     Regular function or class components don’t receive the ref argument, and ref is not available in props either. The second ref argument only exists when you define a component with React.forwardRef call.

   **[⬆ 返回顶部](#table-of-contents)**
    
284. ### Why do you need additional care for component libraries while using forward refs?
     When you start using forwardRef in a component library, you should treat it as a breaking change and release a new major version of your library. This is because your library likely has a different behavior such as what refs get assigned to, and what types are exported. These changes can break apps and other libraries that depend on the old behavior.

   **[⬆ 返回顶部](#table-of-contents)**
    
285. ### How to create react class components without ES6?
     If you don’t use ES6 then you may need to use the create-react-class module instead. For default props, you need to define getDefaultProps() as a function on the passed object. Whereas for initial state, you have to provide a separate getInitialState method that returns the initial state.

     ```javascript
     var Greeting = createReactClass({
       getDefaultProps: function() {
           return {
             name: 'Jhohn'
           };
         },
       getInitialState: function() {
           return {message: this.props.message};
         },
       handleClick: function() {
          console.log(this.state.message);
       },
       render: function() {
         return <h1>Hello, {this.props.name}</h1>;
       }
     });
     ```
     **Note:** If you use createReactClass then auto binding is available for all methods. i.e, You don't need to use `.bind(this)` with in constructor for event handlers.

   **[⬆ 返回顶部](#table-of-contents)**
    
286. ### Is it possible to use react without JSX?
     Yes, JSX is not mandatory for using React. Actually it is convenient when you don’t want to set up compilation in your build environment. Each JSX element is just syntactic sugar for calling `React.createElement(component, props, ...children)`.

     For example, let us take a greeting example with JSX,

     ```javascript
     class Greeting extends React.Component {
       render() {
         return <div>Hello {this.props.message}</div>;
       }
     }

     ReactDOM.render(
       <Greeting message="World" />,
       document.getElementById('root')
     );
     ```

     You can write the same code without JSX as below,

     ```javascript
     class Greeting extends React.Component {
       render() {
         return React.createElement('div', null, `Hello ${this.props.message}`);
       }
     }

     ReactDOM.render(
       React.createElement(Greeting, {message: 'World'}, null),
       document.getElementById('root')
     );
     ```

   **[⬆ 返回顶部](#table-of-contents)**
    
287. ### What is diffing algorithm?
     React needs to use algorithms to find out how to efficiently update the UI to match the most recent tree. The diffing algorithms is generating the minimum number of operations to transform one tree into another. However, the algorithms have a complexity in the order of O(n3) where n is the number of elements in the tree.

     In this case, displaying 1000 elements would require in the order of one billion comparisons. This is far too expensive. Instead, React implements a heuristic O(n) algorithm based on two assumptions:

     1. Two elements of different types will produce different trees.
     2. The developer can hint at which child elements may be stable across different renders with a key prop.

   **[⬆ 返回顶部](#table-of-contents)**
    
288. ### What are the rules covered by diffing algorithm?
     When diffing two trees, React first compares the two root elements. The behavior is different depending on the types of the root elements. It covers the below rules during reconciliation algorithm,

     1. **Elements Of Different Types:**
        Whenever the root elements have different types, React will tear down the old tree and build the new tree from scratch. For example,  elements <a> to <img>, or from <Article> to <Comment> of different types lead a full rebuild.
     2. **DOM Elements Of The Same Type:**
        When comparing two React DOM elements of the same type, React looks at the attributes of both, keeps the same underlying DOM node, and only updates the changed attributes. Lets take an example with same DOM elements except className attribute,
        ```javascript
        <div className="show" title="ReactJS" />

        <div className="hide" title="ReactJS" />
        ```
     3. **Component Elements Of The Same Type:**
        When a component updates, the instance stays the same, so that state is maintained across renders. React updates the props of the underlying component instance to match the new element, and calls componentWillReceiveProps() and componentWillUpdate() on the underlying instance. After that, the render() method is called and the diff algorithm recurses on the previous result and the new result.
     4. **Recursing On Children:**
        when recursing on the children of a DOM node, React just iterates over both lists of children at the same time and generates a mutation whenever there’s a difference. For example, when adding an element at the end of the children, converting between these two trees works well.
        ```javascript
        <ul>
          <li>first</li>
          <li>second</li>
        </ul>

        <ul>
          <li>first</li>
          <li>second</li>
          <li>third</li>
        </ul>

        ```
     5. **Handling keys:**
     React supports a key attribute. When children have keys, React uses the key to match children in the original tree with children in the subsequent tree. For example, adding a key can make the tree conversion efficient,
     ```javascript
     <ul>
       <li key="2015">Duke</li>
       <li key="2016">Villanova</li>
     </ul>

     <ul>
       <li key="2014">Connecticut</li>
       <li key="2015">Duke</li>
       <li key="2016">Villanova</li>
     </ul>
     ```

   **[⬆ 返回顶部](#table-of-contents)**
    
289. ### When do you need to use refs?
     There are few use cases to go for refs,

     1. Managing focus, text selection, or media playback.
     2. Triggering imperative animations.
     3. Integrating with third-party DOM libraries.

   **[⬆ 返回顶部](#table-of-contents)**
    
290. ### Must prop be named as render for render props?
     Even though the pattern named render props, you don’t have to use a prop named render to use this pattern. i.e,  Any prop that is a function that a component uses to know what to render is technically a “render prop”. Lets take an example with the children prop for render props,

     ```javascript
     <Mouse children={mouse => (
       <p>The mouse position is {mouse.x}, {mouse.y}</p>
     )}/>
     ```

     Actually children prop doesn’t need to be named in the list of “attributes” in JSX element. Instead, you can keep it directly inside element,

     ```javascript
     <Mouse>
       {mouse => (
         <p>The mouse position is {mouse.x}, {mouse.y}</p>
       )}
     </Mouse>
     ```

     While using this above technique(without any name), explicitly state that children should be a function in your propTypes.

     ```javascript
     Mouse.propTypes = {
       children: PropTypes.func.isRequired
     };
     ```

   **[⬆ 返回顶部](#table-of-contents)**
    
291. ### What are the problems of using render props with pure components?
     If you create a function inside a render method, it negates the purpose of pure component. Because the shallow prop comparison will always return false for new props, and each render in this case will generate a new value for the render prop. You can solve this issue by defining the render function as instance method.

   **[⬆ 返回顶部](#table-of-contents)**
    
292. ### How do you create HOC using render props?
     You can implement most higher-order components (HOC) using a regular component with a render prop. For example, if you would prefer to have a withMouse HOC instead of a <Mouse> component, you could easily create one using a regular <Mouse> with a render prop.

     ```javascript
     function withMouse(Component) {
       return class extends React.Component {
         render() {
           return (
             <Mouse render={mouse => (
               <Component {...this.props} mouse={mouse} />
             )}/>
           );
         }
       }
     }
     ```

     This way render props gives the flexibility of using either pattern.

   **[⬆ 返回顶部](#table-of-contents)**
    
293. ### What is windowing technique?
     Windowing is a technique that only renders a small subset of your rows at any given time, and can dramatically reduce the time it takes to re-render the components as well as the number of DOM nodes created. If your application renders long lists of data then this technique is recommended. Both react-window and react-virtualized are popular windowing libraries which provides several reusable components for displaying lists, grids, and tabular data.

   **[⬆ 返回顶部](#table-of-contents)**
    
294. ### How do you print falsy values in JSX?
     The falsy values such as false, null, undefined, and true are valid children but they don't render anything. If you still want to display them then you need to convert it to string. Let's take an example on how to convert to a string,

     ```javascript
     <div>
       My JavaScript variable is {String(myVariable)}.
     </div>
     ```

   **[⬆ 返回顶部](#table-of-contents)**
    
295. ### What is the typical use case of portals?
     React portals are very useful when a parent component has overflow: hidden or has properties that affect the stacking context (e.g. z-index, position, opacity) and you need to visually “break out” of its container.

     For example, dialogs, global message notifications, hovercards, and tooltips.

   **[⬆ 返回顶部](#table-of-contents)**
    
296. ### How do you set default value for uncontrolled component?
     In React, the value attribute on form elements will override the value in the DOM. With an uncontrolled component, you might want React to specify the initial value, but leave subsequent updates uncontrolled. To handle this case, you can specify a **defaultValue** attribute instead of **value**.

     ```javascript
     render() {
       return (
         <form onSubmit={this.handleSubmit}>
           <label>
             User Name:
             <input
               defaultValue="John"
               type="text"
               ref={this.input} />
           </label>
           <input type="submit" value="Submit" />
         </form>
       );
     }
     ```
     The same applies for `select` and `textArea` inputs. But you need to use **defaultChecked** for `checkbox` and `radio` inputs.

   **[⬆ 返回顶部](#table-of-contents)**
    
297. ### What is your favorite React stack?
     Even though the tech stack varies from developer to developer, the most popular stack is used in react boilerplate project code. It mainly uses Redux and redux-saga for state management and asynchronous side-effects, react-router for routing purpose, styled-components for styling react components, axios for invoking REST api, and other supported stack such as webpack, reselect, ESNext, Babel.
     You can clone the project https://github.com/react-boilerplate/react-boilerplate and start working on any new react project.

   **[⬆ 返回顶部](#table-of-contents)**
    
298. ### What is the difference between Real DOM and Virtual DOM?
     Below are the main differences between Real DOM and Virtual DOM,

     | Real DOM | Virtual DOM |
     | ----- | ------- |
     | Updates are slow | Updates are fast |
     | DOM manipulation is very expensive. | DOM manipulation is very easy |
     | You can update HTML directly. | You Can’t directly update HTML |
     | It causes too much of memory wastage | 	There is no memory wastage|
     | Creates a new DOM if element updates | It updates the JSX if element update|


   **[⬆ 返回顶部](#table-of-contents)**
    
299. ### How to add Bootstrap to a react application?
     Bootstrap can be added to your React app in a three possible ways,

     1. Using the Bootstrap CDN:
        This is the easiest way to add bootstrap. Add both bootstrap CSS and JS resources in a head tag.
     2. Bootstrap as Dependency:
        If you are using a build tool or a module bundler such as Webpack, then this is the preferred option for adding Bootstrap to your React application
        ```javascript
        npm install bootstrap
        ```
     3. React Bootstrap Package:
        In this case, you can add Bootstrap to our React app is by using a package that has rebuilt Bootstrap components to work particularly as React components. Below packages are popular in this category,
        1. react-bootstrap
        2. reactstrap

   **[⬆ 返回顶部](#table-of-contents)**
    
300. ### Can you list down top websites or applications using react as front end framework?
     Below are the `top 10 websites` using React as their front-end framework,

     1. Facebook
     2. Uber
     3. Instagram
     4. WhatsApp
     5. Khan Academy
     6. Airbnb
     7. Dropbox
     8. Flipboard
     9. Netflix
     10. PayPal

   **[⬆ 返回顶部](#table-of-contents)**
    
301. ### Is it recommended to use CSS In JS technique in React?
     React does not have any opinion about how styles are defined but if you are a beginner then good starting point is to define your styles in a separate *.css file as usual and refer to them using className. This functionality is not part of React but came from third-party libraries. But If you want to try a different approach(CSS-In-JS) then styled-components library is a good option.

   **[⬆ 返回顶部](#table-of-contents)**
    
302. ### Do I need to rewrite all my class components with hooks?
     No. But you can try Hooks in a few components(or new components) without rewriting any existing code. Because there are no plans to remove classes in ReactJS.

   **[⬆ 返回顶部](#table-of-contents)**
    
303. ### How to fetch data with React Hooks?
     The effect hook called `useEffect` is used to fetch the data with axios from the API and to set the data in the local state of the component with the state hook’s update function.

     Let's take an example in which it fetches list of react articles from the API

     ```javascript
     import React, { useState, useEffect } from 'react';
     import axios from 'axios';

     function App() {
       const [data, setData] = useState({ hits: [] });

       useEffect(() => {
         (async () => {
           const result = await axios(
             'http://hn.algolia.com/api/v1/search?query=react',
           );

           setData(result.data);
         })()
       }, []);

       return (
         <ul>
           {data.hits.map(item => (
             <li key={item.objectID}>
               <a href={item.url}>{item.title}</a>
             </li>
           ))}
         </ul>
       );
     }

     export default App;
     ```

     Remember we provided an empty array as second argument to the effect hook to avoid activating it on component updates but only on mounting of the component. i.e, It fetches only on component mount.

   **[⬆ 返回顶部](#table-of-contents)**
    
304. ### Is Hooks cover all use cases for classes?
     Hooks doesn't cover all use cases of classes but there is a plan to add them soon. Currently there are no Hook equivalents to the uncommon **getSnapshotBeforeUpdate** and **componentDidCatch** lifecycles yet.

   **[⬆ 返回顶部](#table-of-contents)**
    
305. ### What is the stable release for hooks support?
     React includes a stable implementation of React Hooks in 16.8 release for below packages

     1. React DOM
     2. React DOM Server
     3. React Test Renderer
     4. React Shallow Renderer

   **[⬆ 返回顶部](#table-of-contents)**
    
306. ### Why do we use array destructuring (square brackets notation) in `useState`?
     When we declare a state variable with `useState`, it returns a pair — an array with two items. The first item is the current value, and the second is a function that updates the value. Using [0] and [1] to access them is a bit confusing because they have a specific meaning. This is why we use array destructuring instead.

     For example, the array index access would look as follows:

     ```javascript
      var userStateVariable = useState('userProfile'); // Returns an array pair
      var user = userStateVariable[0]; // Access first item
      var setUser = userStateVariable[1]; // Access second item
     ```
     Whereas with array destructuring the variables can be accessed as follows:
     ```javascript
     const [user, setUser] = useState('userProfile');
     ```

     **[⬆ 返回顶部](#table-of-contents)**
    
307. ### What are the sources used for introducing hooks?
     Hooks got the ideas from several different sources. Below are some of them,

     1. Previous experiments with functional APIs in the react-future repository
     2. Community experiments with render prop APIs such as Reactions Component
     3. State variables and state cells in DisplayScript.
     4. Subscriptions in Rx.
     5. Reducer components in ReasonReact.

   **[⬆ 返回顶部](#table-of-contents)**
    
308. ### How do you access imperative API of web components?
     Web Components often expose an imperative API to implement its functions. You will need to use a **ref** to interact with the DOM node directly if you want to access imperative API of a web component. But if you are using third-party Web Components, the best solution is to write a React component that behaves as a **wrapper** for your Web Component.

   **[⬆ 返回顶部](#table-of-contents)**
    
309. ### What is formik?
     Formik is a small react form library that helps you with the three major problems,

     1. Getting values in and out of form state
     2. Validation and error messages
     3. Handling form submission


   **[⬆ 返回顶部](#table-of-contents)**
    
310. ### What are typical middleware choices for handling asynchronous calls in Redux?
     Some of the popular middleware choices for handling asynchronous calls in Redux eco system are `Redux Thunk, Redux Promise, Redux Saga`.

   **[⬆ 返回顶部](#table-of-contents)**
    
311. ### Do browsers understand JSX code?
     No, browsers can't understand JSX code. You need a transpiler to convert your JSX to regular Javascript that browsers can understand. The most widely used transpiler right now is Babel.

   **[⬆ 返回顶部](#table-of-contents)**
    
312. ### Describe about data flow in react?
     React implements one-way reactive data flow using props which reduce boilerplate and is easier to understand than traditional two-way data binding.

   **[⬆ 返回顶部](#table-of-contents)**
    
313. ### What is react scripts?
     The `react-scripts` package is a set of scripts from the create-react-app starter pack which helps you kick off projects without configuring. The `react-scripts start` command sets up the development environment and starts a server, as well as hot module reloading.

   **[⬆ 返回顶部](#table-of-contents)**
    
314. ### What are the features of create react app?
     Below are the list of some of the features provided by create react app.

     1. React, JSX, ES6, Typescript and Flow syntax support.
     2. Autoprefixed CSS
     3. CSS Reset/Normalize  
     4. A live development server
     5. A fast interactive unit test runner with built-in support for coverage reporting
     6. A build script to bundle JS, CSS, and images for production, with hashes and sourcemaps
     7. An offline-first service worker and a web app manifest, meeting all the Progressive Web App criteria.


   **[⬆ 返回顶部](#table-of-contents)**
    
315. ### What is the purpose of renderToNodeStream method?
     The `ReactDOMServer#renderToNodeStream` method is used to generate HTML on the server and send the markup down on the initial request for faster page loads. It also helps search engines to crawl your pages easily for SEO purposes.
     **Note:** Remember this method is not available in the browser but only server.

   **[⬆ 返回顶部](#table-of-contents)**
    
316. ### What is MobX?
     MobX is a simple, scalable and battle tested state management solution for applying functional reactive programming (TFRP). For reactJs application, you need to install below packages,
     ```bash
     npm install mobx --save
     npm install mobx-react --save
     ```

   **[⬆ 返回顶部](#table-of-contents)**
    
317. ### What are the differences between Redux and MobX?
     Below are the main differences between Redux and MobX,

     | Topic | Redux | MobX |
     | ----- | ------- | ------- 
     | Definition| It is a javascript library for managing the application state | It is a library for reactively managing the state of your applications |
     | Programming | It is mainly written in ES6 | It is written in JavaScript(ES5) |
     | Data Store | There is only one large store exist for data storage | There is more than one store for storage |
     | Usage | Mainly used for large and complex applications | Used for simple applications |
     | Performance | Need to be improved | Provides better performance |
     | How it stores | Uses JS Object to store | Uses observable to store the data |


   **[⬆ 返回顶部](#table-of-contents)**
    
318. ### Should I learn ES6 before learning ReactJS?
     No, you don’t have to learn es2015/es6 to learn react. But you may find many resources or React ecosystem uses ES6 extensively. Let's see some of the frequently used ES6 features,

     1. **Destructuring:** To get props and use them in a component
         ```javascript
         // in es 5
          var someData = this.props.someData
          var dispatch = this.props.dispatch

         // in es6
         const { someData, dispatch } = this.props
         ```
     2. Spread operator: Helps in passing props down into a component
         ```javascript
         // in es 5
         <SomeComponent someData={this.props.someData} dispatch={this.props.dispatch} />

         // in es6
         <SomeComponent {...this.props} />
         ```
     3. Arrow functions: Makes compact syntax
         ```javascript
         // es 5
         var users = usersList.map(function (user) {
          return <li>{user.name}</li>
         })
         // es 6
         const users = usersList.map(user => <li>{user.name}</li>);
         ```

   **[⬆ 返回顶部](#table-of-contents)**
    
319. ### What is Concurrent Rendering?
     The Concurrent rendering makes React apps to be more responsive by rendering component trees without blocking the main UI thread. It allows React to interrupt a long-running render to handle a high-priority event. i.e, When you enabled concurrent Mode, React will keep an eye on other tasks that need to be done, and if there's something with a higher priority it will pause what it is currently rendering and let the other task finish first. You can enable this in two ways,

     ```javascript
     // 1. Part of an app by wrapping with ConcurrentMode
     <React.unstable_ConcurrentMode>
       <Something />
     </React.unstable_ConcurrentMode>

     // 2. Whole app using createRoot
     ReactDOM.unstable_createRoot(domNode).render(<App />);
     ```

   **[⬆ 返回顶部](#table-of-contents)**
    
320. ### What is the difference between async mode and concurrent mode?
     Both refers the same thing. Previously concurrent Mode being referred to as "Async Mode" by React team. The name has been changed to highlight React’s ability to perform work on different priority levels. So it avoids the confusion from other approaches to Async Rendering.

   **[⬆ 返回顶部](#table-of-contents)**
    
321. ### Can I use javascript urls in react16.9?
     Yes, you can use javascript: URLs but it will log a warning in the console. Because URLs starting with javascript: are dangerous by including unsanitized output in a tag like ```<a href>``` and create a security hole.

     ```javascript
     const companyProfile = {
       website: "javascript: alert('Your website is hacked')",
     };
     // It will log a warning
     <a href={companyProfile.website}>More details</a>
     ```
     Remember that the future versions will throw an error for javascript URLs.
  
   **[⬆ 返回顶部](#table-of-contents)**
   
322. ### What is the purpose of eslint plugin for hooks?
     The ESLint plugin enforces rules of Hooks to avoid bugs. It assumes that any function starting with ”use” and a capital letter right after it is a Hook. In particular, the rule enforces that,

     1. Calls to Hooks are either inside a PascalCase function (assumed to be a component) or another useSomething function (assumed to be a custom Hook).
     2. Hooks are called in the same order on every render.

   **[⬆ 返回顶部](#table-of-contents)**

323. ### What is the difference between Imperative and Declarative in React?
     Imagine a simple UI component, such as a "Like" button. When you tap it, it turns blue if it was previously grey, and grey if it was previously blue.

     The imperative way of doing this would be:

     ```javascript
     if( user.likes() ) {
         if( hasBlue() ) {
             removeBlue();
             addGrey();
         } else {
             removeGrey();
             addBlue();
         }
     }
     ```

     Basically, you have to check what is currently on the screen and handle all the changes necessary to redraw it with the current state, including undoing the changes from the previous state. You can imagine how complex this could be in a real-world scenario.

     In contrast, the declarative approach would be:

     ```javascript
     if( this.state.liked ) {
         return <blueLike />;
     } else {
         return <greyLike />;
     }
     ```

     Because the declarative approach separates concerns, this part of it only needs to handle how the UI should look in a sepecific state, and is therefore much simpler to understand.
     
   **[⬆ 返回顶部](#table-of-contents)**

324. ### What are the benefits of using typescript with reactjs?
     Below are some of the benefits of using typescript with Reactjs,

     1. It is possible to use latest JavaScript features
     2. Use of interfaces for complex type definitions
     3. IDEs such as VS Code was made for TypeScript
     4. Avoid bugs with the ease of readability and Validation

     **[⬆ 返回顶部](#table-of-contents)**

325. ### How do you make sure that user remains authenticated on page refresh while using Context API State Management?
When a user logs in and reload, to persist the state generally we add the load user action in the useEffect hooks in the main App.js. While using Redux, loadUser action can be easily accessed.

**App.js**

```js
import {loadUser}  from '../actions/auth';
store.dispatch(loadUser());
```

* But while using **Context API**, to access context in App.js, wrap the AuthState in index.js so that App.js can access the auth context. Now whenever the page reloads, no matter what route you are on, the user will be authenticated as **loadUser** action will be triggered on each re-render.

**index.js**

```js
import React from 'react';
import ReactDOM from 'react-dom';
import App from './App';
import AuthState from './context/auth/AuthState'

ReactDOM.render(
  <React.StrictMode>
    <AuthState>
      <App />
    </AuthState>
  </React.StrictMode>,
  document.getElementById('root')
);
```
**App.js**

```js
  const authContext = useContext(AuthContext);

  const { loadUser } = authContext;

  useEffect(() => {
    loadUser();
  },[])
```

**loadUser**

```js
    const loadUser = async () => {
        const token = sessionStorage.getItem('token');

        if(!token){
            dispatch({
                type: ERROR
            })
        }
        setAuthToken(token);

        try {
            const res = await axios('/api/auth'); 

            dispatch({
                type: USER_LOADED,
                payload: res.data.data
            })
            
        } catch (err) {
           console.error(err); 
        }
    }
```

  **[⬆ 返回顶部](#table-of-contents)**

326. ### What are the benefits of new JSX transform?
     There are three major benefits of new JSX transform,

     1. It is possible to use JSX without importing React packages
     2. The compiled output might improve the bundle size in a small amount
     3. The future improvements provides the flexibility to reduce the number of concepts to learn React.
                 
  **[⬆ 返回顶部](#table-of-contents)**

327. ### How is the new JSX transform different from old transform??
     The new JSX transform doesn’t require React to be in scope. i.e, You don't need to import React package for simple scenarios.

     Let's take an example to look at the main differences between the old and the new transform,

     **Old Transform:**

     ```js
     import React from 'react';

     function App() {
       return <h1>Good morning!!</h1>;
     }
     ```

     Now JSX transform convert the above code into regular JavaScript as below,

     ```js
     import React from 'react';

     function App() {
       return React.createElement('h1', null, 'Good morning!!');
     }
     ```

     **New Transform:**

     The new JSX transform doesn't require any React imports

     ```js
     function App() {
       return <h1>Good morning!!</h1>;
     }
     ```

     Under the hood JSX transform compiles to below code

     ```js
     import {jsx as _jsx} from 'react/jsx-runtime';

     function App() {
       return _jsx('h1', { children: 'Good morning!!' });
     }
     ```

     **Note:** You still need to import React to use Hooks.
                 
  **[⬆ 返回顶部](#table-of-contents)**
                 
328. ### How do you get redux scaffolding using create-react-app?
     Redux team has provided official redux+js or redux+typescript templates for create-react-app project. The generated project setup includes,
     
     1. Redux Toolkit and React-Redux dependencies
     2. Create and configure Redux store
     3. React-Redux `<Provider>` passing the store to React components
     4. Small "counter" example to demo how to add redux logic and React-Redux hooks API to interact with the store from components
     
     The below commands need to be executed along with template option as below,
     
     1. **Javascript template:**
     ```js
     npx create-react-app my-app --template redux
     ```
     2. **Typescript template:**
     ```js
     npx create-react-app my-app --template redux-typescript
     ````
  **[⬆ 返回顶部](#table-of-contents)**
                 
329. ### What are React Server components?
     React Server Component is a way to write React component that gets rendered in the server-side with the purpose of improving React app performance. These components allow us to load components from the backend. 
    
     **Note:** React Server Components is still under development and not recommended for production yet.
                 
  **[⬆ 返回顶部](#table-of-contents)**
     
330. ### What is prop drilling?
     Prop Drilling is the process by which you pass data from one component of the React Component tree to another by going through other components that do not need the data but only help in passing it around.
                 
  **[⬆ 返回顶部](#table-of-contents)**

331. ### What is state mutation and how to prevent it?
                     
        `State mutation` happens when you try to update the state of a component without actually using `setState` function. This can happen when you are trying to do some computations using a state variable and unknowingly save the result in the same state variable. This is the main reason why it is advised to return new instances of state variables from the reducers by using Object.assign({}, ...) or spread syntax.

        This can cause unknown issues in the UI as the value of the state variable got updated without telling React to check what all components were being affected from this update and it can cause UI bugs.

        Ex:
        ```javascript
        class A extends React.component {
          constructor(props) {
            super(props);
            this.state = {
              loading: false
            }
         }

        componentDidMount() {
          let { loading } = this.state;
          loading = (() => true)(); // Trying to perform an operation and directly saving in a state variable
        }

        ```

        **How to prevent it:** Make sure your state variables are immutable by either enforcing immutability by using plugins like Immutable.js, always using `setState` to make updates, and returning new instances in reducers when sending updated state values.
        
  **[⬆ 返回顶部](#table-of-contents)**
                            
332. ### What is the difference between useState and useRef hook?
     1. useState causes components to re-render after state updates whereas useRef doesn’t cause a component to re-render when the value or state changes.
        Essentially, useRef is like a “box” that can hold a mutable value in its (.current) property.
     2. useState allows us to update the state inside components. While useRef allows refrencing DOM elements.
                 
  **[⬆ 返回顶部](#table-of-contents)**

  333. ### What are the Differences Between Functional and Class Component
  ## Class Component syntax


 ```
class Example extends Reacts.Component {
render(){
return <h1>This is a class component</h1>}
}

```

> I guess we all know that **Pascal Case** is the accepted way of naming a component in react`Example`. 

# Functional Component syntax
Functional component has been improved over the years with some added features like Hooks
Here is a syntax for functional component

```
function App(){
   return <div className="App">
     <h1>Hello, I'm a Nigerian</h1>
    </div>
}

```
### States in Class Component 
states holds information or data about a component in react which may change over time.  in class component we can update the state, when a user interacts with it or maybe a server response using the `setState()` method and the initial state is been assigned in the `Constructor( ) `method using the the  ` this.state` object. different data type can be passed in the this.state object, which can be string, boolean, numbers, etc. 
<strong> A simple example showing how we use the setState() and constructor() <strong>

```
class Example extends Component {
  constructor() {
    super();
    this.state = {
      example: "This is a class component",
    };
  }
  changeText() {
    this.setState({
      example: "implementing the setState() in class component",
    });
  }
  render() {
    return (
      <>
        <h1>{this.state.example}</h1>
        <button
          onClick={() => {
            this.changeText();
          }}>
          Click!!
        </button>
      </>
    );
  }
}

```
## Using Sates in Functional Components
Initially, we could not use state in functional components because it was only supported in class components. over the years hooks were implemented in functional component. The hooks that enable us to use state in functional component is called <strong>useState</strong>
 The useState( ) hook returns an array of the current state and a function ( setState) that we can use to update the value of the current state. The array is being destructured so we can can see the variables the array holds that is, the initial state and the updated state lets see an example

 

```
function App() {
  const [country, setCountry] = useState("i'm a Nigerian");
  const change = () => {
    setCountry("i am a Canadian");
  };
  return (
    <div className="App">
      <h1>Hello, {country} </h1>
      <button onClick={change}>Change</button>
    </div>
  );
}
```

<h4> Props in Class Component</h4>
 Props are referred to as "properties".  props are passed into react component just like arguments are passed into functions . Props are being specified as attribute just like your html. for example if the name attribute is "name " we assign a value to name. so basically, props are object that contains an attribute and its corresponding value. Data can be passed from parent component to the children component, but this data is immutable, which means that we cannot modify the props across another  component. here is an example 
```
class Introduction extends React.Component {
  render() {
    return <h1> Hello, my name is {this.props.name} </h1>;
  }
}

class App extends React.Component {
  render() {
    return (
      <div className="App">
        <Introduction name=" Queen Elizabeth" />
        <Introduction name=" Margret  Edeh" />
      </div>
    );
  }
}
```

## Props in Functional Components

Props in functional components are similar to that of the class components, the difference is the absence of the 'this' keyword. We also destructure in a similar way without the 'this' keyword. they are also immutable in the functional component
```
function Food(props) {
  return <h1>I love {props.fav}</h1>;
}

function App() {
  return (
    <div className="App">
      <Food fav="Beans" />
      <Food fav="Yam and Egg sauce"/>
    </div>
  );
}
``` 
> As you can see in the example above there wasn't a need for the 'this' keyword.

```

function Food(props) {
  const { fav } = props;
  return <h1>I love {fav}</h1>;
}

function App() {
  return (
    <div className="App">
      <Food fav="Beans" />
      <Food fav="Yam and Egg sauce" />
    </div>
  );
}
```
summary:

*The functional components doesn't require the render method          
*Class component require the render() method that returns JSX.                                                  

To use states in functional component we use the **useState** hook.          
To use State in class components we use the constructor method and the setState function.
                                     
Functional components use the useEffect hook instead of lifecycle method [useEffect](https://www.w3schools.com/react/react_useeffect.asp )    
 Class components uses Lifecycle method    **componentWillUnmount** etc. [ Lifecycle methods](https://www.w3schools.com/react/react_lifecycle.asp )

  **[⬆ 返回顶部](#table-of-contents)**





## Disclaimer

The questions provided in this repository are the summary of frequently asked questions across numerous companies. We cannot guarantee that these questions will actually be asked during your interview process, nor should you focus on memorizing all of them. The primary purpose is for you to get a sense of what some companies might ask — do not get discouraged if you don't know the answer to all of them ⁠— that is ok!

Good luck with your interview 😊

---
