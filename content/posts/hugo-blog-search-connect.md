+++
title = 'Hugo Blog Search Connect'
date = 2024-10-07T03:29:43+08:00
draft = false
tags = ["Technology","DevOps"]
author = ["@phil616"]
+++

# Connect the hugo blog search with other website

通过以下步骤从URL中获取查询值：

在 window.onload 函数中，首先创建一个 URLSearchParams 对象，传递 window.location.search，该属性包含当前页面的查询字符串（即 ? 后面的部分）。
```
const urlParams = new URLSearchParams(window.location.search);
```
然后，使用 urlParams.get('q') 方法获取名为 q 的查询参数值。
```
const query = urlParams.get('q');
```
接着，检查 query 是否存在。如果存在，则将其设置为搜索输入框的值，并触发一个 keyup 事件来执行搜索。
```
if (query) {
    sInput.value = query; // set input value
    sInput.dispatchEvent(new Event('keyup')); // trigger search
}
```

这个过程确保了当页面加载时，如果URL中有查询参数 q，则该参数的值会被自动填入搜索框，并且执行相应的搜索操作。

在原始网站中，构建URL: xxx.com/search?q=query_string，其中 `query_string` 是用户输入的搜索词。

参考链接：

 - https://github.com/pleustonpress/blog.pleuston.org/blob/main/assets/js/fastsearch.js
 - https://github.com/pleustonpress/blog.pleuston.org/commit/8304df40b3896e745b8c3b991a7b295609b436da#diff-f0d52d74317f6e946fded09028ef61236a786d1e1cb877bc5862cedc0896675c