# wx_tt_adapter

### 抖音字节 和 微信小游戏开发适配库

//只有这里需要注意下
```javascript
// index.js里面
 //微信使用这一段
 console.warn('微信和字节接入差异')
Object.defineProperty(window, key, {
    value: _window[key]
})
 //抖音使用这一段，至于为啥，我也是傻了
// if(!window[key]){
//     Object.defineProperty(window, key, {
//           value: _window[key]
//         });
//   }
```
