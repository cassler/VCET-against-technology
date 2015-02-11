##USM Against Humanity

NodeJS implementation of Cards Against Humanity. Here's a screenshot:

##Run Locally

Install all the dependencies:

    npm install (you may need to prefix this with sudo if you're on Mac)

Run the app:

    node server.js

Then navigate to `http://localhost:3000`

If you want tests to execute every time you change a file:

    jasmine-node ./spec/describe_Game_spec.js --autotest --watch ./game.js

To run the E2E tests you first must install protractor. see: https://github.com/angular/protractor/blob/master/docs/getting-started.md

If you want the server to load up everytime you change the back end:

    npm install -g nodemon

Then run the following instead of `node server.js`:

    nodemon server.js