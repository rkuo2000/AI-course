---
layout: post # 指定文章佈局，通常是 post
title: RL Gym for Robot
date: 2025-09-12 10:00:00 +0800 # 發表日期和時間 (請根據您當前的時區調整 +0800 代表 UTC+8)
categories: [Lecture] # 文章分類，您可以自訂
tags: [RL, Robotics] # 文章標籤，您可以自訂
description: Reinforcement-Learning Gym for Robot
mathjax: false # 如果這篇文章不需要顯示數學公式，請設false
comments: false # 如果這篇文章需要啟用評論，請設為 true

---
## Gym-Gazebo
**Code:** [erlerobot/gym-gazebo](https://github.com/erlerobot/gym-gazebo)<br>
<table>
<tr>
<td><img src="https://github.com/erlerobot/gym-gazebo/raw/master/imgs/GazeboCircuit2TurtlebotLidar-v0.png"></td>
<td><img src="https://github.com/erlerobot/gym-gazebo/raw/master/imgs/cartpole.jpg"></td>
<td><img src="https://github.com/erlerobot/gym-gazebo/raw/master/imgs/GazeboModularScara3DOF-v3.png"></td>
</tr>
</table>

---
## DART (Dynamic Animation and Robotics Toolkit)

### [Dartsim/dart](https://github.com/dartsim/dart)
* Python bindings: dartpy, pydart2 (deprecated)
* OpenAI Gym with DART support: gym-dart (dartpy based), DartEnv (pydart2 based, deprecated)

<iframe width="742" height="417" src="https://www.youtube.com/embed/Ve_MRMTvGX8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

---
## [PyBullet-Gym](https://github.com/benelot/pybullet-gym)
[PyBullet Quickstart Guide](https://docs.google.com/document/d/10sXEhzFRSnvFcl3XxNGhnD4N2SedqwdAvK3dsihxVUA/edit#heading=h.2ye70wns7io3)<br>

**code:** [rkuo2000/pybullet-gym](https://github.com/rkuo2000/pybullet-gym)<br>
* installation
```
pip install gym
pip install stable-baselines3
git clone https://github.com/rkuo2000/pybullet-gym
export PYTHONPATH=$PATH:/home/yourname/pybullet-gym
```

**Train**<br>
`python train.py Ant 10000000`<br>

**Enjoy** with trained-model<br>
`python enjoy.py Ant`<br>

**Enjoy** with pretrained weights<br>
`python enjoy_Ant.py`<br>
`python enjoy_HumanoidFlagrunHarder.py` (a copy from pybulletgym/examples/roboschool-weights/enjoy_TF_*.py)<br>

---
### [PyBullet-Robots](https://github.com/erwincoumans/pybullet_robots)
<img width="50%" height="50%" src="https://raw.githubusercontent.com/erwincoumans/pybullet_robots/master/images/collection.png">

**env_name = "AtlasPyBulletEnv-v0"**<br>
[atlas_v4_with_multisense.urdf](https://github.com/benelot/pybullet-gym/blob/master/pybulletgym/envs/assets/robots/atlas/atlas_description/atlas_v4_with_multisense.urdf)<br>
<iframe width="580" height="435" src="https://www.youtube.com/embed/aqAk701ylIk" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

---
### OP3 Soccer
**Paper:** [Learning Agile Soccer Skills for a Bipedal Robot with Deep Reinforcement Learning](https://arxiv.org/abs/2304.13653)<br>
<iframe width="932" height="524" src="https://www.youtube.com/embed/X0Zi_T9o2_0" title="OP3 Soccer: overview" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---
## RoboCar Gym

### Pybullet-RoboCar
**Blog:** <br>
[Creating OpenAI Gym Environments with PyBullet (Part 1)](https://gerardmaggiolino.medium.com/creating-openai-gym-environments-with-pybullet-part-1-13895a622b24)<br>
[Creating OpenAI Gym Environments with PyBullet (Part 2)](https://gerardmaggiolino.medium.com/creating-openai-gym-environments-with-pybullet-part-2-a1441b9a4d8e)<br>
![](https://media0.giphy.com/media/VI3OuvQShK3gzENiVz/giphy.gif?cid=790b761131bda06b74fcd9bb06c6a43939cf446edf403a68&rid=giphy.gif&ct=g)

---
## Quadruped Gym

### [Motion Imitation](https://github.com/google-research/motion_imitation)
**Code:** [TF 1.15](https://github.com/google-research/motion_imitation)<br>
<iframe width="784" height="441" src="https://www.youtube.com/embed/NPvuap-SD78" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
**Code:** [PyTorch](https://github.com/newera-001/motor-system)<br>
For Training:<br>
`python motion_imitation/run_torch.py --mode train --motion_file 'dog_pace.txt|dog_spin.txt' \
--int_save_freq 10000000 --visualize --num_envs 50 --type_name 'dog_pace'`<br>
For Testing:<br>
`python motion_imitation/run_torch.py --mode test --motion_file 'dog_pace.txt' --model_file 'file_path' \ 
--encoder_file 'file_path' --visualize`<br>

---
### Rex: an open-source quadruped robot
**Code:** [nicrusso7/rex-gym](https://github.com/nicrusso7/rex-gym)<br>
![](https://github.com/nicrusso7/rex-gym/blob/master/images/intro.gif?raw=true)

---
## Drones Gym

### [PyBullet-Gym for Drones](https://github.com/utiasDSL/gym-pybullet-drones)
![](https://github.com/utiasDSL/gym-pybullet-drones/blob/master/files/readme_images/helix.gif?raw=true)
![](https://github.com/utiasDSL/gym-pybullet-drones/blob/master/files/readme_images/helix.png?raw=true)

* Installation
```
sudo apt install ffmpeg
pip install numpy pillow matplotlib cycler
pip install gym pybullet stable_baselines3 ray[rllib]
git clone https://github.com/rkuo2000/gym-pybullet-drones.git
cd gym-pybullet-drones
```

* Train & Enjoy<br>
`python train.py` # modify train.py for different env, algorithm and timesteps<br>
`python enjoy.py` # modify enjoy.py for different env<br>

* Fly using [DSLPIDControl.py](https://github.com/utiasDSL/gym-pybullet-drones/blob/master/gym_pybullet_drones/control/DSLPIDControl.py):（PID飛行）<br>
`python examples/fly.py --num_drones 1`<br>
![](https://github.com/utiasDSL/gym-pybullet-drones/blob/master/files/readme_images/wp.gif?raw=true)

* To learn take-off:（起飛）  <br>
`python examples/learn.py`<br>
![](https://github.com/utiasDSL/gym-pybullet-drones/blob/master/files/readme_images/learn2.gif?raw=true)

* `compare.py` which replays and compare to a trace saved in `files/example_trace.pkl`

**Experiments**<br>
`cd experiments/learning`<br>

env : hover, takeoff, flythrugate, tune（旋停, 起飛, 穿越, 調整）<br>
algo: a2c, ppo, sac, td3, ddpg<br>

* To learn hover:（旋停）<br>
`python singleagent.py --env hover --algo a2c`<br>

To visualize the best trained agent:<br>
`python test_singleagent.py --exp ./results/save-hover-a2c`<br>

For multi-agent RL, using rllib:<br>
`python multiagent.py --num_drones 3 --env hover --algo a2c --num_workers 2`<br>

---
### [Flightmare](https://github.com/uzh-rpg/flightmare)
Flightmare is a flexible modular quadrotor simulator. 
<iframe width="768" height="432" src="https://www.youtube.com/embed/m9Mx1BCNGFU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<img width="50%" height="50%" src="https://github.com/uzh-rpg/flightmare/raw/master/docs/flightmare.png">
* [Introduction](https://github.com/uzh-rpg/flightmare/wiki/Introduction)
* [Prerequisites](https://github.com/uzh-rpg/flightmare/wiki/Prerequisites)
* [Install Python Packages](https://github.com/uzh-rpg/flightmare/wiki/Install-with-pip)
* [Install ROS](https://github.com/uzh-rpg/flightmare/wiki/Install-with-ROS)

* **running ROS**
```
roslaunch flightros rotors_gazebo.launch
```

* **flighRL**<br>
```
cd /path/to/flightmare/flightrl
pip install .
cd examples
python3 run_drone_control.py --train 1
```

---
### [AirSim](https://github.com/microsoft/AirSim)
<iframe width="768" height="448" src="https://www.youtube.com/embed/-WfTr1-OBGQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
![](https://github.com/microsoft/AirSim/blob/master/docs/images/AirSimDroneManual.gif?raw=true)

---
## Assistive Gym

**Paper:** [Assistive Gym: A Physics Simulation Framework for Assistive Robotics](https://arxiv.org/abs/1910.04700)<br>
![](https://github.com/Healthcare-Robotics/assistive-gym/blob/main/images/assistive_gym.jpg?raw=true)
<iframe width="705" height="397" src="https://www.youtube.com/embed/EFKqNKO3P60" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

* Four collaborative robots (PR2, Jaco, Baxter, Sawyer)<br>
![](https://github.com/Healthcare-Robotics/assistive-gym/raw/main/images/robot_models.gif)

* Support for the Stretch and PANDA robots<br>
<table>
<tr>
<td><img src="https://github.com/Healthcare-Robotics/assistive-gym/blob/main/images/v1_stretch.jpg?raw=true"></td>
<td><img src="https://github.com/Healthcare-Robotics/assistive-gym/blob/main/images/v1_panda.jpg?raw=true"></td>
</tr>
</table>

**Code:** [Healthcare-Robotics/assistive-gym](https://github.com/Healthcare-Robotics/assistive-gym)<br>

---
### Assistive VR Gym
**Paper:** [Assistive VR Gym: Interactions with Real People to Improve Virtual Assistive Robots](https://arxiv.org/abs/2007.04959)<br>
**Code:** [Healthcare-Robotics/assistive-vr-gym](https://github.com/Healthcare-Robotics/assistive-vr-gym)<br>
![](https://github.com/Healthcare-Robotics/assistive-vr-gym/blob/master/images/avr_gym_2.jpg?raw=true)
<iframe width="705" height="397" src="https://www.youtube.com/embed/tcyPMkAphNs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

---
## Learning Dexity
<iframe width="696" height="392" src="https://www.youtube.com/embed/jwSbzNHGflM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

---
### [Dexterous Gym](https://github.com/henrycharlesworth/dexterous-gym)
![](https://github.com/henrycharlesworth/dexterous-gym/raw/master/dexterous_gym/examples/penspin.gif)
![](https://github.com/henrycharlesworth/dexterous-gym/raw/master/dexterous_gym/examples/egghandover.gif)

---
### [DexPilot](https://research.nvidia.com/publication/2020-05_dexpilot-vision-based-teleoperation-dexterous-robotic-hand-arm-system)
**Paper:** [DexPilot: Vision Based Teleoperation of Dexterous Robotic Hand-Arm System](https://arxiv.org/abs/1910.03135)<br>
![](https://research.nvidia.com/sites/default/files/styles/wide/public/publications/dexpilot.jpg?itok=7Re04wXI)
<iframe width="883" height="497" src="https://www.youtube.com/embed/qGE-deYfb8I" title="dexpilot highlights" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

---
### [TriFinger](https://sites.google.com/view/trifinger)
<iframe width="464" height="287" src="https://www.youtube.com/embed/RxkS6dzO1dU" title="Writing" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

**Paper:** [TriFinger: An Open-Source Robot for Learning Dexterity](https://arxiv.org/abs/
2008.03596)<br>
![](https://ai2-s2-public.s3.amazonaws.com/figures/2017-08-08/f223b2a438fe20ac55300c278509bf4a13072ca8/3-Figure2-1.png)
![](https://ai2-s2-public.s3.amazonaws.com/figures/2017-08-08/f223b2a438fe20ac55300c278509bf4a13072ca8/4-Figure3-1.png)
![](https://ai2-s2-public.s3.amazonaws.com/figures/2017-08-08/f223b2a438fe20ac55300c278509bf4a13072ca8/4-Figure4-1.png)

**Code:** [TriFinger Robot Simulation](https://github.com/open-dynamic-robot-initiative/trifinger_simulation)<br>
<iframe width="736" height="410" src="https://www.youtube.com/embed/V767AGlyDOs" title="CoRL 2020, Spotlight Talk 421: TriFinger: An Open-Source Robot for Learning Dexterity" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

--- 
### [Multi-Task Reset-Free (MTRF) Learning](https://sites.google.com/view/mtrf)
**Paper:** [Reset-Free Reinforcement Learning via Multi-Task Learning: Learning Dexterous Manipulation Behaviors without Human Intervention](https://arxiv.org/abs/2104.11203)<br>
<iframe width="562" height="296" src="https://www.youtube.com/embed/64FLPhvqgrw" title="MTRF Overview: Reset-Free Reinforcement Learning via Multi-Task Learning" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

---
### Dexterous Anthropomorphic Robotic Hand
**Blog:** [Robotic hand can crush beer cans and hold eggs without breaking them](https://www.newscientist.com/article/2301641-robotic-hand-can-crush-beer-cans-and-hold-eggs-without-breaking-them/)<br>
![](https://images.newscientist.com/wp-content/uploads/2021/12/14124151/PRI_215070295.jpg?width=778)

**Paper:** [Integrated linkage-driven dexterous anthropomorphic robotic hand](https://www.nature.com/articles/s41467-021-27261-0#Abs1)<br>
![](https://media.springernature.com/lw685/springer-static/image/art%3A10.1038%2Fs41467-021-27261-0/MediaObjects/41467_2021_27261_Fig2_HTML.png?as=webp)

<iframe width="883" height="497" src="https://www.youtube.com/embed/TJzfgipEACU" title="Watch a highly dexterous robotic hand use scissors and tweezers" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

---
### Robotic Telekinesis
[Robotic Telekinesis: Learning a Robotic Hand Imitator by Watching Humans on Youtube](https://arxiv.org/abs/2202.10448)<br>
<iframe width="883" height="497" src="https://www.youtube.com/embed/fVrcBY0lOWw" title="Finally, Robotic Telekinesis is Here! 🤖" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

---
### Fixed-Finger Gripper
**Paper:** [F1 Hand: A Versatile Fixed-Finger Gripper for Delicate Teleoperation and Autonomous Grasping](https://arxiv.org/abs/2205.07066)<br>
<iframe width="884" height="497" src="https://www.youtube.com/embed/iWXXIX4Mkl8" title="F1 Hand: A Versatile Fixed-Finger Gripper for Delicate Teleoperation and Autonomous Grasping" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

---
### Learning Diverse Dexterous Grasps
**Paper:** [Learning Diverse and Physically Feasible Dexterous Grasps with Generative Model and Bilevel Optimization](https://arxiv.org/abs/2207.00195)<br>
<iframe width="883" height="497" src="https://www.youtube.com/embed/9DTrImbN99I" title="Learning Diverse & Physically Feasible Dexterous Grasps w/ Generative Model and Bilevel Optimization" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

---
### ViLa
**Blog:** [https://bangqu.com/9Fa2ra.html](https://bangqu.com/9Fa2ra.html)<br>
![](https://i3.res.bangqu.com/farm/j/news/2023/12/12/42e2981b43a54c3ac7a8647515a0ecaa.gif)

---
### [Mobile ALOHA](https://mobile-aloha.github.io/)
**Paper:** [Mobile ALOHA: Learning Bimanual Mobile Manipulation with Low-Cost Whole-Body Teleoperation](https://arxiv.org/abs/2401.02117)<br>
**Github:** [https://github.com/MarkFzp/mobile-aloha](https://github.com/MarkFzp/mobile-aloha)<br>
**Code:** [https://github.com/MarkFzp/act-plus-plus](https://github.com/MarkFzp/act-plus-plus)<br>
<iframe width="753" height="422" src="https://www.youtube.com/embed/HaaZ8ss-HP4" title="Mobile ALOHA: Your Housekeeping Robot" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---
### ALOHA 2
**Paper:** [ALOHA 2: An Enhanced Low-Cost Hardware for Bimanual Teleoperation](https://arxiv.org/abs/2405.02292)<br>
<iframe width="942" height="530" src="https://www.youtube.com/embed/PHXQFE-Rteo" title="ALOHA 2: An Enhanced Low-Cost Hardware for Bimanual Teleoperation" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---
### [ALOHA unleashed](https://aloha-unleashed.github.io/)
**Paper:** [ALOHA Unleashed: A Simple Recipe for Robot Dexterity](chrome-extension://efaidnbmnnnibpcajpcglclefindmkaj/https://aloha-unleashed.github.io/assets/aloha_unleashed.pdf)<br>
![](<iframe width="942" height="530" src="https://www.youtube.com/embed/1EAsn71O9yA" title="ALOHA Unleashed: Autonomous Policies" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>)

---
### DemoStart
**Paper:** [DemoStart: Demonstration-led auto-curriculum applied to sim-to-real with multi-fingered robots](https://arxiv.org/abs/2409.06613)<br>
**Blog:** [Our latest advances in robot dexterity](https://deepmind.google/discover/blog/advances-in-robot-dexterity/)<br>
![](https://i.gzn.jp/img/2024/09/13/google-deepmind-robot-arm-aloha-unleashed-demostart/01_m.png)
![](https://i.gzn.jp/img/2024/09/13/google-deepmind-robot-arm-aloha-unleashed-demostart/02.jpg)

---
### [ReKep](https://rekep-robot.github.io/)
**Paper:** [ReKep: Spatio-Temporal Reasoning of Relational Keypoint Constraints for Robotic Manipulation](https://arxiv.org/abs/2409.01652)<br>
**Code:** [https://github.com/huangwl18/ReKep](https://github.com/huangwl18/ReKep)<br>

<iframe width="942" height="530" src="https://www.youtube.com/embed/2S8YhBdLdww" title="ReKep | Spatio-Temporal Reasoning of Relational Keypoint Constraints for Robotic Manipulation" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<br>
<br>

*This site was last updated {{ site.time | date: "%B %d, %Y" }}.*


