
### String 字符串

在哪里存储字符串? 如何存储不同的语言
目前，最好的做法是创建一个名为Strings的类
class Strings{
  static String welcomeMessage = "Welcome To Flutter";
}
然后在你的代码中，你可以像访问你的字符串一样：new Text(Strings.welcomeMessage)

### Json序列化

生成序列化模板
flutter packages pub run build_runner build

### 配合AutomaticKeepAliveClientMixin可以keep住tab

### 如何主动刷新refresh，如何设置appbar上的leading和bottom，如何设置tabbar的live

//升级到0.5.7 对三个以上tab还是有问题，TabBarView放弃，使用PageView，实现两个control同步，GlobalKey也没问题了。
https://github.com/flutter/flutter/issues/19809
https://github.com/flutter/flutter/issues/11895 tab alive
_debugUltimatePreviousSiblingOf
GlobalKey可以记录state，但是需要跟随build创建
https://stackoverflow.com/questions/49862572

### webView

https://github.com/flutter/flutter/issues/19030 没有webview，残念
https://github.com/dart-flitter/flutter_webview_plugin/issues/23


### 兼容性 

flutter 的跨平台见兼容性意外的话，得益于flutter engine，skia的渲染，只需要canvas
所以第一次运行意外的没有兼容问题，特别是有生之年在ios上看到完全一模一样的下拉刷新


### dialog上黄色线
https://stackoverflow.com/questions/47114639/yellow-lines-under-text-widgets-in-flutter
Dialog中，没使用Scaffold ，导致文本有黄色溢出线提示，可以使用Material ，color或者type为透明


###

hotload很有优势。