# Apache-Royale-Try-it-now

# 1. Installation

Install [NodeJS](https://nodejs.org/en/)  
Install Restify

    npm install restify
    
Instal uuid

    npm install uuid

# 2. Clone server/server.js from this repo to your local machine

# 3. Start Restify server

    node server.js

# 4. How to use

Send a POST request with your Royale source code as payload:

    POST http://localhost:8080/apache/royale/compiler/targets/html
    
Payload

    {
        "source": "..." 
    }
    
Response

    {
        "_id": "216108f0-e36c-11e7-805a-3dbc2fba1d86",
        "projectURL": "http://localhost:8080/static/216108f0-e36c-11e7-805a-3dbc2fba1d86/bin/js-debug/index.html",
        "compilerOutputURL": "http://localhost:8080/static/216108f0-e36c-11e7-805a-3dbc2fba1d86/compilerOutput.txt",
        "errorURL": "http://localhost:8080/static/216108f0-e36c-11e7-805a-3dbc2fba1d86/compilerError.txt"
    }
