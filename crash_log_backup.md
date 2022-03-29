## Crash Details

**Crash Thread**: `Thread[main,5,main]`  
**Crash Timestamp**: `2022-03-29 17:14:25.193 UTC`  

**Crash Message**:
```
Unable to start activity ComponentInfo{com.termux/com.termux.app.TermuxActivity}: java.lang.IllegalStateException: Not allowed to start service Intent { cmp=com.termux/.app.TermuxService }: app is in background uid UidRecord{5a5dbba u0a302 CEM  idle change:idle|cached procs:1 seq(0,0,0)}
```


### Stacktrace

```
java.lang.RuntimeException: Unable to start activity ComponentInfo{com.termux/com.termux.app.TermuxActivity}: java.lang.IllegalStateException: Not allowed to start service Intent { cmp=com.termux/.app.TermuxService }: app is in background uid UidRecord{5a5dbba u0a302 CEM  idle change:idle|cached procs:1 seq(0,0,0)}
	at android.app.ActivityThread.performLaunchActivity(ActivityThread.java:3537)
	at android.app.ActivityThread.handleLaunchActivity(ActivityThread.java:3692)
	at android.app.servertransaction.LaunchActivityItem.execute(LaunchActivityItem.java:83)
	at android.app.servertransaction.TransactionExecutor.executeCallbacks(TransactionExecutor.java:140)
	at android.app.servertransaction.TransactionExecutor.execute(TransactionExecutor.java:100)
	at android.app.ActivityThread$H.handleMessage(ActivityThread.java:2235)
	at android.os.Handler.dispatchMessage(Handler.java:107)
	at android.os.Looper.loop(Looper.java:240)
	at android.app.ActivityThread.main(ActivityThread.java:7829)
	at java.lang.reflect.Method.invoke(Native Method)
	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:512)
	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:1027)
Caused by: java.lang.IllegalStateException: Not allowed to start service Intent { cmp=com.termux/.app.TermuxService }: app is in background uid UidRecord{5a5dbba u0a302 CEM  idle change:idle|cached procs:1 seq(0,0,0)}
	at android.app.ContextImpl.startServiceCommon(ContextImpl.java:1675)
	at android.app.ContextImpl.startService(ContextImpl.java:1610)
	at android.content.ContextWrapper.startService(ContextWrapper.java:680)
	at com.termux.app.TermuxActivity.onCreate(TermuxActivity.java:242)
	at android.app.Activity.performCreate(Activity.java:7980)
	at android.app.Activity.performCreate(Activity.java:7969)
	at android.app.Instrumentation.callActivityOnCreate(Instrumentation.java:1306)
	at android.app.ActivityThread.performLaunchActivity(ActivityThread.java:3508)
	... 11 more

```
##


## Termux App Info

**APP_NAME**: `Termux`  
**PACKAGE_NAME**: `com.termux`  
**VERSION_NAME**: `0.118.0`  
**VERSION_CODE**: `118`  
**TARGET_SDK**: `28`  
**IS_DEBUGGABLE_BUILD**: `false`  
**APK_RELEASE**: `F-Droid`  
**SIGNING_CERTIFICATE_SHA256_DIGEST**: `228FB2CFE90831C1499EC3CCAF61E96E8E1CE70766B9474672CE427334D41C42`  
##


## Device Info

### Software

**OS_VERSION**: `4.9.190+`  
**SDK_INT**: `29`  
**RELEASE**: `10`  
**ID**: `QP1A.190711.020`  
**DISPLAY**: `CPH2185_11_A.39`  
**INCREMENTAL**: `1646657900`  
**SECURITY_PATCH**: `2022-02-05`  
**IS_DEBUGGABLE**: `0`  
**IS_TREBLE_ENABLED**: `true`  
**TYPE**: `user`  
**TAGS**: `release-keys`  

### Hardware

**MANUFACTURER**: `OPPO`  
**BRAND**: `OPPO`  
**MODEL**: `CPH2185`  
**PRODUCT**: `CPH2185T2`  
**BOARD**: `oppo6765`  
**HARDWARE**: `mt6765`  
**DEVICE**: `OP4F2F`  
**SUPPORTED_ABIS**: `arm64-v8a, armeabi-v7a, armeabi`  
##
