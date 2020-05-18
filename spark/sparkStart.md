`************启动任务************`
SH-lihh:spark zenmen$ ./bin/run-example SparkPi 10

`************hadoop代码加载************`
20/05/18 13:55:48 WARN NativeCodeLoader: Unable to load native-hadoop library for your platform... using builtin-java classes where applicable

`************日志配置************`
Using Spark's default log4j profile: org/apache/spark/log4j-defaults.properties
`************版本号************`
20/05/18 13:55:49 INFO SparkContext: Running Spark version 2.4.4
`************提交任务************`
20/05/18 13:55:49 INFO SparkContext: Submitted application: Spark Pi
`************更改权限************`
20/05/18 13:55:49 INFO SecurityManager: Changing view acls to: zenmen
20/05/18 13:55:49 INFO SecurityManager: Changing modify acls to: zenmen
20/05/18 13:55:49 INFO SecurityManager: Changing view acls groups to:
20/05/18 13:55:49 INFO SecurityManager: Changing modify acls groups to:
20/05/18 13:55:49 INFO SecurityManager: SecurityManager: authentication disabled; ui acls disabled; users  with view permissions: Set(zenmen); groups with view permissions: Set(); users  with modify permissions: Set(zenmen); groups with modify permissions: Set()

`************sparkDriver成功启动************`
20/05/18 13:55:49 INFO Utils: Successfully started service 'sparkDriver' on port 54811.
`************注册组件************`
20/05/18 13:55:49 INFO SparkEnv: Registering MapOutputTracker
20/05/18 13:55:49 INFO SparkEnv: Registering BlockManagerMaster
20/05/18 13:55:49 INFO BlockManagerMasterEndpoint: Using org.apache.spark.storage.DefaultTopologyMapper for getting topology information
20/05/18 13:55:49 INFO BlockManagerMasterEndpoint: BlockManagerMasterEndpoint up
`************本地目录************`
20/05/18 13:55:49 INFO DiskBlockManager: Created local directory at /private/var/folders/wd/_f1695t93f7011__r_09wchc0000gn/T/blockmgr-6d081788-e414-4ff2-b9e3-ef9dfc95c971
20/05/18 13:55:49 INFO MemoryStore: MemoryStore started with capacity 366.3 MB
20/05/18 13:55:49 INFO SparkEnv: Registering OutputCommitCoordinator
`************SparkUI成功启动************`
20/05/18 13:55:50 INFO Utils: Successfully started service 'SparkUI' on port 4040.
20/05/18 13:55:50 INFO SparkUI: Bound SparkUI to 0.0.0.0, and started at http://10.8.13.145:4040
`************添加jar包************`
20/05/18 13:55:50 INFO SparkContext: Added JAR file:///Users/zenmen/Desktop/bigdata/modules/spark/examples/jars/spark-examples_2.11-2.4.4.jar at spark://10.8.13.145:54811/jars/spark-examples_2.11-2.4.4.jar with timestamp 1589781350140
20/05/18 13:55:50 INFO SparkContext: Added JAR file:///Users/zenmen/Desktop/bigdata/modules/spark/examples/jars/scopt_2.11-3.7.0.jar at spark://10.8.13.145:54811/jars/scopt_2.11-3.7.0.jar with timestamp 1589781350141
20/05/18 13:55:50 INFO Executor: Starting executor ID driver on host localhost
`************netty启动************`
20/05/18 13:55:50 INFO Utils: Successfully started service 'org.apache.spark.network.netty.NettyBlockTransferService' on port 54813.
20/05/18 13:55:50 INFO NettyBlockTransferService: Server created on 10.8.13.145:54813
`************块管理器************`
20/05/18 13:55:50 INFO BlockManager: Using org.apache.spark.storage.RandomBlockReplicationPolicy for block replication policy
20/05/18 13:55:50 INFO BlockManagerMaster: Registering BlockManager BlockManagerId(driver, 10.8.13.145, 54813, None)
20/05/18 13:55:50 INFO BlockManagerMasterEndpoint: Registering block manager 10.8.13.145:54813 with 366.3 MB RAM, BlockManagerId(driver, 10.8.13.145, 54813, None)
20/05/18 13:55:50 INFO BlockManagerMaster: Registered BlockManager BlockManagerId(driver, 10.8.13.145, 54813, None)
`************初始化块管理器************`
20/05/18 13:55:50 INFO BlockManager: Initialized BlockManager: BlockManagerId(driver, 10.8.13.145, 54813, None)
`************启动任务************`
20/05/18 13:55:51 INFO SparkContext: Starting job: reduce at SparkPi.scala:38
20/05/18 13:55:51 INFO DAGScheduler: Got job 0 (reduce at SparkPi.scala:38) with 10 output partitions
20/05/18 13:55:51 INFO DAGScheduler: Final stage: ResultStage 0 (reduce at SparkPi.scala:38)
20/05/18 13:55:51 INFO DAGScheduler: Parents of final stage: List()
20/05/18 13:55:51 INFO DAGScheduler: Missing parents: List()
20/05/18 13:55:51 INFO DAGScheduler: Submitting ResultStage 0 (MapPartitionsRDD[1] at map at SparkPi.scala:34), which has no missing parents
20/05/18 13:55:51 INFO MemoryStore: Block broadcast_0 stored as values in memory (estimated size 1936.0 B, free 366.3 MB)
20/05/18 13:55:51 INFO MemoryStore: Block broadcast_0_piece0 stored as bytes in memory (estimated size 1256.0 B, free 366.3 MB)
20/05/18 13:55:51 INFO BlockManagerInfo: Added broadcast_0_piece0 in memory on 10.8.13.145:54813 (size: 1256.0 B, free: 366.3 MB)
20/05/18 13:55:51 INFO SparkContext: Created broadcast 0 from broadcast at DAGScheduler.scala:1161
20/05/18 13:55:51 INFO DAGScheduler: Submitting 10 missing tasks from ResultStage 0 (MapPartitionsRDD[1] at map at SparkPi.scala:34) (first 15 tasks are for partitions Vector(0, 1, 2, 3, 4, 5, 6, 7, 8, 9))
20/05/18 13:55:51 INFO TaskSchedulerImpl: Adding task set 0.0 with 10 tasks
20/05/18 13:55:51 INFO TaskSetManager: Starting task 0.0 in stage 0.0 (TID 0, localhost, executor driver, partition 0, PROCESS_LOCAL, 7866 bytes)
20/05/18 13:55:51 INFO TaskSetManager: Starting task 1.0 in stage 0.0 (TID 1, localhost, executor driver, partition 1, PROCESS_LOCAL, 7866 bytes)
20/05/18 13:55:51 INFO TaskSetManager: Starting task 2.0 in stage 0.0 (TID 2, localhost, executor driver, partition 2, PROCESS_LOCAL, 7866 bytes)
20/05/18 13:55:51 INFO TaskSetManager: Starting task 3.0 in stage 0.0 (TID 3, localhost, executor driver, partition 3, PROCESS_LOCAL, 7866 bytes)
20/05/18 13:55:51 INFO Executor: Running task 1.0 in stage 0.0 (TID 1)
20/05/18 13:55:51 INFO Executor: Running task 0.0 in stage 0.0 (TID 0)
20/05/18 13:55:51 INFO Executor: Running task 2.0 in stage 0.0 (TID 2)
20/05/18 13:55:51 INFO Executor: Running task 3.0 in stage 0.0 (TID 3)
20/05/18 13:55:51 INFO Executor: Fetching spark://10.8.13.145:54811/jars/scopt_2.11-3.7.0.jar with timestamp 1589781350141
20/05/18 13:55:51 INFO TransportClientFactory: Successfully created connection to /10.8.13.145:54811 after 36 ms (0 ms spent in bootstraps)
20/05/18 13:55:51 INFO Utils: Fetching spark://10.8.13.145:54811/jars/scopt_2.11-3.7.0.jar to /private/var/folders/wd/_f1695t93f7011__r_09wchc0000gn/T/spark-5c79144c-1e21-4eef-96da-bdfffb9e59d8/userFiles-eacc289c-9209-4a03-98f9-d19670dd8d56/fetchFileTemp416133723202292948.tmp
20/05/18 13:55:51 INFO Executor: Adding file:/private/var/folders/wd/_f1695t93f7011__r_09wchc0000gn/T/spark-5c79144c-1e21-4eef-96da-bdfffb9e59d8/userFiles-eacc289c-9209-4a03-98f9-d19670dd8d56/scopt_2.11-3.7.0.jar to class loader
20/05/18 13:55:51 INFO Executor: Fetching spark://10.8.13.145:54811/jars/spark-examples_2.11-2.4.4.jar with timestamp 1589781350140
20/05/18 13:55:51 INFO Utils: Fetching spark://10.8.13.145:54811/jars/spark-examples_2.11-2.4.4.jar to /private/var/folders/wd/_f1695t93f7011__r_09wchc0000gn/T/spark-5c79144c-1e21-4eef-96da-bdfffb9e59d8/userFiles-eacc289c-9209-4a03-98f9-d19670dd8d56/fetchFileTemp7659669348812265459.tmp
20/05/18 13:55:51 INFO Executor: Adding file:/private/var/folders/wd/_f1695t93f7011__r_09wchc0000gn/T/spark-5c79144c-1e21-4eef-96da-bdfffb9e59d8/userFiles-eacc289c-9209-4a03-98f9-d19670dd8d56/spark-examples_2.11-2.4.4.jar to class loader
20/05/18 13:55:51 INFO Executor: Finished task 3.0 in stage 0.0 (TID 3). 867 bytes result sent to driver
20/05/18 13:55:51 INFO Executor: Finished task 0.0 in stage 0.0 (TID 0). 867 bytes result sent to driver
20/05/18 13:55:51 INFO Executor: Finished task 1.0 in stage 0.0 (TID 1). 867 bytes result sent to driver
20/05/18 13:55:51 INFO TaskSetManager: Starting task 4.0 in stage 0.0 (TID 4, localhost, executor driver, partition 4, PROCESS_LOCAL, 7866 bytes)
20/05/18 13:55:51 INFO TaskSetManager: Starting task 5.0 in stage 0.0 (TID 5, localhost, executor driver, partition 5, PROCESS_LOCAL, 7866 bytes)
20/05/18 13:55:51 INFO TaskSetManager: Starting task 6.0 in stage 0.0 (TID 6, localhost, executor driver, partition 6, PROCESS_LOCAL, 7866 bytes)
20/05/18 13:55:51 INFO Executor: Running task 6.0 in stage 0.0 (TID 6)
20/05/18 13:55:51 INFO Executor: Finished task 2.0 in stage 0.0 (TID 2). 867 bytes result sent to driver
20/05/18 13:55:51 INFO Executor: Running task 4.0 in stage 0.0 (TID 4)
20/05/18 13:55:51 INFO Executor: Running task 5.0 in stage 0.0 (TID 5)
20/05/18 13:55:51 INFO TaskSetManager: Finished task 0.0 in stage 0.0 (TID 0) in 414 ms on localhost (executor driver) (1/10)
20/05/18 13:55:51 INFO TaskSetManager: Finished task 3.0 in stage 0.0 (TID 3) in 393 ms on localhost (executor driver) (2/10)
20/05/18 13:55:51 INFO TaskSetManager: Finished task 1.0 in stage 0.0 (TID 1) in 395 ms on localhost (executor driver) (3/10)
20/05/18 13:55:51 INFO TaskSetManager: Starting task 7.0 in stage 0.0 (TID 7, localhost, executor driver, partition 7, PROCESS_LOCAL, 7866 bytes)
20/05/18 13:55:51 INFO TaskSetManager: Finished task 2.0 in stage 0.0 (TID 2) in 397 ms on localhost (executor driver) (4/10)
20/05/18 13:55:51 INFO Executor: Running task 7.0 in stage 0.0 (TID 7)
20/05/18 13:55:51 INFO Executor: Finished task 6.0 in stage 0.0 (TID 6). 867 bytes result sent to driver
20/05/18 13:55:51 INFO TaskSetManager: Starting task 8.0 in stage 0.0 (TID 8, localhost, executor driver, partition 8, PROCESS_LOCAL, 7866 bytes)
20/05/18 13:55:51 INFO TaskSetManager: Finished task 6.0 in stage 0.0 (TID 6) in 28 ms on localhost (executor driver) (5/10)
20/05/18 13:55:51 INFO Executor: Running task 8.0 in stage 0.0 (TID 8)
20/05/18 13:55:51 INFO Executor: Finished task 8.0 in stage 0.0 (TID 8). 824 bytes result sent to driver
20/05/18 13:55:51 INFO TaskSetManager: Starting task 9.0 in stage 0.0 (TID 9, localhost, executor driver, partition 9, PROCESS_LOCAL, 7866 bytes)
20/05/18 13:55:51 INFO Executor: Running task 9.0 in stage 0.0 (TID 9)
20/05/18 13:55:51 INFO TaskSetManager: Finished task 8.0 in stage 0.0 (TID 8) in 17 ms on localhost (executor driver) (6/10)
20/05/18 13:55:51 INFO Executor: Finished task 9.0 in stage 0.0 (TID 9). 824 bytes result sent to driver
20/05/18 13:55:51 INFO Executor: Finished task 4.0 in stage 0.0 (TID 4). 824 bytes result sent to driver
20/05/18 13:55:51 INFO TaskSetManager: Finished task 9.0 in stage 0.0 (TID 9) in 26 ms on localhost (executor driver) (7/10)
20/05/18 13:55:51 INFO TaskSetManager: Finished task 4.0 in stage 0.0 (TID 4) in 74 ms on localhost (executor driver) (8/10)
20/05/18 13:55:51 INFO Executor: Finished task 7.0 in stage 0.0 (TID 7). 867 bytes result sent to driver
20/05/18 13:55:51 INFO TaskSetManager: Finished task 7.0 in stage 0.0 (TID 7) in 73 ms on localhost (executor driver) (9/10)
20/05/18 13:55:51 INFO Executor: Finished task 5.0 in stage 0.0 (TID 5). 824 bytes result sent to driver
20/05/18 13:55:51 INFO TaskSetManager: Finished task 5.0 in stage 0.0 (TID 5) in 94 ms on localhost (executor driver) (10/10)
20/05/18 13:55:51 INFO TaskSchedulerImpl: Removed TaskSet 0.0, whose tasks have all completed, from pool
20/05/18 13:55:51 INFO DAGScheduler: ResultStage 0 (reduce at SparkPi.scala:38) finished in 0.715 s
20/05/18 13:55:51 INFO DAGScheduler: Job 0 finished: reduce at SparkPi.scala:38, took 0.797889 s
Pi is roughly 3.1413951413951415
`************停止SparkUI************`
20/05/18 13:55:51 INFO SparkUI: Stopped Spark web UI at http://10.8.13.145:4040
`************停止组件MapOutputTrackerMasterEndpoint************`
20/05/18 13:55:51 INFO MapOutputTrackerMasterEndpoint: MapOutputTrackerMasterEndpoint stopped!
`************内存释放************`
20/05/18 13:55:51 INFO MemoryStore: MemoryStore cleared
`************组件释放************`
20/05/18 13:55:51 INFO BlockManager: BlockManager stopped
20/05/18 13:55:51 INFO BlockManagerMaster: BlockManagerMaster stopped
`************组件释放************`
20/05/18 13:55:51 INFO OutputCommitCoordinator$OutputCommitCoordinatorEndpoint: OutputCommitCoordinator stopped!
`************停止SparkContext************`
20/05/18 13:55:51 INFO SparkContext: Successfully stopped SparkContext
20/05/18 13:55:51 INFO ShutdownHookManager: Shutdown hook called
`************删除临时目录************`
20/05/18 13:55:51 INFO ShutdownHookManager: Deleting directory /private/var/folders/wd/_f1695t93f7011__r_09wchc0000gn/T/spark-78940d92-82fe-47b6-b454-8b5fca8684c0
20/05/18 13:55:51 INFO ShutdownHookManager: Deleting directory /private/var/folders/wd/_f1695t93f7011__r_09wchc0000gn/T/spark-5c79144c-1e21-4eef-96da-bdfffb9e59d8


`************总结： 组件************`
1. 创建临时目录
2. 基本信息
  日志配置
  版本号
  任务名称
  权限总览
  提交任务
3. 注册组件
  1. sparkDriver 服务启动
  2. 组件注册
    MapOutputTracker
    BlockManagerMaster
    OutputCommitCoordinator
  2. 磁盘目录，内存空间申请
  3. SparkUI 服务启动
  4. 添加jar包
  5. NettyBlockTransferService服务启动
  6. 任务启动
  
  8. 停止 SparkUI
  9. 停止 MapOutputTrackerMasterEndpoint
  10. 内存释放
  11. 组件释放
  12. 停止SparkContext
  13. 移除目录
 
  
  
  

