# TCP
Implementation of the TCP protocol to send files between client - server. This project was a part of the Computer Networks class in my junior year. The code runs on top of the unreliable UDP network. Incorporates the following features of the TCP protocol
<li> Reliability (with appropriate re-transmissions) - implements the variant of Go-Back-N protocol</li>
<li> Data Integrity (with checksums) </li>
<li> Connection Management </li>
<li> Optimizations like fast retransmit etc </li>
<li> Implements sliding window algoirhtm to prevent buffer overflows </li>

To execute the code, run the Makefile first to compile the Sender and Receiver files. Then, the commnad line arguments for the client side is java TCPend -p [port] -s [remote-IP] -a [remote-port] –f [file name] -m [mtu] -c [sws]. Where

<li> port: Port number at which the client will run </li>
<li> remote-IP : IP address of the remote process (Receiver) </li>
<li> remote-port: port at which the remote process/ transmission is running </li>
<li> file name: name of the file to be transferred </li>
<li> mtu : Maximum transmission unit </li>
<li> sws: Sliding window size </li>

Similarly, for the Sender side, command line arguments are  java TCPend -p [port] -m [mtu] -c [sws]


