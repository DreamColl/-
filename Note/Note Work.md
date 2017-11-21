# Note Work

#### 1.vueRouter lazy-loading

```
v3.0.1
const Foo = () => Promise.resolve({ /* 组件定义对象 */ })
import('./Foo.vue') // 返回 Promise

const Foo = () => import('./Foo.vue')

把组件按组分块

有时候我们想把某个路由下的所有组件都打包在同个异步块 (chunk) 中。只需要使用 命名 chunk，一个特殊的注释语法来提供 chunk name (需要 Webpack > 2.4)。

const Foo = () => import(/* webpackChunkName: "group-foo" */ './Foo.vue')
const Bar = () => import(/* webpackChunkName: "group-foo" */ './Bar.vue')
const Baz = () => import(/* webpackChunkName: "group-foo" */ './Baz.vue')
```

```
v2.1.1
const Foo = resolve => require(['./Foo.vue'], resolve) //AMD风格

把组件按组分块
 
 有时候我们想把某个路由下的所有组件都打包在同个异步 chunk 中。只需要 给 chunk 命名，提供 `require.ensure` 第三个参数作为 chunk 的名称:

 const Foo = r => require.ensure([], () => r(require('./Foo.vue')), 'group-foo')
 const Bar = r => require.ensure([], () => r(require('./Bar.vue')), 'group-foo')
 const Baz = r => require.ensure([], () => r(require('./Baz.vue')), 'group-foo')
```

