# Questions
- What are all the software protocols used to transfer data?
- What are all the hardware protocols used to route data?
- What is modulation/ demodulation at the physical layer?
- What are data links?
# Terms
- *OSI Model:* 
- *Media Access Control (MAC):*
# Notes
- All devices connected to the internet are either hosts or end systems
	- What is a host?:
	- What is an end system?:
- End systems are connected together via a network of communications links and packet switches.
- The OSI model is an conceptual abstraction of networking that divides network functions into 7 different layers. Each layer of the OSI model is depends on the operations of the layer under it.
	- Layer 1 (The physical layer): Transmits raw bit streams over a physical medium.
		- *Physical Layer Functions:* Turning bits of data into signals that can be transmitted over cables (called encoding), and turning these signals back into data at the reciever (decoding). It uses modulation to ensure data is transmitted correctly and demodulation to retrieve it at the other end. This layer also decides how data flows through transmission modes and controls the speed and timing of data transmission.
		- *Network Topologies:* Networks topologies describe how different devices are connected together. (Expand on this)
		- *Physical Layer Protocols:* Ethernet, widely used for wired networks. Wi-Fi, for wireless communications. Bluetooth, for short-range wireless communication. And USB, for connecting devices over short ranges.
	- Layer 2 (The data link layer): Responsible for node to node delivery of data within the LAN. 
		- The data link layer is further divided into sub layers which go as follows:
			- *Logical Link Control (LLC)/ SNAP:* The sub-layer of the data link layer that deals with synchronization, multiplexing, the flow of data among applications and services, and error checking as well. The basic model of the LLC is modeled after the HDLC protocol. The LLC is encapsulated in the MAC frame.
			- *Media Access Control (MAC):* The mac sublayer manages device interactions. Responsible for addressing frames, and also controls physical media access. The data link layer receives information in the form of packets from the network layer above it. It divides these packets into "frames" and sends those frames bit-by-bit to the underlying physical layer.
			- *Ethernet II:* 
		- *The MAC Frame:* Packets from the network layer are turned into MAC framed at your NIC.
		- There are 7 different protocols that exist on the data link layer, which go as follows:
			- *Synchronous Data Link Protocol (SDLC):* Used with the Systems Network Architecture (SNA) environment. SNA is the proprietary networking architecture of IBM that was developed in 1974. SDLC also supports a huge variety of typologies and different types of data links.
		- A data link refers to the logical or physical connection between two nodes on a network, responsible for reliable data transmission over a direct link (e.g., between two devices, a device and a switch, or across a WAN). Data links can work on different modes of transmission:
			- *Simplex Mode:* Only one device transmits data to the other device.
			- *Half-Duplex Mode:* Both devices can communicate simultaneously, but only one at a time.
			- *Full-Duplex Mode:* Both devices can send and receive data at the same time.
		- Devices operating at the data link layer:
			- *Switch:* Uses MAC addresses to forward data frames to the correct device within a network. Used to connect devices in a LAN
			- *Bridge:* A bridge connects two or more LANs, creating a single, unified network. Exists on the data link layer because it forwards frames based on mac addresses. Used to reduce network traffic and segment a network.
			- *Network Interface Card (NIC):* A NIC is the hardware device responsible for adding MAC addresses to frames and **ensuring proper communication within a network (?)**
			- *Wireless Access Point (WAP):* Allows wireless devices to connect to a wired network. Exists on the data link layer because by managing wireless MAC addresses.
			- *Layer 2 Switch:* Specialized switches that only operate at layer 2, unlike multi-layer switches. Responsible for frame forwarding using MAC address tables
		- Packets from the network layer have to be turned into MAC frames to be transferred over ethernet/ wifi. Your NIC converts a packet into a MAC frame. By default, MAC frames will be Ethernet II instead of LLC, which depending on the type, the frame will be structured differently:
			- Ethernet II: Starts with a "preamble" section of 7 bytes containing alternating 1s and 0s for synchronization **(How does that work?)**. Then 1 byte for the Start Frame Delimiter (SFD) containing 0xAB. Then 6 bytes for the destination MAC address, and 6 bytes for the source MAC address.
# Hardware
- *Hub:* Broadcasts all data sent to it to every device connected to it.
- *Repeater:* Receives signals sent to it and re-transmits it to improve signal strength
- *Switch:* Connects devices in a LAN (local area network)
- *Wireless Access Point (WAP):* Allows wireless devices to connect to a wired network.
- *Router:* Acts as a WAP plus a hub.
# Summary Texts
- How does networking work when reaching end systems on the same network?
	- 
- How does networking work when reaching end systems across the internet?
	- 