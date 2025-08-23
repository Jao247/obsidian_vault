---
date: 2024-11-04T12:52
tags: 
linked-tags:
  - "[[Factorio]]"
  - "[[Game Info]]"
---
Based on info from [[04-11-24 1259 Factorio Train Logistics|LTS in 2.0]]

# Logic
Make use of interrupts in order to send the trains around. All trains of the same length can be used to satisfy a station.

## Systems
- Requester
	- sends out a negative signal of the resource it is requesting.
	- sends a train limit to the station to 1 when resources are requested
	- sends a signal when the train is on the way and removes the negative signal 
- Provider
	- when it can fill a train sets a train limit to 1.
	- sends a positive resource signal to the global network.
- Depot
	- Use a clock to space out trains being sent off.
		- 60 x depots


Rail base has been designed, now just the design needs to be implemented to allow me to conquer Nauvis, [[Space Age - Fulgora|Fulgora]] is not a good planet design for conquering with this as it requires a different train system. It makes more use of the elevated rails and those elevated rails must go between platforms. Without the extra research into the elevated rails support it is impossible to produce a proper attempt at the system.