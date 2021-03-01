## Laboratory Work nr. 2

# Find an example implementation of the A* algorithm and execute it on your computer.

### Answer the following questions:

• What is A*?

• What are 3 examples where A* could be used?

• What are some alternatives to A*?

• What is a heuristic?

• What is a boid?

Intelligence is the strength of the human species; we have used it to improve our lives. Then, we created the concept of artificial intelligence, to amplify human intelligence and to develop and flourish civilizations like never before. A* Search Algorithm is one such algorithm that has been developed to help us.



### What is A*?

#### A* (pronounced "A-star") is a graph traversal and path search algorithm, which is often used in many fields of computer science due to its completeness, optimality, and optimal efficiency.

A* is an informed search algorithm, or a best-first search, meaning that it is formulated in terms of weighted graphs: starting from a specific starting node of a graph, it aims to find a path to the given goal node having the smallest cost (least distance travelled, shortest time, etc.).

![image](https://user-images.githubusercontent.com/34598802/109414840-e4d6e300-79bd-11eb-8657-182615df59f1.png)

So what exactly is the A* algorithm? It is an advanced BFS algorithm that searches for shorter paths first rather than the longer paths. A* is optimal as well as a complete algorithm. What do I mean by Optimal and Complete? Optimal meaning that A* is sure to find the least cost from the source to the destination and Complete meaning that it is going to find all the paths that are available to us from the source to the destination. 
A* algorithm, on the other hand, finds the most optimal path that it can take from the source in reaching the destination. It knows which is the best path that can be taken from its current state and how it needs to reach its destination.


### What are 3 examples where A* could be used?

A* is brilliant when it comes to finding paths from one place to another. It also makes sure that it finds the paths which are the most efficient.

The A* algorithm also has real-world applications. 
1. An example of an A* algorithm in action where nodes are cities connected with roads and h(x) is the straight-line distance to target point. In this example, edges are railroads and h (x) is the great-circle distance (the shortest possible distance on a sphere) to the target. The algorithm is searching for a path between Washington, D.C. and Los Angeles.
2. A* is often used for the common pathfinding problem in applications such as video games, but was originally designed as a general graph traversal algorithm. 
3. It finds applications in diverse problems, including the problem of parsing using stochastic grammars in NLP (Natural language processing). Other cases include an Informational search with online learning.


### What are some alternatives to A*?

Every set of problem needs to be solved with good efficiency with respect to time and space complexities,in order to achieve these landmarks there are some well defined algorithms are available already.

Some common variants of Dijkstra's algorithm can be viewed as a special case of A* where the heuristic h(n) = 0 for all nodes; in turn, both Dijkstra and A* are special cases of dynamic programming. A* itself is a special case of a generalization of branch and bound.
 
#### Dijkstra’s algorithm

It is very powerful algorithm, even i can say if this algorithm would not be implemented then browsing internet never be much efficient. It is used to find the shortest path between two nodes.Router uses this algorithm in making ip tables.although we have much more better solutions are available today but this algorithm is used so widely.Google maps also uses this algorithm to find the shortest path.

Dijkstra's algorithm to find the shortest path between a and b. It picks the unvisited vertex with the lowest distance, calculates the distance through it to each unvisited neighbor, and updates the neighbor's distance if smaller. Mark visited (set to red) when done with neighbors

In some fields, artificial intelligence in particular, Dijkstra's algorithm or a variant of it is known as uniform cost search and formulated as an instance of the more general idea of best-first search.

The Dijkstra algorithm uses labels that are positive integers or real numbers, which are totally ordered. It can be generalized to use any labels that are partially ordered, provided the subsequent labels (a subsequent label is produced when traversing an edge) are monotonically non-decreasing. This generalization is called the generic Dijkstra shortest-path algorithm.


### What is a heuristic?

Heuristics are the strategies derived from previous experiences with similar problems. These strategies depend on using readily accessible, though loosely applicable, information to control problem solving in human beings, machines and abstract issues.

A heuristic can be used in artificial intelligence systems while searching a solution space. The heuristic is derived by using some function that is put into the system by the designer, or by adjusting the weight of branches based on how likely each branch is to lead to a goal node.

1. A Heuristic function is an evaluation function that estimates the cost of getting from one place to another. It is a way to inform the search about the direction to a goal.
2. Basically, it is the cost calculated while going from the current state to the goal state. 
3. Heuristic function is also simply called as a “Heuristic”.
4. It is generally denoted by “h(n)” where it stands for estimated cost of the cheapest path from current state to goal state. The input is the “search state” whereas the output is the “tangible representation of the state”.
5. The problem state description is mapped to the measure of desirability.
6. The objective of a heuristic is to produce a solution in a reasonable time frame that is good enough for solving the problem at hand. 



### What is a boid?

As with most artificial life simulations, Boids is an example of emergent behavior; that is, the complexity of Boids arises from the interaction of individual agents (the boids, in this case) adhering to a set of simple rules. The rules applied in the simplest Boids world are as follows:

1. separation: steer to avoid crowding local flockmates
2. alignment: steer towards the average heading of local flockmates
3. cohesion: steer to move towards the average position (center of mass) of local flockmates
More complex rules can be added, such as obstacle avoidance and goal seeking.

The movement of Boids can be characterized as either chaotic (splitting groups and wild behaviour) or orderly. Unexpected behaviours, such as splitting flocks and reuniting after avoiding obstacles, can be considered emergent.

The Boids model can be used for direct control and stabilization of teams of simple Unmanned Ground Vehicles (UGV)
The boids model has been used for other interesting applications. It has been applied to automatically program Internet multi-channel radio stations. It has also been used for visualizing information and for optimization tasks.



## A* Algorithm Implimentation
 
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
