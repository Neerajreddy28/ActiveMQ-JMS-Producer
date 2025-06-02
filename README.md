To work on this ActiveMQ JMS Producer project, first you need to have ActiveMQ.
After ActiveMQ is installed, To Start the ActiveMQ you need to enter the command, 

    brew services start activemq
  
Next, Gradle or Maven should be installed in your system.

To Setup the project follow the steps below:
1. Create a Gradle project
2. Add all the dependencies in the build.gradle file. The below packages are must to start the connection in activemq and JM.

        'javax.jms:javax.jms-api:2.0.1'
   
        'org.apache.activemq:activemq-client:5.18.7'
   
3.Verify that the active broker is running at tcp://localhost:61616
4.After all the above steps are done. Run the program through gradle using command,

     ./gralew run

5. Once the run command is successful, Build Successful and all the steps below will be displayed,

       JMS Connection started successfully.
       JMS Session created successfully.
       JMS Queue 'myTestQueue' created/found.
       JMS MessageProducer created.
       JMS TextMessage created: 'Hello from ActiveMQ!'
       Message sent successfully to queue: 'myTestQueue'
       JMS Session closed.
       JMS Connection closed.










