# Intelligent_Waste_Segregator
This project segregates waste into three categories namely Rubbish, Organic and Recyclable.

The project utilizes IBM Watson Speech to Text API for recognizing the name of the waste spoken by the person who threw it in the initial buffer part (entrance) of the dustbin. For prototype purposes, we had used round flaps attached to servo motors as the main flaps. In an outside world ready model, there would be pipes covering the entrance of each separate bin category. The project uses IBM Cloudant NoSQL DB for storing and retrieving the waste name and category. It uses ultrasonic distance sensor for detecting the fill level of each bin. When a specified fill level is reached, another Flow which runs on IBM Cloud (formerly known as Bluemix) continuously monitors the fill level of the bin in the Cloudant database then sends a push notification to our Android app of the fill level along with the respective bin name.

The whole Node-RED flow is available in file IWS FLOW.json that anyone can import in their Node-RED dashboard by copying the text contents of the JSON file. Added other JSON files for database insertion and fill level reporting too.

## YouTube Demo: https://www.youtube.com/playlist?list=PLY0iphzPgzGL-QwMpQGF93zOPtqN5SB3v

### IWS Main Flow:
![IWS Main Flow screenshot](https://github.com/Partiks/Intelligent_Waste_Segregator/blob/master/IWS%20Flow-1.png)
