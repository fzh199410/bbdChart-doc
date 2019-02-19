# 配置（config）

### 设置方法

```javascript
     bbdChart.init({
        container: 'map',
        type: 'circle',
        config: {
            nodeSize: 12
        }
     });
```

### 配置属性

```javascript
    const config = {
        edgeArrowSize: 5,                               // 箭头大小
        edgeColor: "rgba(100,100,100,0.3)",             // 边的颜色
        edgeLabelColor: "#73838b",                      // 边文字颜色
        edgeLabelSize: 12,                              // 边文字大小
        edgeSelectedColor: "rgba(255,49,82,0.9)",       // 边选中颜色
        edgeSize: 0.5,                                  // 边的大小
        edgeLevel: 100,                                 // 边层级
        nodeColor: "#3a82a8",                           // 节点颜色
        nodeLabelColor: "#73838b",                      // 节点文字颜色
        nodeSelectedBorder: "rgba(255,49,82,0.9)",      // 节点选中边颜色
        nodeLabelPosition: 'bottom',                    // 节点文字位置
        maxNodeTextLength: '',                          // 节点文字最大长度
        nodeTextEllipsisSymbol: '...',                  // 超过最大长度
        nodeSubNameWidth: 100,                          // 超出这个范围就裁剪
        nodeSubNameHeight: 100,                         // 超出这个范围就裁剪
        nodeSize: 10,                                   // 节点大小
        nodeLevel: 200,                                 // 节点的level层级
        textBgColor: "rgba(0,0,0,0)",                   // 文字背景颜色
        nodeSelectBorderSize: 1.5,                        // 节点选中边大小
        nodeSelectColor: "rgba(255,49,82,0.9)",         // 节点选中颜色
        selectionFillStyle: "rgba(58, 75, 89, 0.3)",    // 框讯填充颜色
        selectionStrokeStyle: "#4b7598",                // 框选外边框颜色
        zoom: 1.4,                                      // 初始缩放
        zoomMax: 3,                                     // 最大缩放
        zoomMin: 0.4,                                   // 最小缩放
        zoomRatio: 0.2,                                 // 每次缩放的比例
        nodesInterval: 40,
        groupsInterval: 100,
        circleInterval: 40,
        time: 1200,                                     // 动画事件
        ease: 'backInOut',                              // 动画方式
        arrowSize: {width: 3, height: 5},               // 箭头大小
        arrowLevel: 100,                                // 箭头层级
        silentSelection: false,                         // 禁止选中
        silentCancelSelection: false,                   // 禁止取消选中
        shadowBlur: 20,                                 // 图片阴影渲染范围
        shadowColor: '#FF0000',                         // 图片阴影颜色
        iconFamily: 'iconfont',                         // 字体库
        scrollDom: 'body'                               // 上一滚动父级
    };
```