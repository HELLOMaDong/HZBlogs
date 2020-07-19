# HiFont业务分析以及HyFont项目伊始
### HiFont前世今生
HiFont是一个替换系统全局字体工具类海外APP但随着各大手机厂商对手机美化有自己的主题商店类似华为主题商店、OPPO主题商店是不允许替换除自己之外的三方手机字体毕竟是在手机商店下载安装字体下载收费的，继而在竞品分析后准备去一个类似于Fonts可以替换特殊符号的键盘项目在公司下面已经有一款成熟的大体量级的海外键盘项目KiKa Keybarod 但也因业务迭代过久代码体量过大很难去直接拿到一套干净的keyboard代码，由此HyFont
### HyFont前期准备
#### 问题分析
1.并无相关项目经验  
2.相关竞品分析 Fonts AnySoftKeyBoard  
3.向其公司他键盘项目组借鉴经验  
4.复杂度    
5.开发周期  
6.适配  
7.兼容性    
8.安全性

### 从0到1的项目启动    
技术选型准备从HiFont搭好的架构  
业务结构并不复杂    
### 技术框架选择
开发语言:Java + Kotlin      
业务架构: MVVM   
网络层:     
数据库:     
UI框架选择: 
### 包结构
功能分包结构->业务模块分包  

### 参考资料    
1.创建输入法 https://developer.android.com/guide/topics/text/creating-input-method?hl=zh-cn     
2.指定输入法类型         https://developer.android.com/training/keyboard-input/style?hl=zh-cn         
3.屏幕输入法                https://android-developers.googleblog.com/2009/04/updating-applications-for-on-screen.html
4.InputMethodService
 https://developer.android.com/reference/android/inputmethodservice/InputMethodService?hl=zh-cn     
 5.键盘布局 https://en.wikipedia.org/wiki/Keyboard_layout#Key_types      
 6.LatinIME KeyboardView.java源码 http://androidxref.com/9.0.0_r3/xref/packages/inputmethods/LatinIME/java/src/com/android/inputmethod/keyboard/KeyboardView.java
 7. Pie - 9.0.0_r3 SDK28 /frameworks/base/core/java/android/inputmethodservice/KeyboardView.java源码
  http://androidxref.com/9.0.0_r3/xref/frameworks/base/core/java/android/inputmethodservice/KeyboardView.java

 
### 项目参考 
1.https://github.com/florisboard/florisboard 正巧赶上这个新项目作者在每天迭代代码可以根据作者学习键盘相关思路    
2.https://github.com/blackcj/AndroidCustomKeyboard 这个键盘项目迭代很久了功能完善度高但是代码体量很大对于阅读开发思路有点费时间   
3.反编译 Fonts APK https://play.google.com/store/apps/details?id=com.fontskeyboard.fonts

## 项目结构

UML https://app.diagrams.net/#G1DbadKCtSKcacOaPYBtmo2XMgzUdVgaI0