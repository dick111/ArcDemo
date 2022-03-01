# ArcDemo
Arc小demo，coding test
## Build
开发语言: Swift 5.0
开发工具: Xcode 13.1
运行系统要求: iOS 13.0

## 设计方法
1.首页
tableview展示数据流，根据数据源type类型，通过factory工厂模式，指向到对应的type的command和cell，进行分类管理，避免首页代码臃肿。同时在装载数据时候计算好高度，controller直接使用。
2.详情页
采用scrollView进行简单的文本布局，适配高度，同时使用第三方图片浏览器JXPhotoBrowser进行图片浏览
3.网页
采用WKWebView进行展示

## 第三方库
用到的三方库有
  pod 'SDWebImage'
  pod 'JXPhotoBrowser'
