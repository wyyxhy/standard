# 前端的规范

## 前言
* 由于历史隔阂和业务风格差异，导致公司内工程结构差别很大，代码风格迥异，代码风格不统一，沟通成本大，效率低，维护成本高。公司发展至今，需要专业化的技术迭代，集约式的发展，而不是动辄重构或者造轮，而真正专业化的团队一定会有统一的开发模式，体现效率、共鸣、可持续。
* 开发的规范绝不是消灭代码内容的创造性、优雅性，而是限制过度个性化，推行的是相对标准化，以一种普遍认可的方式一起做事。
* 综上所述，本规范的目标：
>1. 防患于未然，提升质量意识，降低故障率和维护成本。
>2. 标准统一，提升协作效率。
>3. 追求卓越的工匠精神，打磨精品代码。

## 文件命名
```目录结构
 src/  
|- assets/  
    |- css/
        |- elementTheme/   //在官网设置主题后文件的存放位置
        |- reset.css        //初始化一些全局样式 
        |- skin.scss        //放置项目需要用到的颜色变量 
        |- common.scss      //全局用到的样式
        |- cover-element.scss    //覆盖element的样式
    |- iconfont/          //ui设计的icon
    |- img/               //图片
    |- js/                //js文件
|- components
    |- index.js           //全局组件的输出口
    |- DsButton.vue       //组件命名要求大驼峰
|- config/
|- router/
|- store/
    |- index.js          //vuex的输出口
    |- actions.js         
    |- getters.js
    |- mutations.js
|- views/
    |- modename/       //模块名，尽量单个单词
        |- index.vue   //入口文件
        |- ReportDetail.vue  // 该模块下的直系某个页面或者某个组件
        |- reportDetail/     //如果该模块下不止一个文件，则建文件夹
            |- index.vue    //ReportDetail下的入口文件
            |- AddDialog.vue




