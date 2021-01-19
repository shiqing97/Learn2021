Day1
https://www.yuque.com/bosn/alifecourse/step-by-step

- 环境配置

git clone https://github.com/shiqing97/Learn2021.git  

npx create-react-app react-test-app --template typescript (名称不要有大写)

npm i --save redux react-redux redux-devtools-extension rap

npm i --save-dev @types/react-redux

- 一般项目流程
    1. 产品梳理需求文档
    2. 视觉设计&交互设计
    3. 前后端约定接口规范
    4. 开发
    5. 联调

- 制定接口
    rap平台（管理接口定义）--rap2.taobao.org 
    - 新建仓库 输入标题
    - 编辑模式 新建接口
    - rapper 进阶模式 给 package.json 的 scripts 对象下添加下面一行脚本 
        之后可通过rapper将文档中定义的格式数据拉到项目中
    -  npm run rapper 

    - src 新建文件夹 reducers 下
        新建两个文件 rootReducer.ts / types.ts( redux 全局化状态的一个类型)
        配置rootReducer rap 
    - 在入口index 处引入 进行配置
    - 安装redux的开发者工具  https://github.com/zalmoxisus/redux-devtools-extension#usage
        const composeEnhancers = window.__REDUX_DEVTOOLS_EXTENSION_COMPOSE__ || compose;

- 应用实现
    - mock 需要一层代理 overrideFetch 

    - 引入UI框架 material-ui 
        npm i --save @material-ui/core @material-ui/icons

