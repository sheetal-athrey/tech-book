# Cloud

## History

- place all code onto 1 computer. Vertical Scaling - Increase size of computer (eg. more storage, more stuff that can be done at a given moment in time, less idle compute). Turns out this is expensive and complicated.
- separation of concerns. database and compute.
- redundancy. multiple databases, multiple compute.
- idempotency. same call yields same result every time. Thus, a single computer does not need to know about previous requests. eg. I ask herd of computers to tell me the best milk brand. A random computer in the herd gets the request tells you the best milk brand. If multiple computers got that request than all the computers would tell you the best milk brand. You would care about the first reply, and simply ignore the second. If the first computer failed to tell you the best milk brand, then you can just again without worrying about that first failure. Thus, you can just add in tons and tons of computers to the heard without worrying about whether a single specific computer will work. With enough computers in the herd, you are guaranteed that users can eventually get their questions answered.
- all the above lead to horizontal scaling. Instead of increasing the size of the computer, you get tons of computers and create multiple herds of them. Each herd has its own responsibilities. This allows you to handle more and more requests with cheap, super easy to control computers.


## Timesharing

library. you checkout a computer when you need it. you return it when you are done. a central company can handle the whole making sure that we are aware of where computers are. You get charged very only the small period of time you use the computer, versus having to buy an entire computer and basically have it sitting idle most of the time.

## Moving compute to storage

lots and lots of data.

Within a computer, you have CPUs which do stuff. You then have memory which is just information that your computer knows about. You move the information to the CPUs and the CPU does stuff with it.

Cloud turns this model around. You have lots of information and moving it around is expensive. So, you don't. Instead, you move your CPUs from one large data set to another and have it do compute there.   

## Networking

- VPC. computers that can talk to each other.

## Value

- pay for what you use
- design as you go
- lots of freebies/best practices already provided to you by central provider. eg. security. <-- THIS POINT IS VERY INTERESTING FOR POLICY MAKERS.
- economies of scale of central provider

## Big players

AWS, Azure, GCP, OCI
