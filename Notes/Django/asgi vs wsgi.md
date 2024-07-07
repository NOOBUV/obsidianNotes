Asynchronous service gateway interface vs web service gateway interface
- wsgi is normal way of calling the main function, basically synchronous way you call an api and it will execute and get back with response, used for simple api's with low to moderate traffic
- asgi is basically asynchronous calling of the main function or api and it generally is used for handling complex and large traffic
	- examples: chat application, streaming platforms (real time communication apps)

ASGI allows for more efficient and scalable handling of real-time features like **live video streaming and chat** by providing support for asynchronous programming, bidirectional communication via protocols like WebSockets, and an event-driven architecture.