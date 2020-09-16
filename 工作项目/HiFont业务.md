2019-12-20 入职
##     项目伊始
###     拿到代码编译处理问题
    1.VS版本确认 vs 3.5.3  gradle-5.1.1-all
    
    2.我觉得也是 但是出现资源引用问题 Aapt2Exception: Android resource linking failed
    
    我覺得是這樣 要在 gradle.properties 加上
    android.useAndroidX=true
    android.enableJetifier=true
        
    KEYSTORE_PASSWORD=
     KEY_ALIAS=
    KEY_PASSWORD=

    android.useAndroidX=true
    android.enableJetifier=true

    org.gradle.jvmargs=-XX\:MaxHeapSize\=2048m -Xmx4608M

    android.enableR8=false
    
    主要是因為升級 androidx 了
    
    3.你那邊應該可以用了 拿掉 debug 那一行 release sign key 這一行應該是錯的 但是我這邊不影響比較奇怪
    
    debug config 不應該出現 signingConfig signingConfigs.release
    
    4.沒有接口文檔呢 看代碼吧 之後估計要跟後端一起重整了 可以重新設計
    
    那個接口一團亂
    
    嗯 hifont 是個比較古老的 app 我們這邊改比較多的就是廣告跟導量, 導量這個你們接手以後可以移除了
        
    就是下面那個 locker, launcher 啥的
        
    其他的從來都沒有變過 當初交接的時候就長這樣了
    
    https://docs.google.com/document/d/1WTn1B4wiX1BYWLHVcTpues_KKzYyI5fsAEneafbjZjI/edit?folder=0AMp0vBhkN38nUk9PVA#
    
    5.主要 HiFonr 有兩個模式, 你用三星手機跟其他手機打開是不同的列表 不同的 api
    
    6.om.monti.lib:monti-ads 这是接的google的广告吗
    
    不是的 這是我們家的庫 單純處理廣告邏輯而已 以後你們可以考慮用自己的
    
    對 目前主要是谷歌廣告 是從不同的 app 抽離出來的 以前還有 fb 但是已經很久沒用了
    
    嗯 我們接手以後主要心力都在改收入 還有應付谷歌升級需求 其他的基本沒改 所以算是比較老的代碼
    
    你可以照你的想法改 該拔的都拔
    
    7. 是的 主題包代碼在 https://github.com/KikaTech/ThemeTemplateV3 的 flipfont
    
    https://console.firebase.google.com/u/0/project/hifont-6c7c9/overview
    
    組好像是 group 我不知道他們這個是放哪個組 [捂脸] 我覺得行吧就這樣填吧, 有可以說明的話就說你其實需要的是 flipfont 分支
    
    8.你们一般用firbase处理什么问题 只是数据统计吗
    
    還有看崩潰吧
    
    但是 hifont 比較奇怪 crashlytics 都沒反應 舊的 firebase 就這樣了 所以崩潰只能先看 gp
    
    不過 firebase crashlytics 只能看 java 就是了
    
    hifont 因為牽扯到字體 還是會有 native crash
    
    可能看一下 gp 有沒有比較嚴重的 以前有掃過一次
    
    9.Amy : 应用内下载的资源维护和资源包的app运营维护应该不一样。看看是不是可以问问Franky之前是怎么操作的。

    運營平台基本是不能用的 應用內下載從來就沒有後台 懷疑以前就是一個寫死的列表放在線上而已, 字體包平台以前有, 遷移的時候遷移了一半, 目前已經請張歡那邊去看
    
    10.debug模式下 字体预览页的广告是展示不出来的对吗
    
    是的 3 是 no fill   
    所以 debug 最好自己把 device id 加到 test device, addTestDevice
    
    https://developers.google.com/admob/android/test-ads
    
    也有測試廣告 id
    
    但是要小心不要上了..
    
## 数据迁移处理
    后端处理
## Anroid架构整理
    0.重要建立数据监控体系
    1.预期MVP架构整理 参照 WanAndroid（思路）
    2.图片加载框架策略模式处理
    3.网路框架正在梳理 预期参照WanAndroid
      或者 Des Lesdo  
    
    Okhttp + Rxjava + MVP处理
    4.Kotlin加入
    5.Degerr2 考虑加入成本
    6.更新逻辑未处理
    7.组件化处理导量位慢慢梳理
    8.flutter和原生混编可以考虑一下
    
    优先MVP和网络封装处理
    
   
##    项目优化

    
    2.IO 下载优化
    3.gradle依赖库统一整理
    4.修复Crashlytics
###      一 启动优化
    1.启动白屏优化
    2.7z
    3.
    5.Hardcoder优化