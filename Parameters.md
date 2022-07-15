## Parameters
[rosparam wiki](https://wiki.ros.org/rosparam)

rosparam is a command-line tool for getting and settign ROS parameters.

Some of the commands are `get`, `set`, `delete`, and `dump`.
`get` displays the parameter's current value.
`set` allows you to set a value to the parameter.
`delete` resets the parameter set.
`dump` allows you to dump all of the available parameter to a file

Example of `set`:
`rosparam set /turtlesim/param_a 0`

Example of `dump`:
`rosparam dump file_dump.yaml /turtulesim`
