# node.js-interview-questions

# What is Node.js? Where can you use it?
Node.js is an open-source, cross-platform JavaScript runtime environment and library to run web applications outside the client’s browser. It is used to create server-side web applications.
we can also use it for developing: Real-time web applications, Network applications, General-purpose applications, and Distributed systems.

# How does Node.js work?
#### Clients send requests to the webserver to interact with the web application. Requests can be non-blocking or blocking:
-> #### Querying for data
-> #### Deleting data 
-> #### Updating the data
-> #### Node.js retrieves the incoming requests and adds those to the Event Queue
-> #### The requests are then passed one-by-one through the Event Loop. It checks if the requests are simple enough not to require any external resources
-> #### The Event Loop processes simple requests (non-blocking operations), such as I/O Polling, and returns the responses to the corresponding clients
-> #### A single thread from the Thread Pool is assigned to a single complex request. This thread is responsible for completing a particular blocking request by accessing external resources, such as computation, database, file system, etc.

#### Once the task is carried out completely, the response is sent to the Event Loop that sends that response back to the client.
