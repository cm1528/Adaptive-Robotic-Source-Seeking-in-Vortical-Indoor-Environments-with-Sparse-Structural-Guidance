## Source Code
Robot simulations were conducted using the [Gazebo](https://gazebosim.org/home) simulation environment on the ROS platform. The source-seeking task is performed by a **[TurtleBot3 Burger](https://emanual.robotis.com/docs/en/platform/turtlebot3/overview/)** mobile robot, equipped with a single-line LiDAR, a MOX gas concentration sensor, and an anemometer. The ROS version used in the simulations is **Noetic**.
The simulation and dataset generation pipeline is based on a **secondary development of [AutoGDM](https://github.com/tudelft/AutoGDM)**, which provides integrated support for indoor environment modeling, airflow simulation, and gas dispersion modeling.

## Dataset
The dataset consists of three main categories of data used for robotic indoor source-seeking experiments.
[CAD Files] (https://github.com/tudelft/AutoGDM) : Indoor environment models are represented using CAD files, which define the geometric layouts and obstacle configurations of the simulated indoor scenarios.

[CFD Data] (https://github.com/tudelft/AutoGDM) : Airflow fields within the indoor environments are generated through computational fluid dynamics (CFD) simulations using **[OpenFOAM 7](https://openfoam.org/release/7/)**, following the airflow simulation pipeline provided by AutoGDM.

[Dispersion Data] (https://github.com/tudelft/AutoGDM) :Gas dispersion in the indoor environments is simulated using **[GADEN](https://github.com/MAPIRlab/gaden)**, producing spatial gas concentration distributions used for robotic source-seeking experiments.
