
# PC优化

## 1. 减少http 请求（雪碧图， 文件合并）
```
  CSS雪碧 即CSS Sprites，也有人叫它CSS精灵，是一种CSS图像合并技术，
  该方法是将小图标和背景图像合并到一张图片上，然后利用css的背景定位来显示需要显示的图片部分。
```
Q: [什么是CSS Sprites(雪碧图)？](https://zhidao.baidu.com/question/646556016260409565.html)

## 2. 缓存
```
 使用缓存可以减少向服务器的请求数，节省加载时间，
 所以所有静态资源都要在服务器端设置缓存，并且尽量使用长Cache（长Cache资源的更新可使用时间戳）。
 1. 缓存一切可缓存的资源
 2. 使用长Cache（使用时间戳更新Cache）
 3. 使用外联式引用CSS、JavaScript
```

## 3. 文件压缩
```
  1. 开发生成的js、css文件进过压缩后去掉注释，空格等，减少http请求资源。
  2. 启用gZip压缩。
```
Q： [windows如何启用gZip压缩？](http://blog.sina.com.cn/s/blog_67da14f40101sw29.html);

## 4. 减少DOM节点
```
  每多一层，页面在渲染的时候，查询就会多一层，影响效率。
```

## 5. 无阻塞
```
- css写在文件开头部分用<link />的方式引入。  
- 尽量不在页面中通过style的方式添加样式。  
- js的引用写在文件底部。
```

## 6. 避免跳转
```
 在链接最后面都加上 '/' 反斜杠，比如： http://www.wolongdata.com/news/
```

## 7. 避免压缩
```
  如果图片需要100*100这样大的，就不要用一张大小为500 * 500的，然后压缩成100 * 100大小的。
```
  
## 8. 按需加载
```
1. 懒加载。
2. 滚动加载。
3. 通过Media Query加载。
```

 
[参考网站](http://www.jiangweishan.com/article/Mobile-Optimization.html)
