# WebUI

用户界面

## 特性 Features

- 服务端渲染
- GraphQL + websocket
- CSS-in-JS + SCSS
- 中英文

## 技术栈 Tech stack

- Typescript
- [React](https://reactjs.org/) - A JavaScript library for building user interfaces
- [Next.js](https://nextjs.org/) - The React Framework
- [Material UI](https://material-ui.com/) - React components that implement Google's Material Design.
- [Express](https://expressjs.com/)
- Apollo
- PostgreSQL、pgAdmin
- [dotenv](https://github.com/motdotla/dotenv/) - Loads environment variables from .env for nodejs projects
- [dotenv-webpack](https://github.com/mrsteele/dotenv-webpack/) - A secure webpack plugin that supports dotenv and other environment variables and only exposes what you choose and use.
- react-actions
- **redux** for handling application state
- **redux-saga** for handling async actions and side-effects
- **next-routes** for handling dynamic routes
- **axios** for making HTTP requests
- **redux-devtools** in development
- **redux-logger** in development for managing actions and state changes they cause
- **universal-cookie-express** as a middleware for easily writing cookies
- **compression** for compressing static assets
- **babel-plugin-module-resolver** for importing modules related to the root directory
- **prettier** and **eslint** configured with **airbnb**'s styleguide for formating code
- **husky** and **lint-staged** for autoformatting code before commit

## TODO

- 搭建基本脚手架，添加目录结构及文档

## 约定

- 目录使用小写字母
- 组件文件使用大写字母
- Page 页面使用小写字母
- [关于主题样式](./doc/style.md)
- 组件分类：
  1. 主界面 /pages，页面初始化、路由入口
  1. 容器 /containers，为组件注入状态
  1. 模块 /module
  1. 通用组件 /components/common
  1. 高阶组件 /components/hoc

### quik start

```bash
# prepare `.env` and edit it for your own environments
$ cp .env.example .env

# install dependencies
$ 

# development mode
$ 

# production mode
$ 
$ 
```

## Production Deployment

[pm2](https://github.com/Unitech/pm2/) for Node.js process managements.

```bash
# install pm2
$ npm install --global pm2
$ pm2 start
```

## Roadmaps

- [ ] Security: environment variables both server and client
- [ ] Security: production ready session store
- [ ] Security: custom auth guards
- [ ] Server: integration [nest](https://nestjs.com/) or oat++
- [ ] Feature: authentication
- [ ] Test: unit tests
- [ ] Test: e2e tests

