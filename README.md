### 通过 NW.js (原node-webkit)实现桌面应用程序

1. 安装nwJs

```
npm install nw
```
[How to run apps](https://github.com/nwjs/nw.js/wiki/How-to-run-apps)

2. 启动demo

```
npm start
```

or

```
nw .
```

3. package.json

```json
{
  "name": "demo-nwJs",
  "main": "index.html", // 指定项目主页面
  "description": "Nw.js Demo",
  "version": "0.0.1",//当前版本
  "window": {
    "show": true,       // 是否显示
    "frame": true,      // 是否显示最外层的框架，设为false之后 窗口的最小化、最大化、关闭 就没有了
    "toolbar": false,   // 是否隐藏窗口的工具条
    "icon": "ico.png",
    "width": 430,
    "height": 450,
    "resizable": true,  // 是否可以放大、缩小
    "position": "center",
    "title": "demo-nwJs"  // 如果 index.html没有title,则会显示这里的值
  },
  "scripts": {
    "start": "nw ."
  }
}
```
