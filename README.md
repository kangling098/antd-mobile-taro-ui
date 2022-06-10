# antd-mobile-taro-ui

## components

核心：基于Taro框架以antd-mobile的设计为标准，尽最大可能与Ant Design Mobile 5.13.1的api保持100%一致，目前来看总体代码75%以上会直接复制Ant Design Mobile大佬们的源码，剩余的25%主要还是为了适配小程序(多多学习Ant Design Mobile开发者大佬们写的代码)

站在巨人的肩膀上，造出高质量的轮子

## 进度展示和兼容情况

*由于小程序不支持SVG所以antd所有用到svg图片的地方会使用css3动画或者图片处理*

| `components` | `name`     | `state` | `difference`                                                                            |
| ------------ | ---------- | ------- | --------------------------------------------------------------------------------------- |
| `Checkbox`   | 复选框     | `done`  | no                                                                                      |
| `Radio`      | 单选框     | `done`  | no                                                                                      |
| `Space`      | 间距       | `done`  | no                                                                                      |
| `DotLoading` | 点状加载中 | `done`  | 由于小程序不支持svg，这里使用css3动画完成，动画与antd表现一致，区别是不支持自动适配字号 |
| `Button`     | 按钮       | `done`  | 不支持type、onMouseDown、onMouseUp属性                                                  |
| `List`       | 列表       | `done`  | demo4和demo5不支持展示                                                                  |
| `Mask`       | 遮罩层     | `doing` |                                                                                         |
| `Popup`      | 弹出层     | `doing` |                                                                                         |


## 图表 ec-canvas

拷贝的是echarts-for-weixin的代码，但是Taro3.4.3有bug，进行了修改

目录：/src/charts/ec-canvas 文件夹整体拷贝 然后按照混合开发模式 就可以使用echarts的图表了

参考网站：

* [echarts-for-weixin](https://github.com/ecomfe/echarts-for-weixin)
* [echarts](https://echarts.apache.org/zh/index.html)
