# Vue-ThemeBlock
一个封装好的Vue提取目标Div主题色指令
## 使用的时候直接 v-theme 插入你想要产生效果的地方即可
### 导入方法很简单：直接在项目中注册这个指令即可     
```javascript   
step1:   
//directives.js
     
step2:   
 // 自定义指令 对象，方便注册
const directives = {
  theme,
}
// >--> 批量注册指令
export default {
  install(Vue) {
    Object.keys(directives).forEach((key) => {
      Vue.directive(key, directives[key])
    })
  }
}   
step3:   
// main.js
import install from './directives'
Vue.use(install)   
```   


