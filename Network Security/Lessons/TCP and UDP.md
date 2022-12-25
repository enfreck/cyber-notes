Transport protocols

### TCP: Transmission Control Protocol 
- Connection-oriented protocol
	- handshake between sender and receiver before information is transmitted
	- TCP segments are sent in a stream with the receiver sending acknowledgements for each packet back to the sender
- reliable, in-order delivery, congestion control 

### UDP: User Datagram Protocol 
- Connectionless protocol
	- no handshaking between UDP sender and receiver
	- each UDP segment handled independently of others
- unreliable, unordered delivery, no congestion control
- Used for streaming media, DNS, HTTP/3