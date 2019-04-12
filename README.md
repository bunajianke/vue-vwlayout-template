# vue-vw-template

> vw 自适应 vue 模板，开箱即用

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).

### 教程： https://www.w3cplus.com/mobile/vw-layout-in-vue.html
> 按照 750px 宽度的设计稿制作的页面，可以直接使用 `px` ，系统会自动转换成 `vw` 

##### 长宽比例用法

```
# npm install postcss-aspect-ratio-mini --save

<!-- html 结构 -->
<div aspectratio demo-16-9>
  <div demo-16-9-content></div>
</div>


/* css */
[demo-16-9] {
  width: 90%;
  margin: 10px auto;
  background-color: #eee;
}

[demo-16-9] {
  aspect-ratio: '16:9';
}

[demo-16-9-content] {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  width: 100%;
  height: 100%;
}
```
