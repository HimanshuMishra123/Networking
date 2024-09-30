# Networking OSI Model - Detailed Notes 

Must watch OSI Video : https://www.youtube.com/watch?v=ZF9j3w95swU&list=PLRjPlu6MAom7Kj0efDQJDtdpcazYJOAwf&index=6
Must watch networking linux command : https://www.youtube.com/watch?v=EjiX1cjm_H8&t=66s
![image](https://github.com/HimanshuMishra123/Networing/assets/164254902/d63dbe37-1b05-4bc8-a36e-9c89f4ae7986)



Introduction:
The OSI (Open Systems Interconnection) model is a popular framework for understanding the journey of data across the internet.<br />
It explains the different layers involved in the data transmission process and what happens to the data in each of these layers.<br />
The OSI model consists of 7 layers: Layer 7 to Layer 1, or Layer 1 to Layer 7 if viewed from the end of the data transmission.<br />

## Prerequisites before OSI model:
DNS (Domain Name System) Resolution:<br />
This is the process of mapping a domain name (e.g., www.google.com) to an IP address.<br />
The router or browser first checks the local cache for the IP address mapping, and if not found, it queries the internet service provider's DNS server.<br />
TCP (Transmission Control Protocol) Handshake:<br />
The TCP handshake is a three-way process that establishes a connection between the client (e.g., your laptop) and the server (e.g., the Google server).<br />
The client sends a SYN (synchronize) packet, the server responds with a SYN-ACK (synchronize-acknowledge) packet, and the client completes the handshake by sending an ACK (acknowledge) packet.

## OSI Model Layers:
Layer 7 - Application Layer:<br />
The Application layer is responsible for defining the format and structure of the data being transmitted.<br />
example - The browser initiates an HTTP or HTTPS or FTP request to the server.<br />

Layer 6 - Presentation Layer:<br />
The data is encrypted, and the format and encoding are handled.<br />
The Presentation layer is responsible for translating data between different formats and encodings.<br />
It ensures that the data sent by the Application layer can be understood and processed by the receiving system.<br />
This layer handles tasks such as encryption, decryption, and data compression.<br />

Layer 5 - Session Layer:<br />
A session is created between the client and the server. (jisse baar baar login na manage example - transaction process bich mein na ruk jaye)<br />
The Session layer is responsible for establishing, maintaining, and synchronizing communication sessions between applications.<br />

layer 7,6,5 happening at the browser level<br />

Layer 4 - Transport Layer: (@ Firewall level)<br />
The data is segmented, and the protocol (TCP or UDP) is identified. <br />
example- For http the protocol is TCP and for DNS etc the protocol is UDP. <br />
the Transport layer is responsible for the TCP handshake. It handles tasks such as segmentation means carving up information into smaller pieces(10GB data ko samller piece s mein convert krna jisse bich mein process break na ho) .<br />
The Transport layer is responsible for end-to-end data delivery, ensuring that the data is transmitted reliably and without errors.<br />

Layer 3 - Network Layer: (@ Router level)<br />
The source and destination IP addresses are added to the data segments, which are now called packets.<br />
It determines the best path for the data to travel from the source to the destination.<br />
The Network layer is responsible for logical addressing and routing of data across the network. <br />

Layer 2 - Data Link Layer: (@Switch level) ... Router is connected to switches which  are ethernet ports. <br />
The packets are converted into frames, and MAC addresses/info are added.<br /> 
MAc info tells switch what are the other components within your network <br />

Layer 1 - Physical Layer: (@ Hub or Modem or fiber/optical Cables)<br />
The data is converted into electronic signals and transmitted over the physical network. Fibre cables only understand electronic signals.<br />

Data Journey through the OSI Model:<br />
The data travels through the OSI model layers, from Layer 7 to Layer 1, when the client sends a request.<br />
The reverse process happens when the server responds to the client's request, with the data traveling back through the OSI model layers.<br />

![Learn Networking in 3 Hours _ Networking Fundamentals + AWS VPC Networking 1-8-43 screenshot](https://github.com/HimanshuMishra123/Networing/assets/164254902/93031266-6d2c-4481-b00f-68ded86628a3)
