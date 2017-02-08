# HW1-B

Name: Aakarsh Gopi

Unityid: agopi

###Installing jenkins


####INSTRUCTIONS
* 
* 
* 
* 
* 


####NOTE:
* 
* 

References: http://docs.aws.amazon.com/sdk-for-javascript/v2/developer-guide/ec2-example-creating-an-instance.html

###Screencast
Here's the link to screencast: 

###Running the job


###Concepts

Q1. What are some benefits of continuous integration?

An operation is defined as idempotent if the result remains constant and doesn't depend on the number of times the operation has been called. For ex: Setting a variable i's value as 1. Irrespective of the number of times we call this operation, the result doesn't vary i.e.  the variable i's value is being set to 1. But take the example of decrement operator, the variables value will keep decreasing, thus its not idempotent, as the result keeps varying. 

Examples of Idempotent Operation:
* HTTP GET: This operation will be ideally returning the same value as long as server's state doesn't change
* HTTP HEAD: Just like GET, this will also be ideally returning just the header as long as the server's state doesn't change.

Examples of Non-Idempotent Operation:
* Append operation on a file: It will keep appending the same value in the file, therefore it can't be said as an idempotent operation as the value keeps changing.
* Ping operation: Practically speaking the value will keep changing thus it's not idempotent.


Q2. What are some risks of not using continuous integration?

There are many things that comprise of inventory. It ranges from the ip addresses owned to keys, passwords and API tokens. If we want to provision new servers, without proper inventory management we might request new servers although we still have a couple of servers that are free. 
How can we centralize everything but also ensure that individual teams can still request and gain access to servers without going through a tedious process. 
Imagine there are 100s of teams, how can the inventory be efficiently managed but also ensuring that all teams requirements are met without having to burden other teams requirements. 
Inventory management is a tedious task because of the enormous services it needs to track, and also provision them when requested. Thus, it has to keep track of everything. 
If the requests can't be tackled through the resources present, we will also need to request for additional resources and ensure that its allotted to the team requested. 
Also the compability of tools and the environment needs to be taken into account. 

Q3. What are some reasons why a company may use a dedicated build team?
The two models are Push based and Pull Based.

Push Based Configuration System:

In push based configuration system, the server is responsible for pushing configuration and other important softwares to the nodes where it installs them remotely. Thus, server takes care of configuration of nodes in Push based configuration system.

Advantages:
1. Since the master is responsible for configuring and deployment of nodes, it can orchestrate the node deployment. This would be definitely helpful in scenarios where a particular set of nodes. <br>
2. It is easier to manage when compared to Pull Based system.


Disadvantages:
1. Because server is in charge of configuring, it becomes cumbersome when trying to scale like if you want to deploy 100 images simultaneously it'd load to performance issues.<br>
2. Independent configuration is not usually possible i.e. to boot a new node and have it configure on its own(basically the idea of pull based system).

Pull Based Configuration System:

In pull based configuration system, the individual nodes contact the master server and request their configuration and other importnat softwares and configure themselves. Thus, the individual nodes are responsible for configuration in Pull based configuration system.

Advantages:
1. The nodes can continue configuration of themselves without the intervention of master, thus not impacting the performance of master. Thus scaling becomes comparitively easier as the new nodes that come in just setup on their own after getting instructions from master.<br>
2. It is better at ensuring that the nodes stay in sync.

Disadvantages:
1. In case of instaneous deployment, it'd impact performance of master server because all the nodes will be se ding a request to master server. <br>
2. Security is a big concern because it connects back to the master server. 

Q4. What are some barriers to applying continuous integration in priorierty contexts?

The most important consequences is that its security is compromised. Some other consequences include:<br>
1. It becomes difficult to manage the system due to improper configuration as some nodes maybe running different versions.<br>
2. It can also lead to system failure in certain cases.<br>
3. It becomes difficult to manage all the changes done to items related to software.<br>
4. Thus it also track changes made to the system. It'd make it impossible to track the old versions and their requirements. If a customer running an old version has found a bug, it'd be difficult to fix it.
