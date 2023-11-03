# node.js-interview-questions

# What is Node.js? Where can you use it?
Node.js is an open-source, cross-platform JavaScript runtime environment and library to run web applications outside the client’s browser. It is used to create server-side web applications.
we can also use it for developing: Real-time web applications, Network applications, General-purpose applications, and Distributed systems.

# How does Node.js work?
-> Clients send requests to the webserver to interact with the web application. Requests can be non-blocking or blocking:

-> Querying for data

-> Deleting data

-> Updating the data

-> Node.js retrieves the incoming requests and adds those to the Event Queue

-> The requests are then passed one-by-one through the Event Loop. It checks if the requests are simple enough not to require any external resources

-> The Event Loop processes simple requests (non-blocking operations), such as I/O Polling, and returns the responses to the corresponding clients

-> A single thread from the Thread Pool is assigned to a single complex request. This thread is responsible for completing a particular blocking request by accessing external resources, such as computation, database, file system, etc.

-> Once the task is carried out completely, the response is sent to the Event Loop that sends that response back to the client.

# Why is Node.js Single-threaded?
Node.js is single-threaded for async processing. By doing async processing on a single-thread under typical web loads, more performance and scalability can be achieved instead of the typical thread-based implementation.

# Explain callback in Node.js.
A callback function is called after a given task. It allows other code to be run in the meantime and prevents any blocking.  Being an asynchronous platform, Node.js heavily relies on callback. All APIs of Node are written to support callbacks.

# What are the advantages of using promises instead of callbacks?
-> The control flow of asynchronous logic is more specified and structured.

-> We've built-in error handling.

-> Improved readability.
