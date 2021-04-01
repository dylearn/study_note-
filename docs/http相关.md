

## 1. 实际开发中选择哪种Content-Type呢？

二进制文件选择：multipart/form-data；

大段的json字符串，适合使用payload，因此可以选择：application/json

application/x-www-form-urlencoded：最常见，原生form变动，如果不设置enctype属性，那么默认该类型提交数据。

## 2. axios封装中axios.defaults.headers['x-requested-with'] = 'XMLHttpRequest'？

如果 requestedWith 为 null，则为同步请求。

如果 requestedWith 为 XMLHttpRequest 则为 Ajax 请求。