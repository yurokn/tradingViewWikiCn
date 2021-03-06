# 图表库内容

---

Charting Library 图表库包可在GitHub上获得（必须获得授权才能访问GitHub上的这个私有资源）. 您可以检出最新的稳定版本\(`master`branch\)或最新的开发版本\(`unstable`branch\) 。如果想要访问此资源请联系我们。

您可以通过在浏览器控制台中执行 TradingView.version\(\) 来查看图表库版本。

### [图表库内容](#图表库内容)

```js
+/charting_library
    - charting_library.min.js
+ /datafeed
+ /udf
    - datafeed.js
+ /static
- index.html
```

* /charting\_library 包含所有的库文件。

* /charting\_library/charting\_library.min.js 包含Charting Library widget 接口。不建议修改该文件。

* /charting\_library/datafeeds/udf/datafeed.js 包含[UDF-compatible](/book/UDF.md) 的datafeed包装器（用于实现[JS API](/book/JS-Api.md)以连接Charting Library和UDF连接datafeed）。例子中的datafeed包装器实现了脉冲实时仿真数据。您可以自由编辑此文件。

* /charting\_library/static 文件夹中存储图表库内部资源，不适用于其他目的。

* /index.html 为使用Charting Library widget 的html例子。

* /test.html 为不同的图表库自定义功能使用的示例。

* /mobile\*.html 也是Widget自定义的示例。

从版本1.1开始，所有内部库的JS和CSS代码都被内联和缩小，以减少页面加载时间。 您要编辑的文件不会被缩小。
