# vue 代码注释

## 项目介绍
为了更好的在公司内部使用vue技术栈，我们尝试自己本地维护vue技术栈用到的核心库，在本地开发维护之前，我们需要去了解vue这个核心库的基本原理，而对已有的代码进行注释就是一个很好的学习方式。

### 关于vue
Vue 是一套用于构建用户界面的渐进式框架, 由Google华裔前端工程师 尤雨溪于2014年开源；

### 结构 目前版本(2.5.13) [目录说明](https://github.com/vuejs/vue/blob/dev/.github/CONTRIBUTING.md#development-setup)

```
├── LICENSE
├── README.md
├── dist
│   ├── README.md
│   ├── vue.common.js
│   ├── vue.esm.browser.js
│   ├── vue.esm.js
│   ├── vue.js
│   ├── vue.min.js
│   ├── vue.runtime.common.js
│   ├── vue.runtime.esm.js
│   ├── vue.runtime.js
│   └── vue.runtime.min.js
├── package.json
├── src
│   ├── compiler
│   ├── core
│   ├── platforms
│   ├── server
│   ├── sfc
│   └── shared
└── types
    ├── index.d.ts
    ├── options.d.ts
    ├── plugin.d.ts
    ├── vnode.d.ts
    └── vue.d.ts
```

## 加入我们
注释vue核心库的这个事情，我们希望能有更多的人参与，大家一起共同学习进步，只要加入yxUED这个组，就可以直接把您注释的内容提交上来。

### 近期任务
- 在readme中总结归纳vue的目录结构和各文件的作用，以及框架的设计思想；
- 在各核心文件中把该文件的作用写清楚；
- 注释各主要文件和核心函数和语句；
- 发布整理过的vue到公司内私有仓库，逐步在各项目替换；
- 将一些引用的库本地化，控制在10个以内；
- 关注官网的更新日志，把bug修复和新特性及时同步过来；

### 如何注释
- 先对着官网https://cn.vuejs.org/的教程看源码；
- 后对着官网的API依次去源码找对应文件进行注释；
- 最好把github的源码工程clone到本地，对着提交记录学习后把注释写到本工程；
- 参照网上一些源码分析的教程或文章；

## 发布到内部仓库
- 全局安装cnpm: npm install -g cnpm --registry=https://registry.npm.taobao.org
- 设置全局cnpm的registry：cnpm set registry http://192.168.155.xx:7001
- 登陆：cnpm login 分别输入用户名、密码和邮箱（第一次输入的密码即为初始密码）
- 进入发布包的根目录，如： cd ~/mark/vue
- 输入： cnpm init 生成一个package.json文件，主要项目名必须为加 @yx/ 前缀，如：@yx/vue
- 执行：cnpm publish, 成功后在浏览器端http://192.168.155.xx:7002就能看到
