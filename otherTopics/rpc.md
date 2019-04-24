# Remote Procedure Call (RPC)
- [GeeksForGeeks](https://www.geeksforgeeks.org/operating-system-remote-procedure-call-rpc/)
- [TutorialsPoint](https://www.tutorialspoint.com/remote-procedure-call-rpc)

- Remote Procedure Call (RPC) is a powerful technique for constructing distributed, client-server based applications. 
- A remote procedure call is an interprocess communication technique that is used for client-server based applications. 
- A client has a request message that the RPC translates and sends to the server. This request may be a procedure or a function call to a remote server. When the server receives the request, it sends the required response back to the client. The client is blocked while the server is processing the call and only resumed execution after the server is finished.
- The two processes may be on the same system, or they may be on different systems with a network connecting them. 
- Work flow
  - <img src="https://cdncontribute.geeksforgeeks.org/wp-content/uploads/operating-system-remote-procedure-call-1.png" width="380" height="300">
