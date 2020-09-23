Here's is a client server program, where the client side is implemented in native java script code and the server side is implemented
in Python.
This is a demo program that simulates an Iframe application that navigates to a non-Iframe app.
What I want to check here is what happen when the host app destroys the Iframe (delete it from the DOM) while the Iframe still has some
operations to do.
While destroying the Iframe, the browser throws an unload event that is caught by the Iframe. I want to check if the Iframe can block the 
app that it is hosted by from continue and loading the resource of the second app while it implements the onunload function.

Here are the instructions to run this project:
1. Clone the project to your PyCharm (or other IDE)
2. Run the server.py (by right click on it and choose 'run').
   You will probably need first to install the flask microframework. Let the IDE do that by right clicking on the 'Flask' error 
   in the file server.py
3. After installing Flask, run the server (server.py)
4. Open the following url in the browser: localhost:8000
5. You should see a very basic app, with test for the host and a button for the Iframe
6. By clicking the Iframe button you can navigate to the second non-Iframe app.
7. You can open the Chrome Dev Tool and analyze the results
