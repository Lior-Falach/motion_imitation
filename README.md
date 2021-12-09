# Motion Siulation with Py bullet 

In this repo we have a motion simulation which will enable some data collection 

The file Walking.bag may be directly run (rosbag play Walking.bag) to publisg the Low state message and the ground truth state.

Download repo into the src folder in your Catkin_ws folder

Assume that you have previously compilied our modified unitree messages package

Simply run the catkin_make to compily the a1_motion_control package

Two nodes are available 

Whole_body_controller_robot_example.py
	Which will run the pybullet simulation and publish the lowstate massage and ground stat 	massage (in high resolution ~500 Hz), feel free to paly the the trajectory parameters and get 		different motion,the same is true for the gates.
hi2lowres.py
	This will publish the massages in low_res, i.e., 100Hz









```bash
sudo python3 -m motion_imitation.examples.whole_body_controller_robot_example
```

### Credits

This repo was developed at Google Robotics and is maintained by one of its members, Erwin Coumans.
The original Motion Imitation code was written by Jason Peng as part of an internship and student researcher at Google Robotics.
Some MPC parts for A1 and running on real A1 are written by Yuxiang Yang, a former resident researcher at Google Robotics.

---

*Disclaimer: This is not an official Google product.*

