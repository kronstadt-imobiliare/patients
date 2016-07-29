# patients

Prerequisites: node.js

    wget https://nodejs.org/dist/v6.3.1/node-v6.3.1-linux-x64.tar.xz

    tar xf node-v6.3.1-linux-x64.tar.xz

    Add node-v6.2.2-linux-x64/bin/ folder to path system variable. 

Install:

    git clone https://github.com/kronstadt-imobiliare/patients.git

    cd patients

    npm install

Compile:

    npm run tsc

Compile & watch for changes:

    npm run tsc:w

Run development server:

    npm start

    (it will run at port 3000)

The development server will inject javascript which will refresh the browser tab every time there is a change in the code (the so-called "Browser-Sync"). 

Also, every client opened will mirror every other! (performing an action on one client will perform the same action on the other clients)

Also, it is slow compared to a real webserver. I recommend the nginx webserver.

In patients.service.ts, the basePath will have to be adjusted according to where the backend is deployed.