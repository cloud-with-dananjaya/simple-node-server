# simple-node-server
This code creates a node js server which listens on port 8080.
<br>

<h2>Prerequisites</h2>
Node installed. The node installation process depends on the environment.

<h2>Run server</h2>
cd into the folder with the index.js file. <br>
Then run the following command. <br>

<code>
node index.js
</code>
<br>
<h2>Run server as background service</h2>
Install pm2 process manager and start the server as a background service.

<code>
<pre>
npm install -g pm2
pm2 update
pm2 start -f index.js
</pre>
</code>

<h2>Test</h2>
Test the server by accessing the server by the following url.<br>

<code>
url:8080
</code>

<br>
The page should have 'Hello World';