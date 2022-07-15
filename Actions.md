## ROS Actions
[actionlib wiki](https://wiki.ros.org/actionlib)
[Tutorial Video](https://youtu.be/QvdfJVRj4-8)

Actions follow a similar structure to Services (one-to-many). The difference being the information being sent. When an action client connects to an action server, the client will send a **goal** to the server for it to complete.
The server begins working on the goal and starts sending back serveral **feedback** messages, then finally with a **result** message.
While the server is sending back feedback messages, the client can send cancel command or preemptive command. The preemptive command will give the server a new goal to replace it with.

When looking at an action file, the information is split between 3 sections. The first section is a goal the client gives to the server. The section is the result message being sent back from the server to the client. The third is the feedback message the server will be sending back while it is working on the goal.

Action code can be stored in package/src.