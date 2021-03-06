# Alice Build A Cache

Alice P. Hacker has two types of memory that she’s using to build his system in which to store her objects. The first type, type A, is extremely fast, but it’s expensive and she doesn’t have much of it. She has 10GB of type A memory that can being used to store objects, and reading an object from this memory takes 2ms.
 
The second type of memory, type Z, is a lot slower, but it’s cheap, and so Alice bought a lot of it. She has 1TB of the second type of memory that she can use to store objects, and reading an object from this memory takes 500ms.

Alice decides she’s going to build a system where she keeps all of her objects in the second type of memory, and then also keeps copies of some of those objects in the first type so that she can do some of her reads more quickly. Alice has 2048 objects, all of the same size, which use up all of her second type of memory storage. Alice decides to analyze different ways to pick and choose what she keeps in her type A memory, and how they affect her expected object read performance.

Please round all answers to 3 decimal places

If Alice is naive and decides to randomly fill her type A memory with objects and never change it, what is her expected time to read 10 randomly selected objects out of the 2048 (in ms)? ________ ms

Alice now runs a workload where she reads 20 objects per minute. 50% of the objects she reads are objects she's seen in the past 30 seconds, and the other 50% of the objects are randomly chosen from the full 2048. Using the same naive strategy as before, what is her expected average read time for an object with this workload? _________ms

Alice tries to improve her performance. She decides that, every time she reads an object, if it is not in her type A memory, she will put it there. When she needs to remove something, she will remove the thing that she read least recently. What is Alice's average read time per object in the best case scenario? ______ms 

What is Alice's average read time per object in the worst case scenario? _______ms