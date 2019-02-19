# 基本用法

<iframe src="./examples/baseUsage.html" width="750px" height="300px" frameborder="0" scrolling="no"> </iframe>

### 用法

**引入js**

```javascript
<script src="bbdchart.min.js"></script>
```

**创建容器**

```html
<div id="map"></div>
```

**创建graph**

```javascript
       var bbdChart = new BBDChart();
        bbdChart.init({
            container: 'map',
            type: 'circle',
            config: {
                nodeSize: 12
            }
        });
        var nodes = [...];
        var edges = [...];
        bbdChart.graph.add({nodes: nodes, edges: edges});
        bbdChart.drag(); // 初始化图谱拖动
```

> **new出来的实例对象下面主要的对象是graph(节点、边操作对象)、selection(节点、边选择对象)**。