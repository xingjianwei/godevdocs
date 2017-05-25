# Ant Design

## Ant Design Demo
```
npm install antd-init -g
mkdir ant-design-demo
cd ant-design-demo
npm config set registry "https://registry.npm.taobao.org"
npm config get registry
antd-init
npm start 
```

访问 http://127.0.0.1:8989 查看效果。

或者：

```
npm run build
```

替换src\entries\index.js的内容：

```
import React from 'react';  
import ReactDOM from 'react-dom';  
import { DatePicker, message } from 'antd';  
  
class App extends React.Component {  
  constructor(props) {  
    super(props);  
    this.state = {  
      date: '',  
    };  
  }  
  handleChange(date) {  
    message.info('您选择的日期是: ' + date.toString());  
    this.setState({ date });  
  }  
  render() {  
    return (  
      <div style={{ width: 400, margin: '100px auto' }}>  
        <DatePicker onChange={value => this.handleChange(value)} />  
        <div style={{ marginTop: 20 }}>当前日期：{this.state.date.toString()}</div>  
      </div>  
    );  
  }  
}  
ReactDOM.render(<App />, document.getElementById('root'));  
```

## 使用 dva-cli 进行项目初始化

antd-init@2 仅适用于学习和体验 antd，如果你要开发项目，推荐使用 dva-cli 进行项目初始化。dva 是一个基于 react 和 redux 的轻量应用框架，概念来自 elm，支持 side effects、热替换、动态加载等，已在生产环境广泛应用。
```
Usage:

npm install dva-cli -g
dva new myapp
cd myapp
npm start

Visit https://github.com/dvajs/dva to learn more.
```

## antd-admin

http://scaffold.ant.design/#/scaffolds/antd-admin

https://github.com/zuiidea/antd-admin


## 基于react的企业后台管理开发框架

https://github.com/xingjianwei/react.git

一个已经运用在实际企业项目中的react+redux+webpack+ES6+antd+less的SPA后台管理框架demo。

```
npm config set registry "https://registry.npm.taobao.org"
npm install
```

## webpack构建ant-design

[参考文档](http://www.cnblogs.com/huangguojin/articles/6702873.html)

## 开发示例
https://github.com/xingjianwei/dva-example-user-dashboard

https://github.com/sorrycc/blog/issues/18

http://scaffold.ant.design/#/scaffolds/react-antd-admin-jiangxy

