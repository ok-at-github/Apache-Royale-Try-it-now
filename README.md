# Apache-Royale-Try-it-now
Apache Royale "Try-it-now" app

1. Installation

Install [NodeJS](https://nodejs.org/en/)  
Install Restify

    npm install restify
    
Instal uuid

    npm install uuid

2. Clone server/server.js from this repo to your local machine

3. Start Restify server

    node server.js

How to use

Send a POST request with your Royale source code as payload:

    POST http://localhost:8080/apache/royale/compiler/targets/html
    
Payload

    {
        "source": "..." 
    }
    
    

Example
    {
    "source":"<?xml version=\"1.0\" encoding=\"utf-8\"?>\r\n<js:Application         xmlns:fx=\"http:\/\/ns.adobe.com\/mxml\/2009\"\r\n\t\t\t\txmlns:js=\"library:\/\/ns.apache.org\/royale\/basic\"\r\n\t\t\t\txmlns:local=\"*\"\r\n\t\t\t\tpageTitle=\"HelloWorld\">\r\n\t\t\t   \r\n\t<js:valuesImpl>\r\n\t\t<js:SimpleCSSValuesImpl \/>\r\n\t<\/js:valuesImpl>\r\n\t\r\n\t<js:initialView>\r\n\t\t<js:View width=\"100%\" height=\"100%\">\r\n\t\t\t<js:List labelField=\"label\">\r\n            <js:beads>\r\n                    <js:VerticalLayoutWithPaddingAndGap gap=\"10\"\r\n            paddingTop=\"10\" paddingRight=\"10\" paddingBottom=\"10\" paddingLeft=\"10\"\/>\r\n    <\/js:beads>\r\n\t\t\t\t<js:dataProvider>\r\n\t\t\t\t\t<fx:Array>\r\n\t\t\t\t\t\t<fx:Object label=\"OneAA\"\/>\r\n\t\t\t\t\t\t<fx:Object label=\"Two\"\/>\r\n\t\t\t\t\t\t<fx:Object label=\"Three\"\/>\r\n\t\t\t\t\t\t<fx:Object label=\"Four\"\/>\r\n\t\t\t\t\t\t<fx:Object label=\"Five\"\/>\r\n\t\t\t\t\t<\/fx:Array>\r\n\t\t\t\t<\/js:dataProvider>\r\n\t\t\t<\/js:List>\r\n\t\t<\/js:View>\r\n\t<\/js:initialView>\r\n\t\r\n <\/js:Application>\r\n"
    }
