---
layout: post
title: Visual-Inertial Navigation System
author: [Richard Kuo]
category: [Lecture]
tags: [jekyll, ai]
---

Introduction to Datasets VIO, OpenVINS, VINS-Mono, VINS-Fusion, cm-Level GPS positioning, and (EuRoC-MAV, TUM Visual-Inertial Dataset, UZH-FPV Drone Racing Dataset, KAIST Urban Dataset, KAIST VIO Dataset, KITTI Vision Benchmark suite, Visual Odometry / SLAM Evaluation).

---
## [Visual-Inertial odometry (VIO)](https://www.ifi.uzh.ch/en/rpg/research/research_vo.html)
Visual-Inertial odometry (VIO) is the process of estimating the state (pose and velocity) of an agent (e.g., an aerial robot) by using only the input of one or more cameras plus one or more Inertial Measurement Units (IMUs) attached to it. 

**[Visual-Inertial Odometry of Aerial Robots](https://arxiv.org/pdf/1906.03289.pdf)**<br>
![](https://www.ifi.uzh.ch/ifi/dam/jcr:f42530e2-1c13-41b0-a7cf-2a48191ee72f/Encyclopedia19VIO_Scaramuzza.2019-06-07-21-33-10.png)

---
### [Fisher Information Field for Active Visual Localization](https://www.ifi.uzh.ch/dam/jcr:5a26a3b4-ce01-4647-8cf6-f6a24e579a85/ICRA19_Zhang.pdf)
<iframe width="826" height="465" src="https://www.youtube.com/embed/q3YqIyaFUVE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

---
### [A Tutorial on Quantitative Trajectory Evaluation for Visual(-Inertial) Odometry](https://www.ifi.uzh.ch/dam/jcr:89d3db14-37b1-431d-94c3-8be9f37466d3/IROS18_Zhang.pdf)
  - [PPT](https://www.ifi.uzh.ch/dam/jcr:fd6089ce-2414-4a4f-98ca-8a48ad318990/IROS18_Zhang.pptx)
  - [VO/VIO Evaluation Toolbox](https://github.com/uzh-rpg/rpg_trajectory_evaluation)

---
### On the Comparison of Gauge Freedom Handling in Optimization-based Visual-Inertial State Estimation
* [On the Comparison of Gauge Freedom Handling in Optimization-based Visual-Inertial State Estimation](https://www.ifi.uzh.ch/dam/jcr:3ef325f5-aa80-44e1-9d37-1ab7218ff922/RAL18_Zhang.pdf)
  - [PPT](https://www.ifi.uzh.ch/dam/jcr:f77ffa5e-3496-4b7e-97df-1ff7bb572fd1/RAL18_Zhang.pptx)
  - [Code](https://github.com/uzh-rpg/rpg_vi_cov_transformation)

---
### [Active Exposure Control for Robust Visual Odometry in High Dynamic Range (HDR) Environments](https://www.ifi.uzh.ch/dam/jcr:cc5c71f1-3491-4c7e-9490-bb16278aa75e/ICRA17_Zhang_updated.pdf)
<iframe width="826" height="465" src="https://www.youtube.com/embed/TKJ8vknIXbM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

---
### SVO 2.0 Semi-Direct Visual Odometry
[SVO 2.0: Semi-Direct Visual Odometry for Monocular and Multi-Camera Systems](https://rpg.ifi.uzh.ch/docs/TRO17_Forster-SVO.pdf)
<iframe width="826" height="465" src="https://www.youtube.com/embed/hR8uq1RTUfA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
**[SVO Pro](https://github.com/uzh-rpg/rpg_svo_pro_open)**<br>
![](https://github.com/uzh-rpg/rpg_svo_pro_open/raw/master/doc/images/v102_gm.gif)

---
### 1-point RANSAC
Given a car equipped with an omnidirectional camera, the motion of the vehicle can be purely recovered from salient features tracked over time. We propose the 1-Point RANSAC algorithm which runs at 800 Hz on a normal laptop. 
![](https://www.ifi.uzh.ch/dam/jcr:46cb5ecd-4a84-4c5a-8ef0-dd7709bf32b2/teaser_1.2017-01-05-22-40-09.gif)
<iframe width="826" height="620" src="https://www.youtube.com/embed/t7uKWZtUjCE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

---
### [Visual-Inertial Odometry Benchmarking](https://www.ifi.uzh.ch/ifi/rpg/docs/ICRA18_Delmerico.pdf)
<iframe width="826" height="465" src="https://www.youtube.com/embed/ymI3FmwU9AY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

---
### ROVIO
[Iterated extended Kalman filter based visual-inertial odometry using direct photometric feedback](https://www.research-collection.ethz.ch/bitstream/handle/20.500.11850/263423/ROVIO.pdf?sequence=1&isAllowed=y)<br>
![](https://d3i71xaburhd42.cloudfront.net/6b8ac6a81515f023f45e7f2ffa6a18177682d8be/7-Figure3-1.png)

---
### OKVIS 
**Paper:** [OKVIS: Keyframe-Based Visual-Inertial SLAM using Nonlinear Optimization](http://www.roboticsproceedings.org/rss09/p37.pdf)<br>
**Github:** [https://github.com/ethz-asl/okvis_ros](https://github.com/ethz-asl/okvis_ros)<br>
<iframe width="1004" height="565" src="https://www.youtube.com/embed/TbKEPA2_-m4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

---
### [OpenINVS](https://github.com/rpng/open_vins)
**paper:** [OpenVINS: A Research Platform for Visual-Inertial Estimation](http://udel.edu/~pgeneva/downloads/papers/c10.pdf)<br>
The core filter is an [Extended Kalman filter](https://en.wikipedia.org/wiki/Extended_Kalman_filter) which fuses inertial information
 with sparse visual feature tracks. These visual feature tracks are fused leveraging the [Multi-State Constraint Kalman Filter (MSCKF)](https://www-users.cse.umn.edu/~stergios/papers/ICRA07-MSCKF.pdf) sliding window formulation which allows for 3D features to update the state estimate without directly estimating the feature states in the filter. 

* [Documentation](https://docs.openvins.com/)<br>
* [Getting started guide](https://docs.openvins.com/getting-started.html)
 
* [Publications](https://sites.udel.edu/robot/publications/)

  - [MIMC-VINS: A Versatile and Resilient Multi-IMU Multi-Camera Visual-Inertial Navigation System](https://arxiv.org/abs/2006.15699)<br>
  <iframe width="789" height="444" src="https://www.youtube.com/embed/my1IjdJ4irY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

  - [Multi-IMU VIO: Sensor-Failure-Resilient Multi-IMU Visual-Inertial Navigation](https://udel.edu/~pgeneva/downloads/papers/c06.pdf)<br>
  <iframe width="789" height="444" src="https://www.youtube.com/embed/TqbzqLgnIZc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

--- 
### [VINS-Mobile](https://github.com/HKUST-Aerial-Robotics/VINS-Mobile)
[The Integration of GPS/BDS Real-Time Kinematic Positioning and Visual–Inertial Odometry Based on Smartphones](https://mdpi-res.com/d_attachment/ijgi/ijgi-10-00699/article_deploy/ijgi-10-00699-v2.pdf)
<iframe width="826" height="465" src="https://www.youtube.com/embed/0mTXnIfFisI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

---
### [VINS-Mono](https://github.com/HKUST-Aerial-Robotics/VINS-Mono)
[VINS-Mono: A Robust and Versatile Monocular Visual-Inertial State Estimator](https://arxiv.org/pdf/1708.03852.pdf)<br>
<iframe width="863" height="411" src="https://www.youtube.com/embed/eINyJHB34uU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<iframe width="347" height="206" src="https://www.youtube.com/embed/mv_9snb_bKs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<iframe width="347" height="206" src="https://www.youtube.com/embed/g_wN0Nt0VAU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<iframe width="347" height="206" src="https://www.youtube.com/embed/I4txdvGhT6I" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
![](https://www.researchgate.net/publication/355247417/figure/fig2/AS:1079250023133186@1634324665587/The-framework-of-VINS-mono.png)

---
[VINS-Mono代碼解析——狀態估計器流程](https://www.cxymm.net/article/qq_43247439/107312670)<br>

![](https://img-blog.csdnimg.cn/20190222143043441.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQxODM5MjIy,size_16,color_FFFFFF,t_70)

**vins_estimator**<br>
* factor：
  - imu_factor.h：IMU残差、雅可比
  - intergration_base.h：IMU预积分
  - marginalization.cpp/.h：边缘化
  - pose_local_parameterization.cpp/.h：局部参数化
  - projection_factor.cpp/.h：视觉残差
* initial：
  - initial_alignment.cpp/.h：视觉和IMU校准(陀螺仪偏置、尺度、重力加速度和速度)
  - initial_ex_rotation.cpp/.h：相机和IMU外参标定
  - initial_sfm.cpp/.h：纯视觉SFM、三角化、PNP
  - solve_5pts.cpp/.h：5点法求基本矩阵得到Rt
* utility：
  - CameraPoseVisualization.cpp/.h：相机位姿可视化
  - tic_toc.h：记录时间
  - utility.cpp/.h：各种四元数、矩阵转换
  - visualization.cpp/.h：各种数据发布
  - estimator.cpp/.h：紧耦合的VIO状态估计器实现
  - estimator_node.cpp：ROS 节点函数，回调函数
  - feature_manager.cpp/.h：特征点管理，三角化，关键帧等
  - parameters.cpp/.h：读取参数
  
---
### [VINS-Fusion](https://github.com/HKUST-Aerial-Robotics/VINS-Fusion)
[A General Optimization-based Framework for Local Odometry Estimation with Multiple Sensors](https://arxiv.org/pdf/1901.03638.pdf)

**[Code](https://github.com/rkuo2000/VINS-Fusion)**<br>

**VI-Car**<br>
![](https://github.com/HKUST-Aerial-Robotics/VINS-Fusion/raw/master/support_files/image/car_gif.gif)

**EuRoC-MAV**<br>
![](https://github.com/HKUST-Aerial-Robotics/VINS-Fusion/raw/master/support_files/image/euroc.gif)
  
**KITTI**<br>
![](https://github.com/HKUST-Aerial-Robotics/VINS-Fusion/raw/master/support_files/image/kitti.gif)
* KITTI Odometry (Stereo)
  - Download [KITTI Odometry dataset](http://www.cvlibs.net/datasets/kitti/eval_odometry.php) to YOUR_DATASET_FOLDER. 
  - `roslaunch vins vins_rviz.launch`
  - (optional) `rosrun loop_fusion loop_fusion_node ~/catkin_ws/src/VINS-Fusion/config/kitti_odom/kitti_config00-02.yaml`
  - `rosrun vins kitti_odom_test ~/catkin_ws/src/VINS-Fusion/config/kitti_odom/kitti_config00-02.yaml YOUR_DATASET_FOLDER/sequences/00/`

* KITTI GPS Fusion (Stereo + GPS)
  - Download [KITTI raw dataset](http://www.cvlibs.net/datasets/kitti/raw_data.php) to YOUR_DATASET_FOLDER. 
 Take [2011_10_03_drive_0027_synced](https://s3.eu-central-1.amazonaws.com/avg-kitti/raw_data/2011_10_03_drive_0027/2011_10_03_drive_0027_sync.zip) for example.
  - `roslaunch vins vins_rviz.launch`
  - `rosrun vins kitti_gps_test ~/catkin_ws/src/VINS-Fusion/config/kitti_raw/kitti_10_03_config.yaml YOUR_DATASET_FOLDER/2011_10_03_drive_0027_sync/`
  - `rosrun global_fusion global_fusion_node`
  
* [Recalibrating the KITTI Dataset Camera Setup for Improved Odometry Accuracy](https://arxiv.org/pdf/2109.03462.pdf)
  ![](https://xuwuzhou.top/images/%E8%AE%BA%E6%96%8752%E5%9B%BE%E7%89%873.png) 
 
---
### VINS-Fusion 代碼解析
* [VINS Fusion 笔记](https://scm_mos.gitlab.io/slam/VINS-FUSION/)

* [浅谈VINS中的global fusion节点](https://zhuanlan.zhihu.com/p/75492883)

* [VINS 论文推导及代码解析（一）](https://mp.weixin.qq.com/s/opInITC_BDWz12j1_nUseA)
* [VINS 论文推导及代码解析（二）](https://mp.weixin.qq.com/s/9twYJMOE8oydAzqND0UmFw)
* [VINS 论文推导及代码解析（三）](https://mp.weixin.qq.com/s/xumEhRziRCpnAW36Utuo4A)
* [VINS 论文推导及代码解析（四）](https://mp.weixin.qq.com/s/edAwdBxV-j2bgfpnxxQSzA)

---
### Improved VINS-Mono
[Robust Visual-Inertial Navigation System for Low Precision Sensors under Indoor and Outdoor Environments](https://www.researchgate.net/publication/349465261_Robust_Visual-Inertial_Navigation_System_for_Low_Precision_Sensors_under_Indoor_and_Outdoor_Environments)
![](https://www.researchgate.net/publication/349465261/figure/fig1/AS:993333975474176@1613840683010/The-improved-visual-inertial-navigation-system-VINS-mono-system-architecture-framework.png)

---
### [PL-VIO](https://github.com/HeYijia/PL-VIO)
[PL-VIO: Tightly-Coupled Monocular Visual–Inertial Odometry Using Point and Line Features](https://www.semanticscholar.org/paper/PL-VIO%3A-Tightly-Coupled-Monocular-Visual%E2%80%93Inertial-He-Zhao/6356897ee4a51a1f9de04a8ab959afd97af7f63e)
<table>
<tr>
<td><img src="https://d3i71xaburhd42.cloudfront.net/6356897ee4a51a1f9de04a8ab959afd97af7f63e/4-Figure1-1.png"></td>
<td><img src="https://d3i71xaburhd42.cloudfront.net/6356897ee4a51a1f9de04a8ab959afd97af7f63e/6-Figure2-1.png"></td>
</tr>
</table>
![](https://github.com/rkuo2000/Robotics/blob/main/images/PL-VIO_benchmark.png?raw=true)
**Code:** [HeYijia/PL-VIO](https://github.com/HeYijia/PL-VIO)<br>
![](https://github.com/HeYijia/PL-VIO/raw/master/doc/image/plvio.gif)

---
### PL-VINS
[PL-VINS: Real-Time Monocular Visual-Inertial SLAM with Point and Line Features](https://arxiv.org/abs/2009.07462)<br>
<iframe width="740" height="416" src="https://www.youtube.com/embed/MPf6HufbgdE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
![](https://d3i71xaburhd42.cloudfront.net/148eebf5cddccf37891074d118945de0df2328a7/1-Figure1-1.png)
![](https://d3i71xaburhd42.cloudfront.net/148eebf5cddccf37891074d118945de0df2328a7/3-Figure2-1.png)
*The Blue rectangles represent the differences from VINS-Mono*<br>
![](https://github.com/rkuo2000/Robotics/blob/main/images/PL-VINS_benchmark.png?raw=true)
**[Code](https://github.com/rkuo2000/PL-VINS)**<br>
![](https://github.com/cnqiangfu/PL-VINS/raw/master/support_files/plvins-vinsmono.png)
<span style="color: red">*The build took ~37 hours on i7-920 @2.67GHz !!!*</span><br>
**MH_01_easy**<br>
![](https://github.com/rkuo2000/Robotics/blob/main/images/PL-VINS_MH_01_easy.png?raw=true)
**MH_05_difficult**<br>
![](https://github.com/rkuo2000/Robotics/blob/main/images/PL-VINS_MH_05_difficult.png?raw=true)

---
### IPL-VIO
[Improved Point–Line Visual–Inertial Odometry System Using Helmert Variance Component Estimation](https://www.mdpi.com/2072-4292/12/18/2901/htm)
![](https://www.mdpi.com/remotesensing/remotesensing-12-02901/article_deploy/html/images/remotesensing-12-02901-g001.png)
![](https://www.mdpi.com/remotesensing/remotesensing-12-02901/article_deploy/html/images/remotesensing-12-02901-g006a.png)
![](https://www.mdpi.com/remotesensing/remotesensing-12-02901/article_deploy/html/images/remotesensing-12-02901-g006b.png)
Figure 6 Comparision of the matching effect between line binary descriptors(LBD) matching method and improved mathcing method on the MH_02_easy dataset.
Images(a,b) are LBD descriptor matching scenes - the line of the same color is the corresponding matching line; (c,d) are the matching scenes of the improved matching method, and the line of the same color is the corresponding matching line.
![](https://github.com/rkuo2000/Robotics/blob/main/images/IPL-VIO_benchmark.png?raw=true)

---
### PLS-VIO
[Leveraging Structural Information to Improve Point Line Visual-Inertial Odometry](https://arxiv.org/pdf/2105.04064.pdf)
![](https://ai2-s2-public.s3.amazonaws.com/figures/2017-08-08/b770639b633bb6469a13805ea28ba6626dc682ce/1-Figure1-1.png)
![](https://github.com/rkuo2000/Robotics/blob/main/images/PLS-VIO_benchmark.png?raw=true)
**[Code](https://github.com/rkuo2000/Structural-and-Non-structural-line)**<br>
![](https://github.com/rkuo2000/Structural-and-Non-structural-line/raw/master/bin/demo/simulate_line.gif)

---
### RK-VIF
[An improved SLAM based on RK-VIF: Vision and inertial information fusion via Runge-Kutta method](https://www.sciencedirect.com/science/article/pii/S2214914721001938)

1. Visual-inertial information fusion framework
  ![](https://ars.els-cdn.com/content/image/1-s2.0-S2214914721001938-gr1.jpg)

2. The process of PROSAC algorithm<br>
  The [PROSAC](https://www.researchgate.net/publication/327114888_An_efficient_RANSAC_hypothesis_evaluation_using_sufficient_statistics_for_RGB-D_pose_estimation) is based on the assumption that “the points with good quality are more likely to be interior points”.<br>
  ![](https://ars.els-cdn.com/content/image/1-s2.0-S2214914721001938-gr2.jpg)

3. This paper uses the Runge-Kutta method to discretize the IMU motion formula to improve the pre-integration accuracy. The basic idea of the Runge-Kutta method is to estimate the derivatives of multiple points in the integration interval, take the weighted average of these derivatives to obtain the average derivative, and then use the average derivative to estimate the result at the end of the integration interval. 
  The formula of the fourth-order Runge-Kutta algorithm is as follows:
  ![](https://github.com/rkuo2000/Robotics/blob/main/images/Runge-Kutta_algorithm_formula.png?raw=true) 
  
4. Sensor frequency
  ![](https://ars.els-cdn.com/content/image/1-s2.0-S2214914721001938-gr3.jpg)

5. VINS state and constraints
  ![](https://ars.els-cdn.com/content/image/1-s2.0-S2214914721001938-gr4.jpg)

6. Sliding window optimization range
  ![](https://ars.els-cdn.com/content/image/1-s2.0-S2214914721001938-gr5.jpg)

7. Loop detection process
  ![](https://ars.els-cdn.com/content/image/1-s2.0-S2214914721001938-gr6.jpg)
  After the system successfully detects the loop, it can establish the constraint relationship between the two frames through feature matching. Firstly, we need to fuse the map points matched by the loop and eliminate redundant map points. Then calculate the relative pose between the two keyframes according to Perspective-N-Point (PnP) algorithm, and correct the current keyframe's pose. In addition, other keyframes in the loop also have different degrees of accumulated error and need to be globally optimized.

8. Globally optimized pose
  ![](https://ars.els-cdn.com/content/image/1-s2.0-S2214914721001938-gr7.jpg)

9. Dataset experiment
  ![](https://ars.els-cdn.com/content/image/1-s2.0-S2214914721001938-gr9.jpg)

The RMSE in EuRoC Dataset (unit: m)
![](https://github.com/rkuo2000/Robotics/blob/main/images/RK-VIF_benchmark.png?raw=true)

--- 
## GPS-VIO

### [The Integration of GPS-BDS Real-Time Kinematic Positioning and Visual–Inertial Odometry Based on Smartphones]
**Paper:** (https://www.mdpi.com/2220-9964/10/10/699/pdf)

---
### Tightly-coupled Fusion of Global Positional Measurements in Optimization-based Visual-Inertial Odometry
**Paper:** [https://arxiv.org/abs/2003.04159](https://arxiv.org/abs/2003.04159)<br>
<table>
<tr>
<td><img src="https://d3i71xaburhd42.cloudfront.net/8a83dbab2609a1d204cf431fa4b93aa2b4148e8d/1-Figure1-1.png"></td>
<td><img src="https://d3i71xaburhd42.cloudfront.net/8a83dbab2609a1d204cf431fa4b93aa2b4148e8d/2-Figure2-1.png"></td>
</tr>
</table>
![](https://d3i71xaburhd42.cloudfront.net/8a83dbab2609a1d204cf431fa4b93aa2b4148e8d/6-Figure4-1.png)

---
### GVINS
**Paper:** [GVINS: Tightly Coupled GNSS-Visual-Inertial Fusion for Smooth and Consistent State Estimation](https://arxiv.org/abs/2103.07899)<br>

---
### Tightly Coupled Optimization-based GPS-Visual-Inertial Odometry with Online Calibration and Initialization
**Paper:** [https://arxiv.org/abs/2203.02677](https://arxiv.org/abs/2203.02677)<br>
<table>
<tr>
<td><img src="https://ai2-s2-public.s3.amazonaws.com/figures/2017-08-08/b76f11bfab2e84e42f4d4921eed35af76687e40b/1-Figure1-1.png"></td>
<td><img src="https://ai2-s2-public.s3.amazonaws.com/figures/2017-08-08/b76f11bfab2e84e42f4d4921eed35af76687e40b/3-Figure3-1.png"></td>
</tr>
</table>

---
### EMA-VIO: Deep Visual-Inertial Odometry with External Memory Attention
**Paper:** [https://arxiv.org/abs/2209.08490](https://arxiv.org/abs/2209.08490)<br>

---
### Benchmarking VI Deep Multimodal Fusion
**Paper:** [ttps://arxiv.org/abs/2208.00919](https://arxiv.org/abs/2208.00919)<br>

---
### EMV-LIO: An Efficient Multiple Vision aided LiDAR-Inertial Odometry
**Paper:** [https://arxiv.org/abs/2302.00216](https://arxiv.org/abs/2302.00216)<br>

---
## [Datasets](https://docs.openvins.com/gs-datasets.html)

### [EuRoC MAV Dataset](https://projects.asl.ethz.ch/datasets/doku.php?id=kmavvisualinertialdatasets)
The ETH ASL EuRoC MAV dataset is one of the most used datasets in the visual-inertial / simultaneous localization and mapping (SLAM) research literature. 
<table>
<tr>
<td><img src="https://projects.asl.ethz.ch/datasets/lib/exe/fetch.php?w=230&tok=f969d3&media=overview_ml.jpg"></td>
<td><img src="https://projects.asl.ethz.ch/datasets/lib/exe/fetch.php?w=320&tok=2b9d8d&media=vicon_pointcloud_training_crop.png"></td>
</tr>
</table>
**Platform and Sensors**<br>
![](https://projects.asl.ethz.ch/datasets/lib/exe/fetch.php?w=400&tok=1dbdef&media=platform.jpg)
![](https://projects.asl.ethz.ch/datasets/lib/exe/fetch.php?w=210&tok=3d9fd6&media=front_side_gray.jpg)

---
### [KITTI Vision Benchmark Suite](http://www.cvlibs.net/datasets/kitti/)
![](http://www.cvlibs.net/datasets/kitti/images/passat_sensors.jpg)
<iframe width="920" height="520" src="https://www.youtube.com/embed/KXpZ6B1YB_k" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

  
<br>
<br>

*This site was last updated {{ site.time | date: "%B %d, %Y" }}.*
