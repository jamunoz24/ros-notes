## Nodes
[Nodes wiki](https://wiki.ros.org/Nodes)

<u>From the wiki:</u>
A *node* is a process that performs computation. Nodes are combined together into a graph and cmmunicate with one another using streaming topics, RPC services, and the Parameter Server. These nodes are meant to operate at a fine-grained scale; a robot control system will usually comprise many nodes. For example, one node controls a laser range-finder, one node controls the robot's wheel motors, one node performs localization, one node performs path planning, one node provides a graphical view of the system, and so on.

## Topics
[Topics wiki](https://wiki.ros.org/Topcs)

<u>From the wiki:</u>
Topics are named buses over which nodes exchange messages. Topics have anonymous publish/subscribe semantics, which decouples the production of information from its consumption. In general, nodes are not aware of who they are communicating with. Instead nodes that are interested in data *subscribe* to the relevant topic; nodes that genereate data *publish* to the relevant topic. There can be multiple publishers and subscribers to a topic.

Topics are intended for unidirectional, streaming communication. Nodes that need to perform remote procedure calls, i.e. receive a response to a request, should use services instead. There is also the Parameter Server for maintaining small amounts of state.

## Messages
[Messages wiki](https://wiki.ros.org/Messages)
[msg wiki](https://wiki.ros.org/msg)

<u>From the wiki:</u>
Nodes communicate with each other by publishing **messagers** to topics. A message is a simple data structure, comprising typed fields. Standard primitive types (integer, floating point, boolean, etc.) are supported, as are arrays of primitive types. Messages can include arbitrarily nested structures and arrays (much like C structs).
Nodes can also exchange a *request* and *response* messages as part of a ROS service call. These request and response messages are defined in srv files.

Messages field:
`fieldtype1 fieldname1`

Ros files can be found with `roscd`
Message files can be navigated with `roscd std_msgs`

