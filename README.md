# Infrastructure-mockup

A repo where I put my crazy ideas about Conceptional networking and infrastructure problems.


#1. Wifi Infrastructure

***

We all know the basics of routing. You have two radiowave signals, where x1 and x2 connects to a base tower x3 where x3 takes care of the distribution of the radiowave signals. Got inspired to write this piece after F8 where they targeted vast areas where they do not have wifi signals.

Let me start with a basic sketch of how it would look. 
***

![Alt-tag](http://s18.postimg.org/aeejz6w7d/Facebook.png)

The main idea here is to capture the side effect of laser routing and send it back to the tower instead of having to send a request to the radio tower. I imagine this would be possible through the intersection of the two laser targets. Instead of sending the actual request to the actual drone, it would calculate the difference between the connections of drones and they'd meet half-way. This allows us to:

1. Send the radiowaves through intersection instead of direct manipulation
2. Catch the side effect of this and send the side effect as a radiowave ping back to the radio-tower.


## Issues:

The feedback/request back to the tower would be hard to secure. It would seem reasonable to create an own frequency with an interpeter to securely transmit without any people trying to be sneaky.

Now, this is the tricky part. How could we manage the intersection points? If done right, that could lead to a high-tweakable mid-station through radiowaves. Problem would be to "fine-tune" signals not to crash with each other while still being able to collide and send a new area of signals. 

##Suggestion

My suggestion would be to have x1 (first signal to mid-base) and x2(second signal to mid-base) to have equal frequency. After collision, we would get interference anyway, but how we could make it not a problem needs to be correctly addressed. Maybe we could end up with something like W : = x1 + x2 / c(b) where c is the strength of the signal and b is the base exponent of the area. This would give us an indication of how we could adjust signals in accordance to area, but at the same time it could lead us to have optimization through machine learning algorithms like unsupervised learning. 

***

## Suggestion v2

Lastly, how are we going to catch these signals? I'd say we still need to to research on this, but my suggestion would be somewhat familiar to this: 

S := x1 + x2 - crazyInterferanceAlgorithm(x1, x2) / c(b)

