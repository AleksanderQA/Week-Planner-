 <b>Android Week Planner crashlytics<b>
 ___


![Android_robot svg](https://github.com/UserQA07/Week-Planner-/assets/144763744/5613d4b9-b88f-4c1f-84d3-6af9dae0e2ac)

<details>
  <summary>Android 13</summary>

  - [Galaxy S23 Ultra](ссылка)
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











  



