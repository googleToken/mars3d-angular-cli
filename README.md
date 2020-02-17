# Mars3D三维地球 - Angular脚手架
 Angular技术栈下的一个最简[Mars3D](http://cesium.marsgis.cn)应用的三维地球项目模版,Mars3D等库都是采用import方式引入。
 这是一个基于 [angular-cli](https://github.com/angular/angular-cli/)并整合了Cesium、MarsGIS的基础项目。

当前脚手架内Mars3D等所有js库都是**采用import方式引入的**。
```javascript
import * as Cesium from 'cesium/Source/Cesium';
import mars3d from "./mars3d/mars3d";
```

 其他技术栈，请参考 [Mars3D开源导航](https://github.com/marsgis/MarsGIS-for-Cesium)
 

## 运行效果 
 [在线Demo](http://cesium.marsgis.cn/project/vue-cli/index.html)  

 ![image](http://cesium.marsgis.cn/project/img/vue-cli.jpg)
 
 [更多项目体验](http://cesium.marsgis.cn/project.html)

 
 

## 运行命令
 
### 首次运行前安装依赖
 `npm install` 或 `cnpm install`
 
### http运行项目
 `npm run serve`  运行后访问：`http://localhost:3003/`  。 修改代码自动热部署，无缓存不用手动刷新

### 打包编译项目
 运行`npm run build`来构建项目。 


## 项目说明
 当前仓库是一个最简的项目模板，并且所有第3方js库都是import的标准引入方式（所以Cesium使用的是原生Cesium，因此有少部分mars3d分析相关功能无法使用），该仓库主要提供给 特定简单项目 或 有代码洁癖的童鞋 使用。
 
 
### 更新项目
 此脚手架中类库不保证是最新版本，请您自行拷贝交付资料中任意包下的 lib\mars3d\ 覆盖至: src\map\mars3d\ 目录下。
 覆盖后，需批量替换 cesium/Cesium  为  cesium/Source/Cesium

 

### 与[mars3d-simple-angular](https://github.com/marsgis/mars3d-simple-angular)仓库的区别
1. 当前是import方式的规范方式引入包含mars3d在内的所有lib。而 mars3d-simple-angular是head静态资源引入。
2. 当前仓库使用的是npm原生的Cesium库。

## 版权说明
  本项目主要是为了展示[Mars3D](http://cesium.marsgis.cn)的项目应用，仅限大家学习之用，如需用于商业项目，请联系购买[火星科技](http://cesium.marsgis.cn)SDK授权。
 并且Mars3D-SDK类库并未开源（即`src\map\mars3d\`）,内部有作者公司logo及时效限制。