## 综述

ks-timeline 是一个根据时间轨迹，展现关键节点的 kissy组件
主要交互功能：

##观看效果
[demo](../demo/index.html)


## 组件快速使用

###组件依赖html结构
```xml
<div class="ks-timeline">
    <div id="KT_Navigation" class="kt-navigation"></div>
</div>
```

###组件初始化参数

```javascript
new Timeline({
    panel: $('#KT_Navigation'),
    data: [{}],
    scale: 50,
    minRate: 2,
    maxRate: 2
})
```

参数名 | 说明 | 举个例子 | 截图
------------ | ------------- | -------------
panel  | 容器 | $('#KT_Navigation') | null |
data   | 初始化时间条的数据 | [{'time': '20120101','title': '20110101'},{'time': '2012-3-01','title': '2012.03.01'}] | null |
scale  | 标尺上一个单位刻度，对应到页面的像素值大小 | null |
minRate | 最小可缩小倍数 | 默认值:3 | null |
maxRate | 最大可放大倍数 | 默认值:3 | null |


###组件方法

```javascript
switchTo(NumberIndex);
prev();
next();
```

#事件

change: 
e: {
    target: dom,
    data: dataUnit
}

