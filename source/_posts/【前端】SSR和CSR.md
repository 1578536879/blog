---
title: SSR和CSR
categories: 前端
tag: 前端
---

## SSR

### 工作流程

- 浏览器向网站发起请求

- 服务器接收到请求后，先查询数据库中的动态数据(如用户数据)，然后将数据通过模板引擎编译为HTML字符串，然后再返回给浏览器

- 浏览器接收到HTML文档后，将其渲染为可视的UI

### 优点

有利于SEO，首屏渲染快

## CSR

### 工作流程

- 浏览器发起请求

- 服务器接收到请求后，立即返回静态的HTML部分，这部分内容通常是与用户无关的静态数据

- 浏览器解析html文档，待js脚本加载完成后发起异步请求，获取动态数据

- 服务器接收到异步请求后，查询数据库并将动态数据返回给网络浏览器

- 浏览器接收到动态数据后，使用js将数据编译为html字符串并渲染为可视的UI

### 优点

更好支持离线场景和前后端分离等

