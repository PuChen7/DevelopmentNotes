# Message Queue(MQ) And Java Message Service(JMS)
## Message Queue
- [IBM Intro To MQ](https://www.ibm.com/support/knowledgecenter/en/SSFKSJ_8.0.0/com.ibm.mq.pro.doc/q002620_.htm)
- [IBM MQ Terminology](https://www.ibm.com/support/knowledgecenter/SSFKSJ_8.0.0/com.ibm.mq.pro.doc/q002640_.htm#q002640___Message)

- Message queuing has been used in data processing for many years. It is most commonly used today in electronic mail.
- To communicate with another program, a program must put a message on a predefined queue. The other program retrieves the message from the queue, and processes the requests and information contained in the message. So message queuing is a style of program-to-program communication.
- Queuing is the mechanism by which messages are held until an application is ready to process them. Queuing allows you to:
  - Communicate between programs (which might each be running in different environments) without having to write the communication code.
  - Select the order in which a program processes messages.
  - Balance loads on a system by arranging for more than one program to service a queue when the number of messages exceeds a threshold.
  - Increase the availability of your applications by arranging for an alternative system to service the queues if your primary system is unavailable.
- Queues reside in, and are managed by, a `queue manager`
- Different styles of message queuing
  - Point-to-point
    - One message is placed on the queue and one application receives that message.
    - In point-to-point messaging, a sending application must know information about the receiving application before it can send a message to that application. For example, the sending application might need to know the name of the queue to which to send the information, and might also specify a queue manager name.
  - Publish/Subscribe
    - A copy of each message published by a publishing application is delivered to every interested application. There might be many, one, or no interested applications. In publish/subscribe an interested application is known as a subscriber and the messages are queued on a queue identified by a subscription.
    - Publish/subscribe messaging allows you to decouple the provider of information from the consumers of that information. The sending application and receiving application do not need to know as much about each other for the information to be sent and received.

## JMS
- [JMS Tutorial](https://howtodoinjava.com/jms/jms-java-message-service-tutorial/#need)

- JMS (Java Message Service) is an API that provides the facility to create, send and read messages. It provides loosely coupled, reliable and asynchronous communication.
- JMS API Programming Model
  - <img src="https://cdn2.howtodoinjava.com/wp-content/uploads/2016/04/JMS-API-Programming-Model.png" width="400" height="300">
