 <b>Android Week Planner crashlytics<b>
 ___


# ![Android_robot svg](https://github.com/UserQA07/Week-Planner-/assets/144763744/5613d4b9-b88f-4c1f-84d3-6af9dae0e2ac)
![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/15a70dde-1ae8-46a9-b673-d2b842cf9844)
![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/9285a8ae-1f77-47eb-8297-9fbf90873140)
![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/9719cde5-c799-46da-a896-0c2004b4f414)
![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/89e3629f-d356-447d-9a5c-a32318a35c80)






<details>
  <summary>Android 13</summary>

  - Galaxy S23 Ultra
    
![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/3ba460a3-eb95-40e5-8dca-f86e565206f9)

<details>
 <summary>Text</summary>
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

# ![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/51587895-8c05-4efd-8260-3cdd1e6b919e)


<details>
 <summary>Text</summary>
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

![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/090d3993-057c-4d49-b954-d4d462bd4bac)

<details>
 <summary>Text</summary>
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



  - Redmi Note 11 Pro
    
![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/b92764df-90b1-4bbf-83f6-ed04f6692d59)

<details>
 <summary>Text</summary>
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

OkHttp ConnectionPool:
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

Timer-1:
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

FinalizerWatchdogDaemon:
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

![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/9f16042e-4ad9-4471-9724-200ea41d8f32)

<details>
 <summary>Text</summary>
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


    
  - Redmi Note 11 Pro 5G

![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/5ba7a7c8-93f4-4fd0-a565-2589806ffddd)

<details>
 <summary>Text</summary>
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

  - Redmi Note 10 Pro

![image](https://github.com/UserQA07/Week-Planner-/assets/144763744/a435ca37-7623-44d8-96f7-01746ae3f413)

<details>
 <summary>Text</summary>
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

  - [Ссылка 5](ссылка5)
  - [Ссылка 6](ссылка6)
  - [Ссылка 7](ссылка7)
  - [Ссылка 8](ссылка8)
  - [Ссылка 9](ссылка9)
  - [Ссылка 10](ссылка10)

</details>

<details>
  <summary>Android 12</summary>

  - [Ссылка 1](ссылка1)
  - [Ссылка 2](ссылка2)
  - [Ссылка 3](ссылка3)
  - [Ссылка 4](ссылка4)
  - [Ссылка 5](ссылка5)
  - [Ссылка 6](ссылка6)
  - [Ссылка 7](ссылка7)
  - [Ссылка 8](ссылка8)
  - [Ссылка 9](ссылка9)
  - [Ссылка 10](ссылка10)

</details>

<details>
  <summary>Android 11</summary>

  - [Ссылка 1](ссылка1)
  - [Ссылка 2](ссылка2)
  - [Ссылка 3](ссылка3)
  - [Ссылка 4](ссылка4)
  - [Ссылка 5](ссылка5)
  - [Ссылка 6](ссылка6)
  - [Ссылка 7](ссылка7)
  - [Ссылка 8](ссылка8)
  - [Ссылка 9](ссылка9)
  - [Ссылка 10](ссылка10)

</details>

<details>
  <summary>Android 10</summary>

  - [Ссылка 1](ссылка1)
  - [Ссылка 2](ссылка2)
  - [Ссылка 3](ссылка3)
  - [Ссылка 4](ссылка4)
  - [Ссылка 5](ссылка5)
  - [Ссылка 6](ссылка6)
  - [Ссылка 7](ссылка7)
  - [Ссылка 8](ссылка8)
  - [Ссылка 9](ссылка9)
  - [Ссылка 10](ссылка10)

</details>











  



