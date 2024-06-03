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

