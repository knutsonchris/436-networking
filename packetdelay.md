# Packet Delay

There are exactly four delays:

**(Nodal) Processing Delay**

+ Description: The amount of time needed to process the packet headers, check fot bit errors, and determine the destination host.
+ Where it happens: ***each node, router, or switch***
+ Usually expressed as a constant. For consistency, do not forget to convert to the base unit of seconds.

**Queueing Delay**

+ Description: The amount of time a packet is waiting in the queue (buffer) before it can be pushed to the link. 
+ Where it happens: ***each node, router, or switch***
+ Usually expressed as a constant. For consistency, do not forget to convert to the base unit of seconds.

**Transmission Delay**

+ Description: The amount of time necessary to push all the bits onto the link.
+ Where it happens: ***each node, router, or switch***
+ Formula: (**N**+**p**-1) • (**L**÷**R**)
+ Formula explained: (**N**umber of links + **p**ackets - 1) • (**L**ength of packet (in ***bits***) ÷ **R**ate of transfer (bandwidth in ***bits per second***))

**Propagation Delay**

+ Description: The amount of time it takes the signal's header to travel from the sender to the reciever.
+ Where it happens: ***each link***
+ Formula: **d**÷**s**
+ Formula explained: **d**istance or length (in ***meters***) of the link ÷ **s**peed of the data through the link (in ***meters per second***)

---

The sum of the preceeding delays results in the total end to end delay of a message. Make sure to use the correct units in the equations.

```markdown
| G | Giga  | 1•10^9  |
| M | Mega  | 1•10^6  |
| K | Kilo  | 1•10^3  |
| m | Mili  | 1•10^-3 |
| u | Micro | 1•10^-6 |
| n | Nano  | 1•10^-9 |
```

Be wary of upper and lower case ***b***

1 **B**yte = 8 **b**its

The equations above are in terms of ***bits***

