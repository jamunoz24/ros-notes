## ROS Services
[Services wiki](https://wiki.ros.org/Services)
[Video Tutorial](https://youtu.be/_EtsntSAVKE)

Services are another option to connect nodes in a ROS graph. ROS Services implement a two-way communication structured as a called on response. Whenever a connection is made between a client and a server, the client will send a request message that includes all of the arguments necessary to run the service. When the service is done running, the server will send back a response message that includes all of the output data returned by the service. 

Services are one-to-many.

<u>To see all of the current Services available:</u>
`rosservice list`

<u>To see more information about a Service:</u>
`rosservice info /service`

<u>To see the full structure of the Service:</u>
`rossrv show sim/Service`

The structure displays two sets of information. The first half are the arguments needed to send the request message. The second half is what will be returned by the response message.

<u>We can call the Service by:</u>
`rosservice call /spawn "(request message arguments)"`
Use tab to autocomplete the required arguments.
