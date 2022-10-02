# RideText

![Logo](./logo.png)


## Inspiration

This project is inspired by the experience of one of our group member’s transportation issues during his time living in Newfoundland. The cell reception is terrible and the only available mode of transport is a taxi (aside from public buses) which is extremely expensive. Additionally, we were also inspired by our personal experience of running out of data during a trip which caused us great inconvenience (forcing us to walk around in order to look for free wifi) and delayed our journey.

## What it does

RideText is a provider of software for mobility services that simplifies the booking process and improves the accessibility of transportation services (such as taxis and private car services) for lower-income individuals and people living in areas with subpar cell reception. This is possible due to RideText’s 0% commission ride service which will in turn reduce costs for customers by 20 - 25% (average commission fees charged by existing mobility providers such as Uber and Lyft). RideText utilizes a very basic messaging service (SMS) present in every cell phone which will in turn provide a very accessible transportation service to people in rural areas and those living in areas with subpar cell reception. The use of SMS to book a ride is made possible with the integration of Twilio (a software company providing programmable communication tools to make and receive text messages using its web service APIs) in RideText’s system.

## How we built it

The front-end of the system is built using an app design & development tool FlutterFlow. Using FlutterFlow we were able to quickly produce prototypes for the UI design for RideText’s driver application. We also incorporated Firebase for secured authentication and google maps to help our drivers navigate through their journeys.

The backend of the system is built using node js and express framework. It integrates with Twilio API using a webhook to handle SMS sent by customers. It integrates Google Maps API, using Buf for secured and quick query handling, to compute the closest car to the customer. Then it feeds the incoming data to the driver's app using REST API.

## Challenges we ran into

At the start of the project, none of our team was experienced in the use of FlutterFlow as a development tool or Twilio’s APIs. However, after thorough research (and many stack overflow and youtube searches) we managed to figure out how to implement both technologies into our project. The main challenges of this project were mostly due to the use of new technologies.

## Accomplishments that we're proud of

We are extremely proud that despite our geographic and timezone difference, we were able to collaborate and learn about new technologies effectively. This is especially impressive as we have a few members who are brand new to software engineering work.

## What we learned

Through this hackathon project, we’ve learned the basics and some advanced techniques used when designing a UI with the design tool Flutter flow and its integration with firebase. Additionally, we learned how to store user data in firestore real-time database using collection and fields, helping us perform basic CRUD functions related to user data. Through the implementation of GoogleMaps API using Buf, we learned a lot about protocol buffer and about its advantages over rest API and JSON structure. Though we weren’t able to complete implemented google maps functions due to the restricted timeframe, we were able to learn a lot about Buf Schema Registry (BSR) and its build method to implement the needed google maps API. Learning how systems can be automated simply using SMS services like Twilio was interesting as well.

## What's next for RideText

Our next goal for RideText is to explore its viability in the current marketplace (North America). From our initial research before starting this project, we have discovered that no other company provides the same services we are proposing. Due to the lack of competition and market opportunity, we’ve decided to continue developing this project after this hackathon.






Backend server for RideText application.

## Development setup for node-server

Prerequisites:

- Install node.js
- Install mysql
- Install npm
- Install ngrok

```
cd node-server
npm install
npm start
ngrok http 3000
```
