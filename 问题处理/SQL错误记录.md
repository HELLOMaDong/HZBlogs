    java.lang.RuntimeException: 
      at android.app.ActivityThread.performLaunchActivity (ActivityThread.java:2977)
      at android.app.ActivityThread.handleLaunchActivity (ActivityThread.java:3114)
      at android.app.servertransaction.LaunchActivityItem.execute (LaunchActivityItem.java:78)
      at android.app.servertransaction.TransactionExecutor.executeCallbacks (TransactionExecutor.java:113)
      at android.app.servertransaction.TransactionExecutor.execute (TransactionExecutor.java:71)
      at android.app.ActivityThread$H.handleMessage (ActivityThread.java:1859)
      at android.os.Handler.dispatchMessage (Handler.java:106)
      at android.os.Looper.loop (Looper.java:201)
      at android.app.ActivityThread.main (ActivityThread.java:6831)
      at java.lang.reflect.Method.invoke (Method.java)
      at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run (RuntimeInit.java:547)
      at com.android.internal.os.ZygoteInit.main (ZygoteInit.java:927)
    Caused by: android.database.sqlite.SQLiteException: 
      at android.database.sqlite.SQLiteConnection.nativePrepareStatement (SQLiteConnection.java)
      at android.database.sqlite.SQLiteConnection.acquirePreparedStatement (SQLiteConnection.java:903)
      at android.database.sqlite.SQLiteConnection.prepare (SQLiteConnection.java:514)
      at android.database.sqlite.SQLiteSession.prepare (SQLiteSession.java:588)
      at android.database.sqlite.SQLiteProgram.<init> (SQLiteProgram.java:58)
      at android.database.sqlite.SQLiteQuery.<init> (SQLiteQuery.java:37)
      at android.database.sqlite.SQLiteDirectCursorDriver.query (SQLiteDirectCursorDriver.java:46)
      at android.database.sqlite.SQLiteDatabase.rawQueryWithFactory (SQLiteDatabase.java:1408)
      at android.database.sqlite.SQLiteDatabase.rawQuery (SQLiteDatabase.java:1347)
      at com.liam.coolfont.data.DatabaseOpenHelper.queryData (DatabaseOpenHelper.java:13)
      at com.liam.coolfont.data.DatabaseManager.a (DatabaseManager.java:2)
      at com.liam.coolfont.MainActivity.setupRecyclerview (MainActivity.java:6)
      at com.liam.coolfont.MainActivity.onCreate (MainActivity.java:36)
      at android.app.Activity.performCreate (Activity.java:7224)
      at android.app.Activity.performCreate (Activity.java:7213)
      at android.app.Instrumentation.callActivityOnCreate (Instrumentation.java:1271)
      at android.app.ActivityThread.performLaunchActivity (ActivityThread.java:2957)
      at android.app.ActivityThread.handleLaunchActivity (ActivityThread.java:3114)
      at android.app.servertransaction.LaunchActivityItem.execute (LaunchActivityItem.java:78)
      at android.app.servertransaction.TransactionExecutor.executeCallbacks (TransactionExecutor.java:113)
      at android.app.servertransaction.TransactionExecutor.execute (TransactionExecutor.java:71)
      at android.app.ActivityThread$H.handleMessage (ActivityThread.java:1859)
      at android.os.Handler.dispatchMessage (Handler.java:106)
      at android.os.Looper.loop (Looper.java:201)
      at android.app.ActivityThread.main (ActivityThread.java:6831)
      at java.lang.reflect.Method.invoke (Method.java)
      at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run (RuntimeInit.java:547)
      at com.android.internal.os.ZygoteInit.main (ZygoteInit.java:927)
      
      
      
去查 DatabaseOpenHelper.queryData(DatabaseOpenHelper.java:13)

往下去找到SQLiteConnection.nativePrepareStatement (SQLiteConnection.java)
==只有Android 9.0出现问题==
1.因为sqllite是从Assets文件中拷贝到本地然后进行增删改查，先去对比设备中的sql的完整性，权限

    public void init() {
            if (!canLoadDateBase()) {
                 this.getReadableDatabase();
                 //这句话是关键
            this.close();
            
                try {
                    copyDatabaseFromAsset();
                } catch (IOException e) {
                    throw new Error("Error copying database");
                }
            }
        }
        
        
        
SQLite: No Such Table Error Android P problem
     https://stackoverflow.com/questions/52706557/sqlite-no-such-table-error-android-p-problem