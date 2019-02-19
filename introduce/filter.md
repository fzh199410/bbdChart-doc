# 过滤器（filter）

<iframe src="./examples/filter.html" width="600px" height="750px" frameborder="0" scrolling="no"> </iframe>

### 相关方法

```javascript

    /**
      * 设置图谱的过滤器
      * @param type
      * @param filterName
      * @param conditions 可以为单个函数 或 函数数组
    */
    setFiltersByType (type, filterName, conditions)

   /**
     * 节点过滤
     * @param filterName
     * @param conditions 将保留点的条件传过来 通过filter 去过滤 可以为单个函数 或 函数数组
     */
    updateByNodeFilter (filterName, conditions)

    /**
     * 边过滤
     * @param filterName
     * @param conditions 可以为单个函数 或 函数数组
     */
    updateByEdgeFilter (filterName, conditions)

    /**
     * 获取过滤条件
     * @param type
     */
    getFilterByType (type)

```

### 用法

```javascript

     var filterArr = ["company", "person", "address", "orgcode", "email", "phonenumber"];
     bbdChart.graph.filter.updateByNodeFilter('graphFilter', [function (v) {
                return filterArr.includes(v.properties.label);
     }]);

```


> ** 这里我们将过滤条件分为 nodeFilter 和 edgeFilter ，初始化为空对象（设置过滤条件需设置key值 方便多个条件的管理）, 然后将条件合并并且判断**

### 相关思路

```javascript
    let conditions = Object.keys(nodeFilter).reduce((acc, v) => acc.concat(nodeFilter[v]), []);

     node.show = conditions.reduce((acc, v) => {return (acc && v(node));}, true);
```

