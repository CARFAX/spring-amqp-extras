# spring-amqp-extras
This is a project that contains nice extras to complement spring-amqp.

Carfax src repository:
https://github.com/CARFAX/spring-amqp-extras

Carfax CI server instance: pscim02
http://pscim02:8090/job/spring-amqp-extras%20publish%20from%20master/







=======
## LoggingErrorHandler
This is an implementation of the ErrorHandler interface that you can attach to SimpleMessageListenerContainer to log errors that occur when consuming messages.


## Message Recovery
Two classes that aid in message recovery when a message cannot be consumed are provided: 

* ContentBasesMessageKeyGenerator - generates a unique key based on the message's content
* RepublishMessageRecoverer - publishes messages that erorred out to a specified exchange. 

