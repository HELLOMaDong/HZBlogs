      Process: com.hyfontstudio.fontspro, PID: 8994
        android.view.InflateException: Binary XML file line #150: Error inflating class <unknown>
            at android.view.LayoutInflater.createView(LayoutInflater.java:620)
            at com.android.internal.policy.impl.PhoneLayoutInflater.onCreateView(PhoneLayoutInflater.java:56)
            at android.view.LayoutInflater.onCreateView(LayoutInflater.java:669)
            at android.view.LayoutInflater.createViewFromTag(LayoutInflater.java:694)
            at android.view.LayoutInflater.rInflate(LayoutInflater.java:755)
            at android.view.LayoutInflater.rInflate(LayoutInflater.java:758)
            at android.view.LayoutInflater.parseInclude(LayoutInflater.java:839)
            at android.view.LayoutInflater.rInflate(LayoutInflater.java:745)
            at android.view.LayoutInflater.parseInclude(LayoutInflater.java:839)
            at android.view.LayoutInflater.rInflate(LayoutInflater.java:745)
            at android.view.LayoutInflater.rInflate(LayoutInflater.java:758)
            at android.view.LayoutInflater.inflate(LayoutInflater.java:492)
            at android.view.LayoutInflater.inflate(LayoutInflater.java:397)
            at android.view.LayoutInflater.inflate(LayoutInflater.java:353)
            at com.hyfontstudio.fontspro.ime.core.FontsProKeyboard.onCreateInputView(FontsProKeyboard.kt:98)
            at android.inputmethodservice.InputMethodService.updateInputViewShown(InputMethodService.java:1121)
            at android.inputmethodservice.InputMethodService.showWindowInner(InputMethodService.java:1476)
            at android.inputmethodservice.InputMethodService.showWindow(InputMethodService.java:1451)
            at android.inputmethodservice.InputMethodService$InputMethodImpl.showSoftInput(InputMethodService.java:462)
            at android.inputmethodservice.IInputMethodWrapper.executeMessage(IInputMethodWrapper.java:202)
            at com.android.internal.os.HandlerCaller$MyHandler.handleMessage(HandlerCaller.java:40)
            at android.os.Handler.dispatchMessage(Handler.java:102)
            at android.os.Looper.loop(Looper.java:136)
            at android.app.ActivityThread.main(ActivityThread.java:5143)
            at java.lang.reflect.Method.invokeNative(Native Method)
            at java.lang.reflect.Method.invoke(Method.java:515)
            at com.android.internal.os.ZygoteInit$MethodAndArgsCaller.run(ZygoteInit.java:786)
            at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:602)
            at dalvik.system.NativeStart.main(Native Method)
         Caused by: java.lang.reflect.InvocationTargetException
            at java.lang.reflect.Constructor.constructNative(Native Method)
            at java.lang.reflect.Constructor.newInstance(Constructor.java:423)
            at android.view.LayoutInflater.createView(LayoutInflater.java:594)
            at com.android.internal.policy.impl.PhoneLayoutInflater.onCreateView(PhoneLayoutInflater.java:56) 
            at android.view.LayoutInflater.onCreateView(LayoutInflater.java:669) 
            at android.view.LayoutInflater.createViewFromTag(LayoutInflater.java:694) 
            at android.view.LayoutInflater.rInflate(LayoutInflater.java:755) 
            at android.view.LayoutInflater.rInflate(LayoutInflater.java:758) 
            at android.view.LayoutInflater.parseInclude(LayoutInflater.java:839) 
            at android.view.LayoutInflater.rInflate(LayoutInflater.java:745) 
            at android.view.LayoutInflater.parseInclude(LayoutInflater.java:839) 
            at android.view.LayoutInflater.rInflate(LayoutInflater.java:745) 
            at android.view.LayoutInflater.rInflate(LayoutInflater.java:758) 
            at android.view.LayoutInflater.inflate(LayoutInflater.java:492) 
            at android.view.LayoutInflater.inflate(LayoutInflater.java:397) 
            at android.view.LayoutInflater.inflate(LayoutInflater.java:353) 
            at com.hyfontstudio.fontspro.ime.core.FontsProKeyboard.onCreateInputView(FontsProKeyboard.kt:98) 
            at android.inputmethodservice.InputMethodService.updateInputViewShown(InputMethodService.java:1121) 
            at android.inputmethodservice.InputMethodService.showWindowInner(InputMethodService.java:1476) 
            at android.inputmethodservice.InputMethodService.showWindow(InputMethodService.java:1451) 
            at android.inputmethodservice.InputMethodService$InputMethodImpl.showSoftInput(InputMethodService.java:462) 
            at android.inputmethodservice.IInputMethodWrapper.executeMessage(IInputMethodWrapper.java:202) 
            at com.android.internal.os.HandlerCaller$MyHandler.handleMessage(HandlerCaller.java:40) 
            at android.os.Handler.dispatchMessage(Handler.java:102) 
            at android.os.Looper.loop(Looper.java:136) 
            at android.app.ActivityThread.main(ActivityThread.java:5143) 
            at java.lang.reflect.Method.invokeNative(Native Method) 
            at java.lang.reflect.Method.invoke(Method.java:515) 
            at com.android.internal.os.ZygoteInit$MethodAndArgsCaller.run(ZygoteInit.java:786) 
            at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:602) 
            at dalvik.system.NativeStart.main(Native Method) 
         Caused by: android.content.res.Resources$NotFoundException: File res/drawable/bt_share_oval.xml from drawable resource ID #0x7f070063
            at android.content.res.Resources.loadDrawable(Resources.java:2154)
            at android.content.res.TypedArray.getDrawable(TypedArray.java:602)
            at android.view.View.<init>(View.java:3562)
            at android.widget.ImageView.<init>(ImageView.java:123)
            at android.widget.ImageButton.<init>(ImageButton.java:87)
            at android.widget.ImageButton.<init>(ImageButton.java:83)
            at java.lang.reflect.Constructor.constructNative(Native Method) 
            at java.lang.reflect.Constructor.newInstance(Constructor.java:423) 
            at android.view.LayoutInflater.createView(LayoutInflater.java:594) 
            at com.android.internal.policy.impl.PhoneLayoutInflater.onCreateView(PhoneLayoutInflater.java:56) 
            at android.view.LayoutInflater.onCreateView(LayoutInflater.java:669) 
            at android.view.LayoutInflater.createViewFromTag(LayoutInflater.java:694) 
            at android.view.LayoutInflater.rInflate(LayoutInflater.java:755) 
            at android.view.LayoutInflater.rInflate(LayoutInflater.java:758) 
            at android.view.LayoutInflater.parseInclude(LayoutInflater.java:839) 
            at android.view.LayoutInflater.rInflate(LayoutInflater.java:745) 
            at android.view.LayoutInflater.parseInclude(LayoutInflater.java:839) 
            at android.view.LayoutInflater.rInflate(LayoutInflater.java:745) 
            at android.view.LayoutInflater.rInflate(LayoutInflater.java:758) 
            at android.view.LayoutInflater.inflate(LayoutInflater.java:492) 
            at android.view.LayoutInflater.inflate(LayoutInflater.java:397) 
            at android.view.LayoutInflater.inflate(LayoutInflater.java:353) 
            at com.hyfontstudio.fontspro.ime.core.FontsProKeyboard.onCreateInputView(FontsProKeyboard.kt:98) 
            at android.inputmethodservice.InputMethodService.updateInputViewShown(InputMethodService.java:1121) 
            at android.inputmethodservice.InputMethodService.showWindowInner(InputMethodService.java:1476) 
            at android.inputmethodservice.InputMethodService.showWindow(InputMethodService.java:1451) 
            at android.inputmethodservice.InputMethodService$InputMethodImpl.showSoftInput(InputMethodService.java:462) 
            at android.inputmethodservice.IInputMethodWrapper.executeMessage(IInputMethodWrapper.java:202) 
            at com.android.internal.os.HandlerCaller$MyHandler.handleMessage(HandlerCaller.java:40) 
            at android.os.Handler.dispatchMessage(Handler.java:102) 
            at android.os.Looper.loop(Looper.java:136) 
            at android.app.ActivityThread.main(ActivityThread.java:5143) 
            at java.lang.reflect.Method.invokeNative(Native Method) 
            at java.lang.reflect.Method.invoke(Method.java:515) 
            at com.android.internal.os.ZygoteInit$MethodAndArgsCaller.run(ZygoteInit.java:786) 
            at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:602) 
            at dalvik.system.NativeStart.main(Native Method) 
         Caused by: android.content.res.Resources$NotFoundException: File res/drawable/ic_share_black_24dp.xml from drawable resource ID #0x7f0700bd
            at android.content.res.Resources.loadDrawable(Resources.java:2154)
            at android.content.res.Resources.getDrawable(Resources.java:716)
            at android.graphics.drawable.InsetDrawable.inflate(InsetDrawable.java:103)
            at android.graphics.drawable.Drawable.createFromXmlInner(Drawable.java:937)
            at android.graphics.drawable.LayerDrawable.inflate(LayerDrawable.java:168)
            at android.graphics.drawable.Drawable.createFromXmlInner(Drawable.java:937)
            at android.graphics.drawable.Drawable.createFromXml(Drawable.java:877)
            at android.content.res.Resources.loadDrawable(Resources.java:2150)
            at android.content.res.TypedArray.getDrawable(TypedArray.java:602) 
            at android.view.View.<init>(View.java:3562) 
            at android.widget.ImageView.<init>(ImageView.java:123) 
            at android.widget.ImageButton.<init>(ImageButton.java:87) 
            at android.widget.ImageButton.<init>(ImageButton.java:83) 
            at java.lang.reflect.Constructor.constructNative(Native Method) 
            at java.lang.reflect.Constructor.newInstance(Constructor.java:423) 
            at android.view.LayoutInflater.createView(LayoutInflater.java:594) 
            at com.android.internal.policy.impl.PhoneLayoutInflater.onCreateView(PhoneLayoutInflater.java:56) 
            at android.view.LayoutInflater.onCreateView(LayoutInflater.java:669) 
            at android.view.LayoutInflater.createViewFromTag(LayoutInflater.java:694) 
            at android.view.LayoutInflater.rInflate(LayoutInflater.java:755) 
            at android.view.LayoutInflater.rInflate(LayoutInflater.java:758) 
            at android.view.LayoutInflater.parseInclude(LayoutInflater.java:839) 
            at android.view.LayoutInflater.rInflate(LayoutInflater.java:745) 
            at android.view.LayoutInflater.parseInclude(LayoutInflater.java:839) 
            at android.view.LayoutInflater.rInflate(LayoutInflater.java:745) 
            at android.view.LayoutInflater.rInflate(LayoutInflater.java:758) 
            at android.view.LayoutInflater.inflate(LayoutInflater.java:492) 
            at android.view.LayoutInflater.inflate(LayoutInflater.java:397) 
            at android.view.LayoutInflater.inflate(LayoutInflater.java:353) 
            at com.hyfontstudio.fontspro.ime.core.FontsProKeyboard.onCreateInputView(FontsProKeyboard.kt:98) 
            at android.inputmethodservice.InputMethodService.updateInputViewShown(InputMethodService.java:1121) 
            at android.inputmethodservice.InputMethodService.showWindowInner(InputMethodService.java:1476) 
            at android.inputmethodservice.InputMethodService.showWindow(InputMethodService.java:1451) 
            at android.inputmethodservice.InputMethodService$InputMethodImpl.showSoftInput(InputMethodService.java:462) 
            at android.inputmethodservice.IInputMethodWrapper.executeMessage(IInputMethodWrapper.java:202) 
            at com.android.internal.os.HandlerCaller$MyHandler.handleMessage(HandlerCaller.java:40) 
            at android.os.Handler.dispatchMessage(Handler.java:102) 
            at android.os.Looper.loop(Looper.java:136) 
            at android.app.ActivityThread.main(ActivityThread.java:5143) 
            at java.lang.reflect.Method.invokeNative(Native Method) 
            at java.lang.reflect.Method.invoke(Method.java:515) 
            at com.android.internal.os.ZygoteInit$MethodAndArgsCaller.run(ZygoteInit.java:786) 
            at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:602) 
            at dalvik.system.NativeStart.main(Native Method) 
         Caused by: org.xmlpull.v1.XmlPullParserException: Binary XML file line #1: invalid drawable tag vector
            at android.graphics.drawable.Drawable.createFromXmlInner(Drawable.java:933)
            at android.graphics.drawable.Drawable.createFromXml(Drawable.java:877)
        	at android.cont
        	
        	
这几种机型GP差评较多着手去处理这个问题  	
Galaxy Tab Plus 7.0 (goyave3gsea)   
Galaxy Core 2   
Galaxy Grand Prime (grandprimeve3gdtv)  
Galaxy A7(2016) (a7xeltelgt)
Galaxy Grand Neo Plus (grandneove3g) 
Galaxy A3 (a3lte)
Galaxy Grand Prime
Galaxy Grand Neo Plus   
查到FireBase Crashlytics    
SDK -> 19   
Android -> 4.3 4.4  
出现问题
尝试去查询问题原因大概是因为在Androi 5.0以下的设备可能会报这样的错误：
Caused by: org.xmlpull.v1.XmlPullParserException: Binary XML file line #1: invalid drawable tag vector
### 解决方法尝试
 https://stackoverflow.com/questions/48413124/binary-xml-file-line-1-invalid-drawable-tag-vector          
 
    implementation 'androidx.appcompat:appcompat:{current_version}'
    If the issue is caused by a drawableLeft or drawableRight then replace TextView with androidx.appcompat.widget.AppCompatTextView or EditText with androidx.appcompat.widget.AppCompatEditText.
    
    Then, use one of:
    
    app:drawableLeftCompat
    app:drawableStartCompat
    app:drawableEndCompat
    app:drawableRightCompat


1.在defaultConfig下面添加声明


    android {
          defaultConfig {
              vectorDrawables.useSupportLibrary true
          }
    }

2.Documentation about Vector Graphics says:

Android 4.4 (API level 20) and lower doesn't support vector drawables.

With Support Library you have backward-compatibility using the attribute app:srcCompat, but it is not backported for android:drawableRight.

The solution is to keep using .PNG files for those cases or try to set it by code.    

3.在你的Application中里加上下面的代码来启用Vector        

      /**
         * 兼容5.0以下系统
         */
        static {
            /*获取当前系统的android版本号*/
            int currentApiVersion = android.os.Build.VERSION.SDK_INT;
            if (currentApiVersion < Build.VERSION_CODES.LOLLIPOP)//适配android5.0以下
                AppCompatDelegate.setCompatVectorFromResourcesEnabled(true);
        }

3.替换vector为png