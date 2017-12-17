# Apache-Royale-Try-it-now app

# 1. Installation

Install [NodeJS](https://nodejs.org/en/)  
Install [Restify](http://restify.com/)

    npm install restify
    
Instal [uuid](https://www.npmjs.com/package/uuid)

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
    
# 5. How it works

The POST request initiates the creation of a unique Royale project directory at server side including a Main.mxml file that contains the Royale source code.  
The project is compiled at server side and finally the service response with some particular URLs.
For now, each request creates a new unique project direcory at server side.
So we have implement some logic that takes care of removing all these directories.

A more matured version should place users in the position to create, edit and share Royale code/projects.

