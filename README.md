# temperature-plot
Real-time Temperature Graph using Node.js, Socket.io, Chart.js, Arduino UNO and LM-35 Temperature sensor.

### how to run
Install Arduino IDE. Open temperature.ino file in IDE, connect Arduino board to your PC. In Arduino IDE -> Tools -> Port, see the port name and update it in index.js, Now compile and upload the ino code into Arduino and start Express Server.

To install dependencies:
```npm install```

To run:
```node index```

Go to http://localhost:4000 to see the graph. Or you can open index.html to see the graph. To publically host index.html, host it on any static hosting service.

### working
![Temperature Plot](temperature-plot.gif)

Feel free to fork!


### Things to work on
Store temperature in database, You can use MongoDB, Mongoose to do so.
Show average temperature of last 3 hours 
As user loads the index.html page, send last 15 temperature data points and shift it as new data comes. You can use io.on(‘connection’, (socket) => {…}); to do this.
Feel free to add anything you want!