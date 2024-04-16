版本问题永远是新手的大头，如果你电脑牛逼，系统是最新的，那么全部使用最新版本就行了！https://docs.flutter.dev/get-started/install/macos/mobile-ios

# xcode 版本

一定要选对版本，要么你macos一直升级到最新版本，那么你直接走最新就行了，比如我是macos12版本，那么xcode只能用13版本，再新的用不了了！

如何下载xcode，推荐使用 xcodes https://www.xcodes.app/ 进行管理

![image-20240416135802518](https://tyut.oss-accelerate.aliyuncs.com/image/2024/4-16/5d9fbe6985b1430e8401d74da224a59b.png)

安装看网速和电脑配置，基本上我花了小半个小时吧！此时可以去看看别的

# flutter 版本

我xcode使用的13版本，所以flutter只能用3.0版本，最新的都用不了，这些都可以从flutter release！https://docs.flutter.dev/release/release-notes/release-notes-3.0.0

直接下载安装包解压即可



# CocoaPods

最坑比的就是这个，你需要翻墙，不然安装不成功！最好先升级下 ruby 版本！

```shell
 sudo gem install cocoapods -V
```

# 环境变量

最后我的就是这个！！

```shell
export PATH=$PATH:/Users/bytedance/flutter/flutter/bin
export PATH=/usr/local/lib/ruby/gems/3.2.0/bin:$PATH
```

# 使用

跟着这个文档走就行了 https://codelabs.developers.google.com/codelabs/flutter-codelab-first

执行 `flutter doctor -v`

```shell
~ flutter doctor -v
Running "flutter pub get" in flutter_tools...                      10.2s
[✓] Flutter (Channel stable, 3.0.0, on macOS 12.2.1 21D62 darwin-x64,
    locale zh-Hans-CN)
    • Flutter version 3.0.0 at /Users/bytedance/flutter/flutter
    • Upstream repository https://github.com/flutter/flutter.git
    • Framework revision ee4e09cce0 (1 年 11 个月前), 2022-05-09 16:45:18
      -0700
    • Engine revision d1b9a6938a
    • Dart version 2.17.0
    • DevTools version 2.12.2

[✗] Android toolchain - develop for Android devices
    ✗ Unable to locate Android SDK.
      Install Android Studio from:
      https://developer.android.com/studio/index.html
      On first launch it will assist you in installing the Android SDK
      components.
      (or visit
      https://flutter.dev/docs/get-started/install/macos#android-setup
      for detailed instructions).
      If the Android SDK has been installed to a custom location,
      please use
      `flutter config --android-sdk` to update to that location.


[✓] Xcode - develop for iOS and macOS (Xcode 13.0)
    • Xcode at /Applications/Xcode-13.0.0.app/Contents/Developer
    • CocoaPods version 1.15.2

[✓] Chrome - develop for the web
    • Chrome at /Applications/Google Chrome.app/Contents/MacOS/Google
      Chrome

[!] Android Studio (not installed)
    • Android Studio not found; download from
      https://developer.android.com/studio/index.html
      (or visit
      https://flutter.dev/docs/get-started/install/macos#android-setup
      for detailed instructions).

[✓] IntelliJ IDEA Ultimate Edition (version 2024.1)
    • IntelliJ at /Users/bytedance/Applications/JetBrains
      Toolbox/IntelliJ IDEA Ultimate.app
    • Flutter plugin can be installed from:
      🔨 https://plugins.jetbrains.com/plugin/9212-flutter
    • Dart plugin can be installed from:
      🔨 https://plugins.jetbrains.com/plugin/6351-dart

[✓] VS Code (version 1.85.0)
    • VS Code at /Applications/Visual Studio Code.app/Contents
    • Flutter extension version 3.86.0

[✓] Connected device (3 available)
    • iPhone 12 Pro (mobile) • EFF695A4-6667-4176-A789-83A97AB5F792 •
      ios            • com.apple.CoreSimulator.SimRuntime.iOS-15-0
      (simulator)
    • macOS (desktop)        • macos                                •
      darwin-x64     • macOS 12.2.1 21D62 darwin-x64
    • Chrome (web)           • chrome                               •
      web-javascript • Google Chrome 123.0.6312.124

[✓] HTTP Host Availability
    • All required HTTP hosts are available

! Doctor found issues in 2 categories.
```

使用 vscode 创建项目,最终 运行一下就行了 ！

![image-20240416140507771](https://tyut.oss-accelerate.aliyuncs.com/image/2024/4-16/6818721d8b0043ea8fd0b6355bb5a884.png)

成功界面

![image-20240416140543752](https://tyut.oss-accelerate.aliyuncs.com/image/2024/4-16/f9f3ed05358d4ddfbd799257000215c9.png)