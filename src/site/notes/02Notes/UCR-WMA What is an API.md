---
{"dg-publish":true,"permalink":"/02-notes/ucr-wma-what-is-an-api/","tags":["notes/atomic","UCR-WWA"]}
---


API stands for **Application Programming Interface** it is a way for two programs or systems to talk to each other, safely, predictably and without knowing the other's internal details. 

Each api is defined by the following 
 - **Application Protocol**: A protocol is simply a set of rules of the expected behavior for both sides of the party (ex: HTTP)
 - **Format**: The content structure (ex. JSON)

## Kinds of API's

- [[Request Response API\|Request Response API]]: One to One much like a webserver
- [[Publisher-Subscriber\|Publisher-Subscriber]]: A publisher emits messages and subscribers act on each according to some data in the messages like a subject (example: [[02Notes/ROS\|The Robotic Operating System (ROS)]] )
- [[02Notes/UCR-MWA REST API Design Principles\|REST API]] : A restful uses [[02Notes/HTTP\|HTTP]] and a [[02Notes/Client-Server Architecture\|Client-Server Architecture]], it is stateless (each connection is independent), [[02Notes/Cacheable\|Cacheable]] and resources bases. 