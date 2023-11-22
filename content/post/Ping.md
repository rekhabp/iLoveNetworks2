---
title: "Know Your Command: PING"
date: 2023-11-22T13:16:45+05:30
draft: true
---

Know your command - PING
How a simple command reveals the Network’s secrets…

PING, it sounds exactly like something it does, an Onomatopoeia but it is short for “Packet InterNet Gropper”. We use ping daily to check if we are connected to a device we are trying to reach. It is like throwing chalk at a student in a classroom to check if they are attentive. 
Is that the only thing PING does?
Let’s see what else it tells and can do.

## 1. Checking if we are connected to the device we are trying to reach:

- If we get a reply (Reply from 172.16.1.1: bytes=32 time<1ms TTL=64) then we know we are connected to the network or device we are trying to reach.

![Example Image](/static/ping12.jpg)

- If we do not get a reply instead we get “Destination host unreachable” then we know we are not connected to the network or device we are trying to reach.

- Then in another case we get “Request Timed out” then we know that the destination device did not respond within a certain period of time, this “certain period of time” depends on the Operating system but usually, it is 1 second (1000 milliseconds) by default.
 ## 2. Time taken:
- Bytes: Shows the Payload size (The actual size of the data being sent or received over the network)
- Time: Shows the time taken for a request to reach the destination and receive a reply from the destination.
- TTL: Time-To-Live is the value that a router decrements whenever the packet passes through to avoid the looping of the packing in a network.

## 3. If we start observing the value of “TIME” properly we can see how your network is performing:
- If it ranges from 1ms - 20ms it is in its best condition.
- If it ranges from 20ms - 80ms it is in good condition unless it doesn’t interrupt any of our work.
- If it ranges from 80ms - 120ms it is still in a condition where it will work but you might need to make some efforts to make it better.
- If it goes above 120ms you need to give some serious attention to your network.
- If it goes above 300 you need to fix your network RIGHT NOW.