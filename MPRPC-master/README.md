# MPRPC
集群分布式网络通信框架，基于protobuf、muduo库开发

进入build文件夹，按照HowToUse.md中的步骤生成可执行文件，或者直接运行autobuild.sh（已加上可执行权限）执行来生成可执行文件。

成功生成后进入bin目录，先启动服务器再启动客户端即可测试


docker run -it -d --name dev_01 --privileged=true -v D:/docker_project:/song ubuntu_cpp:v1

docker run -d -e TZ="Asia/Shanghai" -p 21810:2181 -v D:\docker_project\local_zk\data:/data -v D:\docker_project\local_zk\datalog:/datalog -v D:\docker_project\local_zk\conf:/conf --name local-zookeeper zookeeper:3.4.10