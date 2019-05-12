# ScratchSerialExtension
### Info:
This is an edited version from <a href="https://github.com/amandaghassaei/ScratchSerialExtension" target="_blank">amandaghassaei/ScratchSerialExtension</a> to work with the new versions of the required libraries (SerialPort and Socket.io). This project is being maintained.

<img src="https://github.com/amandaghassaei/ScratchSerialExtension/raw/master/screenshot.png" />

This is a Serial Communication extension for Scratch - it allows you to pass serial messages between the scratch interface and any serial device.

To run the extension, go to:

<a href="http://scratchx.org/#scratch" target="_blank">scratchx.org</a>

Download this repo, then go to File>>Load Project in Scratch and open the file called SerialDemo.sb2.
Many blocks will initially load up red and undefined, that's ok.

Click "Load Experimental Extension", and paste in the following link:
<a href="https://cdn.jsdelivr.net/gh/Blake-Tourneur/ScratchSerialExtension/serial_port_extension.js">
https://cdn.jsdelivr.net/gh/Blake-Tourneur/ScratchSerialExtension/serial_port_extension.js</a>

Serial communication happens through a node.js server that must be running concurrently with scratch.
To use the node server, first install nodejs:

<a href="https://nodejs.org/en/download/">node.js</a>

this will also install the node package manager (npm), use npm into install the following dependencies from the terminal:

<a href="https://www.npmjs.com/package/serialport">serialport</a><br/>
**npm install -g serialport**<br/>

<a href="https://www.npmjs.com/package/socket.io">socket-io</a><br/>
**npm install -g socket.io**

Navigate to the parent directory of this repo in the terminal and run:

**node nodeServer.js**

to start the node server.

I used <a href="https://github.com/LLK/scratchx/wiki#adding-blocks">documentation from the Lifelong Kindergarten Group</a> to set up the Scratch interface for this extension.

There is a sample Arduino sketch in this repo that listens for incoming serial messages and repeats them to test
this Scratch extension.

**Attribution:**

Door sound effects from <a href="https://www.freesoundeffects.com/">freesoundeffects.com</a><br/>
Bike Horn sound effect from <a href="http://soundbible.com/1446-Bike-Horn.html">soundbible.com</a><br/>
Swoosh sound effect from <a href="http://soundbible.com/706-Swoosh-3.html">soundbible.com</a>
