 <b>Android Week Planner Crashlytics<b>
 ___


# ![Android_robot svg](https://github.com/UserQA07/Week-Planner-/assets/144763744/5613d4b9-b88f-4c1f-84d3-6af9dae0e2ac)
![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/15a70dde-1ae8-46a9-b673-d2b842cf9844)
![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/9285a8ae-1f77-47eb-8297-9fbf90873140)
![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/9719cde5-c799-46da-a896-0c2004b4f414)
![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/89e3629f-d356-447d-9a5c-a32318a35c80)





<details>
 
  <summary>Android 13</summary><br>                                                

  <details>
 
<summary>Crash list</summary>

![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/9b1903c3-c2a1-4d66-a48e-eba4c0565dd9)

  </details>
 
<details>  



   
   <summary>Galaxy S23 Ultra</summary>
    
![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/0fa89e56-b7e7-41f3-b851-84aca2acdb63)


<details>
 
   *<summary>Details</summary>*
 
  Crashlytics - Stack trace
## Application: com.weeklyplannerapp.weekplan
## Platform: android
## Version: 7.97 (82)
## Issue: 72bd018209352c1b39c33f10f34b265c
## Session: 65576CCF036A0001693CFEA1C2636844_DNE_0_v2
## Date: Fri Nov 17 2023 15:42:19 GMT+0200 (Eastern European Standard Time)


# Fatal Exception: java.lang.RuntimeException: Unable to stop activity {com.weeklyplannerapp.weekplan/com.weeklyplannerapp.weekplan.View.Activities.MainActivity}: io.realm.exceptions.RealmFileException: Failed to open file at path '/data/data/com.weeklyplannerapp.weekplan/17.11.2023 16:42': parent directory does not exist (/data/data/com.weeklyplannerapp.weekplan/17.11.2023 16:42) in /tmp/realm-java/realm/realm-library/src/main/cpp/io_realm_internal_OsSharedRealm.cpp line 404 Kind: NOT_FOUND.
       at android.app.ActivityThread.callActivityOnStop(ActivityThread.java:5843)
       at android.app.ActivityThread.performStopActivityInner(ActivityThread.java:5809)
       at android.app.ActivityThread.handleStopActivity(ActivityThread.java:5880)
       at android.app.servertransaction.StopActivityItem.execute(StopActivityItem.java:43)
       at android.app.servertransaction.ActivityTransactionItem.execute(ActivityTransactionItem.java:45)
       at android.app.servertransaction.TransactionExecutor.executeLifecycleState(TransactionExecutor.java:176)
       at android.app.servertransaction.TransactionExecutor.execute(TransactionExecutor.java:97)
       at android.app.ActivityThread$H.handleMessage(ActivityThread.java:2574)
       at android.os.Handler.dispatchMessage(Handler.java:106)
       at android.os.Looper.loopOnce(Looper.java:226)
       at android.os.Looper.loop(Looper.java:313)
       at android.app.ActivityThread.main(ActivityThread.java:8762)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:604)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:1067)

# Caused by io.realm.exceptions.RealmFileException: Failed to open file at path '/data/data/com.weeklyplannerapp.weekplan/17.11.2023 16:42': parent directory does not exist (/data/data/com.weeklyplannerapp.weekplan/17.11.2023 16:42) in /tmp/realm-java/realm/realm-library/src/main/cpp/io_realm_internal_OsSharedRealm.cpp line 404
       at io.realm.internal.OsSharedRealm.nativeWriteCopy(OsSharedRealm.java)
       at io.realm.internal.OsSharedRealm.writeCopy(OsSharedRealm.java:38)
       at io.realm.BaseRealm.writeCopyTo(BaseRealm.java:1)
       at com.weeklyplannerapp.weekplan.WeeklyPlanApplication$1.onActivityStopped(WeeklyPlanApplication.java:199)
       at android.app.Application.dispatchActivityStopped(Application.java:510)
       at android.app.Activity.dispatchActivityStopped(Activity.java:1548)
       at android.app.Activity.onStop(Activity.java:2679)
       at androidx.fragment.app.FragmentActivity.onStop(FragmentActivity.java:1)
       at androidx.appcompat.app.AppCompatActivity.onStop(AppCompatActivity.java:1)
       at com.weeklyplannerapp.weekplan.View.Activities.MainActivity.onStop(MainActivity.java)
       at android.app.Instrumentation.callActivityOnStop(Instrumentation.java:1551)
       at android.app.Activity.performStop(Activity.java:8829)
       at android.app.ActivityThread.callActivityOnStop(ActivityThread.java:5835)
       at android.app.ActivityThread.performStopActivityInner(ActivityThread.java:5809)
       at android.app.ActivityThread.handleStopActivity(ActivityThread.java:5880)
       at android.app.servertransaction.StopActivityItem.execute(StopActivityItem.java:43)
       at android.app.servertransaction.ActivityTransactionItem.execute(ActivityTransactionItem.java:45)
       at android.app.servertransaction.TransactionExecutor.executeLifecycleState(TransactionExecutor.java:176)
       at android.app.servertransaction.TransactionExecutor.execute(TransactionExecutor.java:97)
       at android.app.ActivityThread$H.handleMessage(ActivityThread.java:2574)
       at android.os.Handler.dispatchMessage(Handler.java:106)
       at android.os.Looper.loopOnce(Looper.java:226)
       at android.os.Looper.loop(Looper.java:313)
       at android.app.ActivityThread.main(ActivityThread.java:8762)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:604)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:1067)

# pool-10-thread-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Timer-1:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.util.TimerThread.mainLoop(Timer.java:534)
       at java.util.TimerThread.run(Timer.java:513)

# OkHttp ConnectionPool:
       at java.lang.Object.wait(Object.java)
       at com.android.okhttp.ConnectionPool$1.run(ConnectionPool.java:106)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1145)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Okio Watchdog:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at com.android.okhttp.okio.AsyncTimeout.awaitTimeout(AsyncTimeout.java:313)
       at com.android.okhttp.okio.AsyncTimeout.access$000(AsyncTimeout.java:42)
       at com.android.okhttp.okio.AsyncTimeout$Watchdog.run(AsyncTimeout.java:288)

# PlayBillingLibrary-4:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Timer-0:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.util.TimerThread.mainLoop(Timer.java:534)
       at java.util.TimerThread.run(Timer.java:513)

# InsetsAnimations:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:335)
       at android.os.Looper.loopOnce(Looper.java:186)
       at android.os.Looper.loop(Looper.java:313)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# com.google.firebase.crashlytics.startup1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# AsyncTask #12:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.SynchronousQueue$TransferStack$SNode.block(SynchronousQueue.java:288)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:397)
       at java.util.concurrent.SynchronousQueue.take(SynchronousQueue.java:886)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# queued-work-looper:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:335)
       at android.os.Looper.loopOnce(Looper.java:186)
       at android.os.Looper.loop(Looper.java:313)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# RealmFinalizingDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:210)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:231)
       at io.realm.internal.FinalizerRunnable.run(FinalizerRunnable.java:3)
       at java.lang.Thread.run(Thread.java:1012)

# GmsDynamite:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at com.google.android.gms.dynamite.zza.run(zza.java:16)

# FinalizerWatchdogDaemon:
       at java.lang.Thread.sleep(Thread.java)
       at java.lang.Thread.sleep(Thread.java:450)
       at java.lang.Thread.sleep(Thread.java:355)
       at java.lang.Daemons$FinalizerWatchdogDaemon.sleepForNanos(Daemons.java:481)
       at java.lang.Daemons$FinalizerWatchdogDaemon.waitForProgress(Daemons.java:544)
       at java.lang.Daemons$FinalizerWatchdogDaemon.runInternal(Daemons.java:412)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# GLThread 54567:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at android.opengl.GLSurfaceView$GLThread.guardedRun(GLSurfaceView.java:1517)
       at android.opengl.GLSurfaceView$GLThread.run(GLSurfaceView.java:1287)

# PlayBillingLibrary-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #0:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# DefaultDispatcher-worker-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# ScionFrontendApi:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.awaitNanos(AbstractQueuedSynchronizer.java:1672)
       at java.util.concurrent.LinkedBlockingQueue.poll(LinkedBlockingQueue.java:460)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Crashlytics Exception Handler1:
       at dalvik.system.VMStack.getThreadStackTrace(VMStack.java)
       at java.lang.Thread.getStackTrace(Thread.java:1841)
       at java.lang.Thread.getAllStackTraces(Thread.java:1909)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateThreadsList(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateExecutionData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateEventApplicationData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.captureEventData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistEvent(SessionReportingCoordinator.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistFatalEvent(SessionReportingCoordinator.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsBackgroundWorker$3.then(CrashlyticsBackgroundWorker.java:16)
       at com.google.android.gms.tasks.zze.run(:8)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1145)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# FinalizerDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:210)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:231)
       at java.lang.Daemons$FinalizerDaemon.runInternal(Daemons.java:309)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# awaitEvenIfOnMainThread task continuation executor1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# DefaultDispatcher-worker-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# Firebase Background Thread #1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# DefaultDispatcher-worker-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# ReferenceQueueDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.lang.Daemons$ReferenceQueueDaemon.runInternal(Daemons.java:239)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# queued-work-looper-data:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# Measurement Worker:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at m.lk.run(:com.google.android.gms.dynamite_measurementdynamite@234414038@23.44.14 (190400-0):71)

# Firebase Blocking Thread #2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:401)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:903)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)
</details>

![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/c6266141-d4cf-4253-bdc0-3f0798adf938)

<details>
 
   *<summary>Details</summary>*
 
 # Crashlytics - Stack trace
# Application: com.weeklyplannerapp.weekplan
# Platform: android
# Version: 7.97 (82)
# Issue: 15de6de17a4ef536a9973eac7f5432c7
# Session: 6553CB3201EC000146B15ABEB28DBD62_DNE_0_v2
# Date: Tue Nov 14 2023 21:35:09 GMT+0200 (Eastern European Standard Time)

# Fatal Exception: java.lang.IndexOutOfBoundsException: replace (17 ... 27) ends beyond length 10
       at android.text.SpannableStringBuilder.checkRange(SpannableStringBuilder.java:1339)
       at android.text.SpannableStringBuilder.replace(SpannableStringBuilder.java:527)
       at androidx.emoji2.text.SpannableBuilder.replace(SpannableBuilder.java:4)
       at android.text.SpannableStringBuilder.delete(SpannableStringBuilder.java:232)
       at androidx.emoji2.text.SpannableBuilder.delete(SpannableBuilder.java:1)
       at androidx.emoji2.text.SpannableBuilder.delete(SpannableBuilder.java:1)
       at android.widget.TextView.deleteText_internal(TextView.java:14763)
       at android.widget.Editor.deleteSourceAfterLocalDrop(Editor.java:3447)
       at android.widget.Editor.onDrop(Editor.java:3427)
       at android.widget.TextView.onDragEvent(TextView.java:14611)
       at androidx.appcompat.widget.AppCompatEditText.onDragEvent(AppCompatEditText.java:92)
       at android.view.View.callDragEventHandler(View.java:29031)
       at android.view.View.dispatchDragEvent(View.java:29019)
       at android.view.ViewGroup.dispatchDragEvent(ViewGroup.java:1838)
       at android.view.ViewGroup.dispatchDragEvent(ViewGroup.java:1838)
       at android.view.ViewGroup.dispatchDragEvent(ViewGroup.java:1838)
       at android.view.ViewGroup.dispatchDragEvent(ViewGroup.java:1838)
       at android.view.ViewGroup.dispatchDragEvent(ViewGroup.java:1838)
       at android.view.ViewGroup.dispatchDragEvent(ViewGroup.java:1838)
       at android.view.ViewGroup.dispatchDragEvent(ViewGroup.java:1838)
       at android.view.ViewGroup.dispatchDragEvent(ViewGroup.java:1838)
       at android.view.ViewGroup.dispatchDragEvent(ViewGroup.java:1838)
       at android.view.ViewGroup.dispatchDragEvent(ViewGroup.java:1838)
       at android.view.ViewRootImpl.handleDragEvent(ViewRootImpl.java:9477)
       at android.view.ViewRootImpl.-$$Nest$mhandleDragEvent()
       at android.view.ViewRootImpl$ViewRootHandler.handleMessageImpl(ViewRootImpl.java:6845)
       at android.view.ViewRootImpl$ViewRootHandler.handleMessage(ViewRootImpl.java:6697)
       at android.os.Handler.dispatchMessage(Handler.java:106)
       at android.os.Looper.loopOnce(Looper.java:226)
       at android.os.Looper.loop(Looper.java:313)
       at android.app.ActivityThread.main(ActivityThread.java:8757)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:604)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:1067)

# PlayBillingLibrary-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Timer-60:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.util.TimerThread.mainLoop(Timer.java:534)
       at java.util.TimerThread.run(Timer.java:513)

# AsyncTask #13:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:401)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:903)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Timer-52:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.util.TimerThread.mainLoop(Timer.java:534)
       at java.util.TimerThread.run(Timer.java:513)

# Timer-58:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.util.TimerThread.mainLoop(Timer.java:534)
       at java.util.TimerThread.run(Timer.java:513)

# Firebase Background Thread #2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# Timer-63:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.util.TimerThread.mainLoop(Timer.java:534)
       at java.util.TimerThread.run(Timer.java:513)

# Firebase Background Thread #3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# InsetsAnimations:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:335)
       at android.os.Looper.loopOnce(Looper.java:186)
       at android.os.Looper.loop(Looper.java:313)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# Timer-56:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.util.TimerThread.mainLoop(Timer.java:534)
       at java.util.TimerThread.run(Timer.java:513)

# GmsDynamite:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at com.google.android.gms.dynamite.zza.run(zza.java:16)

# Crashlytics Exception Handler1:
       at dalvik.system.VMStack.getThreadStackTrace(VMStack.java)
       at java.lang.Thread.getStackTrace(Thread.java:1841)
       at java.lang.Thread.getAllStackTraces(Thread.java:1909)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateThreadsList(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateExecutionData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateEventApplicationData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.captureEventData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistEvent(SessionReportingCoordinator.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistFatalEvent(SessionReportingCoordinator.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsBackgroundWorker$3.then(CrashlyticsBackgroundWorker.java:16)
       at com.google.android.gms.tasks.zze.run(:8)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1145)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# DefaultDispatcher-worker-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# Timer-62:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.util.TimerThread.mainLoop(Timer.java:534)
       at java.util.TimerThread.run(Timer.java:513)

# PlayBillingLibrary-4:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Timer-61:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.util.TimerThread.mainLoop(Timer.java:534)
       at java.util.TimerThread.run(Timer.java:513)

# pool-11-thread-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Timer-1:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.util.TimerThread.mainLoop(Timer.java:534)
       at java.util.TimerThread.run(Timer.java:513)

# Okio Watchdog:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at com.android.okhttp.okio.AsyncTimeout.awaitTimeout(AsyncTimeout.java:313)
       at com.android.okhttp.okio.AsyncTimeout.access$000(AsyncTimeout.java:42)
       at com.android.okhttp.okio.AsyncTimeout$Watchdog.run(AsyncTimeout.java:288)

# AsyncTask #15:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:401)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:903)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Timer-59:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.util.TimerThread.mainLoop(Timer.java:534)
       at java.util.TimerThread.run(Timer.java:513)

# RealmFinalizingDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:210)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:231)
       at io.realm.internal.FinalizerRunnable.run(FinalizerRunnable.java:3)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Blocking Thread #2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:401)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:903)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# queued-work-looper-data:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# DefaultDispatcher-worker-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# ReferenceQueueDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.lang.Daemons$ReferenceQueueDaemon.runInternal(Daemons.java:239)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# Timer-0:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.util.TimerThread.mainLoop(Timer.java:534)
       at java.util.TimerThread.run(Timer.java:513)

# FinalizerDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:210)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:231)
       at java.lang.Daemons$FinalizerDaemon.runInternal(Daemons.java:309)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# queued-work-looper-data:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# DefaultDispatcher-worker-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# Timer-54:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.util.TimerThread.mainLoop(Timer.java:534)
       at java.util.TimerThread.run(Timer.java:513)

# Firebase Background Thread #0:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# Timer-55:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.util.TimerThread.mainLoop(Timer.java:534)
       at java.util.TimerThread.run(Timer.java:513)

# queued-work-looper:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:335)
       at android.os.Looper.loopOnce(Looper.java:186)
       at android.os.Looper.loop(Looper.java:313)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# OkHttp ConnectionPool:
       at java.lang.Object.wait(Object.java)
       at com.android.okhttp.ConnectionPool$1.run(ConnectionPool.java:106)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1145)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# awaitEvenIfOnMainThread task continuation executor1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# Timer-57:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.util.TimerThread.mainLoop(Timer.java:534)
       at java.util.TimerThread.run(Timer.java:513)

# ScionFrontendApi:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.awaitNanos(AbstractQueuedSynchronizer.java:1672)
       at java.util.concurrent.LinkedBlockingQueue.poll(LinkedBlockingQueue.java:460)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# GLThread 170:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at android.opengl.GLSurfaceView$GLThread.guardedRun(GLSurfaceView.java:1517)
       at android.opengl.GLSurfaceView$GLThread.run(GLSurfaceView.java:1287)

# Timer-53:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.util.TimerThread.mainLoop(Timer.java:534)
       at java.util.TimerThread.run(Timer.java:513)

# FinalizerWatchdogDaemon:
       at java.lang.Thread.sleep(Thread.java)
       at java.lang.Thread.sleep(Thread.java:450)
       at java.lang.Thread.sleep(Thread.java:355)
       at java.lang.Daemons$FinalizerWatchdogDaemon.sleepForNanos(Daemons.java:481)
       at java.lang.Daemons$FinalizerWatchdogDaemon.waitForProgress(Daemons.java:527)
       at java.lang.Daemons$FinalizerWatchdogDaemon.runInternal(Daemons.java:412)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# Measurement Worker:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at m.ll.run(:com.google.android.gms.dynamite_measurementdynamite@234313038@23.43.13 (190400-0):71)

# com.google.firebase.crashlytics.startup1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)
</details>


![banner](https://github.com/UserQA07/Week-Planner-/assets/144763744/ea9da887-5820-4cd9-93a5-5acfe45cf452)



<details>
 
   *<summary>Details</summary>*
 
 # Crashlytics - Stack trace
# Application: com.weeklyplannerapp.weekplan
# Platform: android
# Version: 7.97 (82)
# Issue: 60c774d70528f5fe5bf6b2bdbc3f771d
# Session: 65525C17012800010B975FDA306E8529_DNE_0_v2
# Date: Mon Nov 13 2023 22:46:52 GMT+0200 (Eastern European Standard Time)

# Fatal Exception: java.lang.IllegalStateException: Can't erase a recycled bitmap
       at android.graphics.Bitmap.checkRecycled(Bitmap.java:410)
       at android.graphics.Bitmap.eraseColor(Bitmap.java:1884)
       at com.weeklyplannerapp.weekplan.View.SupportClasses.CurlViewOpenGl.CurlPage.recycle(CurlPage.java:1)
       at com.weeklyplannerapp.weekplan.View.SupportClasses.CurlViewOpenGl.CurlPage.reset(CurlPage.java:1)
       at com.weeklyplannerapp.weekplan.View.SupportClasses.CurlViewOpenGl.CurlView.updatePage(CurlView.java:1)
       at com.weeklyplannerapp.weekplan.View.SupportClasses.CurlViewOpenGl.CurlView.updatePages(CurlView.java:79)
       at com.weeklyplannerapp.weekplan.View.SupportClasses.CurlViewOpenGl.CurlView.onPageSizeChanged(CurlView.java:1)
       at com.weeklyplannerapp.weekplan.View.SupportClasses.CurlViewOpenGl.CurlRenderer.updatePageRects(CurlRenderer.java:1)
       at com.weeklyplannerapp.weekplan.View.SupportClasses.CurlViewOpenGl.CurlRenderer.onSurfaceChanged(CurlRenderer.java:28)
       at android.opengl.GLSurfaceView$GLThread.guardedRun(GLSurfaceView.java:1577)
       at android.opengl.GLSurfaceView$GLThread.run(GLSurfaceView.java:1287)

# DefaultDispatcher-worker-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# Firebase Background Thread #0:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# FinalizerWatchdogDaemon:
       at java.lang.Thread.sleep(Thread.java)
       at java.lang.Thread.sleep(Thread.java:450)
       at java.lang.Thread.sleep(Thread.java:355)
       at java.lang.Daemons$FinalizerWatchdogDaemon.sleepForNanos(Daemons.java:481)
       at java.lang.Daemons$FinalizerWatchdogDaemon.waitForProgress(Daemons.java:544)
       at java.lang.Daemons$FinalizerWatchdogDaemon.runInternal(Daemons.java:412)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# queued-work-looper-data:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# DefaultDispatcher-worker-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# Crashlytics Exception Handler1:
       at dalvik.system.VMStack.getThreadStackTrace(VMStack.java)
       at java.lang.Thread.getStackTrace(Thread.java:1841)
       at java.lang.Thread.getAllStackTraces(Thread.java:1909)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateThreadsList(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateExecutionData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateEventApplicationData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.captureEventData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistEvent(SessionReportingCoordinator.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistFatalEvent(SessionReportingCoordinator.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsBackgroundWorker$3.then(CrashlyticsBackgroundWorker.java:16)
       at com.google.android.gms.tasks.zze.run(:8)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1145)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# RealmFinalizingDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:210)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:231)
       at io.realm.internal.FinalizerRunnable.run(FinalizerRunnable.java:3)
       at java.lang.Thread.run(Thread.java:1012)

# ScionFrontendApi:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.awaitNanos(AbstractQueuedSynchronizer.java:1672)
       at java.util.concurrent.LinkedBlockingQueue.poll(LinkedBlockingQueue.java:460)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# FinalizerDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:210)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:231)
       at java.lang.Daemons$FinalizerDaemon.runInternal(Daemons.java:309)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# InsetsAnimations:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:335)
       at android.os.Looper.loopOnce(Looper.java:186)
       at android.os.Looper.loop(Looper.java:313)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# PlayBillingLibrary-4:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# awaitEvenIfOnMainThread task continuation executor1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# com.google.firebase.crashlytics.startup1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# Measurement Worker:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at m.lk.run(:com.google.android.gms.dynamite_measurementdynamite@234414038@23.44.14 (190400-0):71)

# AsyncTask #10:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:401)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:903)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# queued-work-looper-data:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Blocking Thread #5:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:401)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:903)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# main:
       at android.graphics.BaseCanvas.nDrawBitmap(BaseCanvas.java)
       at android.graphics.BaseCanvas.drawBitmap(BaseCanvas.java:168)
       at android.graphics.Canvas.drawBitmap(Canvas.java:1604)
       at android.graphics.drawable.BitmapDrawable.draw(BitmapDrawable.java:560)
       at android.view.View.drawBackground(View.java:24682)
       at android.view.View.draw(View.java:24398)
       at android.view.View.buildDrawingCacheImpl(View.java:23664)
       at android.view.View.buildDrawingCache(View.java:23524)
       at com.weeklyplannerapp.weekplan.View.SupportClasses.Utils.BitmapUtils.viewToBitmap(BitmapUtils.java:1)
       at com.weeklyplannerapp.weekplan.View.Activities.MainActivity$PageProvider.lambda$updatePage$2(MainActivity.java:76)
       at android.app.Activity.runOnUiThread(Activity.java:7494)
       at com.weeklyplannerapp.weekplan.View.Activities.MainActivity$PageProvider.updatePage(MainActivity.java:38)
       at com.weeklyplannerapp.weekplan.View.SupportClasses.CurlViewOpenGl.CurlView.updatePage(CurlView.java:38)
       at com.weeklyplannerapp.weekplan.View.SupportClasses.CurlViewOpenGl.CurlView.updatePages(CurlView.java:79)
       at com.weeklyplannerapp.weekplan.View.Activities.MainActivity.O(MainActivity.java:3)
       at android.os.Handler.handleCallback(Handler.java:942)
       at android.os.Handler.dispatchMessage(Handler.java:99)
       at android.os.Looper.loopOnce(Looper.java:226)
       at android.os.Looper.loop(Looper.java:313)
       at android.app.ActivityThread.main(ActivityThread.java:8762)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:604)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:1067)

# queued-work-looper:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:335)
       at android.os.Looper.loopOnce(Looper.java:186)
       at android.os.Looper.loop(Looper.java:313)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# pool-11-thread-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# ReferenceQueueDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.lang.Daemons$ReferenceQueueDaemon.runInternal(Daemons.java:239)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# Timer-1:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.util.TimerThread.mainLoop(Timer.java:534)
       at java.util.TimerThread.run(Timer.java:513)

# DefaultDispatcher-worker-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# Firebase Background Thread #1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# AsyncTask #9:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:401)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:903)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Timer-0:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.util.TimerThread.mainLoop(Timer.java:534)
       at java.util.TimerThread.run(Timer.java:513)

# Okio Watchdog:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at com.android.okhttp.okio.AsyncTimeout.awaitTimeout(AsyncTimeout.java:313)
       at com.android.okhttp.okio.AsyncTimeout.access$000(AsyncTimeout.java:42)
       at com.android.okhttp.okio.AsyncTimeout$Watchdog.run(AsyncTimeout.java:288)

# GmsDynamite:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at com.google.android.gms.dynamite.zza.run(zza.java:16)
</details>
 </details>


<details>
 
   <summary>Redmi Note 11 Pro</summary>
    
![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/776f24f5-6afd-4ae0-a97f-ae4756984d66)

<details>
 
   *<summary>Details</summary>*
 
 # Crashlytics - Stack trace
# Application: com.weeklyplannerapp.weekplan
# Platform: android
# Version: 7.97 (82)
# Issue: 72bd018209352c1b39c33f10f34b265c
# Session: 6557B0730221000153CAF350374DDB9E_DNE_0_v2
# Date: Fri Nov 17 2023 20:28:02 GMT+0200 (Eastern European Standard Time)

# Fatal Exception: java.lang.RuntimeException: Unable to stop activity {com.weeklyplannerapp.weekplan/com.weeklyplannerapp.weekplan.View.Activities.MainActivity}: io.realm.exceptions.RealmFileException: Failed to open file at path '/data/data/com.weeklyplannerapp.weekplan/17.11.2023 21:28': parent directory does not exist (/data/data/com.weeklyplannerapp.weekplan/17.11.2023 21:28) in /tmp/realm-java/realm/realm-library/src/main/cpp/io_realm_internal_OsSharedRealm.cpp line 404 Kind: NOT_FOUND.
       at android.app.ActivityThread.callActivityOnStop(ActivityThread.java:5454)
       at android.app.ActivityThread.performStopActivityInner(ActivityThread.java:5426)
       at android.app.ActivityThread.handleStopActivity(ActivityThread.java:5491)
       at android.app.servertransaction.StopActivityItem.execute(StopActivityItem.java:43)
       at android.app.servertransaction.ActivityTransactionItem.execute(ActivityTransactionItem.java:45)
       at android.app.servertransaction.TransactionExecutor.executeLifecycleState(TransactionExecutor.java:176)
       at android.app.servertransaction.TransactionExecutor.execute(TransactionExecutor.java:97)
       at android.app.ActivityThread$H.handleMessage(ActivityThread.java:2437)
       at android.os.Handler.dispatchMessage(Handler.java:106)
       at android.os.Looper.loopOnce(Looper.java:211)
       at android.os.Looper.loop(Looper.java:300)
       at android.app.ActivityThread.main(ActivityThread.java:8294)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:580)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:1028)

# Caused by io.realm.exceptions.RealmFileException: Failed to open file at path '/data/data/com.weeklyplannerapp.weekplan/17.11.2023 21:28': parent directory does not exist (/data/data/com.weeklyplannerapp.weekplan/17.11.2023 21:28) in /tmp/realm-java/realm/realm-library/src/main/cpp/io_realm_internal_OsSharedRealm.cpp line 404
       at io.realm.internal.OsSharedRealm.nativeWriteCopy(OsSharedRealm.java)
       at io.realm.internal.OsSharedRealm.writeCopy(OsSharedRealm.java:38)
       at io.realm.BaseRealm.writeCopyTo(BaseRealm.java:1)
       at com.weeklyplannerapp.weekplan.WeeklyPlanApplication$1.onActivityStopped(WeeklyPlanApplication.java:199)
       at android.app.Application.dispatchActivityStopped(Application.java:503)
       at android.app.Activity.dispatchActivityStopped(Activity.java:1579)
       at android.app.Activity.onStop(Activity.java:2737)
       at androidx.fragment.app.FragmentActivity.onStop(FragmentActivity.java:1)
       at androidx.appcompat.app.AppCompatActivity.onStop(AppCompatActivity.java:1)
       at com.weeklyplannerapp.weekplan.View.Activities.MainActivity.onStop(MainActivity.java)
       at android.app.Instrumentation.callActivityOnStop(Instrumentation.java:1604)
       at android.app.Activity.performStop(Activity.java:8794)
       at android.app.ActivityThread.callActivityOnStop(ActivityThread.java:5446)
       at android.app.ActivityThread.performStopActivityInner(ActivityThread.java:5426)
       at android.app.ActivityThread.handleStopActivity(ActivityThread.java:5491)
       at android.app.servertransaction.StopActivityItem.execute(StopActivityItem.java:43)
       at android.app.servertransaction.ActivityTransactionItem.execute(ActivityTransactionItem.java:45)
       at android.app.servertransaction.TransactionExecutor.executeLifecycleState(TransactionExecutor.java:176)
       at android.app.servertransaction.TransactionExecutor.execute(TransactionExecutor.java:97)
       at android.app.ActivityThread$H.handleMessage(ActivityThread.java:2437)
       at android.os.Handler.dispatchMessage(Handler.java:106)
       at android.os.Looper.loopOnce(Looper.java:211)
       at android.os.Looper.loop(Looper.java:300)
       at android.app.ActivityThread.main(ActivityThread.java:8294)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:580)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:1028)

# com.google.firebase.crashlytics.startup1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# ReferenceQueueDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at java.lang.Daemons$ReferenceQueueDaemon.runInternal(Daemons.java:232)
       at java.lang.Daemons$Daemon.run(Daemons.java:140)
       at java.lang.Thread.run(Thread.java:1012)

# LogThread:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:341)
       at android.os.Looper.loopOnce(Looper.java:169)
       at android.os.Looper.loop(Looper.java:300)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# process reaper:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:234)
       at java.util.concurrent.SynchronousQueue$TransferStack.awaitFulfill(SynchronousQueue.java:463)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:361)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:939)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1062)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# Okio Watchdog:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at com.android.okhttp.okio.AsyncTimeout.awaitTimeout(AsyncTimeout.java:313)
       at com.android.okhttp.okio.AsyncTimeout.access$000(AsyncTimeout.java:42)
       at com.android.okhttp.okio.AsyncTimeout$Watchdog.run(AsyncTimeout.java:288)

# AsyncTask #5:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.SynchronousQueue$TransferStack.awaitFulfill(SynchronousQueue.java:461)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:361)
       at java.util.concurrent.SynchronousQueue.take(SynchronousQueue.java:922)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# launch:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:341)
       at android.os.Looper.loopOnce(Looper.java:169)
       at android.os.Looper.loop(Looper.java:300)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# awaitEvenIfOnMainThread task continuation executor1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #0:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# FramePolicy:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:341)
       at android.os.Looper.loopOnce(Looper.java:169)
       at android.os.Looper.loop(Looper.java:300)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# AnimThread-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.SynchronousQueue$TransferStack.awaitFulfill(SynchronousQueue.java:461)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:361)
       at java.util.concurrent.SynchronousQueue.take(SynchronousQueue.java:922)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# AnimRunnerThread:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:341)
       at android.os.Looper.loopOnce(Looper.java:169)
       at android.os.Looper.loop(Looper.java:300)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# ScionFrontendApi:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:234)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.awaitNanos(AbstractQueuedSynchronizer.java:2123)
       at java.util.concurrent.LinkedBlockingQueue.poll(LinkedBlockingQueue.java:458)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1062)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# DefaultDispatcher-worker-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:357)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# DefaultDispatcher-worker-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:357)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# Crashlytics Exception Handler1:
       at dalvik.system.VMStack.getThreadStackTrace(VMStack.java)
       at java.lang.Thread.getStackTrace(Thread.java:1841)
       at java.lang.Thread.getAllStackTraces(Thread.java:1909)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateThreadsList(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateExecutionData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateEventApplicationData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.captureEventData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistEvent(SessionReportingCoordinator.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistFatalEvent(SessionReportingCoordinator.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsBackgroundWorker$3.then(CrashlyticsBackgroundWorker.java:16)
       at com.google.android.gms.tasks.zze.run(:8)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1137)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# GmsDynamite:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at com.google.android.gms.dynamite.zza.run(zza.java:16)

# RealmFinalizingDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:203)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:224)
       at io.realm.internal.FinalizerRunnable.run(FinalizerRunnable.java:3)
       at java.lang.Thread.run(Thread.java:1012)

# FinalizerDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:203)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:224)
       at java.lang.Daemons$FinalizerDaemon.runInternal(Daemons.java:300)
       at java.lang.Daemons$Daemon.run(Daemons.java:140)
       at java.lang.Thread.run(Thread.java:1012)

# Timer-0:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at java.util.TimerThread.mainLoop(Timer.java:534)
       at java.util.TimerThread.run(Timer.java:513)

# InsetsAnimations:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:341)
       at android.os.Looper.loopOnce(Looper.java:169)
       at android.os.Looper.loop(Looper.java:300)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# ScrollPolicy:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:341)
       at android.os.Looper.loopOnce(Looper.java:169)
       at android.os.Looper.loop(Looper.java:300)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# OkHttp ConnectionPool:
       at java.lang.Object.wait(Object.java)
       at com.android.okhttp.ConnectionPool$1.run(ConnectionPool.java:106)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1137)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# GLThread 20118:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at android.opengl.GLSurfaceView$GLThread.guardedRun(GLSurfaceView.java:1505)
       at android.opengl.GLSurfaceView$GLThread.run(GLSurfaceView.java:1280)

# Timer-1:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at java.util.TimerThread.mainLoop(Timer.java:534)
       at java.util.TimerThread.run(Timer.java:513)

# queued-work-looper:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:341)
       at android.os.Looper.loopOnce(Looper.java:169)
       at android.os.Looper.loop(Looper.java:300)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# pool-9-thread-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# FinalizerWatchdogDaemon:
       at java.lang.Thread.sleep(Thread.java)
       at java.lang.Thread.sleep(Thread.java:450)
       at java.lang.Thread.sleep(Thread.java:355)
       at java.lang.Daemons$FinalizerWatchdogDaemon.sleepForNanos(Daemons.java:438)
       at java.lang.Daemons$FinalizerWatchdogDaemon.waitForProgress(Daemons.java:480)
       at java.lang.Daemons$FinalizerWatchdogDaemon.runInternal(Daemons.java:369)
       at java.lang.Daemons$Daemon.run(Daemons.java:140)
       at java.lang.Thread.run(Thread.java:1012)

# DefaultDispatcher-worker-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:357)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# Firebase Background Thread #3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Blocking Thread #1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:234)
       at java.util.concurrent.SynchronousQueue$TransferStack.awaitFulfill(SynchronousQueue.java:463)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:361)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:939)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1062)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# Measurement Worker:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at m.lk.run(:com.google.android.gms.dynamite_measurementdynamite@234414038@23.44.14 (190400-0):71)

</details>

![Screenshot 2023-11-18 120323](https://github.com/UserQA07/Week-Planner-/assets/144763744/83e34f46-4cde-4834-ba2f-6d5a425804c8)


<details>
 
   *<summary>Details</summary>*
 
 # Crashlytics - Stack trace
# Application: com.weeklyplannerapp.weekplan
# Platform: android
# Version: 7.97 (82)
# Issue: 097370c30da6a1331a1a06941b9e3cb9
# Session: 6554ECB8025F00011F874BD5A9F24A42_DNE_0_v2
# Date: Wed Nov 15 2023 18:09:24 GMT+0200 (Eastern European Standard Time)

# Fatal Exception: java.lang.IndexOutOfBoundsException: input indexes are outside the CharSequence
       at miuix.toolbar.util.WordIterator.setCharSequence(WordIterator.java:46)
       at miuix.toolbar.internal.TextActionView.selectCurrentWord(TextActionView.java:186)
       at miuix.toolbar.internal.TextActionView.selectCurrentWord(TextActionView.java:158)
       at miuix.toolbar.internal.ActionView.selectCurrentWord(ActionView.java:61)
       at miuix.textaction.Select$1.onMenuItemClick(Select.java:25)
       at miuix.toolbar.internal.menu.MenuItemImpl.invoke(MenuItemImpl.java:142)
       at miuix.toolbar.internal.menu.MenuBuilder.performItemAction(MenuBuilder.java:938)
       at miuix.toolbar.FloatingActionMode$4.onMenuItemClick(FloatingActionMode.java:123)
       at miuix.toolbar.internal.FloatingToolbar$3.onClick(FloatingToolbar.java:193)
       at android.view.View.performClick(View.java:7575)
       at android.view.View.performClickInternal(View.java:7548)
       at android.view.View.-$$Nest$mperformClickInternal()
       at android.view.View$PerformClick.run(View.java:29848)
       at android.os.Handler.handleCallback(Handler.java:942)
       at android.os.Handler.dispatchMessage(Handler.java:99)
       at android.os.Looper.loopOnce(Looper.java:211)
       at android.os.Looper.loop(Looper.java:300)
       at android.app.ActivityThread.main(ActivityThread.java:8294)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:580)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:1028)

# ScrollPolicy:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:341)
       at android.os.Looper.loopOnce(Looper.java:169)
       at android.os.Looper.loop(Looper.java:300)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# GLThread 194:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at android.opengl.GLSurfaceView$GLThread.guardedRun(GLSurfaceView.java:1505)
       at android.opengl.GLSurfaceView$GLThread.run(GLSurfaceView.java:1280)

# com.google.firebase.crashlytics.startup1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# AnimThread-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.SynchronousQueue$TransferStack$SNode.block(SynchronousQueue.java:288)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:397)
       at java.util.concurrent.SynchronousQueue.take(SynchronousQueue.java:886)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# pool-10-thread-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# AnimThread-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.SynchronousQueue$TransferStack$SNode.block(SynchronousQueue.java:288)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:397)
       at java.util.concurrent.SynchronousQueue.take(SynchronousQueue.java:886)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# AsyncTask #9:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:401)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:903)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# FinalizerDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:210)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:231)
       at java.lang.Daemons$FinalizerDaemon.runInternal(Daemons.java:309)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# DefaultDispatcher-worker-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# DefaultDispatcher-worker-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# PlayBillingLibrary-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# RealmFinalizingDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:210)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:231)
       at io.realm.internal.FinalizerRunnable.run(FinalizerRunnable.java:3)
       at java.lang.Thread.run(Thread.java:1012)

# Okio Watchdog:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at com.android.okhttp.okio.AsyncTimeout.awaitTimeout(AsyncTimeout.java:313)
       at com.android.okhttp.okio.AsyncTimeout.access$000(AsyncTimeout.java:42)
       at com.android.okhttp.okio.AsyncTimeout$Watchdog.run(AsyncTimeout.java:288)

# DefaultDispatcher-worker-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# Firebase Background Thread #2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# AnimThread-4:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.SynchronousQueue$TransferStack$SNode.block(SynchronousQueue.java:288)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:397)
       at java.util.concurrent.SynchronousQueue.take(SynchronousQueue.java:886)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# OkHttp ConnectionPool:
       at java.lang.Object.wait(Object.java)
       at com.android.okhttp.ConnectionPool$1.run(ConnectionPool.java:106)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1145)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# AnimThread-5:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.SynchronousQueue$TransferStack$SNode.block(SynchronousQueue.java:288)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:397)
       at java.util.concurrent.SynchronousQueue.take(SynchronousQueue.java:886)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Timer-1:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.util.TimerThread.mainLoop(Timer.java:534)
       at java.util.TimerThread.run(Timer.java:513)

# awaitEvenIfOnMainThread task continuation executor1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# LogThread:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:341)
       at android.os.Looper.loopOnce(Looper.java:169)
       at android.os.Looper.loop(Looper.java:300)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# PlayBillingLibrary-4:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# launch:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:341)
       at android.os.Looper.loopOnce(Looper.java:169)
       at android.os.Looper.loop(Looper.java:300)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# GmsDynamite:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at com.google.android.gms.dynamite.zza.run(zza.java:16)

# Crashlytics Exception Handler1:
       at dalvik.system.VMStack.getThreadStackTrace(VMStack.java)
       at java.lang.Thread.getStackTrace(Thread.java:1841)
       at java.lang.Thread.getAllStackTraces(Thread.java:1909)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateThreadsList(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateExecutionData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateEventApplicationData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.captureEventData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistEvent(SessionReportingCoordinator.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistFatalEvent(SessionReportingCoordinator.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsBackgroundWorker$3.then(CrashlyticsBackgroundWorker.java:16)
       at com.google.android.gms.tasks.zze.run(:8)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1145)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# AnimThread-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.SynchronousQueue$TransferStack$SNode.block(SynchronousQueue.java:288)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:397)
       at java.util.concurrent.SynchronousQueue.take(SynchronousQueue.java:886)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# FramePolicy:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:341)
       at android.os.Looper.loopOnce(Looper.java:169)
       at android.os.Looper.loop(Looper.java:300)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# InsetsAnimations:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:341)
       at android.os.Looper.loopOnce(Looper.java:169)
       at android.os.Looper.loop(Looper.java:300)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# magnifier pixel copy result handler:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:341)
       at android.os.Looper.loopOnce(Looper.java:169)
       at android.os.Looper.loop(Looper.java:300)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# process reaper:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:401)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:903)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# Timer-0:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.util.TimerThread.mainLoop(Timer.java:534)
       at java.util.TimerThread.run(Timer.java:513)

queued-work-looper:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:341)
       at android.os.Looper.loopOnce(Looper.java:169)
       at android.os.Looper.loop(Looper.java:300)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# PlayBillingLibrary-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# AsyncTask #7:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:401)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:903)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# ReferenceQueueDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.lang.Daemons$ReferenceQueueDaemon.runInternal(Daemons.java:239)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# FinalizerWatchdogDaemon:
       at java.lang.Thread.sleep(Thread.java)
       at java.lang.Thread.sleep(Thread.java:450)
       at java.lang.Thread.sleep(Thread.java:355)
       at java.lang.Daemons$FinalizerWatchdogDaemon.sleepForNanos(Daemons.java:481)
       at java.lang.Daemons$FinalizerWatchdogDaemon.waitForProgress(Daemons.java:544)
       at java.lang.Daemons$FinalizerWatchdogDaemon.runInternal(Daemons.java:412)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# AnimRunnerThread:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:341)
       at android.os.Looper.loopOnce(Looper.java:169)
       at android.os.Looper.loop(Looper.java:300)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# Firebase Background Thread #0:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)
</details>
 </details>


  <details>
   
   <summary>Redmi Note 11 Pro 5G</summary> 

![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/ff8a189c-5a06-454e-8c15-13551d8704c9)

<details>
 
   *<summary>Details</summary>*
    
 # Crashlytics - Stack trace
# Application: com.weeklyplannerapp.weekplan
# Platform: android
# Version: 7.97 (82)
# Issue: 72bd018209352c1b39c33f10f34b265c
# Session: 6557CB0103D5000113698EC20F765155_DNE_0_v2
# Date: Fri Nov 17 2023 22:20:43 GMT+0200 (Eastern European Standard Time)

# Fatal Exception: java.lang.RuntimeException: Unable to stop activity {com.weeklyplannerapp.weekplan/com.weeklyplannerapp.weekplan.View.Activities.MainActivity}: io.realm.exceptions.RealmFileException: Failed to open file at path '/data/data/com.weeklyplannerapp.weekplan/17.11.2023 17:20': parent directory does not exist (/data/data/com.weeklyplannerapp.weekplan/17.11.2023 17:20) in /tmp/realm-java/realm/realm-library/src/main/cpp/io_realm_internal_OsSharedRealm.cpp line 404 Kind: NOT_FOUND.
       at android.app.ActivityThread.callActivityOnStop(ActivityThread.java:5483)
       at android.app.ActivityThread.performStopActivityInner(ActivityThread.java:5455)
       at android.app.ActivityThread.handleStopActivity(ActivityThread.java:5520)
       at android.app.servertransaction.StopActivityItem.execute(StopActivityItem.java:43)
       at android.app.servertransaction.ActivityTransactionItem.execute(ActivityTransactionItem.java:45)
       at android.app.servertransaction.TransactionExecutor.executeLifecycleState(TransactionExecutor.java:176)
       at android.app.servertransaction.TransactionExecutor.execute(TransactionExecutor.java:97)
       at android.app.ActivityThread$H.handleMessage(ActivityThread.java:2415)
       at android.os.Handler.dispatchMessage(Handler.java:106)
       at android.os.Looper.loopOnce(Looper.java:211)
       at android.os.Looper.loop(Looper.java:300)
       at android.app.ActivityThread.main(ActivityThread.java:8410)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:559)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:954)

# Caused by io.realm.exceptions.RealmFileException: Failed to open file at path '/data/data/com.weeklyplannerapp.weekplan/17.11.2023 17:20': parent directory does not exist (/data/data/com.weeklyplannerapp.weekplan/17.11.2023 17:20) in /tmp/realm-java/realm/realm-library/src/main/cpp/io_realm_internal_OsSharedRealm.cpp line 404
       at io.realm.internal.OsSharedRealm.nativeWriteCopy(OsSharedRealm.java)
       at io.realm.internal.OsSharedRealm.writeCopy(OsSharedRealm.java:38)
       at io.realm.BaseRealm.writeCopyTo(BaseRealm.java:1)
       at com.weeklyplannerapp.weekplan.WeeklyPlanApplication$1.onActivityStopped(WeeklyPlanApplication.java:199)
       at android.app.Application.dispatchActivityStopped(Application.java:503)
       at android.app.Activity.dispatchActivityStopped(Activity.java:1580)
       at android.app.Activity.onStop(Activity.java:2738)
       at androidx.fragment.app.FragmentActivity.onStop(FragmentActivity.java:1)
       at androidx.appcompat.app.AppCompatActivity.onStop(AppCompatActivity.java:1)
       at com.weeklyplannerapp.weekplan.View.Activities.MainActivity.onStop(MainActivity.java)
       at android.app.Instrumentation.callActivityOnStop(Instrumentation.java:1607)
       at android.app.Activity.performStop(Activity.java:8796)
       at android.app.ActivityThread.callActivityOnStop(ActivityThread.java:5475)
       at android.app.ActivityThread.performStopActivityInner(ActivityThread.java:5455)
       at android.app.ActivityThread.handleStopActivity(ActivityThread.java:5520)
       at android.app.servertransaction.StopActivityItem.execute(StopActivityItem.java:43)
       at android.app.servertransaction.ActivityTransactionItem.execute(ActivityTransactionItem.java:45)
       at android.app.servertransaction.TransactionExecutor.executeLifecycleState(TransactionExecutor.java:176)
       at android.app.servertransaction.TransactionExecutor.execute(TransactionExecutor.java:97)
       at android.app.ActivityThread$H.handleMessage(ActivityThread.java:2415)
       at android.os.Handler.dispatchMessage(Handler.java:106)
       at android.os.Looper.loopOnce(Looper.java:211)
       at android.os.Looper.loop(Looper.java:300)
       at android.app.ActivityThread.main(ActivityThread.java:8410)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:559)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:954)

# FinalizerDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:210)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:231)
       at java.lang.Daemons$FinalizerDaemon.runInternal(Daemons.java:309)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# FinalizerWatchdogDaemon:
       at java.lang.Thread.sleep(Thread.java)
       at java.lang.Thread.sleep(Thread.java:450)
       at java.lang.Thread.sleep(Thread.java:355)
       at java.lang.Daemons$FinalizerWatchdogDaemon.sleepForNanos(Daemons.java:481)
       at java.lang.Daemons$FinalizerWatchdogDaemon.waitForProgress(Daemons.java:544)
       at java.lang.Daemons$FinalizerWatchdogDaemon.runInternal(Daemons.java:412)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# Crashlytics Exception Handler1:
       at dalvik.system.VMStack.getThreadStackTrace(VMStack.java)
       at java.lang.Thread.getStackTrace(Thread.java:1841)
       at java.lang.Thread.getAllStackTraces(Thread.java:1909)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateThreadsList(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateExecutionData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateEventApplicationData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.captureEventData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistEvent(SessionReportingCoordinator.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistFatalEvent(SessionReportingCoordinator.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsBackgroundWorker$3.then(CrashlyticsBackgroundWorker.java:16)
       at com.google.android.gms.tasks.zze.run(:8)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1145)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# AsyncTask #1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.SynchronousQueue$TransferStack$SNode.block(SynchronousQueue.java:288)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:397)
       at java.util.concurrent.SynchronousQueue.take(SynchronousQueue.java:886)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# DefaultDispatcher-worker-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# PlayBillingLibrary-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# DefaultDispatcher-worker-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# ScionFrontendApi:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.awaitNanos(AbstractQueuedSynchronizer.java:1672)
       at java.util.concurrent.LinkedBlockingQueue.poll(LinkedBlockingQueue.java:460)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# ReferenceQueueDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.lang.Daemons$ReferenceQueueDaemon.runInternal(Daemons.java:239)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #0:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# awaitEvenIfOnMainThread task continuation executor1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# Timer-0:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.util.TimerThread.mainLoop(Timer.java:534)
       at java.util.TimerThread.run(Timer.java:513)

# Firebase Background Thread #3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# DefaultDispatcher-worker-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# GLThread 350612:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at android.opengl.GLSurfaceView$GLThread.guardedRun(GLSurfaceView.java:1497)
       at android.opengl.GLSurfaceView$GLThread.run(GLSurfaceView.java:1272)

# RealmFinalizingDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:210)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:231)
       at io.realm.internal.FinalizerRunnable.run(FinalizerRunnable.java:3)
       at java.lang.Thread.run(Thread.java:1012)

# com.google.firebase.crashlytics.startup1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# Measurement Worker:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at m.lk.run(:com.google.android.gms.dynamite_measurementdynamite@234414038@23.44.14 (190400-0):71)

# pool-9-thread-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Blocking Thread #0:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:401)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:903)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# Timer-1:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.util.TimerThread.mainLoop(Timer.java:534)
       at java.util.TimerThread.run(Timer.java:513)

# queued-work-looper:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:341)
       at android.os.Looper.loopOnce(Looper.java:169)
       at android.os.Looper.loop(Looper.java:300)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# GmsDynamite:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at com.google.android.gms.dynamite.zza.run(zza.java:16)

# Firebase Background Thread #1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-4:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)
</details>
 </details>

 <details>
  
   <summary>Redmi Note 10 Pro</summary>

![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/5341a189-ca1b-43e3-85e3-81a7ef5feae3)


<details>
 
   *<summary>Details</summary>*
 
 # Crashlytics - Stack trace
# Application: com.weeklyplannerapp.weekplan
# Platform: android
# Version: 7.97 (82)
# Issue: 72bd018209352c1b39c33f10f34b265c
# Session: 65522AFC000400013CCDF1E36BA2C08E_DNE_0_v2
# Date: Mon Nov 13 2023 15:58:44 GMT+0200 (Eastern European Standard Time)

# Fatal Exception: java.lang.RuntimeException: Unable to stop activity {com.weeklyplannerapp.weekplan/com.weeklyplannerapp.weekplan.View.Activities.MainActivity}: io.realm.exceptions.RealmFileException: Failed to open file at path '/data/data/com.weeklyplannerapp.weekplan/13.11.2023 14:58': parent directory does not exist (/data/data/com.weeklyplannerapp.weekplan/13.11.2023 14:58) in /tmp/realm-java/realm/realm-library/src/main/cpp/io_realm_internal_OsSharedRealm.cpp line 404 Kind: NOT_FOUND.
       at android.app.ActivityThread.callActivityOnStop(ActivityThread.java:5393)
       at android.app.ActivityThread.performStopActivityInner(ActivityThread.java:5365)
       at android.app.ActivityThread.handleStopActivity(ActivityThread.java:5430)
       at android.app.servertransaction.StopActivityItem.execute(StopActivityItem.java:43)
       at android.app.servertransaction.ActivityTransactionItem.execute(ActivityTransactionItem.java:45)
       at android.app.servertransaction.TransactionExecutor.executeLifecycleState(TransactionExecutor.java:176)
       at android.app.servertransaction.TransactionExecutor.execute(TransactionExecutor.java:97)
       at android.app.ActivityThread$H.handleMessage(ActivityThread.java:2394)
       at android.os.Handler.dispatchMessage(Handler.java:106)
       at android.os.Looper.loopOnce(Looper.java:211)
       at android.os.Looper.loop(Looper.java:300)
       at android.app.ActivityThread.main(ActivityThread.java:8296)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:559)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:954)

# Caused by io.realm.exceptions.RealmFileException: Failed to open file at path '/data/data/com.weeklyplannerapp.weekplan/13.11.2023 14:58': parent directory does not exist (/data/data/com.weeklyplannerapp.weekplan/13.11.2023 14:58) in /tmp/realm-java/realm/realm-library/src/main/cpp/io_realm_internal_OsSharedRealm.cpp line 404
       at io.realm.internal.OsSharedRealm.nativeWriteCopy(OsSharedRealm.java)
       at io.realm.internal.OsSharedRealm.writeCopy(OsSharedRealm.java:38)
       at io.realm.BaseRealm.writeCopyTo(BaseRealm.java:1)
       at com.weeklyplannerapp.weekplan.WeeklyPlanApplication$1.onActivityStopped(WeeklyPlanApplication.java:199)
       at android.app.Application.dispatchActivityStopped(Application.java:500)
       at android.app.Activity.dispatchActivityStopped(Activity.java:1578)
       at android.app.Activity.onStop(Activity.java:2736)
       at androidx.fragment.app.FragmentActivity.onStop(FragmentActivity.java:1)
       at androidx.appcompat.app.AppCompatActivity.onStop(AppCompatActivity.java:1)
       at com.weeklyplannerapp.weekplan.View.Activities.MainActivity.onStop(MainActivity.java)
       at android.app.Instrumentation.callActivityOnStop(Instrumentation.java:1605)
       at android.app.Activity.performStop(Activity.java:8779)
       at android.app.ActivityThread.callActivityOnStop(ActivityThread.java:5385)
       at android.app.ActivityThread.performStopActivityInner(ActivityThread.java:5365)
       at android.app.ActivityThread.handleStopActivity(ActivityThread.java:5430)
       at android.app.servertransaction.StopActivityItem.execute(StopActivityItem.java:43)
       at android.app.servertransaction.ActivityTransactionItem.execute(ActivityTransactionItem.java:45)
       at android.app.servertransaction.TransactionExecutor.executeLifecycleState(TransactionExecutor.java:176)
       at android.app.servertransaction.TransactionExecutor.execute(TransactionExecutor.java:97)
       at android.app.ActivityThread$H.handleMessage(ActivityThread.java:2394)
       at android.os.Handler.dispatchMessage(Handler.java:106)
       at android.os.Looper.loopOnce(Looper.java:211)
       at android.os.Looper.loop(Looper.java:300)
       at android.app.ActivityThread.main(ActivityThread.java:8296)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:559)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:954)

# Crashlytics Exception Handler1:
       at dalvik.system.VMStack.getThreadStackTrace(VMStack.java)
       at java.lang.Thread.getStackTrace(Thread.java:1841)
       at java.lang.Thread.getAllStackTraces(Thread.java:1909)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateThreadsList(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateExecutionData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateEventApplicationData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.captureEventData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistEvent(SessionReportingCoordinator.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistFatalEvent(SessionReportingCoordinator.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsBackgroundWorker$3.then(CrashlyticsBackgroundWorker.java:16)
       at com.google.android.gms.tasks.zze.run(:8)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1137)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# glide-source-thread-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.PriorityBlockingQueue.take(PriorityBlockingQueue.java:549)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultThreadFactory$1.run(GlideExecutor.java:2022)
       at java.lang.Thread.run(Thread.java:1012)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultPriorityThreadFactory$1.run(GlideExecutor.java:12)

# Okio Watchdog:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at com.android.okhttp.okio.AsyncTimeout.awaitTimeout(AsyncTimeout.java:313)
       at com.android.okhttp.okio.AsyncTimeout.access$000(AsyncTimeout.java:42)
       at com.android.okhttp.okio.AsyncTimeout$Watchdog.run(AsyncTimeout.java:288)

# glide-source-thread-0:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.PriorityBlockingQueue.take(PriorityBlockingQueue.java:549)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultThreadFactory$1.run(GlideExecutor.java:2022)
       at java.lang.Thread.run(Thread.java:1012)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultPriorityThreadFactory$1.run(GlideExecutor.java:12)

# FinalizerDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:203)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:224)
       at java.lang.Daemons$FinalizerDaemon.runInternal(Daemons.java:300)
       at java.lang.Daemons$Daemon.run(Daemons.java:140)
       at java.lang.Thread.run(Thread.java:1012)

# ConnectivityThread:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:341)
       at android.os.Looper.loopOnce(Looper.java:169)
       at android.os.Looper.loop(Looper.java:300)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# PlayBillingLibrary-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# glide-disk-cache-thread-0:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.PriorityBlockingQueue.take(PriorityBlockingQueue.java:549)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultThreadFactory$1.run(GlideExecutor.java:2022)
       at java.lang.Thread.run(Thread.java:1012)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultPriorityThreadFactory$1.run(GlideExecutor.java:12)

# Firebase Background Thread #3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# GmsDynamite:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at com.google.android.gms.dynamite.zza.run(zza.java:16)

# DefaultDispatcher-worker-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:357)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# DefaultDispatcher-worker-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:357)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# ScionFrontendApi:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:234)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.awaitNanos(AbstractQueuedSynchronizer.java:2123)
       at java.util.concurrent.LinkedBlockingQueue.poll(LinkedBlockingQueue.java:458)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1062)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# glide-source-thread-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.PriorityBlockingQueue.take(PriorityBlockingQueue.java:549)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultThreadFactory$1.run(GlideExecutor.java:2022)
       at java.lang.Thread.run(Thread.java:1012)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultPriorityThreadFactory$1.run(GlideExecutor.java:12)

# InsetsAnimations:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:341)
       at android.os.Looper.loopOnce(Looper.java:169)
       at android.os.Looper.loop(Looper.java:300)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# AsyncTask #6:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.SynchronousQueue$TransferStack.awaitFulfill(SynchronousQueue.java:461)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:361)
       at java.util.concurrent.SynchronousQueue.take(SynchronousQueue.java:922)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# glide-source-thread-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.PriorityBlockingQueue.take(PriorityBlockingQueue.java:549)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultThreadFactory$1.run(GlideExecutor.java:2022)
       at java.lang.Thread.run(Thread.java:1012)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultPriorityThreadFactory$1.run(GlideExecutor.java:12)

# DefaultDispatcher-worker-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:357)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# GLThread 9013:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at android.opengl.GLSurfaceView$GLThread.guardedRun(GLSurfaceView.java:1497)
       at android.opengl.GLSurfaceView$GLThread.run(GLSurfaceView.java:1272)

# Firebase Blocking Thread #1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:234)
       at java.util.concurrent.SynchronousQueue$TransferStack.awaitFulfill(SynchronousQueue.java:463)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:361)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:939)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1062)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# OkHttp ConnectionPool:
       at java.lang.Object.wait(Object.java)
       at com.android.okhttp.ConnectionPool$1.run(ConnectionPool.java:106)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1137)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #0:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# pool-9-thread-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# glide-active-resources:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:203)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:224)
       at com.bumptech.glide.load.engine.ActiveResources.cleanReferenceQueue(ActiveResources.java:320)
       at com.bumptech.glide.load.engine.ActiveResources$2.run(ActiveResources.java:320)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1137)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.bumptech.glide.load.engine.ActiveResources$1$1.run(ActiveResources.java:2040)
       at java.lang.Thread.run(Thread.java:1012)

# Timer-0:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at java.util.TimerThread.mainLoop(Timer.java:534)
       at java.util.TimerThread.run(Timer.java:513)

# RealmFinalizingDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:203)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:224)
       at io.realm.internal.FinalizerRunnable.run(FinalizerRunnable.java:3)
       at java.lang.Thread.run(Thread.java:1012)

# Timer-1:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at java.util.TimerThread.mainLoop(Timer.java:534)
       at java.util.TimerThread.run(Timer.java:513)

# queued-work-looper:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:341)
       at android.os.Looper.loopOnce(Looper.java:169)
       at android.os.Looper.loop(Looper.java:300)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# Measurement Worker:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at m.lk.run(:com.google.android.gms.dynamite_measurementdynamite@234414038@23.44.14 (190400-0):71)

# ReferenceQueueDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at java.lang.Daemons$ReferenceQueueDaemon.runInternal(Daemons.java:232)
       at java.lang.Daemons$Daemon.run(Daemons.java:140)
       at java.lang.Thread.run(Thread.java:1012)

# awaitEvenIfOnMainThread task continuation executor1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-4:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# com.google.firebase.crashlytics.startup1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# FinalizerWatchdogDaemon:
       at java.lang.Thread.sleep(Thread.java)
       at java.lang.Thread.sleep(Thread.java:450)
       at java.lang.Thread.sleep(Thread.java:355)
       at java.lang.Daemons$FinalizerWatchdogDaemon.sleepForNanos(Daemons.java:438)
       at java.lang.Daemons$FinalizerWatchdogDaemon.waitForProgress(Daemons.java:480)
       at java.lang.Daemons$FinalizerWatchdogDaemon.runInternal(Daemons.java:369)
       at java.lang.Daemons$Daemon.run(Daemons.java:140)
       at java.lang.Thread.run(Thread.java:1012)
</details>
 </details>

<details>
  
  <summary>Galaxy Z Flip5</summary> :iphone:
  
  ![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/f6b8c576-cccf-4363-8229-a4f15a5bd01e)
    
  <details>
   
   *<summary>Details</summary>*
   
# Crashlytics - Stack trace
# Application: com.weeklyplannerapp.weekplan
# Platform: android
# Version: 7.97 (82)
# Issue: 72bd018209352c1b39c33f10f34b265c
# Session: 6554C8090318000162800C143AF275BA_DNE_0_v2
# Date: Wed Nov 15 2023 15:31:13 GMT+0200 (Eastern European Standard Time)

 # Fatal Exception: java.lang.RuntimeException: Unable to stop activity {com.weeklyplannerapp.weekplan/com.weeklyplannerapp.weekplan.View.Activities.MainActivity}: io.realm.exceptions.RealmFileException: Failed to open file at path '/data/data/com.weeklyplannerapp.weekplan/15.11.2023 07:31': parent directory does not exist (/data/data/com.weeklyplannerapp.weekplan/15.11.2023 07:31) in /tmp/realm-java/realm/realm-library/src/main/cpp/io_realm_internal_OsSharedRealm.cpp line 404 Kind: NOT_FOUND.
       at android.app.ActivityThread.callActivityOnStop(ActivityThread.java:5858)
       at android.app.ActivityThread.performStopActivityInner(ActivityThread.java:5824)
       at android.app.ActivityThread.handleStopActivity(ActivityThread.java:5895)
       at android.app.servertransaction.StopActivityItem.execute(StopActivityItem.java:43)
       at android.app.servertransaction.ActivityTransactionItem.execute(ActivityTransactionItem.java:45)
       at android.app.servertransaction.TransactionExecutor.executeLifecycleState(TransactionExecutor.java:176)
       at android.app.servertransaction.TransactionExecutor.execute(TransactionExecutor.java:97)
       at android.app.ActivityThread$H.handleMessage(ActivityThread.java:2584)
       at android.os.Handler.dispatchMessage(Handler.java:106)
       at android.os.Looper.loopOnce(Looper.java:226)
       at android.os.Looper.loop(Looper.java:313)
       at android.app.ActivityThread.main(ActivityThread.java:8805)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:604)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:1067)

# Caused by io.realm.exceptions.RealmFileException: Failed to open file at path '/data/data/com.weeklyplannerapp.weekplan/15.11.2023 07:31': parent directory does not exist (/data/data/com.weeklyplannerapp.weekplan/15.11.2023 07:31) in /tmp/realm-java/realm/realm-library/src/main/cpp/io_realm_internal_OsSharedRealm.cpp line 404
       at io.realm.internal.OsSharedRealm.nativeWriteCopy(OsSharedRealm.java)
       at io.realm.internal.OsSharedRealm.writeCopy(OsSharedRealm.java:38)
       at io.realm.BaseRealm.writeCopyTo(BaseRealm.java:1)
       at com.weeklyplannerapp.weekplan.WeeklyPlanApplication$1.onActivityStopped(WeeklyPlanApplication.java:199)
       at android.app.Application.dispatchActivityStopped(Application.java:510)
       at android.app.Activity.dispatchActivityStopped(Activity.java:1549)
       at android.app.Activity.onStop(Activity.java:2711)
       at androidx.fragment.app.FragmentActivity.onStop(FragmentActivity.java:1)
       at androidx.appcompat.app.AppCompatActivity.onStop(AppCompatActivity.java:1)
       at com.weeklyplannerapp.weekplan.View.Activities.MainActivity.onStop(MainActivity.java)
       at android.app.Instrumentation.callActivityOnStop(Instrumentation.java:1584)
       at android.app.Activity.performStop(Activity.java:8905)
       at android.app.ActivityThread.callActivityOnStop(ActivityThread.java:5850)
       at android.app.ActivityThread.performStopActivityInner(ActivityThread.java:5824)
       at android.app.ActivityThread.handleStopActivity(ActivityThread.java:5895)
       at android.app.servertransaction.StopActivityItem.execute(StopActivityItem.java:43)
       at android.app.servertransaction.ActivityTransactionItem.execute(ActivityTransactionItem.java:45)
       at android.app.servertransaction.TransactionExecutor.executeLifecycleState(TransactionExecutor.java:176)
       at android.app.servertransaction.TransactionExecutor.execute(TransactionExecutor.java:97)
       at android.app.ActivityThread$H.handleMessage(ActivityThread.java:2584)
       at android.os.Handler.dispatchMessage(Handler.java:106)
       at android.os.Looper.loopOnce(Looper.java:226)
       at android.os.Looper.loop(Looper.java:313)
       at android.app.ActivityThread.main(ActivityThread.java:8805)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:604)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:1067)

# DefaultDispatcher-worker-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# PlayBillingLibrary-4:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# FinalizerWatchdogDaemon:
       at java.lang.Thread.sleep(Thread.java)
       at java.lang.Thread.sleep(Thread.java:450)
       at java.lang.Thread.sleep(Thread.java:355)
       at java.lang.Daemons$FinalizerWatchdogDaemon.sleepForNanos(Daemons.java:481)
       at java.lang.Daemons$FinalizerWatchdogDaemon.waitForProgress(Daemons.java:544)
       at java.lang.Daemons$FinalizerWatchdogDaemon.runInternal(Daemons.java:412)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# DefaultDispatcher-worker-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# PlayBillingLibrary-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# ReferenceQueueDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.lang.Daemons$ReferenceQueueDaemon.runInternal(Daemons.java:239)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Blocking Thread #0:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:401)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:903)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# OkHttp ConnectionPool:
       at java.lang.Object.wait(Object.java)
       at com.android.okhttp.ConnectionPool$1.run(ConnectionPool.java:106)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1145)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# ScionFrontendApi:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.awaitNanos(AbstractQueuedSynchronizer.java:1672)
       at java.util.concurrent.LinkedBlockingQueue.poll(LinkedBlockingQueue.java:460)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# GmsDynamite:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at com.google.android.gms.dynamite.zza.run(zza.java:16)

# pool-11-thread-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# FinalizerDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:210)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:231)
       at java.lang.Daemons$FinalizerDaemon.runInternal(Daemons.java:309)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# RealmFinalizingDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:210)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:231)
       at io.realm.internal.FinalizerRunnable.run(FinalizerRunnable.java:3)
       at java.lang.Thread.run(Thread.java:1012)

# Measurement Worker:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at m.lk.run(:com.google.android.gms.dynamite_measurementdynamite@234414039@23.44.14 (190408-0):71)

# awaitEvenIfOnMainThread task continuation executor1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# Okio Watchdog:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at com.android.okhttp.okio.AsyncTimeout.awaitTimeout(AsyncTimeout.java:313)
       at com.android.okhttp.okio.AsyncTimeout.access$000(AsyncTimeout.java:42)
       at com.android.okhttp.okio.AsyncTimeout$Watchdog.run(AsyncTimeout.java:288)

# com.google.firebase.crashlytics.startup1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# AsyncTask #1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.SynchronousQueue$TransferStack$SNode.block(SynchronousQueue.java:288)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:397)
       at java.util.concurrent.SynchronousQueue.take(SynchronousQueue.java:886)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #0:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# DefaultDispatcher-worker-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# Crashlytics Exception Handler1:
       at dalvik.system.VMStack.getThreadStackTrace(VMStack.java)
       at java.lang.Thread.getStackTrace(Thread.java:1841)
       at java.lang.Thread.getAllStackTraces(Thread.java:1909)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateThreadsList(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateExecutionData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateEventApplicationData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.captureEventData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistEvent(SessionReportingCoordinator.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistFatalEvent(SessionReportingCoordinator.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsBackgroundWorker$3.then(CrashlyticsBackgroundWorker.java:16)
       at com.google.android.gms.tasks.zze.run(:8)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1145)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# queued-work-looper-data:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# GLThread 93602:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at android.opengl.GLSurfaceView$GLThread.guardedRun(GLSurfaceView.java:1517)
       at android.opengl.GLSurfaceView$GLThread.run(GLSurfaceView.java:1287)

# queued-work-looper:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:335)
       at android.os.Looper.loopOnce(Looper.java:186)
       at android.os.Looper.loop(Looper.java:313)
       at android.os.HandlerThread.run(HandlerThread.java:67)
  </details>

  



![Screenshot 2023-11-18 125517](https://github.com/UserQA07/Week-Planner-/assets/144763744/79321fcf-4063-4425-9d95-c004c41d5248)

<details>
 
*<summary>Details</summary>*
   
# Crashlytics - Stack trace
# Application: com.weeklyplannerapp.weekplan
# Platform: android
# Version: 7.97 (82)
# Issue: e257c28bfd8eb9d4e5296a7bd068bbbe
# Session: 654E68160286000155B0135BD4763198_DNE_0_v2
# Date: Fri Nov 10 2023 19:29:07 GMT+0200 (Eastern European Standard Time)

# Fatal Exception: android.os.DeadSystemRuntimeException: android.os.DeadSystemException
       at android.view.autofill.AutofillManager.updateSessionLocked(AutofillManager.java:2184)
       at android.view.autofill.AutofillManager.notifyValueChanged(AutofillManager.java:1583)
       at android.widget.TextView.notifyListeningManagersAfterTextChanged(TextView.java:11938)
       at android.widget.TextView.sendAfterTextChanged(TextView.java:11918)
       at android.widget.TextView$ChangeWatcher.afterTextChanged(TextView.java:15296)
       at android.text.SpannableStringBuilder.sendAfterTextChanged(SpannableStringBuilder.java:1291)
       at android.text.SpannableStringBuilder.replace(SpannableStringBuilder.java:591)
       at androidx.emoji2.text.SpannableBuilder.replace(SpannableBuilder.java:4)
       at android.text.SpannableStringBuilder.append(SpannableStringBuilder.java:305)
       at androidx.emoji2.text.SpannableBuilder.append(SpannableBuilder.java:3)
       at androidx.emoji2.text.SpannableBuilder.append(SpannableBuilder.java:3)
       at android.widget.TextView.append(TextView.java:6410)
       at android.widget.TextView.append(TextView.java:6391)
       at com.weeklyplannerapp.weekplan.View.Fragments.SingleDayFragment.addEmptyLinesToTheEnd(SingleDayFragment.java:462)
       at com.weeklyplannerapp.weekplan.View.Fragments.SingleDayFragment.onViewCreated(SingleDayFragment.java:462)
       at androidx.fragment.app.Fragment.performViewCreated(Fragment.java:295)
       at androidx.fragment.app.FragmentStateManager.createView(FragmentStateManager.java:295)
       at androidx.fragment.app.FragmentStateManager.moveToExpectedState(FragmentStateManager.java:148)
       at androidx.fragment.app.FragmentManager.executeOpsTogether(FragmentManager.java:26)
       at androidx.fragment.app.FragmentManager.removeRedundantOperationsAndExecute(FragmentManager.java:92)
       at androidx.fragment.app.FragmentManager.execPendingActions(FragmentManager.java:74)
       at androidx.fragment.app.FragmentManager$5.run(FragmentManager.java:22)
       at android.os.Handler.handleCallback(Handler.java:942)
       at android.os.Handler.dispatchMessage(Handler.java:99)
       at android.os.Looper.loopOnce(Looper.java:226)
       at android.os.Looper.loop(Looper.java:313)
       at android.app.ActivityThread.main(ActivityThread.java:8805)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:604)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:1067)

# Caused by android.os.DeadSystemException:
       at android.view.autofill.AutofillManager.updateSessionLocked(AutofillManager.java:2184)
       at android.view.autofill.AutofillManager.notifyValueChanged(AutofillManager.java:1583)
       at android.widget.TextView.notifyListeningManagersAfterTextChanged(TextView.java:11938)
       at android.widget.TextView.sendAfterTextChanged(TextView.java:11918)
       at android.widget.TextView$ChangeWatcher.afterTextChanged(TextView.java:15296)
       at android.text.SpannableStringBuilder.sendAfterTextChanged(SpannableStringBuilder.java:1291)
       at android.text.SpannableStringBuilder.replace(SpannableStringBuilder.java:591)
       at androidx.emoji2.text.SpannableBuilder.replace(SpannableBuilder.java:4)
       at android.text.SpannableStringBuilder.append(SpannableStringBuilder.java:305)
       at androidx.emoji2.text.SpannableBuilder.append(SpannableBuilder.java:3)
       at androidx.emoji2.text.SpannableBuilder.append(SpannableBuilder.java:3)
       at android.widget.TextView.append(TextView.java:6410)
       at android.widget.TextView.append(TextView.java:6391)
       at com.weeklyplannerapp.weekplan.View.Fragments.SingleDayFragment.addEmptyLinesToTheEnd(SingleDayFragment.java:462)
       at com.weeklyplannerapp.weekplan.View.Fragments.SingleDayFragment.onViewCreated(SingleDayFragment.java:462)
       at androidx.fragment.app.Fragment.performViewCreated(Fragment.java:295)
       at androidx.fragment.app.FragmentStateManager.createView(FragmentStateManager.java:295)
       at androidx.fragment.app.FragmentStateManager.moveToExpectedState(FragmentStateManager.java:148)
       at androidx.fragment.app.FragmentManager.executeOpsTogether(FragmentManager.java:26)
       at androidx.fragment.app.FragmentManager.removeRedundantOperationsAndExecute(FragmentManager.java:92)
       at androidx.fragment.app.FragmentManager.execPendingActions(FragmentManager.java:74)
       at androidx.fragment.app.FragmentManager$5.run(FragmentManager.java:22)
       at android.os.Handler.handleCallback(Handler.java:942)
       at android.os.Handler.dispatchMessage(Handler.java:99)
       at android.os.Looper.loopOnce(Looper.java:226)
       at android.os.Looper.loop(Looper.java:313)
       at android.app.ActivityThread.main(ActivityThread.java:8805)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:604)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:1067)

# Firebase Background Thread #3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# queued-work-looper:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:335)
       at android.os.Looper.loopOnce(Looper.java:186)
       at android.os.Looper.loop(Looper.java:313)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# pool-10-thread-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# Measurement Worker:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at m.ll.run(:com.google.android.gms.dynamite_measurementdynamite@234313039@23.43.13 (190408-0):71)

# magnifier pixel copy result handler:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:335)
       at android.os.Looper.loopOnce(Looper.java:186)
       at android.os.Looper.loop(Looper.java:313)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# FinalizerWatchdogDaemon:
       at java.lang.Thread.sleep(Thread.java)
       at java.lang.Thread.sleep(Thread.java:450)
       at java.lang.Thread.sleep(Thread.java:355)
       at java.lang.Daemons$FinalizerWatchdogDaemon.sleepForNanos(Daemons.java:438)
       at java.lang.Daemons$FinalizerWatchdogDaemon.waitForProgress(Daemons.java:480)
       at java.lang.Daemons$FinalizerWatchdogDaemon.runInternal(Daemons.java:369)
       at java.lang.Daemons$Daemon.run(Daemons.java:140)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# ReferenceQueueDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at java.lang.Daemons$ReferenceQueueDaemon.runInternal(Daemons.java:232)
       at java.lang.Daemons$Daemon.run(Daemons.java:140)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-4:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# GmsDynamite:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at com.google.android.gms.dynamite.zza.run(zza.java:16)

# com.google.firebase.crashlytics.startup1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# Okio Watchdog:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at com.android.okhttp.okio.AsyncTimeout.awaitTimeout(AsyncTimeout.java:313)
       at com.android.okhttp.okio.AsyncTimeout.access$000(AsyncTimeout.java:42)
       at com.android.okhttp.okio.AsyncTimeout$Watchdog.run(AsyncTimeout.java:288)

# Crashlytics Exception Handler1:
       at dalvik.system.VMStack.getThreadStackTrace(VMStack.java)
       at java.lang.Thread.getStackTrace(Thread.java:1841)
       at java.lang.Thread.getAllStackTraces(Thread.java:1909)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateThreadsList(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateExecutionData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateEventApplicationData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.captureEventData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistEvent(SessionReportingCoordinator.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistFatalEvent(SessionReportingCoordinator.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsBackgroundWorker$3.then(CrashlyticsBackgroundWorker.java:16)
       at com.google.android.gms.tasks.zze.run(:8)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1137)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# queued-work-looper-data:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# DefaultDispatcher-worker-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:357)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# OkHttp ConnectionPool:
       at java.lang.Object.wait(Object.java)
       at com.android.okhttp.ConnectionPool$1.run(ConnectionPool.java:106)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1137)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #0:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# DefaultDispatcher-worker-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:357)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# Firebase Background Thread #1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# RealmFinalizingDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:203)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:224)
       at io.realm.internal.FinalizerRunnable.run(FinalizerRunnable.java:3)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# FinalizerDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:203)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:224)
       at java.lang.Daemons$FinalizerDaemon.runInternal(Daemons.java:300)
       at java.lang.Daemons$Daemon.run(Daemons.java:140)
       at java.lang.Thread.run(Thread.java:1012)

# queued-work-looper-data:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# GLThread 813:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at android.opengl.GLSurfaceView$GLThread.guardedRun(GLSurfaceView.java:1517)
       at android.opengl.GLSurfaceView$GLThread.run(GLSurfaceView.java:1287)

# DefaultDispatcher-worker-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:357)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# AsyncTask #6:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.SynchronousQueue$TransferStack.awaitFulfill(SynchronousQueue.java:461)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:361)
       at java.util.concurrent.SynchronousQueue.take(SynchronousQueue.java:922)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# awaitEvenIfOnMainThread task continuation executor1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)
       
   </details>

![Screenshot 2023-11-18 133048](https://github.com/UserQA07/Week-Planner-/assets/144763744/5d95132a-c15d-4378-8cce-a4a785d8cc20)

<details>
 
   *<summary>Details</summary>*
 
 # Crashlytics - Stack trace
# Application: com.weeklyplannerapp.weekplan
# Platform: android
# Version: 7.97 (82)
# Issue: f9dd892237f667190d25b708cad98bb9
# Session: 6554C8F0005A000179060C143AF275BA_DNE_0_v2
# Date: Wed Nov 15 2023 15:36:28 GMT+0200 (Eastern European Standard Time)

# Fatal Exception: io.realm.exceptions.RealmFileException: Failed to open file at path '/data/data/com.weeklyplannerapp.weekplan/A106746187036400090074': parent directory does not exist (/data/data/com.weeklyplannerapp.weekplan/A106746187036400090074) in /tmp/realm-java/realm/realm-library/src/main/cpp/io_realm_internal_OsSharedRealm.cpp line 404
       at io.realm.internal.OsSharedRealm.nativeWriteCopy(OsSharedRealm.java)
       at io.realm.internal.OsSharedRealm.writeCopy(OsSharedRealm.java:38)
       at io.realm.BaseRealm.writeCopyTo(BaseRealm.java:1)
       at com.weeklyplannerapp.weekplan.Presenter.MainActivityPresenter.lambda$backupDataToGoogleCloud$2(MainActivityPresenter.java:115)
       at android.os.Handler.handleCallback(Handler.java:942)
       at android.os.Handler.dispatchMessage(Handler.java:99)
       at android.os.Looper.loopOnce(Looper.java:226)
       at android.os.Looper.loop(Looper.java:313)
       at android.app.ActivityThread.main(ActivityThread.java:8805)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:604)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:1067)

# FinalizerWatchdogDaemon:
       at java.lang.Thread.sleep(Thread.java)
       at java.lang.Thread.sleep(Thread.java:450)
       at java.lang.Thread.sleep(Thread.java:355)
       at java.lang.Daemons$FinalizerWatchdogDaemon.sleepForNanos(Daemons.java:481)
       at java.lang.Daemons$FinalizerWatchdogDaemon.waitForProgress(Daemons.java:544)
       at java.lang.Daemons$FinalizerWatchdogDaemon.runInternal(Daemons.java:412)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# glide-source-thread-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.PriorityBlockingQueue.take(PriorityBlockingQueue.java:538)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultThreadFactory$1.run(GlideExecutor.java:2022)
       at java.lang.Thread.run(Thread.java:1012)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultPriorityThreadFactory$1.run(GlideExecutor.java:12)

# InsetsAnimations:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:335)
       at android.os.Looper.loopOnce(Looper.java:186)
       at android.os.Looper.loop(Looper.java:313)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# PlayBillingLibrary-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# ScionFrontendApi:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.awaitNanos(AbstractQueuedSynchronizer.java:1672)
       at java.util.concurrent.LinkedBlockingQueue.poll(LinkedBlockingQueue.java:460)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# GmsDynamite:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at com.google.android.gms.dynamite.zza.run(zza.java:16)

# DefaultDispatcher-worker-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# pool-11-thread-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# DefaultDispatcher-worker-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# PlayBillingLibrary-4:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# AsyncTask #7:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:401)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:903)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# com.google.firebase.crashlytics.startup1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-5:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# GoogleApiHandler:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:335)
       at android.os.Looper.loopOnce(Looper.java:186)
       at android.os.Looper.loop(Looper.java:313)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# AsyncTask #9:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:401)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:903)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# queued-work-looper:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:335)
       at android.os.Looper.loopOnce(Looper.java:186)
       at android.os.Looper.loop(Looper.java:313)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# RealmFinalizingDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:210)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:231)
       at io.realm.internal.FinalizerRunnable.run(FinalizerRunnable.java:3)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# ReferenceQueueDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.lang.Daemons$ReferenceQueueDaemon.runInternal(Daemons.java:239)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# awaitEvenIfOnMainThread task continuation executor1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #0:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# queued-work-looper-data:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Crashlytics Exception Handler1:
       at dalvik.system.VMStack.getThreadStackTrace(VMStack.java)
       at java.lang.Thread.getStackTrace(Thread.java:1841)
       at java.lang.Thread.getAllStackTraces(Thread.java:1909)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateThreadsList(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateExecutionData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateEventApplicationData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.captureEventData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistEvent(SessionReportingCoordinator.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistFatalEvent(SessionReportingCoordinator.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsBackgroundWorker$3.then(CrashlyticsBackgroundWorker.java:16)
       at com.google.android.gms.tasks.zze.run(:8)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1145)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# DefaultDispatcher-worker-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# glide-active-resources:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:210)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:231)
       at com.bumptech.glide.load.engine.ActiveResources.cleanReferenceQueue(ActiveResources.java:320)
       at com.bumptech.glide.load.engine.ActiveResources$2.run(ActiveResources.java:320)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1145)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.bumptech.glide.load.engine.ActiveResources$1$1.run(ActiveResources.java:2040)
       at java.lang.Thread.run(Thread.java:1012)

# glide-source-thread-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.PriorityBlockingQueue.take(PriorityBlockingQueue.java:538)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultThreadFactory$1.run(GlideExecutor.java:2022)
       at java.lang.Thread.run(Thread.java:1012)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultPriorityThreadFactory$1.run(GlideExecutor.java:12)

# PlayBillingLibrary-4:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# GLThread 93659:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at android.opengl.GLSurfaceView$GLThread.guardedRun(GLSurfaceView.java:1517)
       at android.opengl.GLSurfaceView$GLThread.run(GLSurfaceView.java:1287)

# glide-disk-cache-thread-0:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.PriorityBlockingQueue.take(PriorityBlockingQueue.java:538)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultThreadFactory$1.run(GlideExecutor.java:2022)
       at java.lang.Thread.run(Thread.java:1012)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultPriorityThreadFactory$1.run(GlideExecutor.java:12)

# Firebase Blocking Thread #0:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:401)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:903)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# glide-source-thread-0:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.PriorityBlockingQueue.take(PriorityBlockingQueue.java:538)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultThreadFactory$1.run(GlideExecutor.java:2022)
       at java.lang.Thread.run(Thread.java:1012)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultPriorityThreadFactory$1.run(GlideExecutor.java:12)

# queued-work-looper-data:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# glide-source-thread-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.PriorityBlockingQueue.take(PriorityBlockingQueue.java:538)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultThreadFactory$1.run(GlideExecutor.java:2022)
       at java.lang.Thread.run(Thread.java:1012)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultPriorityThreadFactory$1.run(GlideExecutor.java:12)

# PlayBillingLibrary-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# ConnectivityThread:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:335)
       at android.os.Looper.loopOnce(Looper.java:186)
       at android.os.Looper.loop(Looper.java:313)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# PlayBillingLibrary-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Measurement Worker:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at m.lk.run(:com.google.android.gms.dynamite_measurementdynamite@234414039@23.44.14 (190408-0):71)

# FinalizerDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:210)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:231)
       at java.lang.Daemons$FinalizerDaemon.runInternal(Daemons.java:309)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)
</details>
 </details>


   

  <details>
  
   <summary>Redmi Note 11S</summary> 
   
![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/09fbbbec-b6f4-4dcf-a738-6d1a052efc5c)


<details>
 
   *<summary>Details</summary>*
   
 # Crashlytics - Stack trace
# Application: com.weeklyplannerapp.weekplan
# Platform: android
# Version: 7.97 (82)
# Issue: 72bd018209352c1b39c33f10f34b265c
# Session: 654B6C1E0100000114CF7AB26020C67D_DNE_0_v2
# Date: Wed Nov 08 2023 13:08:39 GMT+0200 (Eastern European Standard Time)

# Fatal Exception: java.lang.RuntimeException: Unable to stop activity {com.weeklyplannerapp.weekplan/com.weeklyplannerapp.weekplan.View.Activities.MainActivity}: io.realm.exceptions.RealmFileException: Failed to open file at path '/data/data/com.weeklyplannerapp.weekplan/08.11.2023 14:08': parent directory does not exist (/data/data/com.weeklyplannerapp.weekplan/08.11.2023 14:08) in /tmp/realm-java/realm/realm-library/src/main/cpp/io_realm_internal_OsSharedRealm.cpp line 404 Kind: NOT_FOUND.
       at android.app.ActivityThread.callActivityOnStop(ActivityThread.java:5454)
       at android.app.ActivityThread.performStopActivityInner(ActivityThread.java:5426)
       at android.app.ActivityThread.handleStopActivity(ActivityThread.java:5491)
       at android.app.servertransaction.StopActivityItem.execute(StopActivityItem.java:43)
       at android.app.servertransaction.ActivityTransactionItem.execute(ActivityTransactionItem.java:45)
       at android.app.servertransaction.TransactionExecutor.executeLifecycleState(TransactionExecutor.java:176)
       at android.app.servertransaction.TransactionExecutor.execute(TransactionExecutor.java:97)
       at android.app.ActivityThread$H.handleMessage(ActivityThread.java:2437)
       at android.os.Handler.dispatchMessage(Handler.java:106)
       at android.os.Looper.loopOnce(Looper.java:211)
       at android.os.Looper.loop(Looper.java:300)
       at android.app.ActivityThread.main(ActivityThread.java:8294)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:580)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:1028)

# Caused by io.realm.exceptions.RealmFileException: Failed to open file at path '/data/data/com.weeklyplannerapp.weekplan/08.11.2023 14:08': parent directory does not exist (/data/data/com.weeklyplannerapp.weekplan/08.11.2023 14:08) in /tmp/realm-java/realm/realm-library/src/main/cpp/io_realm_internal_OsSharedRealm.cpp line 404
       at io.realm.internal.OsSharedRealm.nativeWriteCopy(OsSharedRealm.java)
       at io.realm.internal.OsSharedRealm.writeCopy(OsSharedRealm.java:38)
       at io.realm.BaseRealm.writeCopyTo(BaseRealm.java:1)
       at com.weeklyplannerapp.weekplan.WeeklyPlanApplication$1.onActivityStopped(WeeklyPlanApplication.java:199)
       at android.app.Application.dispatchActivityStopped(Application.java:503)
       at android.app.Activity.dispatchActivityStopped(Activity.java:1579)
       at android.app.Activity.onStop(Activity.java:2737)
       at androidx.fragment.app.FragmentActivity.onStop(FragmentActivity.java:1)
       at androidx.appcompat.app.AppCompatActivity.onStop(AppCompatActivity.java:1)
       at com.weeklyplannerapp.weekplan.View.Activities.MainActivity.onStop(MainActivity.java)
       at android.app.Instrumentation.callActivityOnStop(Instrumentation.java:1604)
       at android.app.Activity.performStop(Activity.java:8794)
       at android.app.ActivityThread.callActivityOnStop(ActivityThread.java:5446)
       at android.app.ActivityThread.performStopActivityInner(ActivityThread.java:5426)
       at android.app.ActivityThread.handleStopActivity(ActivityThread.java:5491)
       at android.app.servertransaction.StopActivityItem.execute(StopActivityItem.java:43)
       at android.app.servertransaction.ActivityTransactionItem.execute(ActivityTransactionItem.java:45)
       at android.app.servertransaction.TransactionExecutor.executeLifecycleState(TransactionExecutor.java:176)
       at android.app.servertransaction.TransactionExecutor.execute(TransactionExecutor.java:97)
       at android.app.ActivityThread$H.handleMessage(ActivityThread.java:2437)
       at android.os.Handler.dispatchMessage(Handler.java:106)
       at android.os.Looper.loopOnce(Looper.java:211)
       at android.os.Looper.loop(Looper.java:300)
       at android.app.ActivityThread.main(ActivityThread.java:8294)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:580)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:1028)

# FinalizerWatchdogDaemon:
       at java.lang.Thread.sleep(Thread.java)
       at java.lang.Thread.sleep(Thread.java:450)
       at java.lang.Thread.sleep(Thread.java:355)
       at java.lang.Daemons$FinalizerWatchdogDaemon.sleepForNanos(Daemons.java:481)
       at java.lang.Daemons$FinalizerWatchdogDaemon.waitForProgress(Daemons.java:544)
       at java.lang.Daemons$FinalizerWatchdogDaemon.runInternal(Daemons.java:412)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# GmsDynamite:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at com.google.android.gms.dynamite.zza.run(zza.java:16)

# PlayBillingLibrary-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# launch:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:341)
       at android.os.Looper.loopOnce(Looper.java:169)
       at android.os.Looper.loop(Looper.java:300)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# Firebase Background Thread #1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# ScrollPolicy:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:341)
       at android.os.Looper.loopOnce(Looper.java:169)
       at android.os.Looper.loop(Looper.java:300)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# com.google.firebase.crashlytics.startup1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# FramePolicy:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:341)
       at android.os.Looper.loopOnce(Looper.java:169)
       at android.os.Looper.loop(Looper.java:300)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# DefaultDispatcher-worker-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# PlayBillingLibrary-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# pool-9-thread-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# InsetsAnimations:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:341)
       at android.os.Looper.loopOnce(Looper.java:169)
       at android.os.Looper.loop(Looper.java:300)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# awaitEvenIfOnMainThread task continuation executor1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# AsyncTask #4:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:401)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:903)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# AsyncTask #5:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:401)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:903)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# DefaultDispatcher-worker-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# DefaultDispatcher-worker-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# Firebase Blocking Thread #0:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:401)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:903)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# ScionFrontendApi:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.awaitNanos(AbstractQueuedSynchronizer.java:1672)
       at java.util.concurrent.LinkedBlockingQueue.poll(LinkedBlockingQueue.java:460)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #0:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-4:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# queued-work-looper:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:341)
       at android.os.Looper.loopOnce(Looper.java:169)
       at android.os.Looper.loop(Looper.java:300)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# Firebase Background Thread #2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# ReferenceQueueDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.lang.Daemons$ReferenceQueueDaemon.runInternal(Daemons.java:239)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# Timer-0:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.util.TimerThread.mainLoop(Timer.java:534)
       at java.util.TimerThread.run(Timer.java:513)

# Crashlytics Exception Handler1:
       at dalvik.system.VMStack.getThreadStackTrace(VMStack.java)
       at java.lang.Thread.getStackTrace(Thread.java:1841)
       at java.lang.Thread.getAllStackTraces(Thread.java:1909)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateThreadsList(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateExecutionData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateEventApplicationData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.captureEventData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistEvent(SessionReportingCoordinator.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistFatalEvent(SessionReportingCoordinator.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsBackgroundWorker$3.then(CrashlyticsBackgroundWorker.java:16)
       at com.google.android.gms.tasks.zze.run(:8)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1145)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# Measurement Worker:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at m.ll.run(:com.google.android.gms.dynamite_measurementdynamite@234313038@23.43.13 (190400-0):71)

# GLThread 66:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at android.opengl.GLSurfaceView$GLThread.guardedRun(GLSurfaceView.java:1505)
       at android.opengl.GLSurfaceView$GLThread.run(GLSurfaceView.java:1280)

# FinalizerDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:210)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:231)
       at java.lang.Daemons$FinalizerDaemon.runInternal(Daemons.java:309)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# RealmFinalizingDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:210)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:231)
       at io.realm.internal.FinalizerRunnable.run(FinalizerRunnable.java:3)
       at java.lang.Thread.run(Thread.java:1012)

# Timer-1:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.util.TimerThread.mainLoop(Timer.java:534)
       at java.util.TimerThread.run(Timer.java:513)

# Firebase Background Thread #3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)
       
</details>
  </details>

  <details>
   
   <summary>Galaxy S21 Ultra 5G</summary> :iphone:

   ![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/3a1f9276-fd74-4482-9e73-66b88cb8a365)

  <details>

 *<summary>Details</summary>*

 # Crashlytics - Stack trace
# Application: com.weeklyplannerapp.weekplan
# Platform: android
# Version: 7.97 (82)
# Issue: 7494e5bb2d3fb35cf07ef562a6952da2
# Session: 65510148019E00014D43093CEF1DEB3C_DNE_0_v2
# Date: Sun Nov 12 2023 18:46:00 GMT+0200 (Eastern European Standard Time)

# Fatal Exception: java.lang.RuntimeException: Unable to start activity ComponentInfo{com.weeklyplannerapp.weekplan/com.weeklyplannerapp.weekplan.View.Activities.MainActivity}: io.realm.exceptions.RealmMigrationNeededException: Migration is required due to the following errors:
- Property 'Note.day' has been made indexed.
- Property 'Note.month' has been made indexed.
- Property 'Note.year' has been made indexed.
       at android.app.ActivityThread.performLaunchActivity(ActivityThread.java:4169)
       at android.app.ActivityThread.handleLaunchActivity(ActivityThread.java:4325)
       at android.app.servertransaction.LaunchActivityItem.execute(LaunchActivityItem.java:101)
       at android.app.servertransaction.TransactionExecutor.executeCallbacks(TransactionExecutor.java:135)
       at android.app.servertransaction.TransactionExecutor.execute(TransactionExecutor.java:95)
       at android.app.ActivityThread$H.handleMessage(ActivityThread.java:2574)
       at android.os.Handler.dispatchMessage(Handler.java:106)
       at android.os.Looper.loopOnce(Looper.java:226)
       at android.os.Looper.loop(Looper.java:313)
       at android.app.ActivityThread.main(ActivityThread.java:8762)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:604)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:1067)

# Caused by io.realm.exceptions.RealmMigrationNeededException: Migration is required due to the following errors:
- Property 'Note.day' has been made indexed.
- Property 'Note.month' has been made indexed.
- Property 'Note.year' has been made indexed.
       at io.realm.internal.OsSharedRealm.nativeGetSharedRealm(OsSharedRealm.java)
       at io.realm.internal.OsSharedRealm.<init>(OsSharedRealm.java:9)
       at io.realm.internal.OsSharedRealm.getInstance(OsSharedRealm.java:3)
       at io.realm.BaseRealm.<init>(BaseRealm.java:10)
       at io.realm.BaseRealm.<init>(BaseRealm.java:10)
       at io.realm.Realm.<init>(Realm.java:4)
       at io.realm.Realm.createInstance(Realm.java:115)
       at io.realm.RealmCache.createInstance(RealmCache.java:115)
       at io.realm.RealmCache.doCreateRealmOrGetFromCache(RealmCache.java:115)
       at io.realm.RealmCache.createRealmOrGetFromCache(RealmCache.java:115)
       at io.realm.Realm.getInstance(Realm.java:115)
       at com.weeklyplannerapp.weekplan.Service.Dagger.Modules.DatabaseModule.provideRealm(DatabaseModule.java:53)
       at com.weeklyplannerapp.weekplan.Service.Dagger.Modules.DatabaseModule_ProvideRealmFactory.provideRealm(DatabaseModule_ProvideRealmFactory.java:53)
       at com.weeklyplannerapp.weekplan.Service.Dagger.Modules.DatabaseModule_ProvideRealmFactory.get(DatabaseModule_ProvideRealmFactory.java:53)
       at com.weeklyplannerapp.weekplan.Service.Dagger.Modules.DatabaseModule_ProvideRealmFactory.get(DatabaseModule_ProvideRealmFactory.java:53)
       at dagger.internal.DoubleCheck.get(DoubleCheck.java:14)
       at com.weeklyplannerapp.weekplan.Service.Dagger.Modules.DatabaseModule_ProvideDatabaseFactory.get(DatabaseModule_ProvideDatabaseFactory.java:11)
       at com.weeklyplannerapp.weekplan.Service.Dagger.Modules.DatabaseModule_ProvideDatabaseFactory.get(DatabaseModule_ProvideDatabaseFactory.java:11)
       at dagger.internal.DoubleCheck.get(DoubleCheck.java:14)
       at com.weeklyplannerapp.weekplan.Service.Dagger.DaggerIDaggerComponent$IDaggerComponentImpl.injectMainActivity(DaggerIDaggerComponent.java:328)
       at com.weeklyplannerapp.weekplan.Service.Dagger.DaggerIDaggerComponent$IDaggerComponentImpl.inject(DaggerIDaggerComponent.java:328)
       at com.weeklyplannerapp.weekplan.View.Activities.MainActivity.initializeData(MainActivity.java:328)
       at com.weeklyplannerapp.weekplan.View.Activities.MainActivity.initializeAll(MainActivity.java:328)
       at com.weeklyplannerapp.weekplan.View.Activities.MainActivity.onCreate(MainActivity.java:328)
       at android.app.Activity.performCreate(Activity.java:8591)
       at android.app.Activity.performCreate(Activity.java:8570)
       at android.app.Instrumentation.callActivityOnCreate(Instrumentation.java:1384)
       at android.app.ActivityThread.performLaunchActivity(ActivityThread.java:4150)
       at android.app.ActivityThread.handleLaunchActivity(ActivityThread.java:4325)
       at android.app.servertransaction.LaunchActivityItem.execute(LaunchActivityItem.java:101)
       at android.app.servertransaction.TransactionExecutor.executeCallbacks(TransactionExecutor.java:135)
       at android.app.servertransaction.TransactionExecutor.execute(TransactionExecutor.java:95)
       at android.app.ActivityThread$H.handleMessage(ActivityThread.java:2574)
       at android.os.Handler.dispatchMessage(Handler.java:106)
       at android.os.Looper.loopOnce(Looper.java:226)
       at android.os.Looper.loop(Looper.java:313)
       at android.app.ActivityThread.main(ActivityThread.java:8762)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:604)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:1067)

# Measurement Worker:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at m.lk.run(:com.google.android.gms.dynamite_measurementdynamite@234414038@23.44.14 (190400-0):71)

# DefaultDispatcher-worker-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# FinalizerDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:210)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:231)
       at java.lang.Daemons$FinalizerDaemon.runInternal(Daemons.java:309)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# queued-work-looper-data:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# ScionFrontendApi:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.awaitNanos(AbstractQueuedSynchronizer.java:1672)
       at java.util.concurrent.LinkedBlockingQueue.poll(LinkedBlockingQueue.java:460)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# DefaultDispatcher-worker-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# Crashlytics Exception Handler1:
       at dalvik.system.VMStack.getThreadStackTrace(VMStack.java)
       at java.lang.Thread.getStackTrace(Thread.java:1841)
       at java.lang.Thread.getAllStackTraces(Thread.java:1909)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateThreadsList(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateExecutionData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateEventApplicationData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.captureEventData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistEvent(SessionReportingCoordinator.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistFatalEvent(SessionReportingCoordinator.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsBackgroundWorker$3.then(CrashlyticsBackgroundWorker.java:16)
       at com.google.android.gms.tasks.zze.run(:8)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1145)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# com.google.firebase.crashlytics.startup1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# queued-work-looper-data:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# FinalizerWatchdogDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.lang.Daemons$FinalizerWatchdogDaemon.sleepUntilNeeded(Daemons.java:428)
       at java.lang.Daemons$FinalizerWatchdogDaemon.runInternal(Daemons.java:408)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# pool-10-thread-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# ReferenceQueueDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.lang.Daemons$ReferenceQueueDaemon.runInternal(Daemons.java:239)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# awaitEvenIfOnMainThread task continuation executor1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #0:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# GLThread 108:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at android.opengl.GLSurfaceView$GLThread.guardedRun(GLSurfaceView.java:1517)
       at android.opengl.GLSurfaceView$GLThread.run(GLSurfaceView.java:1287)

# queued-work-looper:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:335)
       at android.os.Looper.loopOnce(Looper.java:186)
       at android.os.Looper.loop(Looper.java:313)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# DefaultDispatcher-worker-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# Firebase Blocking Thread #0:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:401)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:903)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# GmsDynamite:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at com.google.android.gms.dynamite.zza.run(zza.java:16)

# RealmFinalizingDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:210)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:231)
       at io.realm.internal.FinalizerRunnable.run(FinalizerRunnable.java:3)
       at java.lang.Thread.run(Thread.java:1012)
 
</details>
 </details>
  
   <details>
    
   <summary>Galaxy S21 Ultra 5G</summary> :iphone:
   
![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/ea5e946f-839e-4078-a183-0930823527fd)

<details>

 *<summary>Details</summary>*
# Crashlytics - Stack trace
# Application: com.weeklyplannerapp.weekplan
# Platform: android
# Version: 7.97 (82)
# Issue: 30364b096c1e773c6989f0efeae40e19
# Session: 654E5E2501E40001647761402E3B9D47_DNE_0_v2
# Date: Fri Nov 10 2023 19:08:22 GMT+0200 (Eastern European Standard Time)

# Fatal Exception: java.lang.ArrayIndexOutOfBoundsException: length=0; index=0
       at com.weeklyplannerapp.weekplan.View.settings.importexport.ImportExportFragment.onRequestPermissionsResult(ImportExportFragment.java:1)
       at androidx.fragment.app.FragmentManager$10.onActivityResult(FragmentManager.java:126)
       at androidx.fragment.app.FragmentManager$10.onActivityResult(FragmentManager.java:126)
       at androidx.activity.result.ActivityResultRegistry.doDispatch(ActivityResultRegistry.java:47)
       at androidx.activity.result.ActivityResultRegistry.dispatchResult(ActivityResultRegistry.java:47)
       at androidx.activity.ComponentActivity.onRequestPermissionsResult(ComponentActivity.java:20)
       at androidx.fragment.app.FragmentActivity.onRequestPermissionsResult(FragmentActivity.java:1)
       at android.app.Activity.requestPermissions(Activity.java:5486)
       at androidx.core.app.ActivityCompat$Api23Impl.requestPermissions(ActivityCompat.java:1)
       at androidx.core.app.ActivityCompat.requestPermissions(ActivityCompat.java:120)
       at androidx.activity.ComponentActivity$2.b(ComponentActivity.java:96)
       at androidx.activity.result.ActivityResultRegistry$3.launch(ActivityResultRegistry.java:44)
       at androidx.activity.result.ActivityResultLauncher.launch(ActivityResultLauncher.java:44)
       at androidx.fragment.app.FragmentManager.launchRequestPermissions(FragmentManager.java:29)
       at androidx.fragment.app.Fragment.requestPermissions(Fragment.java:29)
       at com.weeklyplannerapp.weekplan.View.settings.importexport.ImportExportFragment.initListeners$lambda$11(ImportExportFragment.java:963)
       at android.view.View.performClick(View.java:7892)
       at android.widget.TextView.performClick(TextView.java:16220)
       at android.view.View.performClickInternal(View.java:7869)
       at android.view.View.-$$Nest$mperformClickInternal()
       at android.view.View$PerformClick.run(View.java:30891)
       at android.os.Handler.handleCallback(Handler.java:942)
       at android.os.Handler.dispatchMessage(Handler.java:99)
       at android.os.Looper.loopOnce(Looper.java:226)
       at android.os.Looper.loop(Looper.java:313)
       at android.app.ActivityThread.main(ActivityThread.java:8762)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:604)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:1067)

# PlayBillingLibrary-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# DefaultDispatcher-worker-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# PlayBillingLibrary-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# InsetsAnimations:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:335)
       at android.os.Looper.loopOnce(Looper.java:186)
       at android.os.Looper.loop(Looper.java:313)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# com.google.firebase.crashlytics.startup1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# pool-10-thread-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# FinalizerDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:210)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:231)
       at java.lang.Daemons$FinalizerDaemon.runInternal(Daemons.java:309)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# RealmFinalizingDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:210)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:231)
       at io.realm.internal.FinalizerRunnable.run(FinalizerRunnable.java:3)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-4:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #0:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# Timer-718:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.util.TimerThread.mainLoop(Timer.java:534)
       at java.util.TimerThread.run(Timer.java:513)

# Firebase Background Thread #2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# Timer-1:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.util.TimerThread.mainLoop(Timer.java:534)
       at java.util.TimerThread.run(Timer.java:513)

# DefaultDispatcher-worker-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# awaitEvenIfOnMainThread task continuation executor1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-4:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# glide-disk-cache-thread-0:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.PriorityBlockingQueue.take(PriorityBlockingQueue.java:538)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultThreadFactory$1.run(GlideExecutor.java:2022)
       at java.lang.Thread.run(Thread.java:1012)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultPriorityThreadFactory$1.run(GlideExecutor.java:12)

# GoogleApiHandler:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:335)
       at android.os.Looper.loopOnce(Looper.java:186)
       at android.os.Looper.loop(Looper.java:313)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# PlayBillingLibrary-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Crashlytics Exception Handler1:
       at dalvik.system.VMStack.getThreadStackTrace(VMStack.java)
       at java.lang.Thread.getStackTrace(Thread.java:1841)
       at java.lang.Thread.getAllStackTraces(Thread.java:1909)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateThreadsList(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateExecutionData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateEventApplicationData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.captureEventData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistEvent(SessionReportingCoordinator.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistFatalEvent(SessionReportingCoordinator.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsBackgroundWorker$3.then(CrashlyticsBackgroundWorker.java:16)
       at com.google.android.gms.tasks.zze.run(:8)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1145)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# GLThread 81:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at android.opengl.GLSurfaceView$GLThread.guardedRun(GLSurfaceView.java:1517)
       at android.opengl.GLSurfaceView$GLThread.run(GLSurfaceView.java:1287)

# PlayBillingLibrary-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# glide-source-thread-0:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.PriorityBlockingQueue.take(PriorityBlockingQueue.java:538)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultThreadFactory$1.run(GlideExecutor.java:2022)
       at java.lang.Thread.run(Thread.java:1012)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultPriorityThreadFactory$1.run(GlideExecutor.java:12)

# GmsDynamite:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at com.google.android.gms.dynamite.zza.run(zza.java:16)

# Timer-719:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.util.TimerThread.mainLoop(Timer.java:534)
       at java.util.TimerThread.run(Timer.java:513)

queued-work-looper-data:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# DefaultDispatcher-worker-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# Timer-0:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.util.TimerThread.mainLoop(Timer.java:534)
       at java.util.TimerThread.run(Timer.java:513)

# Timer-717:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.util.TimerThread.mainLoop(Timer.java:534)
       at java.util.TimerThread.run(Timer.java:513)

# ReferenceQueueDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.lang.Daemons$ReferenceQueueDaemon.runInternal(Daemons.java:239)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# AsyncTask #151:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.SynchronousQueue$TransferStack$SNode.block(SynchronousQueue.java:288)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:397)
       at java.util.concurrent.SynchronousQueue.take(SynchronousQueue.java:886)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# glide-source-thread-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.PriorityBlockingQueue.take(PriorityBlockingQueue.java:538)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultThreadFactory$1.run(GlideExecutor.java:2022)
       at java.lang.Thread.run(Thread.java:1012)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultPriorityThreadFactory$1.run(GlideExecutor.java:12)

# magnifier pixel copy result handler:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:335)
       at android.os.Looper.loopOnce(Looper.java:186)
       at android.os.Looper.loop(Looper.java:313)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# FinalizerWatchdogDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.lang.Daemons$FinalizerWatchdogDaemon.sleepUntilNeeded(Daemons.java:428)
       at java.lang.Daemons$FinalizerWatchdogDaemon.runInternal(Daemons.java:408)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-4:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Measurement Worker:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at m.lk.run(:com.google.android.gms.dynamite_measurementdynamite@234414038@23.44.14 (190400-0):71)

# glide-source-thread-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.PriorityBlockingQueue.take(PriorityBlockingQueue.java:538)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultThreadFactory$1.run(GlideExecutor.java:2022)
       at java.lang.Thread.run(Thread.java:1012)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultPriorityThreadFactory$1.run(GlideExecutor.java:12)

# glide-active-resources:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:210)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:231)
       at com.bumptech.glide.load.engine.ActiveResources.cleanReferenceQueue(ActiveResources.java:320)
       at com.bumptech.glide.load.engine.ActiveResources$2.run(ActiveResources.java:320)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1145)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.bumptech.glide.load.engine.ActiveResources$1$1.run(ActiveResources.java:2040)
       at java.lang.Thread.run(Thread.java:1012)

# Timer-716:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.util.TimerThread.mainLoop(Timer.java:534)
       at java.util.TimerThread.run(Timer.java:513)

# glide-source-thread-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.PriorityBlockingQueue.take(PriorityBlockingQueue.java:538)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultThreadFactory$1.run(GlideExecutor.java:2022)
       at java.lang.Thread.run(Thread.java:1012)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultPriorityThreadFactory$1.run(GlideExecutor.java:12)

# ConnectivityThread:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:335)
       at android.os.Looper.loopOnce(Looper.java:186)
       at android.os.Looper.loop(Looper.java:313)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# Okio Watchdog:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at com.android.okhttp.okio.AsyncTimeout.awaitTimeout(AsyncTimeout.java:313)
       at com.android.okhttp.okio.AsyncTimeout.access$000(AsyncTimeout.java:42)
       at com.android.okhttp.okio.AsyncTimeout$Watchdog.run(AsyncTimeout.java:288)

# Firebase Background Thread #3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-5:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# ScionFrontendApi:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.awaitNanos(AbstractQueuedSynchronizer.java:1672)
       at java.util.concurrent.LinkedBlockingQueue.poll(LinkedBlockingQueue.java:460)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# queued-work-looper:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:335)
       at android.os.Looper.loopOnce(Looper.java:186)
       at android.os.Looper.loop(Looper.java:313)
       at android.os.HandlerThread.run(HandlerThread.java:67)

</details>

![Screenshot 2023-11-18 140839](https://github.com/UserQA07/Week-Planner-/assets/144763744/987497bf-b3f6-49b7-a15d-5b2480c2ed7a)

<details>

*<summary>Details</summary>*

# Crashlytics - Stack trace
# Application: com.weeklyplannerapp.weekplan
# Platform: android
# Version: 7.97 (82)
# Issue: 60e1a4a0b315661c5942ac36fcf47881
# Session: 6550DC08020A000178104CD6B08B04C3_DNE_0_v2
# Date: Sun Nov 12 2023 18:22:46 GMT+0200 (Eastern European Standard Time)

# Fatal Exception: java.lang.NullPointerException: Attempt to invoke interface method 'int java.lang.CharSequence.length()' on a null object reference
       at android.text.BoringLayout.isBoring(BoringLayout.java:477)
       at android.widget.TextView.makeSingleLayout(TextView.java:10265)
       at android.widget.TextView.makeNewLayout(TextView.java:10115)
       at android.widget.TextView.checkForRelayout(TextView.java:10873)
       at android.widget.TextView.setText(TextView.java:6965)
       at android.widget.TextView.setText(TextView.java:6751)
       at android.widget.TextView.setText(TextView.java:6703)
       at com.weeklyplannerapp.weekplan.View.PurchaseScreenHandler.updatePrice(PurchaseScreenHandler.java:1)
       at com.weeklyplannerapp.weekplan.View.Activities.MainActivity.updatePrice(MainActivity.java:1)
       at com.weeklyplannerapp.weekplan.Service.Billing.BillingServiceImpl$InventoryCallback.onLoadedAvailableProducts(BillingServiceImpl.java:295)
       at com.weeklyplannerapp.weekplan.Service.Billing.BillingServiceImpl$initializeBillingService$1.onBillingSetupFinished$lambda$1(BillingServiceImpl.java:295)
       at com.android.billingclient.api.BillingClientImpl.zzJ(BillingClientImpl.java:2184)
       at com.android.billingclient.api.zzl.run(zzl.java:2184)
       at com.android.billingclient.api.zzw.run(zzw.java:2124)
       at android.os.Handler.handleCallback(Handler.java:942)
       at android.os.Handler.dispatchMessage(Handler.java:99)
       at android.os.Looper.loopOnce(Looper.java:226)
       at android.os.Looper.loop(Looper.java:313)
       at android.app.ActivityThread.main(ActivityThread.java:8762)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:604)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:1067)

# com.google.firebase.crashlytics.startup1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# ReferenceQueueDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.lang.Daemons$ReferenceQueueDaemon.runInternal(Daemons.java:239)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# AsyncTask #5:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.SynchronousQueue$TransferStack$SNode.block(SynchronousQueue.java:288)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:397)
       at java.util.concurrent.SynchronousQueue.take(SynchronousQueue.java:886)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# pool-10-thread-1:
       at android.database.sqlite.SQLiteConnection.nativeExecute(SQLiteConnection.java)
       at android.database.sqlite.SQLiteConnection.execute(SQLiteConnection.java:1015)
       at android.database.sqlite.SQLiteSession.endTransactionUnchecked(SQLiteSession.java:439)
       at android.database.sqlite.SQLiteSession.endTransaction(SQLiteSession.java:403)
       at android.database.sqlite.SQLiteDatabase.endTransaction(SQLiteDatabase.java:974)
       at com.google.android.datatransport.runtime.scheduling.persistence.SQLiteEventStore.runCriticalSection(SQLiteEventStore.java:48)
       at com.google.android.datatransport.runtime.scheduling.DefaultScheduler.lambda$schedule$1(DefaultScheduler.java:65)
       at com.google.android.datatransport.runtime.SafeLoggingExecutor$SafeLoggingRunnable.run(SafeLoggingExecutor.java:9)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1145)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# FinalizerWatchdogDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.lang.Daemons$FinalizerWatchdogDaemon.sleepUntilNeeded(Daemons.java:428)
       at java.lang.Daemons$FinalizerWatchdogDaemon.runInternal(Daemons.java:408)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #0:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-6:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# DefaultDispatcher-worker-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# Firebase Background Thread #2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# DefaultDispatcher-worker-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# PlayBillingLibrary-7:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# GLThread 808:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at android.opengl.GLSurfaceView$GLThread.guardedRun(GLSurfaceView.java:1517)
       at android.opengl.GLSurfaceView$GLThread.run(GLSurfaceView.java:1287)

# Timer-0:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.util.TimerThread.mainLoop(Timer.java:534)
       at java.util.TimerThread.run(Timer.java:513)

# FinalizerDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:210)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:231)
       at java.lang.Daemons$FinalizerDaemon.runInternal(Daemons.java:309)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# RealmFinalizingDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:210)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:231)
       at io.realm.internal.FinalizerRunnable.run(FinalizerRunnable.java:3)
       at java.lang.Thread.run(Thread.java:1012)

# queued-work-looper:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:335)
       at android.os.Looper.loopOnce(Looper.java:186)
       at android.os.Looper.loop(Looper.java:313)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# queued-work-looper-data:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Okio Watchdog:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at com.android.okhttp.okio.AsyncTimeout.awaitTimeout(AsyncTimeout.java:313)
       at com.android.okhttp.okio.AsyncTimeout.access$000(AsyncTimeout.java:42)
       at com.android.okhttp.okio.AsyncTimeout$Watchdog.run(AsyncTimeout.java:288)

# Timer-1:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.util.TimerThread.mainLoop(Timer.java:534)
       at java.util.TimerThread.run(Timer.java:513)

# Crashlytics Exception Handler1:
       at dalvik.system.VMStack.getThreadStackTrace(VMStack.java)
       at java.lang.Thread.getStackTrace(Thread.java:1841)
       at java.lang.Thread.getAllStackTraces(Thread.java:1909)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateThreadsList(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateExecutionData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateEventApplicationData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.captureEventData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistEvent(SessionReportingCoordinator.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistFatalEvent(SessionReportingCoordinator.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsBackgroundWorker$3.then(CrashlyticsBackgroundWorker.java:16)
       at com.google.android.gms.tasks.zze.run(:8)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1145)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# awaitEvenIfOnMainThread task continuation executor1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# GmsDynamite:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at com.google.android.gms.dynamite.zza.run(zza.java:16)

# PlayBillingLibrary-4:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-5:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# DefaultDispatcher-worker-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# PlayBillingLibrary-8:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# InsetsAnimations:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:335)
       at android.os.Looper.loopOnce(Looper.java:186)
       at android.os.Looper.loop(Looper.java:313)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# PlayBillingLibrary-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# queued-work-looper-data:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)
</details>
   </details>

  <details>

   <summary>Galaxy S22 Ultra</summary>

![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/176b5bf6-7e25-47b7-af88-9b1272866a0b)

<details>

*<summary>Details</summary>*

# Crashlytics - Stack trace
# Application: com.weeklyplannerapp.weekplan
# Platform: android
# Version: 7.97 (82)
# Issue: a8a333571d8e84369b076b908a30e05b
# Session: 65511BCF00660001241DBC48E6F251FF_DNE_0_v2
# Date: Sun Nov 12 2023 21:23:26 GMT+0200 (Eastern European Standard Time)

# Fatal Exception: java.lang.ArrayIndexOutOfBoundsException: length=5; index=-2
       at com.weeklyplannerapp.weekplan.View.settings.settingsmain.SettingsFragment$settingsCallback$1.onItemClicked(SettingsFragment.java:357)
       at com.weeklyplannerapp.weekplan.View.settings.settingsmain.SettingItemAdapter$SettingsItemHolder._init_$lambda$0(SettingItemAdapter.java:357)
       at android.view.View.performClick(View.java:7892)
       at android.view.View.performClickInternal(View.java:7869)
       at android.view.View.-$$Nest$mperformClickInternal()
       at android.view.View$PerformClick.run(View.java:30891)
       at android.os.Handler.handleCallback(Handler.java:942)
       at android.os.Handler.dispatchMessage(Handler.java:99)
       at android.os.Looper.loopOnce(Looper.java:226)
       at android.os.Looper.loop(Looper.java:313)
       at android.app.ActivityThread.main(ActivityThread.java:8762)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:604)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:1067)

# DefaultDispatcher-worker-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:357)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# PlayBillingLibrary-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# FinalizerDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:203)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:224)
       at java.lang.Daemons$FinalizerDaemon.runInternal(Daemons.java:300)
       at java.lang.Daemons$Daemon.run(Daemons.java:140)
       at java.lang.Thread.run(Thread.java:1012)

# ConnectivityThread:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:335)
       at android.os.Looper.loopOnce(Looper.java:186)
       at android.os.Looper.loop(Looper.java:313)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# OkHttp ConnectionPool:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:234)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.awaitNanos(AbstractQueuedSynchronizer.java:2123)
       at java.util.concurrent.LinkedBlockingQueue.poll(LinkedBlockingQueue.java:458)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1062)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-6:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

RealmFinalizingDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:203)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:224)
       at io.realm.internal.FinalizerRunnable.run(FinalizerRunnable.java:3)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Blocking Thread #1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:234)
       at java.util.concurrent.SynchronousQueue$TransferStack.awaitFulfill(SynchronousQueue.java:463)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:361)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:939)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1062)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# Okio Watchdog:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at com.android.okhttp.okio.AsyncTimeout.awaitTimeout(AsyncTimeout.java:313)
       at com.android.okhttp.okio.AsyncTimeout.access$000(AsyncTimeout.java:42)
       at com.android.okhttp.okio.AsyncTimeout$Watchdog.run(AsyncTimeout.java:288)

# GLThread 5359:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at android.opengl.GLSurfaceView$GLThread.guardedRun(GLSurfaceView.java:1517)
       at android.opengl.GLSurfaceView$GLThread.run(GLSurfaceView.java:1287)

# PlayBillingLibrary-5:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# DefaultDispatcher-worker-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:357)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# PlayBillingLibrary-4:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# AsyncTask #1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:234)
       at java.util.concurrent.SynchronousQueue$TransferStack.awaitFulfill(SynchronousQueue.java:463)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:361)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:939)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1062)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-5:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# glide-source-thread-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.PriorityBlockingQueue.take(PriorityBlockingQueue.java:549)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultThreadFactory$1.run(GlideExecutor.java:2022)
       at java.lang.Thread.run(Thread.java:1012)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultPriorityThreadFactory$1.run(GlideExecutor.java:12)

# Firebase Background Thread #3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# pool-11-thread-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# Crashlytics Exception Handler1:
       at dalvik.system.VMStack.getThreadStackTrace(VMStack.java)
       at java.lang.Thread.getStackTrace(Thread.java:1841)
       at java.lang.Thread.getAllStackTraces(Thread.java:1909)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateThreadsList(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateExecutionData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateEventApplicationData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.captureEventData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistEvent(SessionReportingCoordinator.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistFatalEvent(SessionReportingCoordinator.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsBackgroundWorker$3.then(CrashlyticsBackgroundWorker.java:16)
       at com.google.android.gms.tasks.zze.run(:8)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1137)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# Measurement Worker:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at m.lk.run(:com.google.android.gms.dynamite_measurementdynamite@234414038@23.44.14 (190400-0):71)

# PlayBillingLibrary-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# Timer-2:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at java.util.TimerThread.mainLoop(Timer.java:534)
       at java.util.TimerThread.run(Timer.java:513)

# ReferenceQueueDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at java.lang.Daemons$ReferenceQueueDaemon.runInternal(Daemons.java:232)
       at java.lang.Daemons$Daemon.run(Daemons.java:140)
       at java.lang.Thread.run(Thread.java:1012)

# DefaultDispatcher-worker-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:357)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# Timer-3:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at java.util.TimerThread.mainLoop(Timer.java:534)
       at java.util.TimerThread.run(Timer.java:513)

# glide-source-thread-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.PriorityBlockingQueue.take(PriorityBlockingQueue.java:549)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultThreadFactory$1.run(GlideExecutor.java:2022)
       at java.lang.Thread.run(Thread.java:1012)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultPriorityThreadFactory$1.run(GlideExecutor.java:12)

# PlayBillingLibrary-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# FinalizerWatchdogDaemon:
       at java.lang.Thread.sleep(Thread.java)
       at java.lang.Thread.sleep(Thread.java:450)
       at java.lang.Thread.sleep(Thread.java:355)
       at java.lang.Daemons$FinalizerWatchdogDaemon.sleepForNanos(Daemons.java:438)
       at java.lang.Daemons$FinalizerWatchdogDaemon.waitForProgress(Daemons.java:480)
       at java.lang.Daemons$FinalizerWatchdogDaemon.runInternal(Daemons.java:369)
       at java.lang.Daemons$Daemon.run(Daemons.java:140)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-7:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-6:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #0:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# glide-disk-cache-thread-0:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.PriorityBlockingQueue.take(PriorityBlockingQueue.java:549)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultThreadFactory$1.run(GlideExecutor.java:2022)
       at java.lang.Thread.run(Thread.java:1012)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultPriorityThreadFactory$1.run(GlideExecutor.java:12)

# PlayBillingLibrary-4:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-8:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# awaitEvenIfOnMainThread task continuation executor1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# queued-work-looper:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:335)
       at android.os.Looper.loopOnce(Looper.java:186)
       at android.os.Looper.loop(Looper.java:313)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# glide-source-thread-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.PriorityBlockingQueue.take(PriorityBlockingQueue.java:549)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultThreadFactory$1.run(GlideExecutor.java:2022)
       at java.lang.Thread.run(Thread.java:1012)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultPriorityThreadFactory$1.run(GlideExecutor.java:12)

# queued-work-looper-data:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# glide-active-resources:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:203)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:224)
       at com.bumptech.glide.load.engine.ActiveResources.cleanReferenceQueue(ActiveResources.java:320)
       at com.bumptech.glide.load.engine.ActiveResources$2.run(ActiveResources.java:320)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1137)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.bumptech.glide.load.engine.ActiveResources$1$1.run(ActiveResources.java:2040)
       at java.lang.Thread.run(Thread.java:1012)

# AsyncTask #3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:234)
       at java.util.concurrent.SynchronousQueue$TransferStack.awaitFulfill(SynchronousQueue.java:463)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:361)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:939)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1062)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# glide-source-thread-0:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.PriorityBlockingQueue.take(PriorityBlockingQueue.java:549)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultThreadFactory$1.run(GlideExecutor.java:2022)
       at java.lang.Thread.run(Thread.java:1012)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultPriorityThreadFactory$1.run(GlideExecutor.java:12)

# PlayBillingLibrary-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-7:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# com.google.firebase.crashlytics.startup1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# Timer-1:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at java.util.TimerThread.mainLoop(Timer.java:534)
       at java.util.TimerThread.run(Timer.java:513)

# Timer-0:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at java.util.TimerThread.mainLoop(Timer.java:534)
       at java.util.TimerThread.run(Timer.java:513)

# PlayBillingLibrary-8:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# GmsDynamite:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at com.google.android.gms.dynamite.zza.run(zza.java:16)

# PlayBillingLibrary-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# ScionFrontendApi:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:234)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.awaitNanos(AbstractQueuedSynchronizer.java:2123)
       at java.util.concurrent.LinkedBlockingQueue.poll(LinkedBlockingQueue.java:458)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1062)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)
 
</details>
  
  </details>

 
  <details>
   
   <summary>Galaxy S20</summary>

![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/1ae90cbd-e989-4cd9-9e9c-9dd2a1d480c3)

<details>

*<summary>Details</summary>*

# Crashlytics - Stack trace
# Application: com.weeklyplannerapp.weekplan
# Platform: android
# Version: 7.97 (82)
# Issue: 0e21321ff6cf393a125939dfa7dbf720
# Session: 654E946E00A100012C58F1A56F45003E_DNE_3_v2
# Date: Fri Nov 10 2023 23:17:17 GMT+0200 (Eastern European Standard Time)

# Fatal Exception: android.os.DeadSystemRuntimeException: android.os.DeadSystemException
       at android.view.autofill.AutofillManager.updateSessionLocked(AutofillManager.java:2184)
       at android.view.autofill.AutofillManager.notifyViewEnteredLocked(AutofillManager.java:1302)
       at android.view.autofill.AutofillManager.notifyViewEntered(AutofillManager.java:1250)
       at android.view.autofill.AutofillManager.notifyViewEntered(AutofillManager.java:1165)
       at android.view.View.notifyEnterOrExitForAutoFillIfNeeded(View.java:8593)
       at android.view.View.performClick(View.java:7889)
       at android.widget.TextView.performClick(TextView.java:16201)
       at android.view.View.performClickInternal(View.java:7858)
       at android.view.View.-$$Nest$mperformClickInternal()
       at android.view.View$PerformClick.run(View.java:30863)
       at android.os.Handler.handleCallback(Handler.java:942)
       at android.os.Handler.dispatchMessage(Handler.java:99)
       at android.os.Looper.loopOnce(Looper.java:226)
       at android.os.Looper.loop(Looper.java:313)
       at android.app.ActivityThread.main(ActivityThread.java:8741)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:571)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:1067)

# Caused by android.os.DeadSystemException:
       at android.view.autofill.AutofillManager.updateSessionLocked(AutofillManager.java:2184)
       at android.view.autofill.AutofillManager.notifyViewEnteredLocked(AutofillManager.java:1302)
       at android.view.autofill.AutofillManager.notifyViewEntered(AutofillManager.java:1250)
       at android.view.autofill.AutofillManager.notifyViewEntered(AutofillManager.java:1165)
       at android.view.View.notifyEnterOrExitForAutoFillIfNeeded(View.java:8593)
       at android.view.View.performClick(View.java:7889)
       at android.widget.TextView.performClick(TextView.java:16201)
       at android.view.View.performClickInternal(View.java:7858)
       at android.view.View.-$$Nest$mperformClickInternal()
       at android.view.View$PerformClick.run(View.java:30863)
       at android.os.Handler.handleCallback(Handler.java:942)
       at android.os.Handler.dispatchMessage(Handler.java:99)
       at android.os.Looper.loopOnce(Looper.java:226)
       at android.os.Looper.loop(Looper.java:313)
       at android.app.ActivityThread.main(ActivityThread.java:8741)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:571)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:1067)

# ConnectivityThread:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:335)
       at android.os.Looper.loopOnce(Looper.java:186)
       at android.os.Looper.loop(Looper.java:313)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# queued-work-looper:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:335)
       at android.os.Looper.loopOnce(Looper.java:186)
       at android.os.Looper.loop(Looper.java:313)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# PlayBillingLibrary-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# DefaultDispatcher-worker-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:357)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# glide-source-thread-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.PriorityBlockingQueue.take(PriorityBlockingQueue.java:549)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultThreadFactory$1.run(GlideExecutor.java:2022)
       at java.lang.Thread.run(Thread.java:1012)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultPriorityThreadFactory$1.run(GlideExecutor.java:12)

# PlayBillingLibrary-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# ReferenceQueueDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at java.lang.Daemons$ReferenceQueueDaemon.runInternal(Daemons.java:232)
       at java.lang.Daemons$Daemon.run(Daemons.java:140)
       at java.lang.Thread.run(Thread.java:1012)

# FinalizerWatchdogDaemon:
       at java.lang.Thread.sleep(Thread.java)
       at java.lang.Thread.sleep(Thread.java:450)
       at java.lang.Thread.sleep(Thread.java:355)
       at java.lang.Daemons$FinalizerWatchdogDaemon.sleepForNanos(Daemons.java:438)
       at java.lang.Daemons$FinalizerWatchdogDaemon.waitForProgress(Daemons.java:480)
       at java.lang.Daemons$FinalizerWatchdogDaemon.runInternal(Daemons.java:369)
       at java.lang.Daemons$Daemon.run(Daemons.java:140)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# RxSchedulerPurge-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:234)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.awaitNanos(AbstractQueuedSynchronizer.java:2123)
       at java.util.concurrent.ScheduledThreadPoolExecutor$DelayedWorkQueue.take(ScheduledThreadPoolExecutor.java:1188)
       at java.util.concurrent.ScheduledThreadPoolExecutor$DelayedWorkQueue.take(ScheduledThreadPoolExecutor.java:905)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-6:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# pool-11-thread-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-7:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# com.google.firebase.crashlytics.startup1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# glide-active-resources:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:203)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:224)
       at com.bumptech.glide.load.engine.ActiveResources.cleanReferenceQueue(ActiveResources.java:320)
       at com.bumptech.glide.load.engine.ActiveResources$2.run(ActiveResources.java:320)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1137)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.bumptech.glide.load.engine.ActiveResources$1$1.run(ActiveResources.java:2040)
       at java.lang.Thread.run(Thread.java:1012)

# awaitEvenIfOnMainThread task continuation executor1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# FinalizerDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:203)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:224)
       at java.lang.Daemons$FinalizerDaemon.runInternal(Daemons.java:300)
       at java.lang.Daemons$Daemon.run(Daemons.java:140)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-5:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-8:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-4:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-7:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-8:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-5:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-4:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-6:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# InsetsAnimations:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:335)
       at android.os.Looper.loopOnce(Looper.java:186)
       at android.os.Looper.loop(Looper.java:313)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# DefaultDispatcher-worker-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:357)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# DefaultDispatcher-worker-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:357)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# PlayBillingLibrary-4:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# Okio Watchdog:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at com.android.okhttp.okio.AsyncTimeout.awaitTimeout(AsyncTimeout.java:313)
       at com.android.okhttp.okio.AsyncTimeout.access$000(AsyncTimeout.java:42)
       at com.android.okhttp.okio.AsyncTimeout$Watchdog.run(AsyncTimeout.java:288)

# PlayBillingLibrary-4:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# magnifier pixel copy result handler:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:335)
       at android.os.Looper.loopOnce(Looper.java:186)
       at android.os.Looper.loop(Looper.java:313)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# ModernAsyncTask #1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-7:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# glide-disk-cache-thread-0:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.PriorityBlockingQueue.take(PriorityBlockingQueue.java:549)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultThreadFactory$1.run(GlideExecutor.java:2022)
       at java.lang.Thread.run(Thread.java:1012)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultPriorityThreadFactory$1.run(GlideExecutor.java:12)

# PlayBillingLibrary-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# GmsDynamite:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at com.google.android.gms.dynamite.zza.run(zza.java:16)

# AsyncTask #37:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.SynchronousQueue$TransferStack.awaitFulfill(SynchronousQueue.java:461)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:361)
       at java.util.concurrent.SynchronousQueue.take(SynchronousQueue.java:922)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-8:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# GoogleApiHandler:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:335)
       at android.os.Looper.loopOnce(Looper.java:186)
       at android.os.Looper.loop(Looper.java:313)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# PlayBillingLibrary-5:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-6:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# glide-source-thread-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.PriorityBlockingQueue.take(PriorityBlockingQueue.java:549)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultThreadFactory$1.run(GlideExecutor.java:2022)
       at java.lang.Thread.run(Thread.java:1012)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultPriorityThreadFactory$1.run(GlideExecutor.java:12)

# Crashlytics Exception Handler1:
       at dalvik.system.VMStack.getThreadStackTrace(VMStack.java)
       at java.lang.Thread.getStackTrace(Thread.java:1841)
       at java.lang.Thread.getAllStackTraces(Thread.java:1909)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateThreadsList(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateExecutionData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateEventApplicationData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.captureEventData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistEvent(SessionReportingCoordinator.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistFatalEvent(SessionReportingCoordinator.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsBackgroundWorker$3.then(CrashlyticsBackgroundWorker.java:16)
       at com.google.android.gms.tasks.zze.run(:8)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1137)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-6:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# GLThread 1702:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at android.opengl.GLSurfaceView$GLThread.guardedRun(GLSurfaceView.java:1517)
       at android.opengl.GLSurfaceView$GLThread.run(GLSurfaceView.java:1287)

# Firebase Background Thread #2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# glide-source-thread-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.PriorityBlockingQueue.take(PriorityBlockingQueue.java:549)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultThreadFactory$1.run(GlideExecutor.java:2022)
       at java.lang.Thread.run(Thread.java:1012)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultPriorityThreadFactory$1.run(GlideExecutor.java:12)

# RxCachedWorkerPoolEvictor-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:234)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.awaitNanos(AbstractQueuedSynchronizer.java:2123)
       at java.util.concurrent.ScheduledThreadPoolExecutor$DelayedWorkQueue.take(ScheduledThreadPoolExecutor.java:1188)
       at java.util.concurrent.ScheduledThreadPoolExecutor$DelayedWorkQueue.take(ScheduledThreadPoolExecutor.java:905)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-8:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# RealmFinalizingDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:203)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:224)
       at io.realm.internal.FinalizerRunnable.run(FinalizerRunnable.java:3)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #0:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# queued-work-looper-data:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-7:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-5:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:433)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at java.lang.Thread.run(Thread.java:1012)

# glide-source-thread-0:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:194)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2081)
       at java.util.concurrent.PriorityBlockingQueue.take(PriorityBlockingQueue.java:549)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1063)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1123)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:637)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultThreadFactory$1.run(GlideExecutor.java:2022)
       at java.lang.Thread.run(Thread.java:1012)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultPriorityThreadFactory$1.run(GlideExecutor.java:12)
 
  </details>
 </details>
</details>


<details>
 
  <summary>Android 12</summary><br>

  <details>
 
<summary>Crash list</summary>

![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/8fa66526-e435-45e0-92a2-5b00ae002a70)


  </details>
 
<details>  



   
   <summary>Galaxy S21+ 5G</summary>
    
![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/bc63e9e0-9b0d-469e-aaa4-a15599e0b8a6)



<details>
 
   *<summary>Details</summary>*

 # Crashlytics - Stack trace
# Application: com.weeklyplannerapp.weekplan
# Platform: android
# Version: 7.97 (82)
# Issue: e004ae243fcb695a9a1a005a3caf8763
# Session: 654D32DB022300012EF274F23454FD50_DNE_0_v2
# Date: Thu Nov 09 2023 22:46:04 GMT+0200 (Eastern European Standard Time)

# Fatal Exception: java.lang.RuntimeException: Unable to stop activity {com.weeklyplannerapp.weekplan/com.weeklyplannerapp.weekplan.View.Activities.MainActivity}: java.lang.RuntimeException: write() failed: No space left on device in /tmp/realm-java/realm/realm-library/src/main/cpp/io_realm_internal_OsSharedRealm.cpp line 404
       at android.app.ActivityThread.callActivityOnStop(ActivityThread.java:5697)
       at android.app.ActivityThread.performStopActivityInner(ActivityThread.java:5633)
       at android.app.ActivityThread.handleStopActivity(ActivityThread.java:5734)
       at android.app.servertransaction.StopActivityItem.execute(StopActivityItem.java:43)
       at android.app.servertransaction.ActivityTransactionItem.execute(ActivityTransactionItem.java:45)
       at android.app.servertransaction.TransactionExecutor.executeLifecycleState(TransactionExecutor.java:176)
       at android.app.servertransaction.TransactionExecutor.execute(TransactionExecutor.java:97)
       at android.app.ActivityThread$H.handleMessage(ActivityThread.java:2425)
       at android.os.Handler.dispatchMessage(Handler.java:106)
       at android.os.Looper.loopOnce(Looper.java:226)
       at android.os.Looper.loop(Looper.java:313)
       at android.app.ActivityThread.main(ActivityThread.java:8582)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:563)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:1133)

# Caused by java.lang.RuntimeException: write() failed: No space left on device in /tmp/realm-java/realm/realm-library/src/main/cpp/io_realm_internal_OsSharedRealm.cpp line 404
       at io.realm.internal.OsSharedRealm.nativeWriteCopy(OsSharedRealm.java)
       at io.realm.internal.OsSharedRealm.writeCopy(OsSharedRealm.java:38)
       at io.realm.BaseRealm.writeCopyTo(BaseRealm.java:1)
       at com.weeklyplannerapp.weekplan.WeeklyPlanApplication$1.onActivityStopped(WeeklyPlanApplication.java:199)
       at android.app.Application.dispatchActivityStopped(Application.java:495)
       at android.app.Activity.dispatchActivityStopped(Activity.java:1503)
       at android.app.Activity.onStop(Activity.java:2678)
       at androidx.fragment.app.FragmentActivity.onStop(FragmentActivity.java:1)
       at androidx.appcompat.app.AppCompatActivity.onStop(AppCompatActivity.java:1)
       at com.weeklyplannerapp.weekplan.View.Activities.MainActivity.onStop(MainActivity.java)
       at android.app.Instrumentation.callActivityOnStop(Instrumentation.java:1496)
       at android.app.Activity.performStop(Activity.java:8528)
       at android.app.ActivityThread.callActivityOnStop(ActivityThread.java:5689)
       at android.app.ActivityThread.performStopActivityInner(ActivityThread.java:5633)
       at android.app.ActivityThread.handleStopActivity(ActivityThread.java:5734)
       at android.app.servertransaction.StopActivityItem.execute(StopActivityItem.java:43)
       at android.app.servertransaction.ActivityTransactionItem.execute(ActivityTransactionItem.java:45)
       at android.app.servertransaction.TransactionExecutor.executeLifecycleState(TransactionExecutor.java:176)
       at android.app.servertransaction.TransactionExecutor.execute(TransactionExecutor.java:97)
       at android.app.ActivityThread$H.handleMessage(ActivityThread.java:2425)
       at android.os.Handler.dispatchMessage(Handler.java:106)
       at android.os.Looper.loopOnce(Looper.java:226)
       at android.os.Looper.loop(Looper.java:313)
       at android.app.ActivityThread.main(ActivityThread.java:8582)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:563)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:1133)

# AsyncTask #6:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.SynchronousQueue$TransferStack$SNode.block(SynchronousQueue.java:288)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:397)
       at java.util.concurrent.SynchronousQueue.take(SynchronousQueue.java:886)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# DefaultDispatcher-worker-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# Firebase Background Thread #0:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# awaitEvenIfOnMainThread task continuation executor1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# com.google.firebase.crashlytics.startup1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# RealmFinalizingDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:210)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:231)
       at io.realm.internal.FinalizerRunnable.run(FinalizerRunnable.java:3)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Measurement Worker:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at m.lk.run(:com.google.android.gms.dynamite_measurementdynamite@234212044@23.42.12 (190400-0):71)

# PlayBillingLibrary-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-4:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# queued-work-looper:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:335)
       at android.os.Looper.loopOnce(Looper.java:186)
       at android.os.Looper.loop(Looper.java:313)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# ReferenceQueueDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.lang.Daemons$ReferenceQueueDaemon.runInternal(Daemons.java:239)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# Okio Watchdog:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at com.android.okhttp.okio.AsyncTimeout.awaitTimeout(AsyncTimeout.java:313)
       at com.android.okhttp.okio.AsyncTimeout.access$000(AsyncTimeout.java:42)
       at com.android.okhttp.okio.AsyncTimeout$Watchdog.run(AsyncTimeout.java:288)

# Firebase Blocking Thread #3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:401)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:903)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# queued-work-looper-data:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# FinalizerDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:210)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:231)
       at java.lang.Daemons$FinalizerDaemon.runInternal(Daemons.java:309)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# FinalizerWatchdogDaemon:
       at java.lang.Thread.sleep(Thread.java)
       at java.lang.Thread.sleep(Thread.java:450)
       at java.lang.Thread.sleep(Thread.java:355)
       at java.lang.Daemons$FinalizerWatchdogDaemon.sleepForNanos(Daemons.java:481)
       at java.lang.Daemons$FinalizerWatchdogDaemon.waitForProgress(Daemons.java:527)
       at java.lang.Daemons$FinalizerWatchdogDaemon.runInternal(Daemons.java:412)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# ScionFrontendApi:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.awaitNanos(AbstractQueuedSynchronizer.java:1672)
       at java.util.concurrent.LinkedBlockingQueue.poll(LinkedBlockingQueue.java:460)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# GLThread 78:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at android.opengl.GLSurfaceView$GLThread.guardedRun(GLSurfaceView.java:1517)
       at android.opengl.GLSurfaceView$GLThread.run(GLSurfaceView.java:1287)

# Firebase Background Thread #2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# DefaultDispatcher-worker-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# queued-work-looper-data:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# pool-10-thread-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# GmsDynamite:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at com.google.android.gms.dynamite.zza.run(zza.java:16)

# InsetsAnimations:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:335)
       at android.os.Looper.loopOnce(Looper.java:186)
       at android.os.Looper.loop(Looper.java:313)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# Crashlytics Exception Handler1:
       at dalvik.system.VMStack.getThreadStackTrace(VMStack.java)
       at java.lang.Thread.getStackTrace(Thread.java:1841)
       at java.lang.Thread.getAllStackTraces(Thread.java:1909)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateThreadsList(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateExecutionData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateEventApplicationData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.captureEventData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistEvent(SessionReportingCoordinator.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistFatalEvent(SessionReportingCoordinator.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsBackgroundWorker$3.then(CrashlyticsBackgroundWorker.java:16)
       at com.google.android.gms.tasks.zze.run(:8)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1145)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# DefaultDispatcher-worker-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)
 
</details>

![Screenshot 2023-11-18 230335](https://github.com/UserQA07/Week-Planner-/assets/144763744/744e60f2-79e7-46cb-9635-7fe49d3973cd)


<details>
 
   *<summary>Details</summary>*

 # Crashlytics - Stack trace
# Application: com.weeklyplannerapp.weekplan
# Platform: android
# Version: 7.97 (82)
# Issue: 72bd018209352c1b39c33f10f34b265c
# Session: 65523E30015D0001413C74F23454FD50_DNE_0_v2
# Date: Mon Nov 13 2023 21:53:30 GMT+0200 (Eastern European Standard Time)

Fatal Exception: io.realm.exceptions.RealmError: Unrecoverable error. Failed to open file at path '/data/data/com.weeklyplannerapp.weekplan/13.11.2023 20:53': No space left on device (/data/data/com.weeklyplannerapp.weekplan/13.11.2023 20:53) in /tmp/realm-java/realm/realm-library/src/main/cpp/io_realm_internal_OsSharedRealm.cpp line 404
       at io.realm.internal.OsSharedRealm.nativeWriteCopy(OsSharedRealm.java)
       at io.realm.internal.OsSharedRealm.writeCopy(OsSharedRealm.java:38)
       at io.realm.BaseRealm.writeCopyTo(BaseRealm.java:1)
       at com.weeklyplannerapp.weekplan.WeeklyPlanApplication$1.onActivityStopped(WeeklyPlanApplication.java:199)
       at android.app.Application.dispatchActivityStopped(Application.java:495)
       at android.app.Activity.dispatchActivityStopped(Activity.java:1503)
       at android.app.Activity.onStop(Activity.java:2678)
       at androidx.fragment.app.FragmentActivity.onStop(FragmentActivity.java:1)
       at androidx.appcompat.app.AppCompatActivity.onStop(AppCompatActivity.java:1)
       at com.weeklyplannerapp.weekplan.View.Activities.MainActivity.onStop(MainActivity.java)
       at android.app.Instrumentation.callActivityOnStop(Instrumentation.java:1496)
       at android.app.Activity.performStop(Activity.java:8528)
       at android.app.ActivityThread.callActivityOnStop(ActivityThread.java:5689)
       at android.app.ActivityThread.performStopActivityInner(ActivityThread.java:5633)
       at android.app.ActivityThread.handleStopActivity(ActivityThread.java:5734)
       at android.app.servertransaction.StopActivityItem.execute(StopActivityItem.java:43)
       at android.app.servertransaction.ActivityTransactionItem.execute(ActivityTransactionItem.java:45)
       at android.app.servertransaction.TransactionExecutor.executeLifecycleState(TransactionExecutor.java:176)
       at android.app.servertransaction.TransactionExecutor.execute(TransactionExecutor.java:97)
       at android.app.ActivityThread$H.handleMessage(ActivityThread.java:2425)
       at android.os.Handler.dispatchMessage(Handler.java:106)
       at android.os.Looper.loopOnce(Looper.java:226)
       at android.os.Looper.loop(Looper.java:313)
       at android.app.ActivityThread.main(ActivityThread.java:8582)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:563)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:1133)

# DefaultDispatcher-worker-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# pool-10-thread-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #0:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# RealmFinalizingDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:210)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:231)
       at io.realm.internal.FinalizerRunnable.run(FinalizerRunnable.java:3)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# FinalizerDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:210)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:231)
       at java.lang.Daemons$FinalizerDaemon.runInternal(Daemons.java:309)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# com.google.firebase.crashlytics.startup1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# ReferenceQueueDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.lang.Daemons$ReferenceQueueDaemon.runInternal(Daemons.java:239)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Blocking Thread #8:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:401)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:903)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# queued-work-looper:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:335)
       at android.os.Looper.loopOnce(Looper.java:186)
       at android.os.Looper.loop(Looper.java:313)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# Firebase Background Thread #3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# Okio Watchdog:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at com.android.okhttp.okio.AsyncTimeout.awaitTimeout(AsyncTimeout.java:313)
       at com.android.okhttp.okio.AsyncTimeout.access$000(AsyncTimeout.java:42)
       at com.android.okhttp.okio.AsyncTimeout$Watchdog.run(AsyncTimeout.java:288)

# GmsDynamite:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at com.google.android.gms.dynamite.zza.run(zza.java:16)

# PlayBillingLibrary-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-4:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# DefaultDispatcher-worker-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# GLThread 77:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at android.opengl.GLSurfaceView$GLThread.guardedRun(GLSurfaceView.java:1517)
       at android.opengl.GLSurfaceView$GLThread.run(GLSurfaceView.java:1287)

# queued-work-looper-data:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# Crashlytics Exception Handler1:
       at dalvik.system.VMStack.getThreadStackTrace(VMStack.java)
       at java.lang.Thread.getStackTrace(Thread.java:1841)
       at java.lang.Thread.getAllStackTraces(Thread.java:1909)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateThreadsList(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateExecutionData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateEventApplicationData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.captureEventData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistEvent(SessionReportingCoordinator.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistFatalEvent(SessionReportingCoordinator.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsBackgroundWorker$3.then(CrashlyticsBackgroundWorker.java:16)
       at com.google.android.gms.tasks.zze.run(:8)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1145)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# InsetsAnimations:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:335)
       at android.os.Looper.loopOnce(Looper.java:186)
       at android.os.Looper.loop(Looper.java:313)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# DefaultDispatcher-worker-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# ScionFrontendApi:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.awaitNanos(AbstractQueuedSynchronizer.java:1672)
       at java.util.concurrent.LinkedBlockingQueue.poll(LinkedBlockingQueue.java:460)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Measurement Worker:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at m.lk.run(:com.google.android.gms.dynamite_measurementdynamite@234212044@23.42.12 (190400-0):71)

# awaitEvenIfOnMainThread task continuation executor1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# queued-work-looper-data:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# FinalizerWatchdogDaemon:
       at java.lang.Thread.sleep(Thread.java)
       at java.lang.Thread.sleep(Thread.java:450)
       at java.lang.Thread.sleep(Thread.java:355)
       at java.lang.Daemons$FinalizerWatchdogDaemon.sleepForNanos(Daemons.java:481)
       at java.lang.Daemons$FinalizerWatchdogDaemon.waitForProgress(Daemons.java:544)
       at java.lang.Daemons$FinalizerWatchdogDaemon.runInternal(Daemons.java:412)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# AsyncTask #52:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.SynchronousQueue$TransferStack$SNode.block(SynchronousQueue.java:288)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:397)
       at java.util.concurrent.SynchronousQueue.take(SynchronousQueue.java:886)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)
 
</details>
 </details>


  <details>
  
   <summary>Poco X3 NFC</summary>

![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/6002e6ce-507f-4767-b75b-c54f14570c2c)



<details>
 
   *<summary>Details</summary>*

 # Crashlytics - Stack trace
# Application: com.weeklyplannerapp.weekplan
# Platform: android
# Version: 7.97 (82)
# Issue: 097370c30da6a1331a1a06941b9e3cb9
# Session: 654E380C026300014DC034E6D58BB165_DNE_0_v2
# Date: Fri Nov 10 2023 16:03:32 GMT+0200 (Eastern European Standard Time)

# Fatal Exception: java.lang.IndexOutOfBoundsException: input indexes are outside the CharSequence
       at miuix.toolbar.util.WordIterator.setCharSequence(WordIterator.java:46)
       at miuix.toolbar.internal.TextActionView.selectCurrentWord(TextActionView.java:186)
       at miuix.toolbar.internal.TextActionView.selectCurrentWord(TextActionView.java:158)
       at miuix.toolbar.internal.ActionView.selectCurrentWord(ActionView.java:61)
       at miuix.textaction.Select$1.onMenuItemClick(Select.java:25)
       at miuix.toolbar.internal.menu.MenuItemImpl.invoke(MenuItemImpl.java:141)
       at miuix.toolbar.internal.menu.MenuBuilder.performItemAction(MenuBuilder.java:938)
       at miuix.toolbar.FloatingActionMode$4.onMenuItemClick(FloatingActionMode.java:123)
       at miuix.toolbar.internal.FloatingToolbar$3.onClick(FloatingToolbar.java:188)
       at android.view.View.performClick(View.java:7745)
       at android.view.View.performClickInternal(View.java:7722)
       at android.view.View.access$3700(View.java:854)
       at android.view.View$PerformClick.run(View.java:29111)
       at android.os.Handler.handleCallback(Handler.java:938)
       at android.os.Handler.dispatchMessage(Handler.java:99)
       at android.os.Looper.loopOnce(Looper.java:210)
       at android.os.Looper.loop(Looper.java:299)
       at android.app.ActivityThread.main(ActivityThread.java:8319)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:556)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:1038)

# queued-work-looper:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:340)
       at android.os.Looper.loopOnce(Looper.java:168)
       at android.os.Looper.loop(Looper.java:299)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# AsyncTask #7:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:401)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:903)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# com.google.firebase.crashlytics.startup1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# AnimThread-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.SynchronousQueue$TransferStack$SNode.block(SynchronousQueue.java:288)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:397)
       at java.util.concurrent.SynchronousQueue.take(SynchronousQueue.java:886)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# AnimThread-5:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.SynchronousQueue$TransferStack$SNode.block(SynchronousQueue.java:288)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:397)
       at java.util.concurrent.SynchronousQueue.take(SynchronousQueue.java:886)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# FinalizerDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:210)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:231)
       at java.lang.Daemons$FinalizerDaemon.runInternal(Daemons.java:309)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# awaitEvenIfOnMainThread task continuation executor1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# ReferenceQueueDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.lang.Daemons$ReferenceQueueDaemon.runInternal(Daemons.java:239)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# GLThread 101:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at android.opengl.GLSurfaceView$GLThread.guardedRun(GLSurfaceView.java:1497)
       at android.opengl.GLSurfaceView$GLThread.run(GLSurfaceView.java:1272)

# PlayBillingLibrary-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# RealmFinalizingDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:210)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:231)
       at io.realm.internal.FinalizerRunnable.run(FinalizerRunnable.java:3)
       at java.lang.Thread.run(Thread.java:1012)

# InsetsAnimations:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:340)
       at android.os.Looper.loopOnce(Looper.java:168)
       at android.os.Looper.loop(Looper.java:299)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# DefaultDispatcher-worker-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# Crashlytics Exception Handler1:
       at dalvik.system.VMStack.getThreadStackTrace(VMStack.java)
       at java.lang.Thread.getStackTrace(Thread.java:1841)
       at java.lang.Thread.getAllStackTraces(Thread.java:1909)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateThreadsList(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateExecutionData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateEventApplicationData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.captureEventData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistEvent(SessionReportingCoordinator.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistFatalEvent(SessionReportingCoordinator.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsBackgroundWorker$3.then(CrashlyticsBackgroundWorker.java:16)
       at com.google.android.gms.tasks.zze.run(:8)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1145)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# process reaper:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:401)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:903)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# AsyncTask #8:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:401)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:903)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# AsyncTask #5:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:401)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:903)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# AnimThread-4:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.SynchronousQueue$TransferStack$SNode.block(SynchronousQueue.java:288)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:397)
       at java.util.concurrent.SynchronousQueue.take(SynchronousQueue.java:886)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-4:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# GmsDynamite:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at com.google.android.gms.dynamite.zza.run(zza.java:16)

# AnimThread-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.SynchronousQueue$TransferStack$SNode.block(SynchronousQueue.java:288)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:397)
       at java.util.concurrent.SynchronousQueue.take(SynchronousQueue.java:886)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# ScionFrontendApi:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.awaitNanos(AbstractQueuedSynchronizer.java:1672)
       at java.util.concurrent.LinkedBlockingQueue.poll(LinkedBlockingQueue.java:460)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# DefaultDispatcher-worker-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# AnimThread-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.SynchronousQueue$TransferStack$SNode.block(SynchronousQueue.java:288)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:397)
       at java.util.concurrent.SynchronousQueue.take(SynchronousQueue.java:886)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# 19904-ScoutStateMachine:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:340)
       at android.os.Looper.loopOnce(Looper.java:168)
       at android.os.Looper.loop(Looper.java:299)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# DefaultDispatcher-worker-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# Firebase Blocking Thread #0:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:401)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:903)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #0:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# LogThread:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:340)
       at android.os.Looper.loopOnce(Looper.java:168)
       at android.os.Looper.loop(Looper.java:299)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# FinalizerWatchdogDaemon:
       at java.lang.Thread.sleep(Thread.java)
       at java.lang.Thread.sleep(Thread.java:450)
       at java.lang.Thread.sleep(Thread.java:355)
       at java.lang.Daemons$FinalizerWatchdogDaemon.sleepForNanos(Daemons.java:481)
       at java.lang.Daemons$FinalizerWatchdogDaemon.waitForProgress(Daemons.java:544)
       at java.lang.Daemons$FinalizerWatchdogDaemon.runInternal(Daemons.java:412)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# pool-10-thread-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# AnimRunnerThread:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:340)
       at android.os.Looper.loopOnce(Looper.java:168)
       at android.os.Looper.loop(Looper.java:299)
       at android.os.HandlerThread.run(HandlerThread.java:67)
 
</details>
 </details>

<details>   
 
   <summary>Redmi Note 9S</summary> 

![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/128b6b2b-9a4f-4418-9e5d-86dccf424c38)

<details>
 
   *<summary>Details</summary>*

   # Crashlytics - Stack trace
# Application: com.weeklyplannerapp.weekplan
# Platform: android
# Version: 7.97 (82)
# Issue: 04b7c6767155e63a5f263a412b42308c
# Session: 6550D89D00B20001766BC4E7519C6E75_DNE_0_v2
# Date: Sun Nov 12 2023 15:52:29 GMT+0200 (Eastern European Standard Time)

# Fatal Exception: java.lang.NullPointerException: Attempt to invoke virtual method 'void android.view.View.setBackground(android.graphics.drawable.Drawable)' on a null object reference
       at com.weeklyplannerapp.weekplan.View.Activities.MainActivity.R(MainActivity.java:35)
       at com.weeklyplannerapp.weekplan.View.Activities.MainActivity.onConfigurationChanged(MainActivity.java:15)
       at android.app.ActivityThread.performActivityConfigurationChanged(ActivityThread.java:6093)
       at android.app.ActivityThread.performConfigurationChangedForActivity(ActivityThread.java:5993)
       at android.app.ActivityThread.handleActivityConfigurationChanged(ActivityThread.java:6383)
       at android.app.servertransaction.ActivityConfigurationChangeItem.execute(ActivityConfigurationChangeItem.java:55)
       at android.app.servertransaction.ActivityTransactionItem.execute(ActivityTransactionItem.java:45)
       at android.app.servertransaction.TransactionExecutor.executeCallbacks(TransactionExecutor.java:135)
       at android.app.servertransaction.TransactionExecutor.execute(TransactionExecutor.java:95)
       at android.app.ActivityThread$H.handleMessage(ActivityThread.java:2291)
       at android.os.Handler.dispatchMessage(Handler.java:106)
       at android.os.Looper.loopOnce(Looper.java:210)
       at android.os.Looper.loop(Looper.java:299)
       at android.app.ActivityThread.main(ActivityThread.java:8319)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:556)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:1038)

# Crashlytics Exception Handler1:
       at dalvik.system.VMStack.getThreadStackTrace(VMStack.java)
       at java.lang.Thread.getStackTrace(Thread.java:1841)
       at java.lang.Thread.getAllStackTraces(Thread.java:1909)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateThreadsList(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateExecutionData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateEventApplicationData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.captureEventData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistEvent(SessionReportingCoordinator.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistFatalEvent(SessionReportingCoordinator.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsBackgroundWorker$3.then(CrashlyticsBackgroundWorker.java:16)
       at com.google.android.gms.tasks.zze.run(:8)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1145)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# DefaultDispatcher-worker-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# ReferenceQueueDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.lang.Daemons$ReferenceQueueDaemon.runInternal(Daemons.java:239)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# GmsDynamite:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at com.google.android.gms.dynamite.zza.run(zza.java:16)

 # 30315-ScoutStateMachine:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:340)
       at android.os.Looper.loopOnce(Looper.java:168)
       at android.os.Looper.loop(Looper.java:299)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# com.google.firebase.crashlytics.startup1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# Measurement Worker:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at m.lk.run(:com.google.android.gms.dynamite_measurementdynamite@234414038@23.44.14 (190400-0):71)

# DefaultDispatcher-worker-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# Firebase Background Thread #0:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# Okio Watchdog:
       at java.lang.Object.wait(Object.java)
       at com.android.okhttp.okio.AsyncTimeout.awaitTimeout(AsyncTimeout.java:325)
       at com.android.okhttp.okio.AsyncTimeout.access$000(AsyncTimeout.java:42)
       at com.android.okhttp.okio.AsyncTimeout$Watchdog.run(AsyncTimeout.java:288)

# OkHttp ConnectionPool:
       at java.lang.Object.wait(Object.java)
       at com.android.okhttp.ConnectionPool$1.run(ConnectionPool.java:106)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1145)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Blocking Thread #1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:401)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:903)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# DefaultDispatcher-worker-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# awaitEvenIfOnMainThread task continuation executor1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# GLThread 124:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at android.opengl.GLSurfaceView$GLThread.guardedRun(GLSurfaceView.java:1497)
       at android.opengl.GLSurfaceView$GLThread.run(GLSurfaceView.java:1272)

# ScionFrontendApi:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.awaitNanos(AbstractQueuedSynchronizer.java:1672)
       at java.util.concurrent.LinkedBlockingQueue.poll(LinkedBlockingQueue.java:460)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Blocking Thread #0:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:401)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:903)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# queued-work-looper:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:340)
       at android.os.Looper.loopOnce(Looper.java:168)
       at android.os.Looper.loop(Looper.java:299)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# FinalizerDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:210)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:231)
       at java.lang.Daemons$FinalizerDaemon.runInternal(Daemons.java:309)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# pool-9-thread-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# FinalizerWatchdogDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.lang.Daemons$FinalizerWatchdogDaemon.sleepUntilNeeded(Daemons.java:428)
       at java.lang.Daemons$FinalizerWatchdogDaemon.runInternal(Daemons.java:408)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)
 
</details>
 </details>

<details>
 
   <summary>Infinix HOT 30</summary> 

![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/77376cad-4fa2-4e3f-8fd2-4de8d8af9a97)


<details>
 
   *<summary>Details</summary>*

   # Crashlytics - Stack trace
# Application: com.weeklyplannerapp.weekplan
# Platform: android
# Version: 7.97 (82)
# Issue: 93e7d779a388e0f520c12d23de37be7f
# Session: 65564BE00189000123277F5C2D2574DA_DNE_0_v2
# Date: Thu Nov 16 2023 19:06:15 GMT+0200 (Eastern European Standard Time)

# Fatal Exception: java.lang.RuntimeException: android.os.TransactionTooLargeException: data parcel size 352080 bytes
       at android.app.ActivityClient.activityStopped(ActivityClient.java:86)
       at android.app.servertransaction.PendingTransactionActions$StopInfo.run(PendingTransactionActions.java:143)
       at android.os.Handler.handleCallback(Handler.java:938)
       at android.os.Handler.dispatchMessage(Handler.java:99)
       at android.os.Looper.loopOnce(Looper.java:201)
       at android.os.Looper.loop(Looper.java:288)
       at android.app.ActivityThread.main(ActivityThread.java:7996)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:553)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:1003)

# Caused by android.os.TransactionTooLargeException: data parcel size 352080 bytes
       at android.os.BinderProxy.transactNative(BinderProxy.java)
       at android.os.BinderProxy.transact(BinderProxy.java:573)
       at android.app.IActivityClientController$Stub$Proxy.activityStopped(IActivityClientController.java:1297)
       at android.app.ActivityClient.activityStopped(ActivityClient.java:83)
       at android.app.servertransaction.PendingTransactionActions$StopInfo.run(PendingTransactionActions.java:143)
       at android.os.Handler.handleCallback(Handler.java:938)
       at android.os.Handler.dispatchMessage(Handler.java:99)
       at android.os.Looper.loopOnce(Looper.java:201)
       at android.os.Looper.loop(Looper.java:288)
       at android.app.ActivityThread.main(ActivityThread.java:7996)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:553)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:1003)

# PlayBillingLibrary-4:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# DefaultDispatcher-worker-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# ReferenceQueueDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.lang.Daemons$ReferenceQueueDaemon.runInternal(Daemons.java:239)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# FinalizerWatchdogDaemon:
       at java.lang.Thread.sleep(Thread.java)
       at java.lang.Thread.sleep(Thread.java:450)
       at java.lang.Thread.sleep(Thread.java:355)
       at java.lang.Daemons$FinalizerWatchdogDaemon.sleepForNanos(Daemons.java:481)
       at java.lang.Daemons$FinalizerWatchdogDaemon.waitForProgress(Daemons.java:544)
       at java.lang.Daemons$FinalizerWatchdogDaemon.runInternal(Daemons.java:412)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# GLThread 80:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at android.opengl.GLSurfaceView$GLThread.guardedRun(GLSurfaceView.java:1497)
       at android.opengl.GLSurfaceView$GLThread.run(GLSurfaceView.java:1272)

# ScionFrontendApi:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.awaitNanos(AbstractQueuedSynchronizer.java:1672)
       at java.util.concurrent.LinkedBlockingQueue.poll(LinkedBlockingQueue.java:460)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# RealmFinalizingDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:210)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:231)
       at io.realm.internal.FinalizerRunnable.run(FinalizerRunnable.java:3)
       at java.lang.Thread.run(Thread.java:1012)

# Crashlytics Exception Handler1:
       at dalvik.system.VMStack.getThreadStackTrace(VMStack.java)
       at java.lang.Thread.getStackTrace(Thread.java:1841)
       at java.lang.Thread.getAllStackTraces(Thread.java:1909)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateThreadsList(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateExecutionData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateEventApplicationData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.captureEventData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistEvent(SessionReportingCoordinator.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistFatalEvent(SessionReportingCoordinator.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsBackgroundWorker$3.then(CrashlyticsBackgroundWorker.java:16)
       at com.google.android.gms.tasks.zze.run(:8)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1145)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# AsyncTask #3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:401)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:903)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# FinalizerDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:210)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:231)
       at java.lang.Daemons$FinalizerDaemon.runInternal(Daemons.java:309)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# AppLiceJDWP:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:335)
       at android.os.Looper.loopOnce(Looper.java:161)
       at android.os.Looper.loop(Looper.java:288)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# DefaultDispatcher-worker-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# Firebase Background Thread #0:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# com.google.firebase.crashlytics.startup1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# Measurement Worker:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at m.lk.run(:com.google.android.gms.dynamite_measurementdynamite@234414038@23.44.14 (190400-0):71)

# DefaultDispatcher-worker-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# GmsDynamite:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at com.google.android.gms.dynamite.zza.run(zza.java:16)

# PlayBillingLibrary-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Blocking Thread #0:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:401)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:903)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:1012)

# awaitEvenIfOnMainThread task continuation executor1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# queued-work-looper:
       at java.io.FileDescriptor.sync(FileDescriptor.java)
       at android.os.FileUtils.sync(FileUtils.java:256)
       at android.app.SharedPreferencesImpl.writeToFile(SharedPreferencesImpl.java:807)
       at android.app.SharedPreferencesImpl.access$900(SharedPreferencesImpl.java:59)
       at android.app.SharedPreferencesImpl$2.run(SharedPreferencesImpl.java:672)
       at android.app.QueuedWork.processPendingWork(QueuedWork.java:265)
       at android.app.QueuedWork.access$000(QueuedWork.java:51)
       at android.app.QueuedWork$QueuedWorkHandler.handleMessage(QueuedWork.java:285)
       at android.os.Handler.dispatchMessage(Handler.java:106)
       at android.os.Looper.loopOnce(Looper.java:201)
       at android.os.Looper.loop(Looper.java:288)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# AsyncTask #2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:401)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:903)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# pool-11-thread-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)
 </details>
 </details>
  </details>

  
 <details>
 
  <summary>Android 11</summary><br>

  <details>
 
<summary>Crash list</summary>

![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/43481b86-7da3-4929-aa02-9636b79243a9)


  </details>
 
<details>  



   
   <summary>Mi A3</summary>
    
![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/25213ba1-d807-4971-a805-281006e87280)



<details>
 
   *<summary>Details</summary>*

 # Crashlytics - Stack trace
# Application: com.weeklyplannerapp.weekplan
# Platform: android
# Version: 7.97 (82)
# Issue: 72bd018209352c1b39c33f10f34b265c
# Session: 65534F2F017600011C4C729F40AC055B_DNE_0_v2
# Date: Tue Nov 14 2023 12:43:12 GMT+0200 (Eastern European Standard Time)

# Fatal Exception: java.lang.RuntimeException: Unable to stop activity {com.weeklyplannerapp.weekplan/com.weeklyplannerapp.weekplan.View.Activities.MainActivity}: io.realm.exceptions.RealmFileException: Failed to open file at path '/data/data/com.weeklyplannerapp.weekplan/14.11.2023 15:43': parent directory does not exist (/data/data/com.weeklyplannerapp.weekplan/14.11.2023 15:43) in /tmp/realm-java/realm/realm-library/src/main/cpp/io_realm_internal_OsSharedRealm.cpp line 404 Kind: NOT_FOUND.
       at android.app.ActivityThread.callActivityOnStop(ActivityThread.java:4851)
       at android.app.ActivityThread.performStopActivityInner(ActivityThread.java:4822)
       at android.app.ActivityThread.handleStopActivity(ActivityThread.java:4896)
       at android.app.servertransaction.StopActivityItem.execute(StopActivityItem.java:40)
       at android.app.servertransaction.TransactionExecutor.executeLifecycleState(TransactionExecutor.java:176)
       at android.app.servertransaction.TransactionExecutor.execute(TransactionExecutor.java:97)
       at android.app.ActivityThread$H.handleMessage(ActivityThread.java:2067)
       at android.os.Handler.dispatchMessage(Handler.java:106)
       at android.os.Looper.loop(Looper.java:223)
       at android.app.ActivityThread.main(ActivityThread.java:7698)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:592)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:952)

# Caused by io.realm.exceptions.RealmFileException: Failed to open file at path '/data/data/com.weeklyplannerapp.weekplan/14.11.2023 15:43': parent directory does not exist (/data/data/com.weeklyplannerapp.weekplan/14.11.2023 15:43) in /tmp/realm-java/realm/realm-library/src/main/cpp/io_realm_internal_OsSharedRealm.cpp line 404
       at io.realm.internal.OsSharedRealm.nativeWriteCopy(OsSharedRealm.java)
       at io.realm.internal.OsSharedRealm.writeCopy(OsSharedRealm.java:38)
       at io.realm.BaseRealm.writeCopyTo(BaseRealm.java:1)
       at com.weeklyplannerapp.weekplan.WeeklyPlanApplication$1.onActivityStopped(WeeklyPlanApplication.java:199)
       at android.app.Application.dispatchActivityStopped(Application.java:496)
       at android.app.Activity.dispatchActivityStopped(Activity.java:1445)
       at android.app.Activity.onStop(Activity.java:2591)
       at androidx.fragment.app.FragmentActivity.onStop(FragmentActivity.java:1)
       at androidx.appcompat.app.AppCompatActivity.onStop(AppCompatActivity.java:1)
       at com.weeklyplannerapp.weekplan.View.Activities.MainActivity.onStop(MainActivity.java)
       at android.app.Instrumentation.callActivityOnStop(Instrumentation.java:1477)
       at android.app.Activity.performStop(Activity.java:8215)
       at android.app.ActivityThread.callActivityOnStop(ActivityThread.java:4843)
       at android.app.ActivityThread.performStopActivityInner(ActivityThread.java:4822)
       at android.app.ActivityThread.handleStopActivity(ActivityThread.java:4896)
       at android.app.servertransaction.StopActivityItem.execute(StopActivityItem.java:40)
       at android.app.servertransaction.TransactionExecutor.executeLifecycleState(TransactionExecutor.java:176)
       at android.app.servertransaction.TransactionExecutor.execute(TransactionExecutor.java:97)
       at android.app.ActivityThread$H.handleMessage(ActivityThread.java:2067)
       at android.os.Handler.dispatchMessage(Handler.java:106)
       at android.os.Looper.loop(Looper.java:223)
       at android.app.ActivityThread.main(ActivityThread.java:7698)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:592)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:952)

# Firebase Background Thread #1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:923)

# DefaultDispatcher-worker-1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:353)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# com.google.firebase.crashlytics.startup1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:923)

# DefaultDispatcher-worker-3:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:353)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# Crashlytics Exception Handler1:
       at dalvik.system.VMStack.getThreadStackTrace(VMStack.java)
       at java.lang.Thread.getStackTrace(Thread.java:1736)
       at java.lang.Thread.getAllStackTraces(Thread.java:1812)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateThreadsList(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateExecutionData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateEventApplicationData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.captureEventData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistEvent(SessionReportingCoordinator.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistFatalEvent(SessionReportingCoordinator.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsBackgroundWorker$3.then(CrashlyticsBackgroundWorker.java:16)
       at com.google.android.gms.tasks.zze.run(:8)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1167)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:923)

# FinalizerDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:190)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:211)
       at java.lang.Daemons$FinalizerDaemon.runInternal(Daemons.java:273)
       at java.lang.Daemons$Daemon.run(Daemons.java:139)
       at java.lang.Thread.run(Thread.java:923)

# Measurement Worker:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at m.lk.run(:com.google.android.gms.dynamite_measurementdynamite@234414031@23.44.14 (150400-0):71)

# PlayBillingLibrary-2:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:923)

# Firebase Blocking Thread #0:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:230)
       at java.util.concurrent.SynchronousQueue$TransferStack.awaitFulfill(SynchronousQueue.java:461)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:362)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:937)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1091)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:923)

# PlayBillingLibrary-1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:923)

# RealmFinalizingDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:190)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:211)
       at io.realm.internal.FinalizerRunnable.run(FinalizerRunnable.java:3)
       at java.lang.Thread.run(Thread.java:923)

# PlayBillingLibrary-4:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:923)

# GmsDynamite:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at com.google.android.gms.dynamite.zza.run(zza.java:16)

# awaitEvenIfOnMainThread task continuation executor1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:923)

# Firebase Background Thread #3:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:923)

# FinalizerWatchdogDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at java.lang.Daemons$FinalizerWatchdogDaemon.sleepUntilNeeded(Daemons.java:341)
       at java.lang.Daemons$FinalizerWatchdogDaemon.runInternal(Daemons.java:321)
       at java.lang.Daemons$Daemon.run(Daemons.java:139)
       at java.lang.Thread.run(Thread.java:923)

# Firebase Background Thread #2:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:923)

# queued-work-looper:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:335)
       at android.os.Looper.loop(Looper.java:183)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# PlayBillingLibrary-3:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:923)

# ScionFrontendApi:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:230)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.awaitNanos(AbstractQueuedSynchronizer.java:2109)
       at java.util.concurrent.LinkedBlockingQueue.poll(LinkedBlockingQueue.java:467)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1091)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:923)

# Firebase Background Thread #0:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:923)

# GLThread 64344:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at android.opengl.GLSurfaceView$GLThread.guardedRun(GLSurfaceView.java:1497)
       at android.opengl.GLSurfaceView$GLThread.run(GLSurfaceView.java:1272)

# DefaultDispatcher-worker-2:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:353)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# AsyncTask #2:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.SynchronousQueue$TransferStack.awaitFulfill(SynchronousQueue.java:459)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:362)
       at java.util.concurrent.SynchronousQueue.take(SynchronousQueue.java:920)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:923)

# ReferenceQueueDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at java.lang.Daemons$ReferenceQueueDaemon.runInternal(Daemons.java:217)
       at java.lang.Daemons$Daemon.run(Daemons.java:139)
       at java.lang.Thread.run(Thread.java:923)

# pool-10-thread-1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:923)
 
</details>
 </details>

<details>   

   <summary>Redmi 9A</summary> 

![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/d091239f-e136-45e8-9451-e9c5ad173646)


<details>
 
   *<summary>Details</summary>*

   # Crashlytics - Stack trace
# Application: com.weeklyplannerapp.weekplan
# Platform: android
# Version: 7.97 (82)
# Issue: 72bd018209352c1b39c33f10f34b265c
# Session: 65524D6701DA00016312977267885598_DNE_0_v2
# Date: Mon Nov 13 2023 18:23:05 GMT+0200 (Eastern European Standard Time)

# Fatal Exception: java.lang.RuntimeException: Unable to stop activity {com.weeklyplannerapp.weekplan/com.weeklyplannerapp.weekplan.View.Activities.MainActivity}: io.realm.exceptions.RealmFileException: Failed to open file at path '/data/data/com.weeklyplannerapp.weekplan/13.11.2023 21:23': parent directory does not exist (/data/data/com.weeklyplannerapp.weekplan/13.11.2023 21:23) in /tmp/realm-java/realm/realm-library/src/main/cpp/io_realm_internal_OsSharedRealm.cpp line 404 Kind: NOT_FOUND.
       at android.app.ActivityThread.callActivityOnStop(ActivityThread.java:4998)
       at android.app.ActivityThread.performStopActivityInner(ActivityThread.java:4969)
       at android.app.ActivityThread.handleStopActivity(ActivityThread.java:5043)
       at android.app.servertransaction.StopActivityItem.execute(StopActivityItem.java:40)
       at android.app.servertransaction.TransactionExecutor.executeLifecycleState(TransactionExecutor.java:176)
       at android.app.servertransaction.TransactionExecutor.execute(TransactionExecutor.java:97)
       at android.app.ActivityThread$H.handleMessage(ActivityThread.java:2161)
       at android.os.Handler.dispatchMessage(Handler.java:106)
       at android.os.Looper.loop(Looper.java:236)
       at android.app.ActivityThread.main(ActivityThread.java:7912)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:620)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:1011)

# Caused by io.realm.exceptions.RealmFileException: Failed to open file at path '/data/data/com.weeklyplannerapp.weekplan/13.11.2023 21:23': parent directory does not exist (/data/data/com.weeklyplannerapp.weekplan/13.11.2023 21:23) in /tmp/realm-java/realm/realm-library/src/main/cpp/io_realm_internal_OsSharedRealm.cpp line 404
       at io.realm.internal.OsSharedRealm.nativeWriteCopy(OsSharedRealm.java)
       at io.realm.internal.OsSharedRealm.writeCopy(OsSharedRealm.java:38)
       at io.realm.BaseRealm.writeCopyTo(BaseRealm.java:1)
       at com.weeklyplannerapp.weekplan.WeeklyPlanApplication$1.onActivityStopped(WeeklyPlanApplication.java:199)
       at android.app.Application.dispatchActivityStopped(Application.java:498)
       at android.app.Activity.dispatchActivityStopped(Activity.java:1495)
       at android.app.Activity.onStop(Activity.java:2666)
       at androidx.fragment.app.FragmentActivity.onStop(FragmentActivity.java:1)
       at androidx.appcompat.app.AppCompatActivity.onStop(AppCompatActivity.java:1)
       at com.weeklyplannerapp.weekplan.View.Activities.MainActivity.onStop(MainActivity.java)
       at android.app.Instrumentation.callActivityOnStop(Instrumentation.java:1475)
       at android.app.Activity.performStop(Activity.java:8358)
       at android.app.ActivityThread.callActivityOnStop(ActivityThread.java:4990)
       at android.app.ActivityThread.performStopActivityInner(ActivityThread.java:4969)
       at android.app.ActivityThread.handleStopActivity(ActivityThread.java:5043)
       at android.app.servertransaction.StopActivityItem.execute(StopActivityItem.java:40)
       at android.app.servertransaction.TransactionExecutor.executeLifecycleState(TransactionExecutor.java:176)
       at android.app.servertransaction.TransactionExecutor.execute(TransactionExecutor.java:97)
       at android.app.ActivityThread$H.handleMessage(ActivityThread.java:2161)
       at android.os.Handler.dispatchMessage(Handler.java:106)
       at android.os.Looper.loop(Looper.java:236)
       at android.app.ActivityThread.main(ActivityThread.java:7912)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:620)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:1011)

# Firebase Blocking Thread #0:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:230)
       at java.util.concurrent.SynchronousQueue$TransferStack.awaitFulfill(SynchronousQueue.java:461)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:362)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:937)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1091)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:923)

# Timer-0:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.util.TimerThread.mainLoop(Timer.java:559)
       at java.util.TimerThread.run(Timer.java:512)

# AsyncTask #1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:230)
       at java.util.concurrent.SynchronousQueue$TransferStack.awaitFulfill(SynchronousQueue.java:461)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:362)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:937)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1091)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:923)

# GmsDynamite:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at com.google.android.gms.dynamite.zza.run(zza.java:16)

# ScionFrontendApi:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:230)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.awaitNanos(AbstractQueuedSynchronizer.java:2109)
       at java.util.concurrent.LinkedBlockingQueue.poll(LinkedBlockingQueue.java:467)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1091)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:923)

# ReferenceQueueDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at java.lang.Daemons$ReferenceQueueDaemon.runInternal(Daemons.java:218)
       at java.lang.Daemons$Daemon.run(Daemons.java:140)
       at java.lang.Thread.run(Thread.java:923)

# pool-9-thread-1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:923)

# AsyncTask #2:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:230)
       at java.util.concurrent.SynchronousQueue$TransferStack.awaitFulfill(SynchronousQueue.java:461)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:362)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:937)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1091)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:923)

# Firebase Background Thread #2:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:923)

# DefaultDispatcher-worker-1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:353)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# Firebase Background Thread #3:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:923)

# GLThread 105715:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at android.opengl.GLSurfaceView$GLThread.guardedRun(GLSurfaceView.java:1505)
       at android.opengl.GLSurfaceView$GLThread.run(GLSurfaceView.java:1280)

# FinalizerDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:190)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:211)
       at java.lang.Daemons$FinalizerDaemon.runInternal(Daemons.java:274)
       at java.lang.Daemons$Daemon.run(Daemons.java:140)
       at java.lang.Thread.run(Thread.java:923)

# AsyncTask #3:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:230)
       at java.util.concurrent.SynchronousQueue$TransferStack.awaitFulfill(SynchronousQueue.java:461)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:362)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:937)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1091)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:923)

# DefaultDispatcher-worker-3:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:353)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# Measurement Worker:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at m.jd.run(:com.google.android.gms.dynamite_measurementdynamite@233717033@23.37.17 (150300-0):71)

# RealmFinalizingDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:190)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:211)
       at io.realm.internal.FinalizerRunnable.run(FinalizerRunnable.java:3)
       at java.lang.Thread.run(Thread.java:923)

# Firebase Background Thread #1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:923)

# DefaultDispatcher-worker-2:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:353)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# Firebase Background Thread #0:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:923)

# FinalizerWatchdogDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at java.lang.Daemons$FinalizerWatchdogDaemon.sleepUntilNeeded(Daemons.java:342)
       at java.lang.Daemons$FinalizerWatchdogDaemon.runInternal(Daemons.java:322)
       at java.lang.Daemons$Daemon.run(Daemons.java:140)
       at java.lang.Thread.run(Thread.java:923)

# com.google.firebase.crashlytics.startup1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:923)

# queued-work-looper:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:335)
       at android.os.Looper.loop(Looper.java:193)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# Crashlytics Exception Handler1:
       at dalvik.system.VMStack.getThreadStackTrace(VMStack.java)
       at java.lang.Thread.getStackTrace(Thread.java:1736)
       at java.lang.Thread.getAllStackTraces(Thread.java:1812)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateThreadsList(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateExecutionData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateEventApplicationData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.captureEventData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistEvent(SessionReportingCoordinator.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistFatalEvent(SessionReportingCoordinator.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsBackgroundWorker$3.then(CrashlyticsBackgroundWorker.java:16)
       at com.google.android.gms.tasks.zze.run(:8)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1167)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:923)

# awaitEvenIfOnMainThread task continuation executor1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:923)
 
  </details>
   </details>
    </details>

<details>
 
  <summary>Android 10</summary><br>

  <details>
 
<summary>Crash list</summary>

![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/b9460b9b-5fe7-4622-b18e-b89abb40219b)

  </details>
  
 
<details>  

   <summary>P20</summary>
    
![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/5e805642-b2f7-4681-b95e-65f17b63ea48)



<details>
 
   *<summary>Details</summary>*

 # Crashlytics - Stack trace
# Application: com.weeklyplannerapp.weekplan
# Platform: android
# Version: 7.97 (82)
# Issue: 72bd018209352c1b39c33f10f34b265c
# Session: 65514EB001FF0001203973FCDA9A41E9_DNE_0_v2
# Date: Mon Nov 13 2023 00:17:12 GMT+0200 (Eastern European Standard Time)

# Fatal Exception: java.lang.RuntimeException: Unable to stop activity {com.weeklyplannerapp.weekplan/com.weeklyplannerapp.weekplan.Compact.View.Activities.CompactMainActivity}: io.realm.exceptions.RealmFileException: Failed to open file at path '/data/data/com.weeklyplannerapp.weekplan/13.11.2023 01:17': parent directory does not exist (/data/data/com.weeklyplannerapp.weekplan/13.11.2023 01:17) in /tmp/realm-java/realm/realm-library/src/main/cpp/io_realm_internal_OsSharedRealm.cpp line 404 Kind: NOT_FOUND.
       at android.app.ActivityThread.callActivityOnStop(ActivityThread.java:5546)
       at android.app.ActivityThread.performStopActivityInner(ActivityThread.java:5516)
       at android.app.ActivityThread.handleStopActivity(ActivityThread.java:5591)
       at android.app.servertransaction.TransactionExecutor.performLifecycleSequence(TransactionExecutor.java:247)
       at android.app.servertransaction.TransactionExecutor.cycleToPath(TransactionExecutor.java:215)
       at android.app.servertransaction.TransactionExecutor.executeLifecycleState(TransactionExecutor.java:187)
       at android.app.servertransaction.TransactionExecutor.execute(TransactionExecutor.java:105)
       at android.app.ActivityThread$H.handleMessage(ActivityThread.java:2613)
       at android.os.Handler.dispatchMessage(Handler.java:110)
       at android.os.Looper.loop(Looper.java:219)
       at android.app.ActivityThread.main(ActivityThread.java:8668)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:513)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:1109)

# Caused by io.realm.exceptions.RealmFileException: Failed to open file at path '/data/data/com.weeklyplannerapp.weekplan/13.11.2023 01:17': parent directory does not exist (/data/data/com.weeklyplannerapp.weekplan/13.11.2023 01:17) in /tmp/realm-java/realm/realm-library/src/main/cpp/io_realm_internal_OsSharedRealm.cpp line 404
       at io.realm.internal.OsSharedRealm.nativeWriteCopy(OsSharedRealm.java)
       at io.realm.internal.OsSharedRealm.writeCopy(OsSharedRealm.java:38)
       at io.realm.BaseRealm.writeCopyTo(BaseRealm.java:1)
       at com.weeklyplannerapp.weekplan.WeeklyPlanApplication$1.onActivityStopped(WeeklyPlanApplication.java:199)
       at android.app.Application.dispatchActivityStopped(Application.java:503)
       at android.app.Activity.dispatchActivityStopped(Activity.java:1390)
       at android.app.Activity.onStop(Activity.java:2578)
       at androidx.fragment.app.FragmentActivity.onStop(FragmentActivity.java:1)
       at androidx.appcompat.app.AppCompatActivity.onStop(AppCompatActivity.java:1)
       at com.weeklyplannerapp.weekplan.Compact.View.Activities.CompactMainActivity.onStop(CompactMainActivity.java)
       at android.app.Instrumentation.callActivityOnStop(Instrumentation.java:1494)
       at android.app.Activity.performStop(Activity.java:8447)
       at android.app.ActivityThread.callActivityOnStop(ActivityThread.java:5538)
       at android.app.ActivityThread.performStopActivityInner(ActivityThread.java:5516)
       at android.app.ActivityThread.handleStopActivity(ActivityThread.java:5591)
       at android.app.servertransaction.TransactionExecutor.performLifecycleSequence(TransactionExecutor.java:247)
       at android.app.servertransaction.TransactionExecutor.cycleToPath(TransactionExecutor.java:215)
       at android.app.servertransaction.TransactionExecutor.executeLifecycleState(TransactionExecutor.java:187)
       at android.app.servertransaction.TransactionExecutor.execute(TransactionExecutor.java:105)
       at android.app.ActivityThread$H.handleMessage(ActivityThread.java:2613)
       at android.os.Handler.dispatchMessage(Handler.java:110)
       at android.os.Looper.loop(Looper.java:219)
       at android.app.ActivityThread.main(ActivityThread.java:8668)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:513)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:1109)

# magnifier pixel copy result handler:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:363)
       at android.os.Looper.loop(Looper.java:176)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# Firebase Blocking Thread #0:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:230)
       at java.util.concurrent.SynchronousQueue$TransferStack.awaitFulfill(SynchronousQueue.java:461)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:362)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:937)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1091)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:929)

# DefaultDispatcher-worker-3:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:353)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# OkHttp ConnectionPool:
       at java.lang.Object.wait(Object.java)
       at com.android.okhttp.ConnectionPool$1.run(ConnectionPool.java:106)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1167)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:929)

# AppEyeUiProbeThread:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:363)
       at android.os.Looper.loop(Looper.java:176)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# PlayBillingLibrary-1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:929)

# PlayBillingLibrary-3:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:929)

# Firebase Background Thread #1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:929)

# DefaultDispatcher-worker-2:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:353)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# RealmFinalizingDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:190)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:211)
       at io.realm.internal.FinalizerRunnable.run(FinalizerRunnable.java:3)
       at java.lang.Thread.run(Thread.java:929)

# ReferenceQueueDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at java.lang.Daemons$ReferenceQueueDaemon.runInternal(Daemons.java:215)
       at java.lang.Daemons$Daemon.run(Daemons.java:137)
       at java.lang.Thread.run(Thread.java:929)

# Crashlytics Exception Handler1:
       at dalvik.system.VMStack.getThreadStackTrace(VMStack.java)
       at java.lang.Thread.getStackTrace(Thread.java:1730)
       at java.lang.Thread.getAllStackTraces(Thread.java:1806)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateThreadsList(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateExecutionData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateEventApplicationData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.captureEventData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistEvent(SessionReportingCoordinator.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistFatalEvent(SessionReportingCoordinator.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsBackgroundWorker$3.then(CrashlyticsBackgroundWorker.java:16)
       at com.google.android.gms.tasks.zze.run(:8)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1167)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:929)

# awaitEvenIfOnMainThread task continuation executor1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:929)

# DefaultDispatcher-worker-1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:353)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# Firebase Background Thread #3:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:929)

# AsyncTask #1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.SynchronousQueue$TransferStack.awaitFulfill(SynchronousQueue.java:459)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:362)
       at java.util.concurrent.SynchronousQueue.take(SynchronousQueue.java:920)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:929)

# queued-work-looper:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:363)
       at android.os.Looper.loop(Looper.java:176)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# pool-8-thread-1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:929)

# FinalizerWatchdogDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at java.lang.Daemons$FinalizerWatchdogDaemon.sleepUntilNeeded(Daemons.java:339)
       at java.lang.Daemons$FinalizerWatchdogDaemon.runInternal(Daemons.java:319)
       at java.lang.Daemons$Daemon.run(Daemons.java:137)
       at java.lang.Thread.run(Thread.java:929)

# PlayBillingLibrary-2:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:929)

# ScionFrontendApi:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:230)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.awaitNanos(AbstractQueuedSynchronizer.java:2109)
       at java.util.concurrent.LinkedBlockingQueue.poll(LinkedBlockingQueue.java:467)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1091)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:929)

# GmsDynamite:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at com.google.android.gms.dynamite.zza.run(zza.java:16)

# Firebase Background Thread #0:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:929)

# FinalizerDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:190)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:211)
       at java.lang.Daemons$FinalizerDaemon.runInternal(Daemons.java:271)
       at java.lang.Daemons$Daemon.run(Daemons.java:137)
       at java.lang.Thread.run(Thread.java:929)

# PlayBillingLibrary-4:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:929)

# Measurement Worker:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at m.ll.run(:com.google.android.gms.dynamite_measurementdynamite@234414022@23.44.14 (100400-0):71)

# Firebase Background Thread #2:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:929)

# Okio Watchdog:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at com.android.okhttp.okio.AsyncTimeout.awaitTimeout(AsyncTimeout.java:313)
       at com.android.okhttp.okio.AsyncTimeout.access$000(AsyncTimeout.java:42)
       at com.android.okhttp.okio.AsyncTimeout$Watchdog.run(AsyncTimeout.java:288)

# com.google.firebase.crashlytics.startup1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:929)
 
</details>

![Screenshot 2023-11-18 234009](https://github.com/UserQA07/Week-Planner-/assets/144763744/11ce96a2-00e2-4a82-98fb-dd6a43ecd8a5)


<details>
 
   *<summary>Details</summary>*

 # Crashlytics - Stack trace
# Application: com.weeklyplannerapp.weekplan
# Platform: android
# Version: 7.97 (82)
# Issue: 7494e5bb2d3fb35cf07ef562a6952da2
# Session: 65549BEE00090001224EA8A4242A790B_DNE_0_v2
# Date: Wed Nov 15 2023 12:22:38 GMT+0200 (Eastern European Standard Time)

# Fatal Exception: java.lang.RuntimeException: Unable to start activity ComponentInfo{com.weeklyplannerapp.weekplan/com.weeklyplannerapp.weekplan.View.Activities.MainActivity}: io.realm.exceptions.RealmMigrationNeededException: Migration is required due to the following errors:
- Property 'Note.day' has been made indexed.
- Property 'Note.month' has been made indexed.
- Property 'Note.year' has been made indexed.
       at android.app.ActivityThread.performLaunchActivity(ActivityThread.java:4060)
       at android.app.ActivityThread.handleLaunchActivity(ActivityThread.java:4247)
       at android.app.servertransaction.LaunchActivityItem.execute(LaunchActivityItem.java:91)
       at android.app.servertransaction.TransactionExecutor.executeCallbacks(TransactionExecutor.java:149)
       at android.app.servertransaction.TransactionExecutor.execute(TransactionExecutor.java:103)
       at android.app.ActivityThread$H.handleMessage(ActivityThread.java:2613)
       at android.os.Handler.dispatchMessage(Handler.java:110)
       at android.os.Looper.loop(Looper.java:219)
       at android.app.ActivityThread.main(ActivityThread.java:8668)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:513)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:1109)

# Caused by io.realm.exceptions.RealmMigrationNeededException: Migration is required due to the following errors:
- Property 'Note.day' has been made indexed.
- Property 'Note.month' has been made indexed.
- Property 'Note.year' has been made indexed.
       at io.realm.internal.OsSharedRealm.nativeGetSharedRealm(OsSharedRealm.java)
       at io.realm.internal.OsSharedRealm.<init>(OsSharedRealm.java:9)
       at io.realm.internal.OsSharedRealm.getInstance(OsSharedRealm.java:3)
       at io.realm.BaseRealm.<init>(BaseRealm.java:10)
       at io.realm.BaseRealm.<init>(BaseRealm.java:10)
       at io.realm.Realm.<init>(Realm.java:4)
       at io.realm.Realm.createInstance(Realm.java:115)
       at io.realm.RealmCache.createInstance(RealmCache.java:115)
       at io.realm.RealmCache.doCreateRealmOrGetFromCache(RealmCache.java:115)
       at io.realm.RealmCache.createRealmOrGetFromCache(RealmCache.java:115)
       at io.realm.Realm.getInstance(Realm.java:115)
       at com.weeklyplannerapp.weekplan.Service.Dagger.Modules.DatabaseModule.provideRealm(DatabaseModule.java:53)
       at com.weeklyplannerapp.weekplan.Service.Dagger.Modules.DatabaseModule_ProvideRealmFactory.provideRealm(DatabaseModule_ProvideRealmFactory.java:53)
       at com.weeklyplannerapp.weekplan.Service.Dagger.Modules.DatabaseModule_ProvideRealmFactory.get(DatabaseModule_ProvideRealmFactory.java:53)
       at com.weeklyplannerapp.weekplan.Service.Dagger.Modules.DatabaseModule_ProvideRealmFactory.get(DatabaseModule_ProvideRealmFactory.java:53)
       at dagger.internal.DoubleCheck.get(DoubleCheck.java:14)
       at com.weeklyplannerapp.weekplan.Service.Dagger.Modules.DatabaseModule_ProvideDatabaseFactory.get(DatabaseModule_ProvideDatabaseFactory.java:11)
       at com.weeklyplannerapp.weekplan.Service.Dagger.Modules.DatabaseModule_ProvideDatabaseFactory.get(DatabaseModule_ProvideDatabaseFactory.java:11)
       at dagger.internal.DoubleCheck.get(DoubleCheck.java:14)
       at com.weeklyplannerapp.weekplan.Service.Dagger.DaggerIDaggerComponent$IDaggerComponentImpl.injectMainActivity(DaggerIDaggerComponent.java:328)
       at com.weeklyplannerapp.weekplan.Service.Dagger.DaggerIDaggerComponent$IDaggerComponentImpl.inject(DaggerIDaggerComponent.java:328)
       at com.weeklyplannerapp.weekplan.View.Activities.MainActivity.initializeData(MainActivity.java:328)
       at com.weeklyplannerapp.weekplan.View.Activities.MainActivity.initializeAll(MainActivity.java:328)
       at com.weeklyplannerapp.weekplan.View.Activities.MainActivity.onCreate(MainActivity.java:328)
       at android.app.Activity.performCreate(Activity.java:8214)
       at android.app.Activity.performCreate(Activity.java:8202)
       at android.app.Instrumentation.callActivityOnCreate(Instrumentation.java:1320)
       at android.app.ActivityThread.performLaunchActivity(ActivityThread.java:4033)
       at android.app.ActivityThread.handleLaunchActivity(ActivityThread.java:4247)
       at android.app.servertransaction.LaunchActivityItem.execute(LaunchActivityItem.java:91)
       at android.app.servertransaction.TransactionExecutor.executeCallbacks(TransactionExecutor.java:149)
       at android.app.servertransaction.TransactionExecutor.execute(TransactionExecutor.java:103)
       at android.app.ActivityThread$H.handleMessage(ActivityThread.java:2613)
       at android.os.Handler.dispatchMessage(Handler.java:110)
       at android.os.Looper.loop(Looper.java:219)
       at android.app.ActivityThread.main(ActivityThread.java:8668)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:513)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:1109)

# Firebase Background Thread #2:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:929)

# OkHttp ConnectionPool:
       at java.lang.Object.wait(Object.java)
       at com.android.okhttp.ConnectionPool$1.run(ConnectionPool.java:106)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1167)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:929)

# AsyncTask #1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.SynchronousQueue$TransferStack.awaitFulfill(SynchronousQueue.java:459)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:362)
       at java.util.concurrent.SynchronousQueue.take(SynchronousQueue.java:920)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:929)

# Measurement Worker:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at m.ll.run(:com.google.android.gms.dynamite_measurementdynamite@234414022@23.44.14 (100400-0):71)

# Firebase Background Thread #1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:929)

# Crashlytics Exception Handler1:
       at dalvik.system.VMStack.getThreadStackTrace(VMStack.java)
       at java.lang.Thread.getStackTrace(Thread.java:1730)
       at java.lang.Thread.getAllStackTraces(Thread.java:1806)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateThreadsList(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateExecutionData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateEventApplicationData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.captureEventData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistEvent(SessionReportingCoordinator.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistFatalEvent(SessionReportingCoordinator.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsBackgroundWorker$3.then(CrashlyticsBackgroundWorker.java:16)
       at com.google.android.gms.tasks.zze.run(:8)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1167)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:929)

# Firebase Background Thread #3:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:929)

# ScionFrontendApi:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:230)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.awaitNanos(AbstractQueuedSynchronizer.java:2109)
       at java.util.concurrent.LinkedBlockingQueue.poll(LinkedBlockingQueue.java:467)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1091)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:929)

# com.google.firebase.crashlytics.startup1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:929)

# Firebase Background Thread #0:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:929)

# DefaultDispatcher-worker-1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:353)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# GLThread 85379:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at android.opengl.GLSurfaceView$GLThread.guardedRun(GLSurfaceView.java:1516)
       at android.opengl.GLSurfaceView$GLThread.run(GLSurfaceView.java:1281)

# AppEyeUiProbeThread:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:363)
       at android.os.Looper.loop(Looper.java:176)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# DefaultDispatcher-worker-2:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:353)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# awaitEvenIfOnMainThread task continuation executor1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:929)

# ReferenceQueueDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at java.lang.Daemons$ReferenceQueueDaemon.runInternal(Daemons.java:215)
       at java.lang.Daemons$Daemon.run(Daemons.java:137)
       at java.lang.Thread.run(Thread.java:929)

# queued-work-looper:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:363)
       at android.os.Looper.loop(Looper.java:176)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# queued-work-looper-schedule-handler:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:363)
       at android.os.Looper.loop(Looper.java:176)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# RealmFinalizingDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:190)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:211)
       at io.realm.internal.FinalizerRunnable.run(FinalizerRunnable.java:3)
       at java.lang.Thread.run(Thread.java:929)

 # FinalizerDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:190)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:211)
       at java.lang.Daemons$FinalizerDaemon.runInternal(Daemons.java:271)
       at java.lang.Daemons$Daemon.run(Daemons.java:137)
       at java.lang.Thread.run(Thread.java:929)

 # FinalizerWatchdogDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at java.lang.Daemons$FinalizerWatchdogDaemon.sleepUntilNeeded(Daemons.java:339)
       at java.lang.Daemons$FinalizerWatchdogDaemon.runInternal(Daemons.java:319)
       at java.lang.Daemons$Daemon.run(Daemons.java:137)
       at java.lang.Thread.run(Thread.java:929)

# Firebase Blocking Thread #0:
       at com.android.org.conscrypt.NativeCrypto.SSL_read(NativeCrypto.java)
       at com.android.org.conscrypt.NativeSsl.read(NativeSsl.java:411)
       at com.android.org.conscrypt.ConscryptFileDescriptorSocket$SSLInputStream.read(ConscryptFileDescriptorSocket.java:549)
       at com.android.okhttp.okio.Okio$2.read(Okio.java:138)
       at com.android.okhttp.okio.AsyncTimeout$2.read(AsyncTimeout.java:213)
       at com.android.okhttp.okio.RealBufferedSource.indexOf(RealBufferedSource.java:307)
       at com.android.okhttp.okio.RealBufferedSource.indexOf(RealBufferedSource.java:301)
       at com.android.okhttp.okio.RealBufferedSource.readUtf8LineStrict(RealBufferedSource.java:197)
       at com.android.okhttp.internal.http.Http1xStream.readResponse(Http1xStream.java:188)
       at com.android.okhttp.internal.http.Http1xStream.readResponseHeaders(Http1xStream.java:129)
       at com.android.okhttp.internal.http.HttpEngine.readNetworkResponse(HttpEngine.java:750)
       at com.android.okhttp.internal.http.HttpEngine.readResponse(HttpEngine.java:622)
       at com.android.okhttp.internal.huc.HttpURLConnectionImpl.execute(HttpURLConnectionImpl.java:475)
       at com.android.okhttp.internal.huc.HttpURLConnectionImpl.getResponse(HttpURLConnectionImpl.java:411)
       at com.android.okhttp.internal.huc.HttpURLConnectionImpl.getResponseCode(HttpURLConnectionImpl.java:542)
       at com.android.okhttp.internal.huc.DelegatingHttpsURLConnection.getResponseCode(DelegatingHttpsURLConnection.java:106)
       at com.android.okhttp.internal.huc.HttpsURLConnectionImpl.getResponseCode(HttpsURLConnectionImpl.java:30)
       at com.google.firebase.installations.remote.FirebaseInstallationServiceClient.createFirebaseInstallation(FirebaseInstallationServiceClient.java:199)
       at com.google.firebase.installations.FirebaseInstallations.registerFidWithServer(FirebaseInstallations.java:199)
       at com.google.firebase.installations.FirebaseInstallations.doNetworkCallIfNecessary(FirebaseInstallations.java:110)
       at com.google.firebase.installations.FirebaseInstallations.lambda$doRegistrationOrRefresh$3(FirebaseInstallations.java:110)
       at com.google.firebase.concurrent.SequentialExecutor$1.run(SequentialExecutor.java:30)
       at com.google.firebase.concurrent.SequentialExecutor$QueueWorker.workOnQueue(SequentialExecutor.java:79)
       at com.google.firebase.concurrent.SequentialExecutor$QueueWorker.run(SequentialExecutor.java:7)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1167)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:929)

# Okio Watchdog:
       at java.lang.Object.wait(Object.java)
       at com.android.okhttp.okio.AsyncTimeout.awaitTimeout(AsyncTimeout.java:325)
       at com.android.okhttp.okio.AsyncTimeout.access$000(AsyncTimeout.java:42)
       at com.android.okhttp.okio.AsyncTimeout$Watchdog.run(AsyncTimeout.java:288)

# DefaultDispatcher-worker-3:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:353)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# queued-work-looper:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:363)
       at android.os.Looper.loop(Looper.java:176)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# magnifier pixel copy result handler:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:363)
       at android.os.Looper.loop(Looper.java:176)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# Firebase Blocking Thread #1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:230)
       at java.util.concurrent.SynchronousQueue$TransferStack.awaitFulfill(SynchronousQueue.java:461)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:362)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:937)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1091)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:929)

# GmsDynamite:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at com.google.android.gms.dynamite.zza.run(zza.java:16)

# pool-8-thread-1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:929)
 
</details>
 </details>

 <details>
   
   <summary>Galaxy M01 Core</summary> 

![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/416d5490-0aa7-4b98-ba92-ecfa8695c8d5)


<details>
 
   *<summary>Details</summary>*

   # Crashlytics - Stack trace
# Application: com.weeklyplannerapp.weekplan
# Platform: android
# Version: 7.97 (82)
# Issue: 49bac065e671918743fe5a66dced9112
# Session: 654B2A3C031000017225EE3ECA8FEF95_DNE_0_v2
# Date: Wed Nov 08 2023 08:48:09 GMT+0200 (Eastern European Standard Time)

# Fatal Exception: java.lang.NullPointerException: Attempt to invoke virtual method 'int android.text.Layout.getLineCount()' on a null object reference
       at android.widget.TextView.onMeasure(TextView.java:9518)
       at androidx.appcompat.widget.AppCompatTextView.onMeasure(AppCompatTextView.java:27)
       at android.view.View.measure(View.java:24876)
       at android.view.ViewGroup.measureChildWithMargins(ViewGroup.java:6831)
       at android.widget.LinearLayout.measureChildBeforeLayout(LinearLayout.java:1552)
       at android.widget.LinearLayout.measureVertical(LinearLayout.java:842)
       at android.widget.LinearLayout.onMeasure(LinearLayout.java:721)
       at android.view.View.measure(View.java:24876)
       at androidx.constraintlayout.widget.ConstraintLayout$Measurer.measure(ConstraintLayout.java:503)
       at androidx.constraintlayout.core.widgets.analyzer.BasicMeasure.measure(BasicMeasure.java:101)
       at androidx.constraintlayout.core.widgets.analyzer.BasicMeasure.measureChildren(BasicMeasure.java:1310)
       at androidx.constraintlayout.core.widgets.analyzer.BasicMeasure.solverMeasure(BasicMeasure.java:1310)
       at androidx.constraintlayout.core.widgets.ConstraintWidgetContainer.measure(ConstraintWidgetContainer.java:1310)
       at androidx.constraintlayout.widget.ConstraintLayout.resolveSystem(ConstraintLayout.java:1310)
       at androidx.constraintlayout.widget.ConstraintLayout.onMeasure(ConstraintLayout.java:1310)
       at android.view.View.measure(View.java:24876)
       at androidx.core.widget.NestedScrollView.measureChildWithMargins(NestedScrollView.java:38)
       at android.widget.FrameLayout.onMeasure(FrameLayout.java:194)
       at androidx.core.widget.NestedScrollView.onMeasure(NestedScrollView.java)
       at android.view.View.measure(View.java:24876)
       at androidx.constraintlayout.widget.ConstraintLayout$Measurer.measure(ConstraintLayout.java:503)
       at androidx.constraintlayout.core.widgets.analyzer.BasicMeasure.measure(BasicMeasure.java:101)
       at androidx.constraintlayout.core.widgets.analyzer.BasicMeasure.solverMeasure(BasicMeasure.java:1542)
       at androidx.constraintlayout.core.widgets.ConstraintWidgetContainer.measure(ConstraintWidgetContainer.java:1542)
       at androidx.constraintlayout.widget.ConstraintLayout.resolveSystem(ConstraintLayout.java:1542)
       at androidx.constraintlayout.widget.ConstraintLayout.onMeasure(ConstraintLayout.java:1542)
       at android.view.View.measure(View.java:24876)
       at android.view.ViewGroup.measureChildWithMargins(ViewGroup.java:6831)
       at android.widget.FrameLayout.onMeasure(FrameLayout.java:194)
       at android.view.View.measure(View.java:24876)
       at android.view.ViewGroup.measureChildWithMargins(ViewGroup.java:6831)
       at android.widget.FrameLayout.onMeasure(FrameLayout.java:194)
       at androidx.appcompat.widget.ContentFrameLayout.onMeasure(ContentFrameLayout.java:159)
       at android.view.View.measure(View.java:24876)
       at android.view.ViewGroup.measureChildWithMargins(ViewGroup.java:6831)
       at android.widget.LinearLayout.measureChildBeforeLayout(LinearLayout.java:1552)
       at android.widget.LinearLayout.measureVertical(LinearLayout.java:842)
       at android.widget.LinearLayout.onMeasure(LinearLayout.java:721)
       at android.view.View.measure(View.java:24876)
       at android.view.ViewGroup.measureChildWithMargins(ViewGroup.java:6831)
       at android.widget.FrameLayout.onMeasure(FrameLayout.java:194)
       at android.view.View.measure(View.java:24876)
       at android.view.ViewGroup.measureChildWithMargins(ViewGroup.java:6831)
       at android.widget.LinearLayout.measureChildBeforeLayout(LinearLayout.java:1552)
       at android.widget.LinearLayout.measureVertical(LinearLayout.java:842)
       at android.widget.LinearLayout.onMeasure(LinearLayout.java:721)
       at android.view.View.measure(View.java:24876)
       at android.view.ViewGroup.measureChildWithMargins(ViewGroup.java:6831)
       at android.widget.FrameLayout.onMeasure(FrameLayout.java:194)
       at com.android.internal.policy.DecorView.onMeasure(DecorView.java:753)
       at android.view.View.measure(View.java:24876)
       at android.view.ViewRootImpl.performMeasure(ViewRootImpl.java:3139)
       at android.view.ViewRootImpl.measureHierarchy(ViewRootImpl.java:1910)
       at android.view.ViewRootImpl.performTraversals(ViewRootImpl.java:2210)
       at android.view.ViewRootImpl.doTraversal(ViewRootImpl.java:1793)
       at android.view.ViewRootImpl$TraversalRunnable.run(ViewRootImpl.java:7828)
       at android.view.Choreographer$CallbackRecord.run(Choreographer.java:966)
       at android.view.Choreographer.doCallbacks(Choreographer.java:790)
       at android.view.Choreographer.doFrame(Choreographer.java:725)
       at android.view.Choreographer$FrameDisplayEventReceiver.run(Choreographer.java:951)
       at android.os.Handler.handleCallback(Handler.java:883)
       at android.os.Handler.dispatchMessage(Handler.java:100)
       at android.os.Looper.loop(Looper.java:214)
       at android.app.ActivityThread.main(ActivityThread.java:7438)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:493)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:989)

# Okio Watchdog:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at com.android.okhttp.okio.AsyncTimeout.awaitTimeout(AsyncTimeout.java:313)
       at com.android.okhttp.okio.AsyncTimeout.access$000(AsyncTimeout.java:42)
       at com.android.okhttp.okio.AsyncTimeout$Watchdog.run(AsyncTimeout.java:288)

# glide-source-thread-1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.PriorityBlockingQueue.take(PriorityBlockingQueue.java:548)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultThreadFactory$1.run(GlideExecutor.java:2022)
       at java.lang.Thread.run(Thread.java:919)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultPriorityThreadFactory$1.run(GlideExecutor.java:12)

# Firebase Background Thread #1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:919)

# glide-active-resources:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:190)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:211)
       at com.bumptech.glide.load.engine.ActiveResources.cleanReferenceQueue(ActiveResources.java:320)
       at com.bumptech.glide.load.engine.ActiveResources$2.run(ActiveResources.java:320)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1167)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.bumptech.glide.load.engine.ActiveResources$1$1.run(ActiveResources.java:2040)
       at java.lang.Thread.run(Thread.java:919)

# Firebase Background Thread #3:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:919)

# FinalizerDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:190)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:211)
       at java.lang.Daemons$FinalizerDaemon.runInternal(Daemons.java:271)
       at java.lang.Daemons$Daemon.run(Daemons.java:137)
       at java.lang.Thread.run(Thread.java:919)

# FinalizerWatchdogDaemon:
       at java.lang.Thread.sleep(Thread.java)
       at java.lang.Thread.sleep(Thread.java:440)
       at java.lang.Thread.sleep(Thread.java:356)
       at java.lang.Daemons$FinalizerWatchdogDaemon.sleepForMillis(Daemons.java:383)
       at java.lang.Daemons$FinalizerWatchdogDaemon.waitForFinalization(Daemons.java:411)
       at java.lang.Daemons$FinalizerWatchdogDaemon.runInternal(Daemons.java:323)
       at java.lang.Daemons$Daemon.run(Daemons.java:137)
       at java.lang.Thread.run(Thread.java:919)

# AsyncTask #42:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:230)
       at java.util.concurrent.SynchronousQueue$TransferStack.awaitFulfill(SynchronousQueue.java:461)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:362)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:937)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1091)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:919)

# Firebase Background Thread #0:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:919)

# ReferenceQueueDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at java.lang.Daemons$ReferenceQueueDaemon.runInternal(Daemons.java:215)
       at java.lang.Daemons$Daemon.run(Daemons.java:137)
       at java.lang.Thread.run(Thread.java:919)

# AsyncTask #39:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:230)
       at java.util.concurrent.SynchronousQueue$TransferStack.awaitFulfill(SynchronousQueue.java:461)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:362)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:937)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1091)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:919)

# RealmFinalizingDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:190)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:211)
       at io.realm.internal.FinalizerRunnable.run(FinalizerRunnable.java:3)
       at java.lang.Thread.run(Thread.java:919)

# PlayBillingLibrary-3:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:919)

# Firebase Background Thread #2:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:919)

# pool-10-thread-1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:919)

GLThread 107440:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at android.opengl.GLSurfaceView$GLThread.guardedRun(GLSurfaceView.java:1524)
       at android.opengl.GLSurfaceView$GLThread.run(GLSurfaceView.java:1293)

# PlayBillingLibrary-1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:919)

# PlayBillingLibrary-2:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:919)

# PlayBillingLibrary-1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:919)

# glide-disk-cache-thread-0:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.PriorityBlockingQueue.take(PriorityBlockingQueue.java:548)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultThreadFactory$1.run(GlideExecutor.java:2022)
       at java.lang.Thread.run(Thread.java:919)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultPriorityThreadFactory$1.run(GlideExecutor.java:12)

# PlayBillingLibrary-3:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:919)

# PlayBillingLibrary-4:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:919)

# PlayBillingLibrary-3:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:919)

# PlayBillingLibrary-4:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:919)

# glide-source-thread-0:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.PriorityBlockingQueue.take(PriorityBlockingQueue.java:548)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultThreadFactory$1.run(GlideExecutor.java:2022)
       at java.lang.Thread.run(Thread.java:919)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultPriorityThreadFactory$1.run(GlideExecutor.java:12)

# GmsDynamite:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at com.google.android.gms.dynamite.zza.run(zza.java:16)

# DefaultDispatcher-worker-3:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:353)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# awaitEvenIfOnMainThread task continuation executor1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:919)

# PlayBillingLibrary-1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:919)

# DefaultDispatcher-worker-1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:353)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# PlayBillingLibrary-2:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:919)

# PlayBillingLibrary-2:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:919)

# DefaultDispatcher-worker-2:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:353)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# Measurement Worker:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at m.ll.run(:com.google.android.gms.dynamite_measurementdynamite@234313051@23.43.13 (110300-0):71)

# PlayBillingLibrary-4:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:919)

# Crashlytics Exception Handler1:
       at dalvik.system.VMStack.getThreadStackTrace(VMStack.java)
       at java.lang.Thread.getStackTrace(Thread.java:1720)
       at java.lang.Thread.getAllStackTraces(Thread.java:1796)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateThreadsList(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateExecutionData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateEventApplicationData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.captureEventData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistEvent(SessionReportingCoordinator.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistFatalEvent(SessionReportingCoordinator.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsBackgroundWorker$3.then(CrashlyticsBackgroundWorker.java:16)
       at com.google.android.gms.tasks.zze.run(:8)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1167)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:919)

# ConnectivityThread:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:336)
       at android.os.Looper.loop(Looper.java:174)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# com.google.firebase.crashlytics.startup1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:919)

# ScionFrontendApi:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:230)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.awaitNanos(AbstractQueuedSynchronizer.java:2109)
       at java.util.concurrent.LinkedBlockingQueue.poll(LinkedBlockingQueue.java:467)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1091)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:919)

# magnifier pixel copy result handler:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:336)
       at android.os.Looper.loop(Looper.java:174)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# queued-work-looper:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:336)
       at android.os.Looper.loop(Looper.java:174)
       at android.os.HandlerThread.run(HandlerThread.java:67)
    
 
</details>
 </details>

<details>
   
   <summary>Galaxy A5</summary> 

![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/aa0f14bb-d2be-43de-9a55-c3c97526fd59)


<details>
 
   *<summary>Details</summary>*

   # Crashlytics - Stack trace
# Application: com.weeklyplannerapp.weekplan
# Platform: android
# Version: 7.97 (82)
# Issue: 04b7c6767155e63a5f263a412b42308c
# Session: 65550EF9017F00013009F594AC00E775_DNE_0_v2
# Date: Wed Nov 15 2023 22:04:29 GMT+0200 (Eastern European Standard Time)

# Fatal Exception: java.lang.NullPointerException: Attempt to invoke virtual method 'void android.view.View.setBackground(android.graphics.drawable.Drawable)' on a null object reference
       at com.weeklyplannerapp.weekplan.View.Activities.MainActivity.R(MainActivity.java:35)
       at com.weeklyplannerapp.weekplan.View.Activities.MainActivity.onConfigurationChanged(MainActivity.java:15)
       at android.app.ActivityThread.performActivityConfigurationChanged(ActivityThread.java:6071)
       at android.app.ActivityThread.performConfigurationChangedForActivity(ActivityThread.java:5915)
       at android.app.ActivityThread.performConfigurationChangedForActivity(ActivityThread.java:5893)
       at android.app.ActivityThread.handleActivityConfigurationChanged(ActivityThread.java:6401)
       at android.app.servertransaction.ActivityConfigurationChangeItem.execute(ActivityConfigurationChangeItem.java:48)
       at android.app.servertransaction.TransactionExecutor.executeCallbacks(TransactionExecutor.java:135)
       at android.app.servertransaction.TransactionExecutor.execute(TransactionExecutor.java:95)
       at android.app.ActivityThread$H.handleMessage(ActivityThread.java:2267)
       at android.os.Handler.dispatchMessage(Handler.java:107)
       at android.os.Looper.loop(Looper.java:237)
       at android.app.ActivityThread.main(ActivityThread.java:8167)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:496)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:1100)

# FinalizerDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:190)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:211)
       at java.lang.Daemons$FinalizerDaemon.runInternal(Daemons.java:271)
       at java.lang.Daemons$Daemon.run(Daemons.java:137)
       at java.lang.Thread.run(Thread.java:919)

# com.google.firebase.crashlytics.startup1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:919)

# awaitEvenIfOnMainThread task continuation executor1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:919)

# DefaultDispatcher-worker-3:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:353)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# Firebase Background Thread #1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:919)

# DefaultDispatcher-worker-2:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:353)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# magnifier pixel copy result handler:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:336)
       at android.os.Looper.loop(Looper.java:197)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# ReferenceQueueDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at java.lang.Daemons$ReferenceQueueDaemon.runInternal(Daemons.java:215)
       at java.lang.Daemons$Daemon.run(Daemons.java:137)
       at java.lang.Thread.run(Thread.java:919)

# GmsDynamite:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at com.google.android.gms.dynamite.zza.run(zza.java:16)

# Firebase Background Thread #0:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:919)

# Firebase Background Thread #2:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:919)

# Crashlytics Exception Handler1:
       at dalvik.system.VMStack.getThreadStackTrace(VMStack.java)
       at java.lang.Thread.getStackTrace(Thread.java:1720)
       at java.lang.Thread.getAllStackTraces(Thread.java:1796)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateThreadsList(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateExecutionData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateEventApplicationData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.captureEventData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistEvent(SessionReportingCoordinator.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistFatalEvent(SessionReportingCoordinator.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsBackgroundWorker$3.then(CrashlyticsBackgroundWorker.java:16)
       at com.google.android.gms.tasks.zze.run(:8)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1167)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:919)

# Firebase Background Thread #3:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:919)

# ScionFrontendApi:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:230)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.awaitNanos(AbstractQueuedSynchronizer.java:2109)
       at java.util.concurrent.LinkedBlockingQueue.poll(LinkedBlockingQueue.java:467)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1091)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:919)

# queued-work-looper:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:336)
       at android.os.Looper.loop(Looper.java:197)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# GLThread 11818:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at android.opengl.GLSurfaceView$GLThread.guardedRun(GLSurfaceView.java:1516)
       at android.opengl.GLSurfaceView$GLThread.run(GLSurfaceView.java:1285)

# DefaultDispatcher-worker-1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:353)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# FinalizerWatchdogDaemon:
       at java.lang.Thread.sleep(Thread.java)
       at java.lang.Thread.sleep(Thread.java:440)
       at java.lang.Thread.sleep(Thread.java:356)
       at java.lang.Daemons$FinalizerWatchdogDaemon.sleepForMillis(Daemons.java:383)
       at java.lang.Daemons$FinalizerWatchdogDaemon.waitForFinalization(Daemons.java:411)
       at java.lang.Daemons$FinalizerWatchdogDaemon.runInternal(Daemons.java:323)
       at java.lang.Daemons$Daemon.run(Daemons.java:137)
       at java.lang.Thread.run(Thread.java:919)

# pool-10-thread-1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:919)
 
</details>
 </details>

<details>
   
   <summary>Redmi Note 9 Pro</summary> 

![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/0ba6a41b-1ece-40af-a97b-c2eaf21e18d1)


<details>
 
   *<summary>Details</summary>*

   # Crashlytics - Stack trace
# Application: com.weeklyplannerapp.weekplan
# Platform: android
# Version: 7.97 (82)
# Issue: 49bac065e671918743fe5a66dced9112
# Session: 6551A1A802B300017B001E3CF941D5D0_DNE_0_v2
# Date: Mon Nov 13 2023 06:30:18 GMT+0200 (Eastern European Standard Time)

# Fatal Exception: java.lang.NullPointerException: Attempt to invoke virtual method 'int android.text.Layout.getLineCount()' on a null object reference
       at android.widget.TextView.onMeasure(TextView.java:9437)
       at androidx.appcompat.widget.AppCompatTextView.onMeasure(AppCompatTextView.java:27)
       at android.view.View.measure(View.java:24855)
       at android.view.ViewGroup.measureChildWithMargins(ViewGroup.java:6893)
       at android.widget.LinearLayout.measureChildBeforeLayout(LinearLayout.java:1552)
       at android.widget.LinearLayout.measureVertical(LinearLayout.java:842)
       at android.widget.LinearLayout.onMeasure(LinearLayout.java:721)
       at android.view.View.measure(View.java:24855)
       at androidx.constraintlayout.widget.ConstraintLayout$Measurer.measure(ConstraintLayout.java:503)
       at androidx.constraintlayout.core.widgets.analyzer.BasicMeasure.measure(BasicMeasure.java:101)
       at androidx.constraintlayout.core.widgets.analyzer.BasicMeasure.measureChildren(BasicMeasure.java:1310)
       at androidx.constraintlayout.core.widgets.analyzer.BasicMeasure.solverMeasure(BasicMeasure.java:1310)
       at androidx.constraintlayout.core.widgets.ConstraintWidgetContainer.measure(ConstraintWidgetContainer.java:1310)
       at androidx.constraintlayout.widget.ConstraintLayout.resolveSystem(ConstraintLayout.java:1310)
       at androidx.constraintlayout.widget.ConstraintLayout.onMeasure(ConstraintLayout.java:1310)
       at android.view.View.measure(View.java:24855)
       at androidx.core.widget.NestedScrollView.measureChildWithMargins(NestedScrollView.java:38)
       at android.widget.FrameLayout.onMeasure(FrameLayout.java:194)
       at androidx.core.widget.NestedScrollView.onMeasure(NestedScrollView.java)
       at android.view.View.measure(View.java:24855)
       at androidx.constraintlayout.widget.ConstraintLayout$Measurer.measure(ConstraintLayout.java:503)
       at androidx.constraintlayout.core.widgets.analyzer.BasicMeasure.measure(BasicMeasure.java:101)
       at androidx.constraintlayout.core.widgets.analyzer.BasicMeasure.solverMeasure(BasicMeasure.java:1542)
       at androidx.constraintlayout.core.widgets.ConstraintWidgetContainer.measure(ConstraintWidgetContainer.java:1542)
       at androidx.constraintlayout.widget.ConstraintLayout.resolveSystem(ConstraintLayout.java:1542)
       at androidx.constraintlayout.widget.ConstraintLayout.onMeasure(ConstraintLayout.java:1542)
       at android.view.View.measure(View.java:24855)
       at android.view.ViewGroup.measureChildWithMargins(ViewGroup.java:6893)
       at android.widget.FrameLayout.onMeasure(FrameLayout.java:194)
       at android.view.View.measure(View.java:24855)
       at android.view.ViewGroup.measureChildWithMargins(ViewGroup.java:6893)
       at android.widget.FrameLayout.onMeasure(FrameLayout.java:194)
       at androidx.appcompat.widget.ContentFrameLayout.onMeasure(ContentFrameLayout.java:159)
       at android.view.View.measure(View.java:24855)
       at android.view.ViewGroup.measureChildWithMargins(ViewGroup.java:6893)
       at android.widget.LinearLayout.measureChildBeforeLayout(LinearLayout.java:1552)
       at android.widget.LinearLayout.measureVertical(LinearLayout.java:842)
       at android.widget.LinearLayout.onMeasure(LinearLayout.java:721)
       at android.view.View.measure(View.java:24855)
       at android.view.ViewGroup.measureChildWithMargins(ViewGroup.java:6893)
       at android.widget.FrameLayout.onMeasure(FrameLayout.java:194)
       at android.view.View.measure(View.java:24855)
       at android.view.ViewGroup.measureChildWithMargins(ViewGroup.java:6893)
       at android.widget.LinearLayout.measureChildBeforeLayout(LinearLayout.java:1552)
       at android.widget.LinearLayout.measureVertical(LinearLayout.java:842)
       at android.widget.LinearLayout.onMeasure(LinearLayout.java:721)
       at android.view.View.measure(View.java:24855)
       at android.view.ViewGroup.measureChildWithMargins(ViewGroup.java:6893)
       at android.widget.FrameLayout.onMeasure(FrameLayout.java:194)
       at com.android.internal.policy.DecorView.onMeasure(DecorView.java:773)
       at android.view.View.measure(View.java:24855)
       at android.view.ViewRootImpl.performMeasure(ViewRootImpl.java:3117)
       at android.view.ViewRootImpl.measureHierarchy(ViewRootImpl.java:1931)
       at android.view.ViewRootImpl.performTraversals(ViewRootImpl.java:2225)
       at android.view.ViewRootImpl.doTraversal(ViewRootImpl.java:1819)
       at android.view.ViewRootImpl$TraversalRunnable.run(ViewRootImpl.java:7781)
       at android.view.Choreographer$CallbackRecord.run(Choreographer.java:1031)
       at android.view.Choreographer.doCallbacks(Choreographer.java:854)
       at android.view.Choreographer.doFrame(Choreographer.java:789)
       at android.view.Choreographer$FrameDisplayEventReceiver.run(Choreographer.java:1016)
       at android.os.Handler.handleCallback(Handler.java:883)
       at android.os.Handler.dispatchMessage(Handler.java:100)
       at android.os.Looper.loop(Looper.java:224)
       at android.app.ActivityThread.main(ActivityThread.java:7562)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:539)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:950)

# PlayBillingLibrary-1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:919)

# Firebase Background Thread #2:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:919)

# ScionFrontendApi:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:230)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.awaitNanos(AbstractQueuedSynchronizer.java:2109)
       at java.util.concurrent.LinkedBlockingQueue.poll(LinkedBlockingQueue.java:467)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1091)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:919)

# FinalizerWatchdogDaemon:
       at java.lang.Thread.sleep(Thread.java)
       at java.lang.Thread.sleep(Thread.java:440)
       at java.lang.Thread.sleep(Thread.java:356)
       at java.lang.Daemons$FinalizerWatchdogDaemon.sleepForMillis(Daemons.java:385)
       at java.lang.Daemons$FinalizerWatchdogDaemon.waitForFinalization(Daemons.java:413)
       at java.lang.Daemons$FinalizerWatchdogDaemon.runInternal(Daemons.java:325)
       at java.lang.Daemons$Daemon.run(Daemons.java:139)
       at java.lang.Thread.run(Thread.java:919)

# AsyncTask #8:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:230)
       at java.util.concurrent.SynchronousQueue$TransferStack.awaitFulfill(SynchronousQueue.java:461)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:362)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:937)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1091)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:919)

# PlayBillingLibrary-1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:919)

# PlayBillingLibrary-3:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:919)

# PlayBillingLibrary-2:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:919)

# magnifier pixel copy result handler:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:336)
       at android.os.Looper.loop(Looper.java:181)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# RealmFinalizingDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:190)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:211)
       at io.realm.internal.FinalizerRunnable.run(FinalizerRunnable.java:3)
       at java.lang.Thread.run(Thread.java:919)

# GLThread 101486:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at android.opengl.GLSurfaceView$GLThread.guardedRun(GLSurfaceView.java:1497)
       at android.opengl.GLSurfaceView$GLThread.run(GLSurfaceView.java:1272)

# PlayBillingLibrary-3:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:919)

# DefaultDispatcher-worker-3:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:353)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# PlayBillingLibrary-4:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:919)

# DefaultDispatcher-worker-1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:353)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# PlayBillingLibrary-2:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:919)

# FinalizerDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:190)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:211)
       at java.lang.Daemons$FinalizerDaemon.runInternal(Daemons.java:273)
       at java.lang.Daemons$Daemon.run(Daemons.java:139)
       at java.lang.Thread.run(Thread.java:919)

# Firebase Background Thread #1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:919)

# Firebase Background Thread #0:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:919)

# Crashlytics Exception Handler1:
       at dalvik.system.VMStack.getThreadStackTrace(VMStack.java)
       at java.lang.Thread.getStackTrace(Thread.java:1720)
       at java.lang.Thread.getAllStackTraces(Thread.java:1796)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateThreadsList(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateExecutionData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateEventApplicationData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.captureEventData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistEvent(SessionReportingCoordinator.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistFatalEvent(SessionReportingCoordinator.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsBackgroundWorker$3.then(CrashlyticsBackgroundWorker.java:16)
       at com.google.android.gms.tasks.zze.run(:8)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1167)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:919)

# awaitEvenIfOnMainThread task continuation executor1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:919)

# Okio Watchdog:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at com.android.okhttp.okio.AsyncTimeout.awaitTimeout(AsyncTimeout.java:313)
       at com.android.okhttp.okio.AsyncTimeout.access$000(AsyncTimeout.java:42)
       at com.android.okhttp.okio.AsyncTimeout$Watchdog.run(AsyncTimeout.java:288)

# Firebase Background Thread #3:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:919)

# com.google.firebase.crashlytics.startup1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:919)

# Firebase Blocking Thread #3:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:230)
       at java.util.concurrent.SynchronousQueue$TransferStack.awaitFulfill(SynchronousQueue.java:461)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:362)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:937)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1091)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:919)

# AsyncTask #7:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:230)
       at java.util.concurrent.SynchronousQueue$TransferStack.awaitFulfill(SynchronousQueue.java:461)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:362)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:937)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1091)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:919)

# Measurement Worker:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at m.lm.run(:com.google.android.gms.dynamite_measurementdynamite@234313022@23.43.13 (100400-0):71)

# TcmReceiver:
       at android.net.LocalSocketImpl.readba_native(LocalSocketImpl.java)
       at android.net.LocalSocketImpl.access$300(LocalSocketImpl.java:37)
       at android.net.LocalSocketImpl$SocketInputStream.read(LocalSocketImpl.java:113)
       at com.qti.tcmclient.DpmTcmClient$TcmReceiver.run(DpmTcmClient.java:149)
       at java.lang.Thread.run(Thread.java:919)

# GmsDynamite:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at com.google.android.gms.dynamite.zza.run(zza.java:16)

# ReferenceQueueDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at java.lang.Daemons$ReferenceQueueDaemon.runInternal(Daemons.java:217)
       at java.lang.Daemons$Daemon.run(Daemons.java:139)
       at java.lang.Thread.run(Thread.java:919)

# pool-9-thread-1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:919)

# queued-work-looper:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:336)
       at android.os.Looper.loop(Looper.java:181)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# PlayBillingLibrary-4:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:919)

# DefaultDispatcher-worker-2:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:353)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# AsyncTask #9:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:230)
       at java.util.concurrent.SynchronousQueue$TransferStack.awaitFulfill(SynchronousQueue.java:461)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:362)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:937)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1091)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:919)
 
</details>
 </details>

 <details>
   
   <summary>Redmi Note 7</summary> 

![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/66bfb306-56ed-4c9e-a96b-aa6af8f8b91f)


<details>
 
   *<summary>Details</summary>*

   # Crashlytics - Stack trace
# Application: com.weeklyplannerapp.weekplan
# Platform: android
# Version: 7.97 (82)
# Issue: 04b7c6767155e63a5f263a412b42308c
# Session: 6551DCBC01F9000125D4618050E44D86_DNE_0_v2
# Date: Mon Nov 13 2023 10:22:22 GMT+0200 (Eastern European Standard Time)

# Fatal Exception: java.lang.NullPointerException: Attempt to invoke virtual method 'void android.view.View.setBackground(android.graphics.drawable.Drawable)' on a null object reference
       at com.weeklyplannerapp.weekplan.View.Activities.MainActivity.R(MainActivity.java:35)
       at com.weeklyplannerapp.weekplan.View.Activities.MainActivity.onConfigurationChanged(MainActivity.java:15)
       at android.app.ActivityThread.performActivityConfigurationChanged(ActivityThread.java:5640)
       at android.app.ActivityThread.performConfigurationChangedForActivity(ActivityThread.java:5507)
       at android.app.ActivityThread.performConfigurationChangedForActivity(ActivityThread.java:5485)
       at android.app.ActivityThread.handleActivityConfigurationChanged(ActivityThread.java:5911)
       at android.app.servertransaction.ActivityConfigurationChangeItem.execute(ActivityConfigurationChangeItem.java:48)
       at android.app.servertransaction.TransactionExecutor.executeCallbacks(TransactionExecutor.java:135)
       at android.app.servertransaction.TransactionExecutor.execute(TransactionExecutor.java:95)
       at android.app.ActivityThread$H.handleMessage(ActivityThread.java:2047)
       at android.os.Handler.dispatchMessage(Handler.java:107)
       at android.os.Looper.loop(Looper.java:224)
       at android.app.ActivityThread.main(ActivityThread.java:7590)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:539)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:950)

# ReferenceQueueDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at java.lang.Daemons$ReferenceQueueDaemon.runInternal(Daemons.java:217)
       at java.lang.Daemons$Daemon.run(Daemons.java:139)
       at java.lang.Thread.run(Thread.java:919)

# GmsDynamite:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at com.google.android.gms.dynamite.zza.run(zza.java:16)

# Firebase Blocking Thread #1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:230)
       at java.util.concurrent.SynchronousQueue$TransferStack.awaitFulfill(SynchronousQueue.java:461)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:362)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:937)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1091)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:919)

# Measurement Worker:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at m.ll.run(:com.google.android.gms.dynamite_measurementdynamite@234414022@23.44.14 (100400-0):71)

# Firebase Background Thread #1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:919)

# DefaultDispatcher-worker-3:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:353)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# awaitEvenIfOnMainThread task continuation executor1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:919)

# queued-work-looper:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:336)
       at android.os.Looper.loop(Looper.java:181)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# magnifier pixel copy result handler:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:336)
       at android.os.Looper.loop(Looper.java:181)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# GLThread 253793:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at android.opengl.GLSurfaceView$GLThread.guardedRun(GLSurfaceView.java:1497)
       at android.opengl.GLSurfaceView$GLThread.run(GLSurfaceView.java:1272)

# DefaultDispatcher-worker-1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:353)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# TcmReceiver:
       at android.net.LocalSocketImpl.readba_native(LocalSocketImpl.java)
       at android.net.LocalSocketImpl.access$300(LocalSocketImpl.java:37)
       at android.net.LocalSocketImpl$SocketInputStream.read(LocalSocketImpl.java:113)
       at com.qti.tcmclient.DpmTcmClient$TcmReceiver.run(DpmTcmClient.java:149)
       at java.lang.Thread.run(Thread.java:919)

# com.google.firebase.crashlytics.startup1:
       at libcore.io.Linux.android_getaddrinfo(Linux.java)
       at libcore.io.ForwardingOs.android_getaddrinfo(ForwardingOs.java:74)
       at libcore.io.BlockGuardOs.android_getaddrinfo(BlockGuardOs.java:200)
       at libcore.io.ForwardingOs.android_getaddrinfo(ForwardingOs.java:74)
       at java.net.Inet6AddressImpl.lookupHostByName(Inet6AddressImpl.java:135)
       at java.net.Inet6AddressImpl.lookupAllHostAddr(Inet6AddressImpl.java:103)
       at java.net.InetAddress.getAllByName(InetAddress.java:1152)
       at com.android.okhttp.Dns$1.lookup(Dns.java:41)
       at com.android.okhttp.internal.http.RouteSelector.resetNextInetSocketAddress(RouteSelector.java:178)
       at com.android.okhttp.internal.http.RouteSelector.nextProxy(RouteSelector.java:144)
       at com.android.okhttp.internal.http.RouteSelector.next(RouteSelector.java:86)
       at com.android.okhttp.internal.http.StreamAllocation.findConnection(StreamAllocation.java:176)
       at com.android.okhttp.internal.http.StreamAllocation.findHealthyConnection(StreamAllocation.java:128)
       at com.android.okhttp.internal.http.StreamAllocation.newStream(StreamAllocation.java:97)
       at com.android.okhttp.internal.http.HttpEngine.connect(HttpEngine.java:289)
       at com.android.okhttp.internal.http.HttpEngine.sendRequest(HttpEngine.java:232)
       at com.android.okhttp.internal.huc.HttpURLConnectionImpl.execute(HttpURLConnectionImpl.java:465)
       at com.android.okhttp.internal.huc.HttpURLConnectionImpl.connect(HttpURLConnectionImpl.java:131)
       at com.android.okhttp.internal.huc.DelegatingHttpsURLConnection.connect(DelegatingHttpsURLConnection.java:90)
       at com.android.okhttp.internal.huc.HttpsURLConnectionImpl.connect(HttpsURLConnectionImpl.java:30)
       at com.google.firebase.crashlytics.internal.network.HttpGetRequest.execute(HttpGetRequest.java:104)
       at com.google.firebase.crashlytics.internal.settings.DefaultSettingsSpiCall.invoke(DefaultSettingsSpiCall.java:108)
       at com.google.firebase.crashlytics.internal.settings.SettingsController$1.then(SettingsController.java:108)
       at com.google.firebase.crashlytics.internal.settings.SettingsController$1.then(SettingsController.java:108)
       at com.google.android.gms.tasks.zzo.run(:12)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1167)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:919)

# FinalizerDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:190)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:211)
       at java.lang.Daemons$FinalizerDaemon.runInternal(Daemons.java:273)
       at java.lang.Daemons$Daemon.run(Daemons.java:139)
       at java.lang.Thread.run(Thread.java:919)

# Firebase Blocking Thread #2:
       at libcore.io.Linux.android_getaddrinfo(Linux.java)
       at libcore.io.ForwardingOs.android_getaddrinfo(ForwardingOs.java:74)
       at libcore.io.BlockGuardOs.android_getaddrinfo(BlockGuardOs.java:200)
       at libcore.io.ForwardingOs.android_getaddrinfo(ForwardingOs.java:74)
       at java.net.Inet6AddressImpl.lookupHostByName(Inet6AddressImpl.java:135)
       at java.net.Inet6AddressImpl.lookupAllHostAddr(Inet6AddressImpl.java:103)
       at java.net.InetAddress.getAllByName(InetAddress.java:1152)
       at com.android.okhttp.Dns$1.lookup(Dns.java:41)
       at com.android.okhttp.internal.http.RouteSelector.resetNextInetSocketAddress(RouteSelector.java:178)
       at com.android.okhttp.internal.http.RouteSelector.nextProxy(RouteSelector.java:144)
       at com.android.okhttp.internal.http.RouteSelector.next(RouteSelector.java:86)
       at com.android.okhttp.internal.http.StreamAllocation.findConnection(StreamAllocation.java:176)
       at com.android.okhttp.internal.http.StreamAllocation.findHealthyConnection(StreamAllocation.java:128)
       at com.android.okhttp.internal.http.StreamAllocation.newStream(StreamAllocation.java:97)
       at com.android.okhttp.internal.http.HttpEngine.connect(HttpEngine.java:289)
       at com.android.okhttp.internal.http.HttpEngine.sendRequest(HttpEngine.java:232)
       at com.android.okhttp.internal.huc.HttpURLConnectionImpl.execute(HttpURLConnectionImpl.java:465)
       at com.android.okhttp.internal.huc.HttpURLConnectionImpl.getResponse(HttpURLConnectionImpl.java:411)
       at com.android.okhttp.internal.huc.HttpURLConnectionImpl.getResponseCode(HttpURLConnectionImpl.java:542)
       at com.android.okhttp.internal.huc.DelegatingHttpsURLConnection.getResponseCode(DelegatingHttpsURLConnection.java:106)
       at com.android.okhttp.internal.huc.HttpsURLConnectionImpl.getResponseCode(HttpsURLConnectionImpl.java:30)
       at com.google.firebase.sessions.settings.RemoteSettingsFetcher$doConfigFetch$2.invokeSuspend(RemoteSettingsFetcher.java:106)
       at kotlin.coroutines.jvm.internal.BaseContinuationImpl.resumeWith(BaseContinuationImpl.java:8)
       at kotlinx.coroutines.DispatchedTask.run(DispatchedTask.java:1)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1167)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:919)

# FinalizerWatchdogDaemon:
       at java.lang.Thread.sleep(Thread.java)
       at java.lang.Thread.sleep(Thread.java:440)
       at java.lang.Thread.sleep(Thread.java:356)
       at java.lang.Daemons$FinalizerWatchdogDaemon.sleepForMillis(Daemons.java:385)
       at java.lang.Daemons$FinalizerWatchdogDaemon.waitForFinalization(Daemons.java:413)
       at java.lang.Daemons$FinalizerWatchdogDaemon.runInternal(Daemons.java:325)
       at java.lang.Daemons$Daemon.run(Daemons.java:139)
       at java.lang.Thread.run(Thread.java:919)

# pool-8-thread-1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:919)

# DefaultDispatcher-worker-2:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:353)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# Firebase Background Thread #0:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:919)

# Crashlytics Exception Handler1:
       at dalvik.system.VMStack.getThreadStackTrace(VMStack.java)
       at java.lang.Thread.getStackTrace(Thread.java:1720)
       at java.lang.Thread.getAllStackTraces(Thread.java:1796)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateThreadsList(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateExecutionData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateEventApplicationData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.captureEventData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistEvent(SessionReportingCoordinator.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistFatalEvent(SessionReportingCoordinator.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsBackgroundWorker$3.then(CrashlyticsBackgroundWorker.java:16)
       at com.google.android.gms.tasks.zze.run(:8)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1167)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:919)

# Firebase Background Thread #2:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:919)

# Firebase Background Thread #3:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:919)

# ScionFrontendApi:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:230)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.awaitNanos(AbstractQueuedSynchronizer.java:2109)
       at java.util.concurrent.LinkedBlockingQueue.poll(LinkedBlockingQueue.java:467)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1091)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:919)

# Firebase Blocking Thread #0:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:230)
       at java.util.concurrent.SynchronousQueue$TransferStack.awaitFulfill(SynchronousQueue.java:461)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:362)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:937)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1091)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:919)
 
</details>
 </details>

<details>
   
   <summary>Redmi 8</summary> 

![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/82bec5b8-4d42-490e-a9dd-43aa4ef97cdd)


<details>
 
   *<summary>Details</summary>*

    # Crashlytics - Stack trace
# Application: com.weeklyplannerapp.weekplan
# Platform: android
# Version: 7.97 (82)
# Issue: 72bd018209352c1b39c33f10f34b265c
# Session: 654FC4CD0104000142B4DDD826A6ED20_DNE_0_v2
# Date: Sat Nov 11 2023 20:16:31 GMT+0200 (Eastern European Standard Time)

# Fatal Exception: java.lang.RuntimeException: Unable to stop activity {com.weeklyplannerapp.weekplan/com.weeklyplannerapp.weekplan.View.Activities.MainActivity}: io.realm.exceptions.RealmFileException: Failed to open file at path '/data/data/com.weeklyplannerapp.weekplan/11.11.2023 20:16': parent directory does not exist (/data/data/com.weeklyplannerapp.weekplan/11.11.2023 20:16) in /tmp/realm-java/realm/realm-library/src/main/cpp/io_realm_internal_OsSharedRealm.cpp line 404 Kind: NOT_FOUND.
       at android.app.ActivityThread.callActivityOnStop(ActivityThread.java:4711)
       at android.app.ActivityThread.performStopActivityInner(ActivityThread.java:4681)
       at android.app.ActivityThread.handleStopActivity(ActivityThread.java:4756)
       at android.app.servertransaction.StopActivityItem.execute(StopActivityItem.java:41)
       at android.app.servertransaction.TransactionExecutor.executeLifecycleState(TransactionExecutor.java:176)
       at android.app.servertransaction.TransactionExecutor.execute(TransactionExecutor.java:97)
       at android.app.ActivityThread$H.handleMessage(ActivityThread.java:2044)
       at android.os.Handler.dispatchMessage(Handler.java:107)
       at android.os.Looper.loop(Looper.java:223)
       at android.app.ActivityThread.main(ActivityThread.java:7562)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:539)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:950)

# Caused by io.realm.exceptions.RealmFileException: Failed to open file at path '/data/data/com.weeklyplannerapp.weekplan/11.11.2023 20:16': parent directory does not exist (/data/data/com.weeklyplannerapp.weekplan/11.11.2023 20:16) in /tmp/realm-java/realm/realm-library/src/main/cpp/io_realm_internal_OsSharedRealm.cpp line 404
       at io.realm.internal.OsSharedRealm.nativeWriteCopy(OsSharedRealm.java)
       at io.realm.internal.OsSharedRealm.writeCopy(OsSharedRealm.java:38)
       at io.realm.BaseRealm.writeCopyTo(BaseRealm.java:1)
       at com.weeklyplannerapp.weekplan.WeeklyPlanApplication$1.onActivityStopped(WeeklyPlanApplication.java:199)
       at android.app.Application.dispatchActivityStopped(Application.java:521)
       at android.app.Activity.dispatchActivityStopped(Activity.java:1363)
       at android.app.Activity.onStop(Activity.java:2516)
       at androidx.fragment.app.FragmentActivity.onStop(FragmentActivity.java:1)
       at androidx.appcompat.app.AppCompatActivity.onStop(AppCompatActivity.java:1)
       at com.weeklyplannerapp.weekplan.View.Activities.MainActivity.onStop(MainActivity.java)
       at android.app.Instrumentation.callActivityOnStop(Instrumentation.java:1474)
       at android.app.Activity.performStop(Activity.java:8156)
       at android.app.ActivityThread.callActivityOnStop(ActivityThread.java:4703)
       at android.app.ActivityThread.performStopActivityInner(ActivityThread.java:4681)
       at android.app.ActivityThread.handleStopActivity(ActivityThread.java:4756)
       at android.app.servertransaction.StopActivityItem.execute(StopActivityItem.java:41)
       at android.app.servertransaction.TransactionExecutor.executeLifecycleState(TransactionExecutor.java:176)
       at android.app.servertransaction.TransactionExecutor.execute(TransactionExecutor.java:97)
       at android.app.ActivityThread$H.handleMessage(ActivityThread.java:2044)
       at android.os.Handler.dispatchMessage(Handler.java:107)
       at android.os.Looper.loop(Looper.java:223)
       at android.app.ActivityThread.main(ActivityThread.java:7562)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:539)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:950)

# ReferenceQueueDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at java.lang.Daemons$ReferenceQueueDaemon.runInternal(Daemons.java:217)
       at java.lang.Daemons$Daemon.run(Daemons.java:139)
       at java.lang.Thread.run(Thread.java:919)

# com.google.firebase.crashlytics.startup1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:919)

# Firebase Blocking Thread #0:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:230)
       at java.util.concurrent.SynchronousQueue$TransferStack.awaitFulfill(SynchronousQueue.java:461)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:362)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:937)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1091)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:919)

# FinalizerDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:190)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:211)
       at java.lang.Daemons$FinalizerDaemon.runInternal(Daemons.java:273)
       at java.lang.Daemons$Daemon.run(Daemons.java:139)
       at java.lang.Thread.run(Thread.java:919)

# ConnectivityThread:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:336)
       at android.os.Looper.loop(Looper.java:180)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# Firebase Blocking Thread #2:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:230)
       at java.util.concurrent.SynchronousQueue$TransferStack.awaitFulfill(SynchronousQueue.java:461)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:362)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:937)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1091)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:919)

# DefaultDispatcher-worker-3:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:353)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# pool-9-thread-1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:919)

# GmsDynamite:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at com.google.android.gms.dynamite.zza.run(zza.java:16)

# Firebase Blocking Thread #1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:230)
       at java.util.concurrent.SynchronousQueue$TransferStack.awaitFulfill(SynchronousQueue.java:461)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:362)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:937)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1091)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:919)

# glide-source-thread-0:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.PriorityBlockingQueue.take(PriorityBlockingQueue.java:548)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultThreadFactory$1.run(GlideExecutor.java:2022)
       at java.lang.Thread.run(Thread.java:919)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultPriorityThreadFactory$1.run(GlideExecutor.java:12)

# Firebase Background Thread #1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:919)

# PlayBillingLibrary-4:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:919)

# ScionFrontendApi:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:230)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.awaitNanos(AbstractQueuedSynchronizer.java:2109)
       at java.util.concurrent.LinkedBlockingQueue.poll(LinkedBlockingQueue.java:467)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1091)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:919)

# glide-source-thread-1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.PriorityBlockingQueue.take(PriorityBlockingQueue.java:548)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultThreadFactory$1.run(GlideExecutor.java:2022)
       at java.lang.Thread.run(Thread.java:919)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultPriorityThreadFactory$1.run(GlideExecutor.java:12)

# DefaultDispatcher-worker-1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:353)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# OkHttp ConnectionPool:
       at java.lang.Object.wait(Object.java)
       at com.android.okhttp.ConnectionPool$1.run(ConnectionPool.java:107)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1167)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:919)

# TcmReceiver:
       at android.net.LocalSocketImpl.readba_native(LocalSocketImpl.java)
       at android.net.LocalSocketImpl.access$300(LocalSocketImpl.java:37)
       at android.net.LocalSocketImpl$SocketInputStream.read(LocalSocketImpl.java:113)
       at com.qti.tcmclient.DpmTcmClient$TcmReceiver.run(DpmTcmClient.java:149)
       at java.lang.Thread.run(Thread.java:919)

# glide-disk-cache-thread-0:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.PriorityBlockingQueue.take(PriorityBlockingQueue.java:548)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultThreadFactory$1.run(GlideExecutor.java:2022)
       at java.lang.Thread.run(Thread.java:919)
       at com.bumptech.glide.load.engine.executor.GlideExecutor$DefaultPriorityThreadFactory$1.run(GlideExecutor.java:12)

# AsyncTask #3:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:230)
       at java.util.concurrent.SynchronousQueue$TransferStack.awaitFulfill(SynchronousQueue.java:461)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:362)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:937)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1091)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:919)

# Measurement Worker:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at m.lm.run(:com.google.android.gms.dynamite_measurementdynamite@234313022@23.43.13 (100400-0):71)

# GLThread 3451:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at android.opengl.GLSurfaceView$GLThread.guardedRun(GLSurfaceView.java:1497)
       at android.opengl.GLSurfaceView$GLThread.run(GLSurfaceView.java:1272)

# DefaultDispatcher-worker-2:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:353)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:225)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:225)

# awaitEvenIfOnMainThread task continuation executor1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:919)

# Firebase Background Thread #3:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:919)

# Okio Watchdog:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at com.android.okhttp.okio.AsyncTimeout.awaitTimeout(AsyncTimeout.java:313)
       at com.android.okhttp.okio.AsyncTimeout.access$000(AsyncTimeout.java:42)
       at com.android.okhttp.okio.AsyncTimeout$Watchdog.run(AsyncTimeout.java:288)

# RealmFinalizingDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:190)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:211)
       at io.realm.internal.FinalizerRunnable.run(FinalizerRunnable.java:3)
       at java.lang.Thread.run(Thread.java:919)

# Firebase Background Thread #2:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:919)

# AsyncTask #4:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:230)
       at java.util.concurrent.SynchronousQueue$TransferStack.awaitFulfill(SynchronousQueue.java:461)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:362)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:937)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1091)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:919)

# PlayBillingLibrary-2:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:919)

# Crashlytics Exception Handler1:
       at dalvik.system.VMStack.getThreadStackTrace(VMStack.java)
       at java.lang.Thread.getStackTrace(Thread.java:1720)
       at java.lang.Thread.getAllStackTraces(Thread.java:1796)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateThreadsList(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateExecutionData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateEventApplicationData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.captureEventData(CrashlyticsReportDataCapture.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistEvent(SessionReportingCoordinator.java:142)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistFatalEvent(SessionReportingCoordinator.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:58)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsBackgroundWorker$3.then(CrashlyticsBackgroundWorker.java:16)
       at com.google.android.gms.tasks.zze.run(:8)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1167)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:919)

# glide-active-resources:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:190)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:211)
       at com.bumptech.glide.load.engine.ActiveResources.cleanReferenceQueue(ActiveResources.java:320)
       at com.bumptech.glide.load.engine.ActiveResources$2.run(ActiveResources.java:320)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1167)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.bumptech.glide.load.engine.ActiveResources$1$1.run(ActiveResources.java:2040)
       at java.lang.Thread.run(Thread.java:919)

# Firebase Background Thread #0:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:162)
       at java.lang.Thread.run(Thread.java:919)

# PlayBillingLibrary-3:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:919)

# magnifier pixel copy result handler:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:336)
       at android.os.Looper.loop(Looper.java:180)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# queued-work-looper:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:336)
       at android.os.Looper.loop(Looper.java:180)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# PlayBillingLibrary-1:
       at sun.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:190)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:2067)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:442)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1092)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1152)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
       at java.lang.Thread.run(Thread.java:919)

# FinalizerWatchdogDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:442)
       at java.lang.Object.wait(Object.java:568)
       at java.lang.Daemons$FinalizerWatchdogDaemon.sleepUntilNeeded(Daemons.java:341)
       at java.lang.Daemons$FinalizerWatchdogDaemon.runInternal(Daemons.java:321)
       at java.lang.Daemons$Daemon.run(Daemons.java:139)
       at java.lang.Thread.run(Thread.java:919)
 
</details>
 </details>
  </details>
  
 ![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/cda627a8-4550-4cfc-ac9c-74d99abe643a)

<details>

  <summary>Android 13</summary><br>

  <details>
 
<summary>All devices</summary>

![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/9ba91182-0031-462d-ba59-4fb3d9ef9525)

  </details>


  
<details>  
   
   <summary>Redmi Note 11 Pro 5G</summary>
    
![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/79792b05-e8e3-4d4f-a6c3-c316e2ca9cfb)



<details>
 
   *<summary>Details</summary>*

 # Crashlytics - Stack trace
# Application: com.weeklyplannerapp.weekplan
# Platform: android
# Version: 7.98.2 (84)
# Issue: 72bd018209352c1b39c33f10f34b265c
# Session: 656B311202E200013BAF8EC20F765155_DNE_0_v2
# Date: Sat Dec 02 2023 15:32:50 GMT+0200 (Eastern European Standard Time)

# Fatal Exception: java.lang.RuntimeException: Unable to stop activity {com.weeklyplannerapp.weekplan/com.weeklyplannerapp.weekplan.View.Activities.MainActivity}: io.realm.exceptions.RealmFileException: Failed to open file at path '/data/data/com.weeklyplannerapp.weekplan/02.12.2023 10:32': parent directory does not exist (/data/data/com.weeklyplannerapp.weekplan/02.12.2023 10:32) in /tmp/realm-java/realm/realm-library/src/main/cpp/io_realm_internal_OsSharedRealm.cpp line 404 Kind: NOT_FOUND.
       at android.app.ActivityThread.callActivityOnStop(ActivityThread.java:5483)
       at android.app.ActivityThread.performStopActivityInner(ActivityThread.java:5455)
       at android.app.ActivityThread.handleStopActivity(ActivityThread.java:5520)
       at android.app.servertransaction.StopActivityItem.execute(StopActivityItem.java:43)
       at android.app.servertransaction.ActivityTransactionItem.execute(ActivityTransactionItem.java:45)
       at android.app.servertransaction.TransactionExecutor.executeLifecycleState(TransactionExecutor.java:176)
       at android.app.servertransaction.TransactionExecutor.execute(TransactionExecutor.java:97)
       at android.app.ActivityThread$H.handleMessage(ActivityThread.java:2415)
       at android.os.Handler.dispatchMessage(Handler.java:106)
       at android.os.Looper.loopOnce(Looper.java:211)
       at android.os.Looper.loop(Looper.java:300)
       at android.app.ActivityThread.main(ActivityThread.java:8410)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:559)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:954)

# Caused by io.realm.exceptions.RealmFileException: Failed to open file at path '/data/data/com.weeklyplannerapp.weekplan/02.12.2023 10:32': parent directory does not exist (/data/data/com.weeklyplannerapp.weekplan/02.12.2023 10:32) in /tmp/realm-java/realm/realm-library/src/main/cpp/io_realm_internal_OsSharedRealm.cpp line 404
       at io.realm.internal.OsSharedRealm.nativeWriteCopy(OsSharedRealm.java)
       at io.realm.internal.OsSharedRealm.writeCopy(OsSharedRealm.java:38)
       at io.realm.BaseRealm.writeCopyTo(BaseRealm.java:1)
       at com.weeklyplannerapp.weekplan.WeeklyPlanApplication$1.onActivityStopped(WeeklyPlanApplication.java:209)
       at android.app.Application.dispatchActivityStopped(Application.java:503)
       at android.app.Activity.dispatchActivityStopped(Activity.java:1580)
       at android.app.Activity.onStop(Activity.java:2738)
       at androidx.fragment.app.FragmentActivity.onStop(FragmentActivity.java:1)
       at androidx.appcompat.app.AppCompatActivity.onStop(AppCompatActivity.java:1)
       at com.weeklyplannerapp.weekplan.View.Activities.MainActivity.onStop(MainActivity.java)
       at android.app.Instrumentation.callActivityOnStop(Instrumentation.java:1607)
       at android.app.Activity.performStop(Activity.java:8796)
       at android.app.ActivityThread.callActivityOnStop(ActivityThread.java:5475)
       at android.app.ActivityThread.performStopActivityInner(ActivityThread.java:5455)
       at android.app.ActivityThread.handleStopActivity(ActivityThread.java:5520)
       at android.app.servertransaction.StopActivityItem.execute(StopActivityItem.java:43)
       at android.app.servertransaction.ActivityTransactionItem.execute(ActivityTransactionItem.java:45)
       at android.app.servertransaction.TransactionExecutor.executeLifecycleState(TransactionExecutor.java:176)
       at android.app.servertransaction.TransactionExecutor.execute(TransactionExecutor.java:97)
       at android.app.ActivityThread$H.handleMessage(ActivityThread.java:2415)
       at android.os.Handler.dispatchMessage(Handler.java:106)
       at android.os.Looper.loopOnce(Looper.java:211)
       at android.os.Looper.loop(Looper.java:300)
       at android.app.ActivityThread.main(ActivityThread.java:8410)
       at java.lang.reflect.Method.invoke(Method.java)
       at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:559)
       at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:954)

# awaitEvenIfOnMainThread task continuation executor1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# DefaultDispatcher-worker-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:302)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:302)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:302)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:302)

# PlayBillingLibrary-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# RealmFinalizingDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:210)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:231)
       at io.realm.internal.FinalizerRunnable.run(FinalizerRunnable.java:3)
       at java.lang.Thread.run(Thread.java:1012)

# GmsDynamite:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at com.google.android.gms.dynamite.zza.run(zza.java:16)

# AnimRunnerThread:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:341)
       at android.os.Looper.loopOnce(Looper.java:169)
       at android.os.Looper.loop(Looper.java:300)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# Measurement Worker:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at com.google.android.gms.measurement.internal.zzhc.run(zzhc.java:71)

# LogThread:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:341)
       at android.os.Looper.loopOnce(Looper.java:169)
       at android.os.Looper.loop(Looper.java:300)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# Firebase Background Thread #0:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:794)
       at java.lang.Thread.run(Thread.java:1012)

# queued-work-looper:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:341)
       at android.os.Looper.loopOnce(Looper.java:169)
       at android.os.Looper.loop(Looper.java:300)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# PlayBillingLibrary-3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:794)
       at java.lang.Thread.run(Thread.java:1012)

# ScionFrontendApi:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.awaitNanos(AbstractQueuedSynchronizer.java:1672)
       at java.util.concurrent.LinkedBlockingQueue.poll(LinkedBlockingQueue.java:460)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# GLThread 160088:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at android.opengl.GLSurfaceView$GLThread.guardedRun(GLSurfaceView.java:1497)
       at android.opengl.GLSurfaceView$GLThread.run(GLSurfaceView.java:1272)

# Firebase Background Thread #3:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:794)
       at java.lang.Thread.run(Thread.java:1012)

# Okio Watchdog:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at com.android.okhttp.okio.AsyncTimeout.awaitTimeout(AsyncTimeout.java:313)
       at com.android.okhttp.okio.AsyncTimeout.access$000(AsyncTimeout.java:42)
       at com.android.okhttp.okio.AsyncTimeout$Watchdog.run(AsyncTimeout.java:288)

# AnimThread-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.SynchronousQueue$TransferStack$SNode.block(SynchronousQueue.java:288)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:397)
       at java.util.concurrent.SynchronousQueue.take(SynchronousQueue.java:886)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# InsetsAnimations:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:341)
       at android.os.Looper.loopOnce(Looper.java:169)
       at android.os.Looper.loop(Looper.java:300)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# magnifier pixel copy result handler:
       at android.os.MessageQueue.nativePollOnce(MessageQueue.java)
       at android.os.MessageQueue.next(MessageQueue.java:341)
       at android.os.Looper.loopOnce(Looper.java:169)
       at android.os.Looper.loop(Looper.java:300)
       at android.os.HandlerThread.run(HandlerThread.java:67)

# FinalizerWatchdogDaemon:
       at java.lang.Thread.sleep(Thread.java)
       at java.lang.Thread.sleep(Thread.java:450)
       at java.lang.Thread.sleep(Thread.java:355)
       at java.lang.Daemons$FinalizerWatchdogDaemon.sleepForNanos(Daemons.java:481)
       at java.lang.Daemons$FinalizerWatchdogDaemon.waitForProgress(Daemons.java:544)
       at java.lang.Daemons$FinalizerWatchdogDaemon.runInternal(Daemons.java:412)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# AsyncTask #10:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.SynchronousQueue$TransferStack$SNode.block(SynchronousQueue.java:288)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:397)
       at java.util.concurrent.SynchronousQueue.take(SynchronousQueue.java:886)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# Timer-0:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.util.TimerThread.mainLoop(Timer.java:534)
       at java.util.TimerThread.run(Timer.java:513)

# Crashlytics Exception Handler1:
       at dalvik.system.VMStack.getThreadStackTrace(VMStack.java)
       at java.lang.Thread.getStackTrace(Thread.java:1841)
       at java.lang.Thread.getAllStackTraces(Thread.java:1909)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateThreadsList(CrashlyticsReportDataCapture.java:204)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateExecutionData(CrashlyticsReportDataCapture.java:204)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.populateEventApplicationData(CrashlyticsReportDataCapture.java:204)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsReportDataCapture.captureEventData(CrashlyticsReportDataCapture.java:204)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistEvent(SessionReportingCoordinator.java:204)
       at com.google.firebase.crashlytics.internal.common.SessionReportingCoordinator.persistFatalEvent(SessionReportingCoordinator.java:59)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:59)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsController$2.call(CrashlyticsController.java:59)
       at com.google.firebase.crashlytics.internal.common.CrashlyticsBackgroundWorker$3.then(CrashlyticsBackgroundWorker.java:12)
       at com.google.android.gms.tasks.zze.run(:8)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1145)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# FinalizerDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:210)
       at java.lang.ref.ReferenceQueue.remove(ReferenceQueue.java:231)
       at java.lang.Daemons$FinalizerDaemon.runInternal(Daemons.java:309)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Blocking Thread #1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)
       at java.util.concurrent.SynchronousQueue$TransferStack.transfer(SynchronousQueue.java:401)
       at java.util.concurrent.SynchronousQueue.poll(SynchronousQueue.java:903)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1070)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:794)
       at java.lang.Thread.run(Thread.java:1012)

# com.google.firebase.crashlytics.startup1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.crashlytics.internal.common.ExecutorUtils$1$1.onRun(ExecutorUtils.java:1)
       at com.google.firebase.crashlytics.internal.common.BackgroundPriorityRunnable.run(BackgroundPriorityRunnable.java:1)
       at java.lang.Thread.run(Thread.java:1012)

# Firebase Background Thread #1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at com.google.firebase.concurrent.CustomThreadFactory.lambda$newThread$0(CustomThreadFactory.java:794)
       at java.lang.Thread.run(Thread.java:1012)

# PlayBillingLibrary-4:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# ReferenceQueueDaemon:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.lang.Daemons$ReferenceQueueDaemon.runInternal(Daemons.java:239)
       at java.lang.Daemons$Daemon.run(Daemons.java:145)
       at java.lang.Thread.run(Thread.java:1012)

# DefaultDispatcher-worker-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:302)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:302)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:302)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:302)

# Timer-1:
       at java.lang.Object.wait(Object.java)
       at java.lang.Object.wait(Object.java:386)
       at java.lang.Object.wait(Object.java:524)
       at java.util.TimerThread.mainLoop(Timer.java:534)
       at java.util.TimerThread.run(Timer.java:513)

# DefaultDispatcher-worker-2:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:376)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.park(CoroutineScheduler.java:302)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.tryPark(CoroutineScheduler.java:302)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.java:302)
       at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.java:302)

# pool-9-thread-1:
       at jdk.internal.misc.Unsafe.park(Unsafe.java)
       at java.util.concurrent.locks.LockSupport.park(LockSupport.java:341)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(AbstractQueuedSynchronizer.java:506)
       at java.util.concurrent.ForkJoinPool.unmanagedBlock(ForkJoinPool.java:3466)
       at java.util.concurrent.ForkJoinPool.managedBlock(ForkJoinPool.java:3437)
       at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(AbstractQueuedSynchronizer.java:1623)
       at java.util.concurrent.LinkedBlockingQueue.take(LinkedBlockingQueue.java:435)
       at java.util.concurrent.ThreadPoolExecutor.getTask(ThreadPoolExecutor.java:1071)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1131)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)

# OkHttp ConnectionPool:
       at java.lang.Object.wait(Object.java)
       at com.android.okhttp.ConnectionPool$1.run(ConnectionPool.java:106)
       at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1145)
       at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:644)
       at java.lang.Thread.run(Thread.java:1012)
 
</details>
 </details>

