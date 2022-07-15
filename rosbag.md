## ROS bag
[rosbag wiki](http://wiki.ros.org/rosbag)

This is a set of tools for recording from and playing back to ROS topics. It is intended to be high performance and avoids deserialization and reserialization of the messages.

<u>Example usage:</u>
1. Start a simulator (turtlesim):
	`rosrun turtlesim turtlesim_node`
2. Run the teleop key:
	`rosrun turtlesim turtle_teleop_key`
	Now, the teleop key will begin recording inputs from the keyboard. When finished a .bag file will be generated at the current directory.
3. Once the recording is finished, play back the recording:
	`rosbag play generated_file.bag`
	The command above will miss the first command recorded, so we will add a delay to get the proper recording.
	`rosbag play generated_file.bag -d 0.5`
	Now, the recording should generate the correct commands.