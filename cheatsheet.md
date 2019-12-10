# DS19 Open Lab | Connecting a Conveyor Belt Simulator to IBM Watson IoT Platform

The below markdown file consists of commands and code snippets that will help you complete and understand the lab - Connecting a Conveyor Belt Simulator to IBM Watson IoT Platform.

## Code Snippets

To install NPM modules
```
npm install
```
To run the application in Conveyor_Belt_Simulator/bin
```
npm start
```
Change the following in VCAP_SERVICES.json,

```
{
  "iotf-service":  [
      {
        "credentials": {
          "org": "<your-Org-ID>",
          "apiKey": "<your-API-KEY>",
          "apiToken": "<your-API-Token>",
		  "serviceName": "internetofthings.ibmcloud.com" 
        },
        "name": "<your-service-name>"
      }
    ]
}
```

Change the following in conveyor-belt.js,

```
var deviceInfo = {
    // You can configure these to your liking, or automate the generation of them
    deviceId:   "",
    typeId:     "<your-device-type>",
    password:   ""
```
