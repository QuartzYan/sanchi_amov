# sanchi_amov

## 1.安装依赖
```bash
sudo apt-get install ros-[your ros version]-rviz-imu-plugin
```

## 2.下载，编译
```bash
# git clone pkg tou you workspace
catkin_make
```

## 3.启动
```bash
# 根据IMU的型号启动对应的launch文件
roslaunch sanchi_amov imu_100D2.launch # 100D2运行此条命令
roslaunch sanchi_amov imu_100S.launch  # 100S运行此条命令
roslaunch sanchi_amov imu_200A.launch  # 200A运行此条命令
roslaunch sanchi_amov imu_200S.launch  # 200S运行此条命令
roslaunch sanchi_amov imu_300A.launch  # 300A运行此条命令
```

## 4.测试数据
```bash
rostopic echo /imu/data
```

## 5.可视化
```bash
roslaunch sanchi_amov rviz.launch
```