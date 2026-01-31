View Paper
(Code will be released after acceptance)

## Source Code
Robot simulations were conducted using the [Gazebo](https://gazebosim.org/home) simulation environment on the [ROS](https://www.ros.org/) platform. The source-seeking task is performed by a [TurtleBot3 Burger](https://emanual.robotis.com/docs/en/platform/turtlebot3/overview/) mobile robot, equipped with a single-line LiDAR, a MOX gas concentration sensor, and an anemometer. The ROS version used in the simulations is [Noetic](https://wiki.ros.org/noetic).
The dataset generation pipeline is based on a secondary development of [AutoGDM](https://github.com/tudelft/AutoGDM), which provides integrated support for indoor environment modeling, airflow simulation, and gas dispersion modeling.

## Dataset
The dataset consists of three main categories of data used for robotic indoor source-seeking experiments.

• [CAD Files](https://huggingface.co/datasets/): Indoor environment models are represented using CAD files, which define the geometric layouts and obstacle configurations of the simulated indoor scenarios.

• [CFD Data](https://huggingface.co/datasets/): Airflow fields within the indoor environments are generated through CFD simulations using [OpenFOAM](https://openfoam.org/) 7 software, following the airflow simulation pipeline provided by AutoGDM.

• [Dispersion Data](https://huggingface.co/datasets/): Gas dispersion in the indoor environments is simulated using [GADEN](https://github.com/MAPIRlab/gaden), producing spatial gas concentration distributions used for robotic source-seeking experiments.

## Videos
(Videos will be released after acceptance)

• CaseA-01-26-28-04-DI  
• CaseB-04-27-26-04-UO  
• Scenario 1  
• Scenario 2  

## Cite this paper
@article{Jing2026adaptive,

  author={Jing, Mengjie and Xin, Bin and Wang, Miao and Bian, Wenjing},
  
  journal={xxx}, 
  
  title={Adaptive Robotic Source Seeking in Vortical Indoor Environments with Sparse Structural Guidance}, 
  
  year={2026}
  
}
