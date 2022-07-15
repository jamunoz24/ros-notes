## ROS launch system
[roslaunch wiki](https://wiki.ros.org/roslaunch)

Starting and configuring individual nodes could be time intensive. The roslaunch system lets us run and launch multiple nodes with a single command. They can be ran locally and remotely via SSH.

The .launch should be stored in:
`src/package_name/launch/`

Once the file is set up, you can run it with:
`roslaunch package_name file.launch`