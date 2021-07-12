
# TiM-Controller Software Specifications
## Controller-side
### Backend
The backend is currently a node.js server daemon, handling controller inputs, firmware updates,  as well as communicating with the attached computer over Websockets, with an Ethernet connection via USB. This could be changed to Serial, removing the need for an Ethernet connection over USB (maybe less overhead?)

### Frontend
If there is a display attached, then the backend will launch TrainView-2, in a single windowed X Server session. The only difference is that TrainView-2 will communicate with the daemon locally instead of over the network.  

## Computer Side
### Minecraft
Currently, the communications between the computer and controller in-game are handled via TiM-Link. 

### Configurator
The configurator allows you to update the software, map buttons, check the info about the device, and SSH into it, if needed. This is also made in Flutter.
