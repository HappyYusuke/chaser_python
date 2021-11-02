# chaser_python

## 概　要  

　　chaser19をpython化したもの<dr>  

## 作成者  
　　堀井天満（金沢工業大学 工学部 ロボティクス学科 出村研究室）<dr>  

## 環　境<dr>  
　　Xubuntu18.04 <dr>  
  
## ビルド </l1>  
　　$ cd ~/catkin_ws <dr>  
　　$ catkin build chaser_python<dr>      
　　$ sudo chmod +x 〜/catkin_ws/src/chaser_python/scripts/chaser_python.py<dr>    
## 実　行 <dr>  

　(1)　インターフェースの起動 <dr>  
　　$ roslaunch turtlebot_bringup minimal.launch <dr>  
　　$ roslaunch turtlebot_bringup 3dsensor.launch <dr>  

　(2)　起動topic送信 <dr>  
　　$ rostopic pub /follow_human std_msgs/String start <dr>  

　(4)　追従プログラムの起動 <dr>  
　　$ rosrun chaser_python chaser_python.py <dr>  
# chaser_python
