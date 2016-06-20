##VCET Against Technology 

NodeJS implementation of Cards Against Humanity.

##Run Locally

Install all the dependencies:

    npm install (you may need to prefix this with sudo if you're on Mac)

Run the app:

    node server.js

Then navigate to `http://localhost:3000`

If you are running the game on a machine with a public static IP address, you can instead navigate to `http://youipordomain.com:3000`

NodeJS runs on port 3000 by default as to avoid conflicting with other HTTP servers. If you want the game to run on port 80 so just a domain or IP is needed, modify `server.js:30`. Simply change the '3000' value to '80'. Make sure to restart Node after making a change; Nodemon will automatically restart when a change is detected.

`server.listen(process.env.PORT || 3000);`

If you want tests to execute every time you change a file:

    jasmine-node ./spec/describe_Game_spec.js --autotest --watch ./game.js

To run the E2E tests you first must install protractor. see: https://github.com/angular/protractor/blob/master/docs/getting-started.md

If you want the server to load up everytime you change the back end:

    npm install -g nodemon

Then run the following instead of `node server.js`:

    nodemon server.js
