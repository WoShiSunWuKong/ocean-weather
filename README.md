# ocean-weather

> A Vue.js project

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```

For detailed explanation on how things work, checkout the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).


# 在线demo
[在线demo](https://danwild.github.io/leaflet-velocity/)

# step1: 在leaflet上绘制canvas图层
[在leaflet上绘制canvas图](https://github.com/Sumbera/gLayers.Leaflet)

# step2: 完整的leaflet-wind版本
[完整的leaflet-wind版本](https://github.com/danwild/leaflet-velocity)

# 理论依据

* [数据来源](http://nomads.ncep.noaa.gov/)
* [grib](http://www.cpc.ncep.noaa.gov/products/wesley/reading_grib.html)
* [数据转换](https://github.com/cambecc/grib2json)
* [双线性插值算法](https://github.com/cambecc/earth)


20170927

https://www.windy.com

https://github.com/windyty/API

1、全球跨180度展示  worldCopyJump:true 【完成】【显示相邻两个】

[https://github.com/Leaflet/Leaflet/pull/1293](https://github.com/Leaflet/Leaflet/pull/1293)

[polyline/polygon跨180度就近绘制算法](https://github.com/Leaflet/Leaflet/pull/1293/commits/66b5054b21646fa835b99d47c94bfbb0e8b42062)

2、风的动态效果 【完成】

3、跟宝船网类似 【完成】

4、线光滑 【完成】 http://turfjs.org/docs/#bezier

5、文字效果 【未完成】【折线等分点算法、文字跟随曲线算法】

6、等值面生成【未完成】

7、海洋陆地分隔 【未完成】【canvas剪辑区域】

8、不同级别下数据抽稀 【未完成】 【空间抽稀算法（根据空间位置、根据线长度、根据值大小）】

// me

7、不同等级的风不同颜色

8、https://github.com/Leaflet/Leaflet.heat

https://github.com/ursudio/leaflet-webgl-heatmap

http://gallery.echartsjs.com/editor.html?c=xHJD3BZY5-

https://www.patrick-wied.at/static/heatmapjs/?utm_source=npm_leaflet&utm_medium=webpack

[风力等级](http://www.cma.gov.cn/2011xzt/20120816/2012081601/201208160101/201407/t20140717_252607.html)

单位转化

1海里(nmi)=1852米(m)

1kt = 0.5144444m/s

mb=mbar 毫巴(=百帕)

1Bar=0.1MPa=1000mba=1000hpa=100*7.5mmhg=75mmhg=1个大气压

地球周长： 40042.739962655505 （公里）
