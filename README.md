# PhilipsAssignment
This code is created as per the requirments of the Assignment. 
I have used AngularJs for clientside graph rendering. NodeJs for backend.
Socket.io library has beem used to establish a real-time data communication between the client and the server.
socket.io had been integrated with the Node.JS HTTP Server & "socket.io-client" deals with loading process on the client side.


# Running the app
Note: In local the app is working as expected. But, I had tried deploying the appication in aws, there was a CORS error which held me back.

Kindly pull the code into local your local and share your feedback :-). 

Steps to build after pulling: 

For serverside(backend) :  1) RUN "npm install" to manage dependencies.
                            2) Run "node app.js" 
                        Notice that an instance of socket.io has been initialised by passing the http object which will
                         listening(on port 4444) for the  incoming sockets on connection event, and once the connection establish it will
                         send random data for every 200ms.
                            
For clientside : 1)  Make sure you have the latest [Angular CLI]nstalled globally and RUN "npm install" to manage dependencies.
                 2)  Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. 
                 Once the app loads in the browser it will automatically establishes connection to with server and gets data for every                      200ms, stores in channel array. For evey 500ms the graph will be updated with new point.
                 
                 
# ScreenShot
![Screenshot (9)](https://user-images.githubusercontent.com/14186664/60034661-c7ba1f00-96c8-11e9-8c68-97a5253e5d71.png)
