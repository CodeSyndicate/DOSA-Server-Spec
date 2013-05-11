CodeSyndicate - Server 
======

The inter-server communication layer for all CodeSyndicate applications.

## Vision

### Distributed Open Source Application (DOSA)

The internet is designed to be a distributed network where taking out any single point wouldn't bring the entire network down. The problem is that we're stuck in the constant eb and flow of corporations who create applications and then shut them down; almost all of the applications online are centralized to a single entity and this is inconsistant with the way the web operates. The answer is distributed open source applications.

These types of applications are designed to be comprised of two parts: a server installation and a client installation. The server application is installed on a personal or home server and interacts with other personal servers through standard APIs. The client installation may be a smartphone app or it might be a web application installed on the same personal server as the server installation.

### Communication

The basic flow of communication in a DOSA environment is very similar to how it currently works in a client-server relationship. The two endpoints transfer information back and forth as needed. The only difference here is that your client is designed to interact with your server and only your server. The server then handles any necessary interaction with other DOSA servers. Email functions this way: the client sends an email to their smtp server which forwards the message on to the appropriate mx server which delivers it to the appropriate account on that server. An account in a DOSA environment resembles an email address because it contains the username and the personal server address (e.g. phil@homeserver.net).

### Code Syndicate

We hope to introduce this new way of looking at application development so that all web-based applications will no longer be forced to rely on a central point of failure. We're starting this idea but it is open-source, please continue to refine the idea with us. We'll be working on building the initial prototype server infrastructre in C# but the idea isn't reliant on a single technology; we want this to evolve.


## Server Responsibilities

 - Communicate with other DOSA server.
 - Queue server requests.
 - Maintain distrubuted server lists.
 - Trigger events/requests to the appropriate application.
