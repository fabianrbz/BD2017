## Teragen
  * time hadoop jar ${HADOOP_HOME}/libexec/share/hadoop/mapreduce/hadoop-mapreduce-examples-2.8.0.jar teragen -Dmapreduce.job.maps=6 -Ddfs.blocksize=16m 50000000 /fabianrbz/terasort-input
  * 68.88s user 7.85s system 111% cpu 1:08.60 total

## Terasort
  * time hadoop jar ${HADOOP_HOME}/libexec/share/hadoop/mapreduce/hadoop-mapreduce-examples-2.8.0.jar  terasort /fabianrbz/terasort-input /fabianrbz/terasort-output
  * 349.48s user 143.44s system 85% cpu 9:38.08 total
