# 前端的规范

## 前言
* 由于历史隔阂和业务风格差异，导致公司内工程结构差别很大，代码风格迥异，代码风格不统一，沟通成本大，效率低，维护成本高。公司发展至今，需要专业化的技术迭代，集约式的发展，而不是动辄重构或者造轮，而真正专业化的团队一定会有统一的开发模式，体现效率、共鸣、可持续。
* 开发的规范绝不是消灭代码内容的创造性、优雅性，而是限制过度个性化，推行的是相对标准化，以一种普遍认可的方式一起做事。

* 综上所述，本规范的目标：
>1. 防患于未然，提升质量意识，降低故障率和维护成本。
>2. 标准统一，提升协作效率。
>3. 追求卓越的工匠精神，打磨精品代码。

## 文件目录
```目录结构
src/  
|- assets/  
    |- css/
        |- elementTheme/      //在官网设置主题后文件的存放位置
        |- reset.css          //初始化一些全局样式 
        |- skin.scss          //放置项目需要用到的颜色变量 
        |- common.scss        //全局用到的样式
        |- cover-element.scss    //覆盖element的样式
    |- iconfont/              //ui设计的icon
    |- img/                   //图片
    |- js/                    //js文件
|- components
    |- index.js               //全局组件的输出口
    |- DsButton.vue           //组件命名要求首写大写，且以特定的前缀
|- config/
|- router/                    //以异步加载的方式
|- store/
    |- index.js               //vuex的输出口
    |- actions.js             //所有改变vuex数据的方法只能从此处调用，参照health-view项目
    |- getters.js
    |- mutations.js
|- views/
    |- modename/             //模块名，尽量单个单词
        |- index.vue         //入口文件
        |- ReportDetail.vue  // 该模块下的直系某个页面
        |- components/       //该模块下多个下级模块会公用的组件
        |- reportList/       //如果二级模块下不止一个文件，则建文件夹
            |- index.vue     //ReportDetail下的入口文件
            |- AddDialog.vue
            |- components/   //该模块页面下的组件
```

## vue代码风格
按照vue官网风格指南来书写Vue代码。[链接](https://cn.vuejs.org/v2/style-guide/)
## js代码规范
* 按照airbnb的规范来编写eslint配置  
[英文版](https://github.com/airbnb/javascript)  
[中文版](https://github.com/libertyAlone/airbnb-javascript-style-guide-cn)
  
* 约定规范
> 1、在dom上的方法以handle开头命名。例如：handleAddFile。  
>2、自己定义的方法以易懂的命名方式命名。例如：getFileList。  
> 3、handle开头的方法放在methods中的前面，自定义的方法放在后面，这样代码清晰易看。  
>4、尽量在方法前写注释，表明此方法的用处。
## css代码规范
* class起名请以xx-xx-xx这样的形式。
* pc端用Element组件库，请用scss(less中的@会影响动态路由),且颜色用变量。
* app端用[Vant组件库](https://youzan.github.io/vant/#/zh-CN/intro)。








