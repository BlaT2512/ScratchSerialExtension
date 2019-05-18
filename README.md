# ScratchSerialExtension
### Info
This is an edited version from <a href="https://github.com/amandaghassaei/ScratchSerialExtension" target="_blank">amandaghassaei/ScratchSerialExtension</a> to work with the new versions of the required libraries (SerialPort and Socket.io). This project is being maintained.

<img src="https://github.com/amandaghassaei/ScratchSerialExtension/raw/master/screenshot.png" />

This is a Serial Communication extension for Scratch - it allows you to pass serial messages between the scratch interface and any serial device.

### Usage
Serial communication happens through a node.js server that must be running concurrently with scratch.<br>

To run the node server, first install <a href="https://nodejs.org/en/download/">node.js</a>. This will also install the node package manager (npm), use npm into install the following dependencies from the terminal, [serialport](https://www.npmjs.com/package/serialport) and [socket-io](https://www.npmjs.com/package/socket.io):<br>
`npm install -g serialport`<br>
`npm install -g socket.io`

Navigate to the parent directory of this repo in the terminal and run:

`node nodeServer.js`

to start the node server.

The go to this link and accept the warning: http://scratchx.org/?url=https://cdn.jsdelivr.net/gh/Blake-Tourneur/ScratchSerialExtension/serial_port_extension.js#scratch. You will see the block in the **More Blocks** tab.

Alternatively, go to the [Scratch X editor](scratchx.org/#scratch), go to the **More Blocks** tab and click "Load Experimental Extension". Paste in the following link:
<a href="https://cdn.jsdelivr.net/gh/Blake-Tourneur/ScratchSerialExtension/serial_port_extension.js">
https://cdn.jsdelivr.net/gh/Blake-Tourneur/ScratchSerialExtension/serial_port_extension.js</a> Accept the warning, and you will now see all the blocks in the **More Blocks** tab.

I used <a href="https://github.com/LLK/scratchx/wiki#adding-blocks">documentation from the Lifelong Kindergarten Group</a> to set up the Scratch interface for this extension.

There is a sample Arduino sketch in this repo that listens for incoming serial messages and repeats them to test
this Scratch extension. There is also a sample scratch project which can be loaded into ScratchX (File>>Load Project).

### Attribution
Door sound effects from <a href="https://www.freesoundeffects.com/">freesoundeffects.com</a><br/>
Bike Horn sound effect from <a href="http://soundbible.com/1446-Bike-Horn.html">soundbible.com</a><br/>
Swoosh sound effect from <a href="http://soundbible.com/706-Swoosh-3.html">soundbible.com</a>
