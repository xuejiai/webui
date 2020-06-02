# 学记助理-WebUI

**学记助理**，一款基于统一语义结合智能助理（小五）对话式交互的智能文档，主要用于辅助高效学习与知识管理，目的在于探索一种新的**知识载体与交互方式**，通过开放社区、人机协作的方式，化繁为简降低信息熵，协同积累知识财富！

## 特性 Features

## 技术栈

- [React](https://github.com/facebook/react/) - A declarative, efficient, and flexible JavaScript library for building user interfaces. 
- [Next.js](https://nextjs.org/) - The React Framework
- [Material UI](https://material-ui.com/) - React components for faster and easier web development. Build your own design system, or start with Material Design.
- [Typescript](https://github.com/Microsoft/TypeScript) - A superset of JavaScript that compiles to clean JavaScript output.
- [Redux](https://github.com/reduxjs/redux) - Predictable state container for JavaScript apps
- [Redux-saga](https://github.com/redux-saga/redux-saga) - An alternative side effect model for Redux apps
- [GraphQL](https://graphql.com/) - GraphQL is an open spec for a flexible API layer.
- [JSS](https://github.com/cssinjs/jss) - JSS is an authoring tool for CSS which uses JavaScript as a host language.
- [Three.js](https://github.com/mrdoob/three.js/) - JavaScript 3D library.
- [Konva.js](https://konvajs.org/) - HTML5 2d canvas js library for desktop and mobile applications 
- [Recharts](http://recharts.org/en-US/) - A composable charting library built on React components
- [Prettier](https://github.com/prettier/prettier) - Prettier is an opinionated code formatter.
- [Eslint](https://github.com/eslint/eslint) - Find and fix problems in your JavaScript code. 
- [PM2](https://github.com/Unitech/pm2) - Node.js Production Process Manager with a built-in Load Balancer. 
- Websocket

## 约定

- 目录使用小写字母
- 组件文件使用大写字母
- 页面文件使用小写字母
- 组件分类：
  1. 页面组件 /pages，页面初始化、路由入口
  1. 容器组件 src/containers，为组件注入状态
  1. 通用组件 src/components/common
  1. 高阶组件 src/components/hoc
  1. 模块组件 src/module

- [关于主题样式](./doc/style.md)

## 开发

```bash
# 配置变量
$ cp .env.example .env

# 安装依赖
$ cnpm i

# 开发模式
$ cnpm run dev
```

## 部署到生产环境

[pm2](https://github.com/Unitech/pm2/) Node.js Production Process Manager 

```bash
# install pm2
$ npm install --global pm2
$ pm2 start
```

## Roadmaps

- [ ] Client: nextjs Typescript material-ui redux threejs
- [ ] Deployment: nginx pm2 nodejs
- [ ] Test: unit tests
- [ ] Test: e2e tests
- [ ] Api: OpenAPI websocket GraphQL
- [ ] Server: integration oat++
- [ ] Feature: authentication

