#how to use rosserial
作用：提供一种方法，可以让机器发布一个ros的topic 通过TCP/USART两种方式传输数据
可实现数据传输，可视化，远程打印。

#Server: PC端
start server: roslaunch rosserial_python serial_node.py tcp 

rostopic list //查看发布的topic
rostopic echo <topic_name> //监听该topic发布的信息



#client: 扫地机端
1.将ros_lib添加到所需要的工程当中
2.cmake_list添加相应的头文件路径
3.参考examples/helloROS 使用rosserial 
4.include <ros.h>

注意事项：
1.rosserial单次传输 最大不超过 512byte.

更多资料：
1.ros wiki
