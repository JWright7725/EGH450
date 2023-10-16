# EGH450
Github repository for all software developed by Group 1 throughout EGH450

The software used throughout this project includes a number of submodules that have been forked from the QUTAS Github repository and updated to provide additional functionality. Additionally, a number of submodules within the QUTAS repository have also been directly forked into this repository, as no changes to their functionality were required.

## SPAR:

The Spar submodule contains the software programs written to complete the Autopilot, Navigation and Localisation requirements of the project. This includes the generation of the low-level waypoints through the use of the breadcrumb path planning service, the software responsible for localisation of the target positions within the world frame, and all other miscellaneous program used for testing and verification of the individual system components.
This submodule also contains the code utilised for payload deployment as a portion of the ANL program which activates one of two servo motors attached to the airframe to release a trapdoor below either payload.

This software within this submodule is run during flight testing by running the 'final_simulation_code' python file through a running ROS session.

## QUTAS_LAB_450:

This submodule is used for the generation of the necessary world environment for flying within the QUT GP O-134 flight area. This software is primarily cloned from the provided QUT repo, with minimal changes made to alter the given name of the UAV to 'skittles'. This software is run through the use of the 'control.launch' file, and must be started before flight testing is undertaken.

## DEPTH_AI_PUBLISHER:

This submodule is utilised to provide the necessary image processing capabilities to the UAV for the UAV to orient and observe its flight environment. This software includes a number of ROS publisher nodes which publish the necessary information for the Spar submodule to localise and fly towards the desired targets and ArUco markers. The generated software is run through the use of the 'dai_publisher_yolov5_runner' file throguh a running ROS session.

## 
