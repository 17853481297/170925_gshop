# day01
## 1. 项目开发准备
    项目描述
    技术选型
    API接口
    你能从此项目中学到什么?

## 2. 开启项目开发
    使用脚手架创建项目
    安装所有依赖/指定依赖
    开发环境运行
    生产环境打包与发布

## 3. 搭建项目整体界面结构
    stylus的理解和使用
        结构化, 变量, 函数/minxin(混合)
    vue-router的理解和使用
        $router: 路由器对象, 包含一些操作路由的功能函数, 来实现编程式导航(跳转路由)
        $route: 当前路由对象, 一些当前路由信息数据的容器, path/meta/query/params
    项目路由拆分
    底部导航组件: FooterGuide
    导航路由组件: Msite/Search/Order/Profile

## 4. 抽取组件
    头部组件: HeaderTop, 通过slot来实现组件通信标签结构
    商家列表组件: ShopList
    
## 5. 登陆路由组件
     静态组件
     FooterGuide的显示/隐藏: 通过路由的meta
     
# day02
## 1. 重要问题
    * 如何查看你的应用是否发送某个ajax请求?  
        浏览器的network
    * 发ajax请求404
        请求的路径的对
        代理是否生效(配置和重启)
        服务器应用是否运行
    * 后台返回了数据, 但页面没有显示?
        vuex中是否有
        组件中是否读取
        
## 2. 异步显示轮播图:
    1. 通过vuex获取foodTypes数组(发请求, 读取)
    2. 对数据进行整合计算(一维变为特定的二维数组)
    3. 使用Swiper显示轮播, 如何在界面更新之后创建Swiper对象?
        1). 使用回调+$nextTick()
        2). 使用watch+$nextTick()

      