# Robotic Indoor Source-Seeking Simulation and Dataset

## Source Code

Robot simulations were conducted using the Gazebo simulation environment on the ROS platform.  
The source-seeking task is performed by a **TurtleBot3 Burger** mobile robot, equipped with a single-line LiDAR, a MOX gas concentration sensor, and an anemometer.  
The ROS version used in the simulations is **Noetic**.

The simulation and dataset generation pipeline is based on a **secondary development of AutoGDM**  
(https://github.com/tudelft/AutoGDM), which provides integrated support for indoor environment modeling, airflow simulation, and gas dispersion modeling.

---

## Dataset

The dataset consists of three main categories of data used for robotic indoor source-seeking experiments.

### CAD Files  
Indoor environment models are represented using CAD files, which define the geometric layouts and obstacle configurations of the simulated indoor scenarios.

### CFD Data  
Airflow fields within the indoor environments are generated through computational fluid dynamics (CFD) simulations using **OpenFOAM 7**, following the airflow simulation pipeline provided by AutoGDM.

### Dispersion Data  
Gas dispersion in the indoor environments is simulated using **GADEN**, producing spatial gas concentration distributions used for robotic source-seeking experiments.

---

## Scenario Naming Convention

To facilitate systematic analysis and reproducibility, all test cases adhere to a unified naming convention:
CaseX1-X2-X3-X4-X5-X6X7

where:

- **X1**: Scenario type (`A–C`)  
- **X2**: Environment index (`01–06`)  
- **X3 / X4**: Airflow inlet and outlet numbers  
- **X5**: Inlet wind speed (e.g., `04` for 0.4 m/s)  
- **X6**: Source position relative to airflow  
  - `U` = Upstream  
  - `D` = Downstream  
- **X7**: Source location relative to the plume  
  - `I` = Inside  
  - `O` = Outside  

### Example

`CaseB-03-1-4-08-UI` describes a vortex-type scenario in **Environment 03**, with airflow inlet **1**, outlet **4**, wind speed **0.8 m/s**, and a source placed **upstream and inside the plume**.

