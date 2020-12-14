Data Plane Key Management (DPKM)
====================================
This GitHub Repository contains extensions to the Floodlight Web UI for integration of the Data Plane Key Management scheme DPKM.
DPKM enables automated configuration of WireGuard network tunnels between nodes in the data plane. Floodlight Web UI has been extended with a new page located in [/pages/dpkm.html](https://github.com/lukehengstenberg/DPKM_Floodlight-webui/blob/master/pages/dpkm.html).
Eight procedures have been added for Configuring WireGuard, Unconfiguring WireGuard, Adding Peers, Deleting Peers, Starting Encrypted Communication, Ending Encrypted Communication, Rekeying, and Compromise/Key Revocation. New REST APIs were defined in Floodlight for initiating the procedures from the interface.
OpenFlow has been extended with Loxigen to include six new messages, a new OXM, and fifteen new error messages. <br />
DPKM relies on the modified Floodlight controller set-up from [Here](https://github.com/lukehengstenberg/DPKM_Floodlight) and OVS nodes set-up from [Here](https://github.com/lukehengstenberg/DPKM_OVS). The UI is packaged with the controller so does not need to be pulled directly.<br /><br /> 

DPKM was completed as part of an MSc project at Swansea University and is still a work in progress.
Extensive testing with multiple nodes is needed since the project was built and tested for a single controller with two nodes. UI design was kept basic and will be enhanced with additional styling and formatting. Login access control mechanisms are also needed before deployment on a public network. The project would benefit from a professionals expertise to clean-up code and integrate better native support in Floodlight and OVS.<br /><br />
For any questions or queries, contact the developer at this [email](mailto:lukehengstenberg@gmail.com)!
