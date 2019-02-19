# 节点（node）

<iframe src="./examples/node.html" width="750px" height="300px" frameborder="0" scrolling="no"> </iframe>

### 属性

#### 格式: 属性名 (对应字节){示例}(注释)

- **节点颜色 (color){"#aec7e8"}**

- **字体颜色 (fontColor){"#132637"}**

- **字体大小 (fontSize){12}**

- **字体图标 (icon){" & # xe616; "}(字体文件的unicode)**

- **节点id (id){"48260c9987a6404b9cd2c4928910edae"}**

- **节点label (label){"中国原子能工业有限公司"}**

- **节点属性 (properties){obj}**

- **节点尺寸 (size){10}**

- **x坐标 (x){60}**

- **y坐标 (y){60}**

> **默认iconfont字体文件，如要使用其它字体，可以设置config中的iconFamily字段**

### 方法

> **add(nodes, edges, cb)  添加节点和边 **

  - ** nodes{object|Array}: nodes数据 **
  - ** edges{object|Array}: edges数据 **
  - ** cb{function(nodes){}}: 回调 **

> **remove()  清除数据 **

  - ** empty **

> **addNode(nodes, cb)  添加节点 **

  - ** nodes{object|Array}: nodes数据 **
  - ** cb{function(nodes){}}: 回调 **

> **removeNode(ids, cb)  删除点 **

  - ** ids{string|Array}: id数组 **
  - ** cb{function(nodes){}}: 回调 **

> **updateNode(ids, attr={}, cb)  更新点 **

  - ** ids{string|Array}: id数组 **
  - ** attr{obj}: 修改属性 **
  - ** cb{function(nodes){}}: 回调 **

