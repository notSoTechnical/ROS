# ROS (Robot Operating System)

For Mac users, VM is the best option for now.  Download the software from the following link (The 64 bits VM): 

**https://wiki.epfl.ch/roscontrol/rosinstall**

or 

https://nootrix.com/diy-tutos/ros-indigo-virtual-machine/

login: viki <br>
password: viki


-------------------------------------------------------------------------------------------------------------------------


Another option: https://ubuntu.com/download/desktop

Install Ubuntu version 18.04 to your VM.  Make sure to change 10GB to 25GB during setup.  You would mostly likely run into space issues. Also, delete large files from your computer if needed. Use software https://www.omnigroup.com/more

Troubleshooting tips: 

**Note: Make sure no whitespace** <br>
Ex: <br>
Do       => echo $ROS_PACKAGE_PATH/home/notsotechnical/catkin_ws/src:/opt/ros/kinetic/share <br>
Don't do => echo <br>
$ROS_PACKAGE_PATH/home/notsotechnical/catkin_ws/src:/opt/ros/kinetic/share

**If you see this error: ERROR: Couldn't connect to Docker daemon at http+docker://localunixsocket - is it running?**

=> Add **sudo** in front of every command 

**E: Unable to acquire the dpkg frontend lock (/var/lib/dpkg/lock-frontend), are you root?**

=> sudo apt --fix-broken install
