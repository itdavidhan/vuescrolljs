---
sidebarDepth: 1
---

# Demo 页面

## 自定义滚动条.

### vuescroll 可以设置滚动条是否保持显示,颜色等。

<ClientOnly>
<Demo-Basic-SetPositionAndKeepShow />
</ClientOnly>

[源码](https://github.com/YvesCoding/vuescrolljs/blob/master/docs/.vuepress/components/Demo/Basic/SetPositionAndKeepShow.vue)

## 检测内容发生变动

### Vuescroll 支持检测内容的尺寸是否发生了变动, 它受了 [element-resize-detector](https://github.com/wnr/element-resize-detector)的启发。

::: tip 提示
你可以自己打开 dev-tool 然后调节元素的样式再查看效果。
:::

<ClientOnly>
<Demo-Basic-DetectSizeChange />
</ClientOnly>

[源码](https://github.com/YvesCoding/vuescrolljs/blob/master/docs/.vuepress/components/Demo/Basic/DetectSizeChange.vue)

## 下拉刷新和上推加载

### Vuescroll 支持下来刷新和上推加载. 在你想展示一个列表的数据的时候很有用。

<ClientOnly>
<Demo-Basic-PullRefreshOrPushLoad />
</ClientOnly>

[源码](https://github.com/YvesCoding/vuescrolljs/blob/master/docs/.vuepress/components/Demo/Basic/PullRefreshOrPushLoad.vue)

## 分页模式.

### Vuescroll 支持分页模式， 当你想要展示一个像[这样](http://element-cn.eleme.io/#/zh-CN/component/carousel)一个轮播图的时候有用。

<ClientOnly>
<Demo-Basic-Paging />
</ClientOnly>

[源码](https://github.com/YvesCoding/vuescrolljs/blob/master/docs/.vuepress/components/Demo/Basic/Paging.vue)

::: tip
如果要禁止 X 或 Y 方向上的滚动， 你可以设置 scrollPanel 的 scrollingY 为 false， X 是同理的。

```javascript
ops: {
  scrollPanel: {
    scrollingY: false; // or scrollingX: false
  }
}
```

你最好设置每个分页的尺寸等同于你的父 dom 的大小， 这样你才不会在一个页面中看到另一个页面的内容在当前视图下， 也就是说，确保每次只显示一个页面。
:::

## 截断模式

Vuescroll 支持 snapping 但是原生的不支持. Snapping 有点像`Paging`, 但是也有一些不同指出: **Paging 每次滑动一整页, 但是 snapping 每次滑动一个用户指定的距离**.

<ClientOnly>
<Demo-Basic-Snapping />
</ClientOnly>

[源码](https://github.com/YvesCoding/vuescrolljs/blob/master/docs/.vuepress/components/Demo/Basic/Snapping.vue)

## 在不同模式之间切换

### 你甚至能在运行期间改变模式， 并且滚动的位置不会变。

<ClientOnly>
<Demo-Basic-SwitchMode />
</ClientOnly>

[源码](https://github.com/YvesCoding/vuescrolljs/blob/master/docs/.vuepress/components/Demo/Basic/SwitchMode.vue)

::: warning 警告
可能在移动端效果不太好， 因为移动端原生的滑动模式的滚动条是一样的
:::

## 轮播图

这两个轮播图是用官方的 vuescroll 插件 - [`vuescroll-carousel`](https://github.com/YvesCoding/vuescroll-carousel)制作成的。

 <Demo-Advance-MakeACarousel />

<br><br>

 <Demo-Advance-MakeACarousel type="v"/>
 
<br>

[源码](https://github.com/YvesCoding/vuescrolljs/blob/master/docs/.vuepress/components/Demo/Advance/MakeACarousel.vue)

## 时间选择器

### 你可以通过设置 `snapping` 为 true 并且 `bouncing` 为 `false`, `scrollingX` 为 false 来做一个时间选择器。

<ClientOnly>
<Demo-Advance-MakeATimePicker />
</ClientOnly>

[源码](https://github.com/YvesCoding/vuescrolljs/blob/master/docs/.vuepress/components/Demo/Advance/MakeATimePicker.vue)

## SSR(服务端渲染) Demo

这里有两个不同环境下的`vuescroll` `ssr` demo， 如果你 ssr 方面有什么问题，可以参考下：

### Node 环境

Node 环境下的 [Demo](https://github.com/YvesCoding/vuescroll-ssr-node)

### PHP 环境

Php 环境下的 [Demo](https://github.com/YvesCoding/vuescroll-ssr-php)

### Nuxt 环境

Nuxt 环境下的 [Demo](https://github.com/YvesCoding/vuescroll-nuxt-demo)
