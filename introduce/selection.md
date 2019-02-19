# 选择器（selection）

<iframe src="./examples/selection.html" width="750px" height="300px" frameborder="0" scrolling="no"> </iframe>

### 框选(brush)

- ** auto （任意路径） **
- ** rect  (矩形)     **
- ** circle(圆形)     **

#### 用法

```javascript
    bbdChart.brush('rect', function (data) {
        console.log(data);
    });
```

### 选择方法(selection)

> `selectNodes` 、  `selectEdges` 、  `unSelectNodes` 、  `unSelectEdges` 、  `getSelectedNodes` 、  `getSelectedEdges` 、  `isNodeSelected` 、 `isEdgeSelected`

```javascript
    /**
     * 选择点(single or arr)
     * @param ids
     * @param isAdd 默认false
     */
    selectNodes(ids, isAdd)

    /**
     * 选择边(single or arr)
     * @param ids
     * @param isAdd 默认false
     */
    selectEdges(ids, isAdd)

    /**
     * 取消选择点(unSelect all nodes when ids is undefined or null)
     * @param ids
     */
    unSelectNodes(ids)

    /**
     * 取消选择边(unSelect all edges when ids is undefined or null)
     * @param ids
     */
    unSelectEdges(ids)

    /**
     * 获取选中的节点
     */
    getSelectedNodes()

    /**
     * 获取选中的边
     */
    getSelectedEdges()

    /**
     * 是否为选中边
     * @param id
     */
    isNodeSelected(id)

    /**
     * 是否为选中边
     * @param id
     */
    isEdgeSelected(id)
```