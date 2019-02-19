# 事件（on）

<iframe src="./examples/on.html" width="750px" height="300px" frameborder="0" scrolling="no"> </iframe>


### 事件绑定

```javascript

        var bbdChart = new BBDChart();
        bbdChart.init({
            container: 'map',
            type: 'circle',
            config: {
                nodeSize: 12
            }
        });

       bbdChart.on('nodeClick', function (data, e) {
            // data：触发事件的对象  e：事件对象
        });

```

> ** 可绑定的事件名: `nodeClick`, `nodeRightClick`, `edgeClick`, `edgeRightClick`, `stageRightClick`, `stageClick`, `mouseover`, `mouseout` **