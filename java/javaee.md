# Content
* [Intro](## Intro)
  * [Execution of Servlets](#### Execution of Servlets)
  * [Life Cycle](#### Life Cycle)

## Intro
Servlets are the Java programs that runs on the Java-enabled web server or application server(works on **server-side** to create dynamic Web pages). They are used to handle the request obtained from the web server, process the request, produce the response, then send response back to the web server.
#### Execution of Servlets
1. The clients send the request to the web server.
2. The web server receives the request.
3. The web server passes the request to the corresponding servlet.
4. The servlet processes the request and generate the response in the form of output.
5. The servlet send the response back to the web server.
6. The web server sends the response back to the client and the client browser displays it on the screen.
#### Life Cycle
1. The servlet is initialized by calling the **init()** method.
  * one-time initializations
2. The servlet calls **service()** method to process a client's request. 
  * main method to perform the actual task
  * The service () method is called by the container and service method invokes(ovveride) doGet, doPost, doPut, doDelete, etc.
3. The servlet is terminated by calling the **destroy()** method.
4. Finally, servlet is garbage collected by the **garbage collector** of the JVM.

