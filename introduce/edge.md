# 边（edge）

<iframe src="./examples/edge.html" width="750px" height="300px" frameborder="0" scrolling="no"> </iframe>

### 属性

#### 格式: 属性名 (对应字节){示例}

- **边颜色 (color){"#d2dbe1"}**

- **标签背景色 (labelBgColor){"#132637"}**

- **标签颜色 (labelColor){"#132637"}**

- **标签字体大小 (edgeLabelSize){12}**

- **边形状 (lineDash){默认[2]，虚线[4, 1]}(描边虚线样式，参考 [SVG stroke-dasharray](https://developer.mozilla.org/en-US/docs/Web/SVG/Attribute/stroke-dasharray))**

- **边label (label){"老李"}**

- **边id (id){"4b9fa9f4a7eb93c1aff389ece93fbe38_czgs|company|invest|company"}**

- **边属性 (properties){obj}**

- **起始点id (source){"4b9fa9f4a7eb93c1aff389ece93fbe38_czgs"}**

- **到达点id (target){"4b9fa9f4a7eb93c1aff389ece93fbe38_czgs"}**

### 方法

> **addEdge(edges, cb)  添加边 **

  - ** edges{object|Array}: edges数据 **
  - ** cb{function(nodes){}}: 回调 **

> **removeEdge(ids, cb)  删除边 **

  - ** ids{string|Array}: id数组 **
  - ** cb{function(nodes){}}: 回调 **

> **updateEdge(ids, attr={}, cb)  更新边 **

  - ** ids{string|Array}: id数组 **
  - ** attr{obj}: 修改属性 **
  - ** cb{function(nodes){}}: 回调 **
