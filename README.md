knn 算法

使用指南：
1. 打包源码；
2. 运行命令：
hadoop jar /opt/knn1.0.jar knn.KnnDriver -i train -t test/test.csv -o output_train73m -fs node101:8020 -rm node101:8032 -knnk 5 -reducernum 2 -column 785 -delimiter ,

命令解释：
Usage:
-i input 	 input train data path.
-t test 	 test file data path(only support one single file)
-o output 	 output data path.
-fs filesystem 	 namenode and port <namenode:port>
-rm resourcemanager 	 resourcemanager and port <resourcemanager:port>
-knnk knn_k 	 knn method k ,default is 5
-reducernum reducer number,default is 1
-column column train data column, default is 6 .
-delimiter  data delimiter , default is comma  .