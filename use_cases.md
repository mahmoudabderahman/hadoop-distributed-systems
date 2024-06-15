# Case Study Example 1
- Assume we have a file contains 1TB of text lines, and we need to convert the text to be upper case, for example (The -> THE).
- We need to design the program without using any ready distributed system framework.
- You can use any number (n) of machines. Assume n specs are 8 GB of memory, hard desk 128 GB, and 2 cores of CPU.

![image](https://github.com/mahmoudabderahman/hadoop-distributed-systems/assets/30775657/6dc6f44d-3ce1-431d-8b55-af0341df8954)

![image](https://github.com/mahmoudabderahman/hadoop-distributed-systems/assets/30775657/a8507186-fbc8-49b4-9bfa-978a09e04ae0)

![image](https://github.com/mahmoudabderahman/hadoop-distributed-systems/assets/30775657/04b241d8-844a-419c-945f-380c98f85025)

![image](https://github.com/mahmoudabderahman/hadoop-distributed-systems/assets/30775657/7130f28b-2c08-4b2c-bef1-e3047d94b0f9)

![image](https://github.com/mahmoudabderahman/hadoop-distributed-systems/assets/30775657/6e285de8-4c13-46cf-bc05-3f8822c7ac3d)

## Management Box
- How do we distribute the data across the nodes?
- How do we know the number of active nodes (or the status of the node)?
- How do we know if some tasks are stucking?
- How do we track the tasks passed to the nodes?
- What will happen if this box is down? How can we avoid this?
- How do we track the available resources (containers) in our clusters)?

## File System
- How can we store a massive amount of data in distributed systems?
- How can we design a file system which supports highly fault-tolerance?
- Do we require special hardware to design a distributed storage system?
- How can we design storage systems to support distributed processing?

## Data Nodes
- How datanodes continously communicate with the management node?
- How datanodes receive the tasks instructed by the management node?
- Can datanodes store data besides their roles for processing?

# Case Study Example 2
Assume we have a file contains **1TB** of text lines, and we need to calculate the word count across the document, for example, The cat came back the very next day -> (the, 2), (cat, 1), (came, 1), (back, 1), (very, 1), (next, 1), (day, 1).

One of the distributed architecture solutions for this problem is to use **map-reduce**.

## The basic idea of MapReduce
- Assume we need to launch a high-throughput bulk-production sandwich shop.
- This sandwich has a lot of raw ingredients, and our target is to produce the sandwich as quickly as possible. 
- To make the production very quickly we need to distribute the tasks between the **workers**.

We break this into three stages:
- Map
- Shuffle/Group
- Reduce

![image](https://github.com/mahmoudabderahman/hadoop-distributed-systems/assets/30775657/af463a30-161a-4377-82c0-62f43c3b8485)

![image](https://github.com/mahmoudabderahman/hadoop-distributed-systems/assets/30775657/3bb0182f-d7ce-4c7f-9afe-129f0424acdb)

![image](https://github.com/mahmoudabderahman/hadoop-distributed-systems/assets/30775657/0e639700-081c-49ef-9e6d-3d0628db83fb)

![image](https://github.com/mahmoudabderahman/hadoop-distributed-systems/assets/30775657/bf5b6a0f-678e-4e25-92d9-9d08725cb02c)



