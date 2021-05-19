# vue-card-swiper

[![standard-readme compliant](https://img.shields.io/badge/standard--readme-OK-green.svg?style=flat-square)](https://github.com/RichardLitt/standard-readme)

一款基于vue的单排轮播组件


## Table of Contents

- [Security](#security)
- [Install](#install)
- [Module](#module)
- [Usage](#usage)
- [API](#api)
- [Example](#example)
- [Affirm](#affirm)
- [Maintainers](#maintainers)
- [Contributing](#contributing)
- [License](#license)

## Security

## Install

```
npm install vue-card-swiper
```
## Module

```js
import vueCardSwiper from 'vue-card-swiper'
Vue.use(vueCardSwiper)
```


## Usage

```vue
 <vue-card-swiper v-model="select"
                     :swiperData="swiperData"
                     @change="changeData"></vue-card-swiper>
```

## API
| Props          | Description         |  Type  | Dafult                |
| :------------- | ------------------- | :----: | --------------------- |
| v-model/:model | 默认选定值          | String | "value"               |
| :swiperData    | 数据源;默认         | Array  | []                    |
| :width         | 图片宽度 单位:px    | String | "150",图片默认150px； |
| :height        | 图片高度 单位:px    | String | "100",图片默认100px； |
| v-on:change    | 选中图片回调methods | method | Function(val) {}      |

## Example

![](http://mmbiz.qpic.cn/mmbiz_jpg/qRJazDfIbDzJibxraX10kEgLBq39bT33aibyNRvVaicKCOkhnicaLctPr3JDvTCIclMibVvzGEz9BOFiaQ9icEmQ37tFw/0)

```vue

<template>
  <div id="app">
    <vue-card-swiper v-model="select"
                     :swiperData="swiperData"
                     @change="changeData"></vue-card-swiper>
  </div>
</template>

<script>
export default {
  name: 'app',
  data() {
    return {
      select: '1',
      swiperData: [
        {
          id: '1',
          name: '深海蔚蓝',
          label: '深海蔚蓝',
          src:
            'https://images.unsplash.com/photo-1505118380757-91f5f5632de0?ixid=MXwxMjA3fDB8MHxzZWFyY2h8Mnx8c2VhfGVufDB8fDB8&ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60'
        },
        {
          id: '2',
          name: '黑色商务',
          label: '黑色商务',
          src:
            'https://images.unsplash.com/photo-1486406146926-c627a92ad1ab?ixid=MXwxMjA3fDB8MHxzZWFyY2h8OXx8YnVzaW5lc3N8ZW58MHx8MHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60'
        },
        {
          id: '3',
          name: '蒲公英',
          label: '蒲公英',
          src:
            'https://img0.baidu.com/it/u=2697908820,3912332944&fm=26&fmt=auto&gp=0.jpg'
        },
        {
          id: '4',
          name: '湖山',
          label: '湖山',
          src:
            'https://img2.baidu.com/it/u=3482128345,2137456532&fm=26&fmt=auto&gp=0.jpg'
        },
        {
          id: '5',
          name: '江河',
          label: '江河',
          src:
            'https://img0.baidu.com/it/u=1314033957,2045802411&fm=26&fmt=auto&gp=0.jpg'
        },
        {
          id: '6',
          name: '城市',
          label: '城市',
          src:
            'https://img0.baidu.com/it/u=1506378410,1346982694&fm=26&fmt=auto&gp=0.jpg'
        },
        {
          id: '7',
          name: '流动星空',
          label: '流动星空',
          src:
            'https://images.unsplash.com/photo-1436891620584-47fd0e565afb?ixid=MXwxMjA3fDB8MHxzZWFyY2h8MTV8fHN0YXJ8ZW58MHx8MHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60'
        }
      ]
    }
  },
  methods: {
    // 选中回显method
    changeData(val) {
      console.log(val)
    }
  }
}
</script>
```

## Affirm

> ​	demo中部分图片引自网络，如有雷同，请联系本人删除
>
> ​	WeChat: 735568868

## Maintainers

[@[@Kyle](https://github.com/MarthaRen/vue-card-swiper.git)](https://github.com/[@Kyle](https://github.com/MarthaRen/vue-card-swiper.git))

## Contributing

Small note: If editing the README, please conform to the [standard-readme](https://github.com/RichardLitt/standard-readme) specification.


## License

MIT © 2021 Kyle
