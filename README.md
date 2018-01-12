# AndroidToRN
原生android中嵌入React Native<br>
使用codepush热更新
# 环境：
Android studio3.0<br>
react native 0.50<br>
Mac 10.12.6 <br>
如有问题请提issue

项目下载后<br>
1: cd testApp<br>
2: yarn install<br>
3: npm start<br>
4: android studio打开项目testApp 报错<br>
![buildbug.png](http://upload-images.jianshu.io/upload_images/3353755-9b998a898ab7e1c7.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)<br>
5：按照[codepush3之Android原生引用集成codepush](http://blog.csdn.net/u014041033/article/details/79004351)所示修改路径<br>
或者如下修改<br>
修改codepush.gradle的35行node_modules路径<br>
![codepushgradle.png](http://upload-images.jianshu.io/upload_images/3353755-556775a7c87ade9e.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

修改react.gradle的14行reactRoot路径<br>
![reactbuild.png](http://upload-images.jianshu.io/upload_images/3353755-3ff148637def7335.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)<br>
6：andorid studio 运行项目即可<br>

# ChangeLog:<br>

1.0.3<br>
添加下拉刷新[react-native-pullview](https://github.com/wuyunqiang/react-native-pullview)<br>
效果：<br>
![pullview.gif](http://upload-images.jianshu.io/upload_images/3353755-2d90319bf4a5e3a8.gif?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


1.0.2<br>
纯原生->一半rn一半原生->纯rn<br>
效果：<br>
![nativetiRN.gif](http://upload-images.jianshu.io/upload_images/3353755-2db0558b7af4f3d1.gif?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


1.0.1<br>
1:添加react navigation可以跳转页面<br>
2:添加code push(bug fixed) 有关codepush问题https://github.com/wuyunqiang/ReactNativeUtil/issues/26<br>
3:优化添加预加载reactnative页面 (参考：https://github.com/songxiaoliang/ReactNativeApp)<br>


运行效果：<br>
![androidtoRN.gif](http://upload-images.jianshu.io/upload_images/3353755-e91c00dcdaec7956.gif?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
<br>
代码仅供参考：
如要运行，需要下载node_modules。
另外本人在学习的过程中遇到很多坑，深知找解决问题的路途艰难险阻
所以我正在做一个收集react native的bug解决+工具的库，
希望可以帮助大家在学习中更有效率的写代码。<br>
详情[ReactNativeUtil](https://github.com/wuyunqiang/ReactNativeUtil)<br>
通过label搜索关键字,也欢迎大家丰富内容。
