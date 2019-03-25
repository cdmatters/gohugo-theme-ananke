---
date: 2017-04-09T10:58:08-04:00
description: "a poker bot server in C++" 
paragraph: "a poker server in C++ to allow bots to play each other over a ZMQ sockets" 
featured_image: "/images/smithers.png"
tags: ["C++", "infrastructure", "ZMQ", "smithers/monty"]
title: "smithers"
---
Smithers is a poker bot server in C++. It allows your bots to play poker against each other very fast over a network. It is implemented in C++, partly as an exercise, partly as a learning opportunity in learning a low level stack, and partly because it's fast.

In terms of its structure, Smithers is composed of a configuration for a mongrel2 server (which hooks up the http/websockets requests to ZeroMQ endpoints) and an executable which communicates with those endpoints and effectively runs the game. The central server deals out cards and broadcasts all messages to players, while also handling the game logic. 

You can watch a very naive game between bots (prerecorded and slowed down to human-viewing speed) [here](/pdfs/smithers/).

## Write Up Coming Soon

### The Stack

* C++
* ZMQ
* websockets
* Docker

### [Github](https://github.com/condnsdmatters/smithers)