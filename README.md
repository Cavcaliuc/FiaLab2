## Laboratory Work nr. 2

# Find an example implementation of the A* algorithm and execute it on your computer.

### Answer the following questions:

• What is A*?

• What are 3 examples where A* could be used?

• What are some alternatives to A*?

• What is a heuristic?

• What is a boid?




## A* Algorithm
 
1. GENERATE A LIST of all possible next steps towards goal from current position;
 
2. STORE CHILDREN in priority queue based on distance to goal, closest first;
 
3. SELECT CLOSEST child and REPEAT until goal reached or no more children.


## Implementing A* Algorithm In Python

### Creating Base Class
First of all import PriorityQueue from queue. then I have to define a class named as State. This class is basically the base class.

### Creating Sub Class
Create a subclass that will contain two methods GetDistance() and CreateChildren( ) method. 

### Creating A_Star_Solver Sub Class
Create a class where the real magic would be happened. 

### Creating Main Function
Create a final code that actually calls everything that exists. 
