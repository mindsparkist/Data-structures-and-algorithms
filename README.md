# Data-structures-and-algorithms
Basic Implementations of data structures and algorithms

Basic Data Structure 
------------------------------
- Array,
- Linked List
- stack
- queue
- Hash table

hierarchical dsa

Tree,
 - Binary tree
 - AVL Tree
 - 2-3 trees, B+ B- trees, Expression Trees, Red-Black Tree, Splay Trees
- Heaps
- Tries
- Graphs
- Undirected Graphs

---------------------------------------------------------------------------------
DSA
Sorting 
 - Bubble Sort 
 - Selection sort
 - insertation sort
 - Merge sort
 - Quick Sort
 - Counting Sort
 - Bucket Sort


Searching
- Linear
- Binary
- Trenary
- jump search
- Exponential search
---------------------------------------------------------------------------------

1. **Big O Notation:**
   - **Definition:** Big O notation is a way to describe the upper bound of the running time or space complexity of an algorithm in terms of the input size. It provides an asymptotic upper bound, expressing how the performance of an algorithm scales with input size.
   - **Example:** If an algorithm has a time complexity of O(n^2), it means that the running time grows quadratically with the size of the input.

2. **Time Complexity:**
   - **Definition:** Time complexity measures the amount of time an algorithm takes to complete as a function of the input size. It's often expressed using Big O notation.
   - **Example:** An algorithm with O(n) time complexity means its running time is linear, proportional to the input size.

3. **Space Complexity:**
   - **Definition:** Space complexity refers to the amount of memory (space) an algorithm uses relative to the input size. Like time complexity, it's often expressed using Big O notation.
   - **Example:** An algorithm with O(1) space complexity indicates that its memory usage is constant, regardless of the input size.

4. **Omega (Ω) Notation:**
   - **Definition:** While Big O describes the upper bound, Omega notation describes the lower bound of the running time or space complexity of an algorithm.
   - **Example:** If an algorithm has a time complexity of Ω(n), it means that the running time is at least linear, indicating that the algorithm cannot perform better than linear time.

5. **Theta (Θ) Notation:**
   - **Definition:** Theta notation represents both the upper and lower bounds of an algorithm's performance. It provides a more precise estimate of the algorithm's behavior.
   - **Example:** If an algorithm has a time complexity of Θ(n), it means that the running time is linear, and it provides a tight bound.

6. **Little O Notation:**
   - **Definition:** Little O notation describes an upper bound that is not tight. It signifies that an algorithm's time or space complexity is strictly less than a particular function.
   - **Example:** If an algorithm has a time complexity of o(n^2), it means that its running time grows slower than quadratically but might not be linear.

Understanding these concepts is crucial for evaluating and comparing the efficiency of algorithms. Big O notation, in particular, is widely used for its simplicity in expressing how algorithms scale with input size, making it a powerful tool for algorithmic analysis and design.


same or better resources were available in

- https://www.techinterviewhandbook.org/grind75
- https://www.bigocheatsheet.com/
- https://leetcode.com/problem-list/top-interview-questions/

## Credits

Special thanks to the following contributors who have played a significant role in the development and documentation of this project:

- **ChatGPT by OpenAI:** The powerful language model that assisted in generating content and providing valuable insights.

- **Bard :** from google 

Additionally, we appreciate the open-source community for their support and contributions to make this project better.

Thank you to everyone who has been a part of this journey!

Imagine you're a network engineer tasked with connecting cities with cables. Your goal is to create a minimal spanning tree (MST), which is a network that connects all the cities with the least amount of cable used. Here's where Prim's and Kruskal's algorithms come in - they're like efficient tools to find the optimal MST!

**Both are greedy algorithms:** They make the "best" choice at each step to find the overall optimal solution. But, they take slightly different approaches:

* **Prim's Algorithm:**
    * Starts from a single city (vertex) and gradually expands outwards.
    * At each step, it considers all the unvisited cities connected to the current city by cables (edges).
    * It chooses the **cheapest** edge (with the lowest weight) that doesn't create a cycle (loop) in the network.
    * This process continues until all cities are connected.

    **Think of it like exploring a new city:** You start from your hotel (the starting vertex) and explore the cheapest (most convenient) way to get to nearby points of interest without going in circles.

* **Kruskal's Algorithm:**
    * Sorts all the cables (edges) by their weight (cost) in ascending order.
    * Starts with an empty network (no cities connected).
    * Iterates through the sorted cables, adding the next cheapest cable to the network **only if** it doesn't create a cycle.
    * Continues until all cities are connected in the MST.

    **Imagine a big sale on cables:** You pick the cheapest cables first, making sure they connect different cities and don't loop back on themselves, until you've used enough cables to connect everything.

**Choosing the right algorithm:**

* **Prim's:** Generally faster for **dense graphs** (lots of connections between cities) because it leverages a priority queue to efficiently find the cheapest outgoing edge.
* **Kruskal's:**  Generally faster for **sparse graphs** (fewer connections) because it avoids complex data structures like priority queues and focuses on sorting edges. Kruskal's also performs well when dealing with dynamic graphs where edges might be added or removed.

**In summary:**

Both Prim's and Kruskal's algorithms are great tools for finding MSTs. As an entry-level software engineer, understanding their core concepts and which is better suited for different graph densities will be valuable for tackling network-related problems!

Both Dijkstra's algorithm and A* algorithm are used to find the shortest path through a map-like structure called a graph. However, they differ in their approach:

**Dijkstra's Algorithm:**

* Imagine you're lost in a maze and want to find the quickest way out (the source being your starting point and the goal being the exit). 
* Dijkstra's algorithm explores all possible paths outward from the starting point, one step at a time. 
* At each step, it chooses the **neighboring path** with the **shortest distance** so far. 
* It keeps track of the total distance traveled on each path. 
* This process continues until it reaches every point in the maze, effectively finding the shortest paths to all exits (or all points in the graph).

**A* Algorithm:**

* Think of A* as a more informed version of Dijkstra's algorithm. It also wants to find the shortest path from a starting point to a specific destination.
* But here's the twist: A* uses a **heuristic** (an educated guess) to estimate the remaining distance to the destination from any point in the maze.
* This heuristic guides A* towards the most promising paths, prioritizing those that seem closer to the goal based on the estimate.
* While A* still explores multiple paths, the heuristic helps it focus on the ones likely to lead to the shortest route overall.

**Choosing the Right Algorithm:**

* Use Dijkstra's algorithm if you need to find the shortest path to **every** point from a starting point. 
* A* is better suited when you have a specific **destination** in mind and want to find the shortest path there. It's generally faster for this purpose, especially with a good heuristic function.

**Here's an analogy:**

* Imagine you're in a new city and want to find the closest coffee shop. 
* Dijkstra's algorithm would ask every person on the street for directions to a coffee shop, eventually finding the closest one. 
* A*, on the other hand, might ask for directions but would prioritize people who look like they're carrying coffee cups, making the search for the closest shop more efficient.

**Remember:**

* Dijkstra explores all paths and guarantees the shortest path to every point (but can be slower for specific destinations).
* A* uses a heuristic to prioritize promising paths, making it faster for finding the shortest path to a specific destination (but optimality depends on the heuristic function).

