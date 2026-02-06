# POINT TRANSFORMER TERRAIN SEGMENTATION FROM 3D-LIDAR POINT CLOUDS
This repo is the official project repository of my project **_POINT TRANSFORMER TERRAIN SEGMENTATION FROM 3D-LIDAR POINT CLOUDS_**, which will display and explain key features. The motivation behind the idea is to provide a system that can accurately segment off-road terrain into drivable vs non-drivable regions for vehicles equipped with LiDAR sensors. Point Cloud data is captured using LiDAR sensors and recorded using a combination of Rviz and rosbag. The recorded point cloud data is then converted into datasets with binary target labels(drivable and non-drivable), which are derived from the original terrain meshes that are painted/sectioned. Finally, the data is fed into a Point Transformer v3 model for training and evaluation. The PTv3 repository can be found at: [https://github.com/Pointcept/PointTransformerV3](https://github.com/Pointcept/PointTransformerV3).

<div align="center">
  <img src="assets/terrain_images/t3.png" height="210" />
  <img src="assets/agilex_scout_mini/Scout_mini__74935.png" height="210" />
</div>





<!-- Connect with me -->
## Tech Stack
<div align="center">

![image](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue)
![image](https://img.shields.io/badge/ROS-22314E?style=for-the-badge&logo=ROS&logoColor=white)
![image](https://img.shields.io/badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)
![image](https://img.shields.io/badge/MySQL-005C84?style=for-the-badge&logo=mysql&logoColor=white)
![image](https://img.shields.io/badge/blender-%23F5792A.svg?style=for-the-badge&logo=blender&logoColor=white)
![image](https://img.shields.io/badge/Pandas-2C2D72?style=for-the-badge&logo=pandas&logoColor=white)
![image](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)

</div>

## Environment + Simulation tools
Below is the required environment setup for the project due to compatibility issues regarding the AgileX Scout Mini simulation model.

  * OS: Ubuntu 20.04
      * Installation: [https://releases.ubuntu.com/focal/](https://releases.ubuntu.com/focal/)
  * ROS version: ROS 1 Noetic
      * Installation: [https://wiki.ros.org/noetic/Installation/Ubuntu](https://wiki.ros.org/noetic/Installation/Ubuntu)
  * Simulaton Environment: Gazebo Classic
      * Installation: [https://classic.gazebosim.org/](https://classic.gazebosim.org/)
  * Data Recording: Rviz
      * Included with the installation of ROS 1 Noetic
  * AgileX Scout Mini UGV Gazebo Sim repo: [https://github.com/agilexrobotics/ugv_gazebo_sim](https://github.com/agilexrobotics/ugv_gazebo_sim)





## Key Features/Steps
Below is a list of features involved in the creation of this project

1. Custom, procedurally generated 3D terrains that maintain an even distribution of smooth, drivable areas and steep, rugged terrain.
   
    * 3D terrains were built with Blender using a Geometry Node system. The following link was used as a guide to create the Geometry Node system: [https://www.youtube.com/watch?v=0VIK1Ct6jLM&t=120s](https://www.youtube.com/watch?v=0VIK1Ct6jLM&t=120s)
   
    * 28 total terrains created, each exported as Collada(DAE) files for simulation compatibility.
  


## Recordings


Point cloud display via VLP-16 LiDAR sensor in Rviz:

<div align="center">
  <img src="captures/recording2-MadewithClipchamp-ezgif.com-crop.gif" />
</div>



<div align="center">
*Point cloud colors displayed with AxisColor: Purple(High Elevation) -> Red(Low Elevation)*
</div>


<!-- CONTACT -->
## Contact

Kcey Stadalman - kceystad7@outlook.com

Project Link: [https://github.com/CNTRL-tek91/POINT-TRANSFORMER-TERRAIN-SEGMENTATION-FROM-3D-LIDAR-POINT-CLOUDS](https://github.com/CNTRL-tek91/POINT-TRANSFORMER-TERRAIN-SEGMENTATION-FROM-3D-LIDAR-POINT-CLOUDS))

<p align="right">(<a href="#readme-top">back to top</a>)</p>


