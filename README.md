# simple-node-server
This code creates a node js server which listens on port 8080.
<br>

<h2>Prerequisites</h2>
Node installed. The node installation process depends on the environment.

<h3>Install nodejs on Mac/Windows</h3>
<ul>
    <li>Go to the nodejs download page. https://nodejs.org/en/download</li>
    <li>Download the installer</li>
    <li>Install nodejs using the installer</li>
</ul>
<br>

<h3>Install nodejs on EC2</h3>
<ul>
    <li>Install NVM (node version manager)<br>
    <code>
    curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.5/install.sh | bash
    </code>
    </li>
    <li>Activate nvm<br>
    <code>
    . ~/.nvm/nvm.sh
    </code>
    </li>
    <li>Install node<br>
    <code>
    nvm install node
    </code>
    </li>
</ul>
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