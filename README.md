# vue-app-verify
仿app输入验证码效果的vue组件

![example](./imgs/example.png)

## github
有意见和建议,欢迎到我的gihub项目[vue-app-verify](https://github.com/70hnXX/vue-app-verify.git)提issue

## 开发计划
- [ ] 可选的前端验证功能.配置一个验证码,前端校验验证码是否正确


## Installation - 安装
`yarn add vue-app-verify`
或者,如果你使用npm的话
`npm i vue-app-verify -S`

## Usage - 用法
### 全局引入:
1.main.js:
``` js
import vueAppVerify from 'vue-app-verify'
Vue.use(vueAppVerify)
```
2.组件中:
``` vue
<template>
  <div id="app">
    <vueAppVerify @completed="completed"/>
  </div>
</template>
```
### 按需引入
组件中:
``` vue
<template>
  <div id="app">
    <vueAppVerify @completed="completed"/>
  </div>
</template>

<script>
import vueAppVerify from 'vue-app-verify'
export default {
  ...
  components: {
    vueAppVerify
  },
  ...
}
</script>
```

## Props - 属性
参数|说明|类型|默认值
---|:--:|---:|---:
length|验证码长度|Number|4
enableWord|是否允许输入字母|Boolean|false

## events - 事件
事件名称|说明|回调参数
---|:--:|---:
completed|完成输入|验证码(字符串)