```
Ricardos-MacBook-Pro-9:java-marbles-client olivieri$ mvn exec:java -Dexec.mainClass="com.mycompany.app.App"
[INFO] Scanning for projects...
[INFO] 
[INFO] ----------------------< com.mycompany.app:my-app >----------------------
[INFO] Building my-app 1.0-SNAPSHOT
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] 
[INFO] --- exec-maven-plugin:1.6.0:java (default-cli) @ my-app ---
[com.mycompany.app.App.main()] INFO  com.mycompany.app.App  - Starting Fabric client application...
[com.mycompany.app.App.main()] INFO  com.mycompany.app.App  - About to create a new marble... invoking initMarble() method in chaincode...
[com.mycompany.app.App.main()] INFO  com.mycompany.app.App  - About to call readMarble() method in chaincode...
[com.mycompany.app.App.main()] INFO  com.mycompany.app.App  - Result from calling readMarble: {"color":"blue","docType":"marble","name":"0a61e932-ab2e-48b4-8c58-f6a2087b53d4","owner":"tom","size":35}
[com.mycompany.app.App.main()] INFO  com.mycompany.app.App  - Finished executing Fabric client application...
[WARNING] thread Thread[grpc-default-worker-ELG-1-1,5,com.mycompany.app.App] was interrupted but is still alive after waiting at least 14997msecs
[WARNING] thread Thread[grpc-default-worker-ELG-1-1,5,com.mycompany.app.App] will linger despite being asked to die via interruption
[WARNING] thread Thread[grpc-default-executor-0,5,com.mycompany.app.App] will linger despite being asked to die via interruption
[WARNING] thread Thread[grpc-default-worker-ELG-1-2,5,com.mycompany.app.App] will linger despite being asked to die via interruption
[WARNING] thread Thread[grpc-default-worker-ELG-1-3,5,com.mycompany.app.App] will linger despite being asked to die via interruption
[WARNING] thread Thread[grpc-default-worker-ELG-1-4,5,com.mycompany.app.App] will linger despite being asked to die via interruption
[WARNING] thread Thread[pool-3-thread-1,5,com.mycompany.app.App] will linger despite being asked to die via interruption
[WARNING] thread Thread[grpc-default-worker-ELG-1-5,5,com.mycompany.app.App] will linger despite being asked to die via interruption
[WARNING] thread Thread[grpc-default-worker-ELG-1-6,5,com.mycompany.app.App] will linger despite being asked to die via interruption
[WARNING] thread Thread[grpc-default-worker-ELG-1-7,5,com.mycompany.app.App] will linger despite being asked to die via interruption
[WARNING] thread Thread[grpc-default-worker-ELG-1-8,5,com.mycompany.app.App] will linger despite being asked to die via interruption
[WARNING] thread Thread[grpc-default-worker-ELG-1-9,5,com.mycompany.app.App] will linger despite being asked to die via interruption
[WARNING] thread Thread[grpc-default-worker-ELG-1-10,5,com.mycompany.app.App] will linger despite being asked to die via interruption
[WARNING] thread Thread[grpc-default-worker-ELG-1-11,5,com.mycompany.app.App] will linger despite being asked to die via interruption
[WARNING] thread Thread[grpc-default-worker-ELG-1-12,5,com.mycompany.app.App] will linger despite being asked to die via interruption
[WARNING] thread Thread[grpc-default-worker-ELG-1-13,5,com.mycompany.app.App] will linger despite being asked to die via interruption
[WARNING] thread Thread[grpc-default-worker-ELG-1-14,5,com.mycompany.app.App] will linger despite being asked to die via interruption
[WARNING] thread Thread[grpc-default-worker-ELG-1-15,5,com.mycompany.app.App] will linger despite being asked to die via interruption
[WARNING] thread Thread[grpc-default-worker-ELG-1-16,5,com.mycompany.app.App] will linger despite being asked to die via interruption
[WARNING] thread Thread[pool-1-thread-1,5,com.mycompany.app.App] will linger despite being asked to die via interruption
[WARNING] thread Thread[pool-1-thread-2,5,com.mycompany.app.App] will linger despite being asked to die via interruption
[WARNING] thread Thread[pool-1-thread-3,5,com.mycompany.app.App] will linger despite being asked to die via interruption
[WARNING] thread Thread[pool-1-thread-4,5,com.mycompany.app.App] will linger despite being asked to die via interruption
[WARNING] thread Thread[pool-1-thread-5,5,com.mycompany.app.App] will linger despite being asked to die via interruption
[WARNING] thread Thread[pool-1-thread-6,5,com.mycompany.app.App] will linger despite being asked to die via interruption
[WARNING] thread Thread[pool-1-thread-7,5,com.mycompany.app.App] will linger despite being asked to die via interruption
[WARNING] thread Thread[pool-1-thread-8,5,com.mycompany.app.App] will linger despite being asked to die via interruption
[WARNING] thread Thread[pool-1-thread-9,5,com.mycompany.app.App] will linger despite being asked to die via interruption
[WARNING] thread Thread[grpc-default-executor-1,5,com.mycompany.app.App] will linger despite being asked to die via interruption
[WARNING] NOTE: 28 thread(s) did not finish despite being asked to  via interruption. This is not a problem with exec:java, it is a problem with the running code. Although not serious, it should be remedied.
[WARNING] Couldn't destroy threadgroup org.codehaus.mojo.exec.ExecJavaMojo$IsolatedThreadGroup[name=com.mycompany.app.App,maxpri=10]
java.lang.IllegalThreadStateException
    at java.lang.ThreadGroup.destroy (ThreadGroup.java:778)
    at org.codehaus.mojo.exec.ExecJavaMojo.execute (ExecJavaMojo.java:321)
    at org.apache.maven.plugin.DefaultBuildPluginManager.executeMojo (DefaultBuildPluginManager.java:137)
    at org.apache.maven.lifecycle.internal.MojoExecutor.execute (MojoExecutor.java:210)
    at org.apache.maven.lifecycle.internal.MojoExecutor.execute (MojoExecutor.java:156)
    at org.apache.maven.lifecycle.internal.MojoExecutor.execute (MojoExecutor.java:148)
    at org.apache.maven.lifecycle.internal.LifecycleModuleBuilder.buildProject (LifecycleModuleBuilder.java:117)
    at org.apache.maven.lifecycle.internal.LifecycleModuleBuilder.buildProject (LifecycleModuleBuilder.java:81)
    at org.apache.maven.lifecycle.internal.builder.singlethreaded.SingleThreadedBuilder.build (SingleThreadedBuilder.java:56)
    at org.apache.maven.lifecycle.internal.LifecycleStarter.execute (LifecycleStarter.java:128)
    at org.apache.maven.DefaultMaven.doExecute (DefaultMaven.java:305)
    at org.apache.maven.DefaultMaven.doExecute (DefaultMaven.java:192)
    at org.apache.maven.DefaultMaven.execute (DefaultMaven.java:105)
    at org.apache.maven.cli.MavenCli.execute (MavenCli.java:956)
    at org.apache.maven.cli.MavenCli.doMain (MavenCli.java:288)
    at org.apache.maven.cli.MavenCli.main (MavenCli.java:192)
    at sun.reflect.NativeMethodAccessorImpl.invoke0 (Native Method)
    at sun.reflect.NativeMethodAccessorImpl.invoke (NativeMethodAccessorImpl.java:62)
    at sun.reflect.DelegatingMethodAccessorImpl.invoke (DelegatingMethodAccessorImpl.java:43)
    at java.lang.reflect.Method.invoke (Method.java:498)
    at org.codehaus.plexus.classworlds.launcher.Launcher.launchEnhanced (Launcher.java:282)
    at org.codehaus.plexus.classworlds.launcher.Launcher.launch (Launcher.java:225)
    at org.codehaus.plexus.classworlds.launcher.Launcher.mainWithExitCode (Launcher.java:406)
    at org.codehaus.plexus.classworlds.launcher.Launcher.main (Launcher.java:347)
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  43.311 s
[INFO] Finished at: 2019-10-02T16:45:54-04:00
[INFO] ------------------------------------------------------------------------
Ricardos-MacBook-Pro-9:java-marbles-client olivieri$
```