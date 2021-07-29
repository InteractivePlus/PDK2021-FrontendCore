<h1 align="center">PDK2021-FrontendCore</h1>

## 项目说明 | Introduction
此项目是形随意动公用开发套件PDK（Public Development Kit）的前端部分。目前为单页面应用。  
技术栈：React，Material-UI，antd  
接口文档：https://github.com/InteractivePlus/InteractivePDK2021-DesignDoc/blob/master/Backend/API.md  


## 参与此项目 | Contribute to this project
### 参与方式
我们非常欢迎你的贡献，可以通过以下方式：
- 通过 [Issue](https://github.com/InteractivePlus/PDK2021-FrontendCore/issues) 报告 bug 或进行咨询。
- 提交 [Pull Request](https://github.com/InteractivePlus/PDK2021-FrontendCore/pulls) 改进代码。

### 环境说明
该版本可正常运行，若使用高版本出现问题，请提交issue，我们将及时跟进。  
- node 12.15
- yarn 1.22

### 初始化
```
npm install
```

### 开发模式
`npm run start` 或 `yarn start`

### 生产模式
`npm run build` 或 `yarn build`

### 补充
该项目前后端分离，部署在不同服务器上。接口对跨域作了限制，而浏览器默认不支持跨域访问，所以本地调试时需要做些调整。  
Chrome用户可参考 https://www.cnblogs.com/duchaoqun/p/12792451.html

vscode用户可参考以下配置，修改`launch.json`实现Chrome跨域调试启动（本repo已经包含了这一配置，在.vscode文件夹下）
```json
"configurations": [
        
        {
            "type": "chrome",
            "request": "launch",
            "name": "Launch Chrome against localhost",
            "url": "http://localhost:3000",
            "webRoot": "${workspaceFolder}",
            "runtimeArgs": ["--disable-web-security"]
        }
    ]
```
在vscode启动调试前需要先进入开发模式（无论是跨域还是普通开发）。

### 开发者
感谢以下做出贡献的开发者：

<a href="https://github.com/InteractivePlus
/
PDK2021-FrontendCore/contributors">
  <img src="https://contributors-img.web.app/image?repo=InteractivePlus
/
PDK2021-FrontendCore" />
</a>

以及OpenAPI-Frontend（PDK前端项目前身）的开发者：
<a href="https://github.com/InteractivePlus
/
OPENAPI2020-Frontend-React/contributors">
  <img src="https://contributors-img.web.app/image?repo=InteractivePlus
/
OPENAPI2020-Frontend-React" />
</a>

## 亿些小细节
记录一下开发中的问题  
1. 如果有问题，优先考虑删除node_modules，然后重新install
