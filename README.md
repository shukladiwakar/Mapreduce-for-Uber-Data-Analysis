# Uber Data Ananlysis with the help of mapreduce!
Analysis of Basement having active and current trips

The problem statements can be found in the problemstatement.txt file. The corresponding jar file is Uber which has solutions for Uber1 and Uber2 class for the corresponding problems.





# Hadoop Version Used in the Project
hduser@Diwakar:/home/diwakar$ hadoop version
Hadoop 2.6.0
Subversion https://git-wip-us.apache.org/repos/asf/hadoop.git -r e3496499ecb8d220fba99dc5ed4c99c8f9e33bb1
Compiled by jenkins on 2014-11-13T21:10Z
Compiled with protoc 2.5.0
From source with checksum 18e43357c8f927c0695f1e9522859d6a
This command was run using /usr/local/hadoop/share/hadoop/common/hadoop-common-2.6.0.jar
hduser@Diwakar:/home/diwakar$ 

# How to get the output for second

hduser@Diwakar:/home/diwakar$ hadoop jar '/home/diwakar/Desktop/Hadoop/final-jarfiles/Uber.jar' Uber2 /Projects/uber /op4

# demo output

hduser@Diwakar:/home/diwakar$ hadoop jar '/home/diwakar/Desktop/Hadoop/final-jarfiles/Uber.jar' Uber2 /Projects/uber /op4
17/04/24 22:35:37 WARN util.NativeCodeLoader: Unable to load native-hadoop library for your platform... using builtin-java classes where applicable
17/04/24 22:35:38 INFO Configuration.deprecation: session.id is deprecated. Instead, use dfs.metrics.session-id
17/04/24 22:35:38 INFO jvm.JvmMetrics: Initializing JVM Metrics with processName=JobTracker, sessionId=
17/04/24 22:35:38 WARN mapreduce.JobSubmitter: Hadoop command-line option parsing not performed. Implement the Tool interface and execute your application with ToolRunner to remedy this.
17/04/24 22:35:38 INFO input.FileInputFormat: Total input paths to process : 1
17/04/24 22:35:38 INFO mapreduce.JobSubmitter: number of splits:1
17/04/24 22:35:38 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_local1723100134_0001
17/04/24 22:35:38 INFO mapreduce.Job: The url to track the job: http://localhost:8080/
17/04/24 22:35:38 INFO mapreduce.Job: Running job: job_local1723100134_0001
17/04/24 22:35:38 INFO mapred.LocalJobRunner: OutputCommitter set in config null
17/04/24 22:35:38 INFO mapred.LocalJobRunner: OutputCommitter is org.apache.hadoop.mapreduce.lib.output.FileOutputCommitter
17/04/24 22:35:39 INFO mapred.LocalJobRunner: Waiting for map tasks
17/04/24 22:35:39 INFO mapred.LocalJobRunner: Starting task: attempt_local1723100134_0001_m_000000_0
17/04/24 22:35:39 INFO mapred.Task:  Using ResourceCalculatorProcessTree : [ ]
17/04/24 22:35:39 INFO mapred.MapTask: Processing split: hdfs://localhost:54310/Projects/uber:0+9460
17/04/24 22:35:39 INFO mapred.MapTask: (EQUATOR) 0 kvi 26214396(104857584)
17/04/24 22:35:39 INFO mapred.MapTask: mapreduce.task.io.sort.mb: 100
17/04/24 22:35:39 INFO mapred.MapTask: soft limit at 83886080
17/04/24 22:35:39 INFO mapred.MapTask: bufstart = 0; bufvoid = 104857600
17/04/24 22:35:39 INFO mapred.MapTask: kvstart = 26214396; length = 6553600
17/04/24 22:35:39 INFO mapred.MapTask: Map output collector class = org.apache.hadoop.mapred.MapTask$MapOutputBuffer
17/04/24 22:35:39 INFO mapred.LocalJobRunner: 
17/04/24 22:35:39 INFO mapred.MapTask: Starting flush of map output
17/04/24 22:35:39 INFO mapred.MapTask: Spilling map output
17/04/24 22:35:39 INFO mapred.MapTask: bufstart = 0; bufend = 5310; bufvoid = 104857600
17/04/24 22:35:39 INFO mapred.MapTask: kvstart = 26214396(104857584); kvend = 26212984(104851936); length = 1413/6553600
17/04/24 22:35:39 INFO mapred.MapTask: Finished spill 0
17/04/24 22:35:39 INFO mapred.Task: Task:attempt_local1723100134_0001_m_000000_0 is done. And is in the process of committing
17/04/24 22:35:39 INFO mapred.LocalJobRunner: map
17/04/24 22:35:39 INFO mapred.Task: Task 'attempt_local1723100134_0001_m_000000_0' done.
17/04/24 22:35:39 INFO mapred.LocalJobRunner: Finishing task: attempt_local1723100134_0001_m_000000_0
17/04/24 22:35:39 INFO mapred.LocalJobRunner: map task executor complete.
17/04/24 22:35:39 INFO mapred.LocalJobRunner: Waiting for reduce tasks
17/04/24 22:35:39 INFO mapred.LocalJobRunner: Starting task: attempt_local1723100134_0001_r_000000_0
17/04/24 22:35:39 INFO mapred.Task:  Using ResourceCalculatorProcessTree : [ ]
17/04/24 22:35:39 INFO mapred.ReduceTask: Using ShuffleConsumerPlugin: org.apache.hadoop.mapreduce.task.reduce.Shuffle@4e761248
17/04/24 22:35:39 INFO reduce.MergeManagerImpl: MergerManager: memoryLimit=334338464, maxSingleShuffleLimit=83584616, mergeThreshold=220663392, ioSortFactor=10, memToMemMergeOutputsThreshold=10
17/04/24 22:35:39 INFO reduce.EventFetcher: attempt_local1723100134_0001_r_000000_0 Thread started: EventFetcher for fetching Map Completion Events
17/04/24 22:35:39 INFO reduce.LocalFetcher: localfetcher#1 about to shuffle output of map attempt_local1723100134_0001_m_000000_0 decomp: 716 len: 720 to MEMORY
17/04/24 22:35:39 INFO reduce.InMemoryMapOutput: Read 716 bytes from map-output for attempt_local1723100134_0001_m_000000_0
17/04/24 22:35:39 INFO reduce.MergeManagerImpl: closeInMemoryFile -> map-output of size: 716, inMemoryMapOutputs.size() -> 1, commitMemory -> 0, usedMemory ->716
17/04/24 22:35:39 INFO reduce.EventFetcher: EventFetcher is interrupted.. Returning
17/04/24 22:35:39 INFO mapred.LocalJobRunner: 1 / 1 copied.
17/04/24 22:35:39 INFO reduce.MergeManagerImpl: finalMerge called with 1 in-memory map-outputs and 0 on-disk map-outputs
17/04/24 22:35:39 INFO mapred.Merger: Merging 1 sorted segments
17/04/24 22:35:39 INFO mapred.Merger: Down to the last merge-pass, with 1 segments left of total size: 703 bytes
17/04/24 22:35:39 INFO reduce.MergeManagerImpl: Merged 1 segments, 716 bytes to disk to satisfy reduce memory limit
17/04/24 22:35:39 INFO reduce.MergeManagerImpl: Merging 1 files, 720 bytes from disk
17/04/24 22:35:39 INFO reduce.MergeManagerImpl: Merging 0 segments, 0 bytes from memory into reduce
17/04/24 22:35:39 INFO mapred.Merger: Merging 1 sorted segments
17/04/24 22:35:39 INFO mapred.Merger: Down to the last merge-pass, with 1 segments left of total size: 703 bytes
17/04/24 22:35:39 INFO mapred.LocalJobRunner: 1 / 1 copied.
17/04/24 22:35:39 INFO Configuration.deprecation: mapred.skip.on is deprecated. Instead, use mapreduce.job.skiprecords
17/04/24 22:35:39 INFO mapreduce.Job: Job job_local1723100134_0001 running in uber mode : false
17/04/24 22:35:39 INFO mapreduce.Job:  map 100% reduce 0%
17/04/24 22:35:40 INFO mapred.Task: Task:attempt_local1723100134_0001_r_000000_0 is done. And is in the process of committing
17/04/24 22:35:40 INFO mapred.LocalJobRunner: 1 / 1 copied.
17/04/24 22:35:40 INFO mapred.Task: Task attempt_local1723100134_0001_r_000000_0 is allowed to commit now
17/04/24 22:35:40 INFO output.FileOutputCommitter: Saved output of task 'attempt_local1723100134_0001_r_000000_0' to hdfs://localhost:54310/op4/_temporary/0/task_local1723100134_0001_r_000000
17/04/24 22:35:40 INFO mapred.LocalJobRunner: reduce > reduce
17/04/24 22:35:40 INFO mapred.Task: Task 'attempt_local1723100134_0001_r_000000_0' done.
17/04/24 22:35:40 INFO mapred.LocalJobRunner: Finishing task: attempt_local1723100134_0001_r_000000_0
17/04/24 22:35:40 INFO mapred.LocalJobRunner: reduce task executor complete.
17/04/24 22:35:40 INFO mapreduce.Job:  map 100% reduce 100%
17/04/24 22:35:40 INFO mapreduce.Job: Job job_local1723100134_0001 completed successfully
17/04/24 22:35:41 INFO mapreduce.Job: Counters: 38
	File System Counters
		FILE: Number of bytes read=17876
		FILE: Number of bytes written=519512
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=18920
		HDFS: Number of bytes written=688
		HDFS: Number of read operations=13
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=4
	Map-Reduce Framework
		Map input records=354
		Map output records=354
		Map output bytes=5310
		Map output materialized bytes=720
		Input split bytes=101
		Combine input records=354
		Combine output records=42
		Reduce input groups=42
		Reduce shuffle bytes=720
		Reduce input records=42
		Reduce output records=42
		Spilled Records=84
		Shuffled Maps =1
		Failed Shuffles=0
		Merged Map outputs=1
		GC time elapsed (ms)=95
		CPU time spent (ms)=0
		Physical memory (bytes) snapshot=0
		Virtual memory (bytes) snapshot=0
		Total committed heap usage (bytes)=865075200
	Shuffle Errors
		BAD_ID=0
		CONNECTION=0
		IO_ERROR=0
		WRONG_LENGTH=0
		WRONG_MAP=0
		WRONG_REDUCE=0
	File Input Format Counters 
		Bytes Read=9460
	File Output Format Counters 
		Bytes Written=688
