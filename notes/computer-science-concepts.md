**Big O**

![](https://github.com/kylpo/dev-playbook/blob/master/assets/big-o.png?raw=true)

*No clue where I took this from long ago, sorry!*

**Primitive Data structures**: their operations, what types they store, complexities of the operations
- Array
  - a contiguous block of memory containing elements of the same type, accessed by numeric index
  - indexing: O(1)
  - search: O(n)
  - space: O(n)
- Singly-Linked List
  - indexing: O(n)
  - Search: O(n)
  - insertion: O(1)
  - deletion: O(1)
  - space: O(n)
- Doubly-Linked List
  - indexing: O(n)
  - Search: O(n)
  - insertion: O(1)
  - deletion: O(1)
  - space: O(n)
- Tree
  - An abstract data type that stores elements hierarchically
  - parent, children, ancestors

**ADT**: Their inputs/outputs, operations, complexities of the operations
- Hash Table
  - Search: O(n)
  - insertion: O(n)
  - deletion: O(n)
  - space: O(n)
- Binary Search Tree
  - indexing: O(n)
  - Search: O(n)
  - insertion: O(n)
  - deletion: O(n)
  - space: O(n)
- B-Tree
  - indexing: O(log(n))
  - Search: O(log(n))
  - insertion: O(log(n))
  - deletion: O(log(n))
  - space: O(n)
- Red-Black Tree
  - indexing: O(log(n))
  - Search: O(log(n))
  - insertion: O(log(n))
  - deletion: O(log(n))
  - space: O(n)
- Trie
- Binary Heap
- Heap
  - An efficient realization of a priority queue allowing insertion removal in logarithmic time
- Queue
  - A collection of objects that are inserted and removed according to the FIFO principle
  - Priority Queue
    - An abstract data type for storing a collection of elements that supports arbitrary element insertion but removal of elements is based on priority
    - array
    - bin heap
- Map
  - A collection of key-value pairs, where each key is unique
- Hash Table/Map
  - Map implementation consisting of a bucket array and a hash function, good if you have an idea of maximum size
- Stack
  - A collection of objects that are inserted and removed according to the LIFO principle
- Terms:
  - Hash Function
    - Maps each key k in our map to an integer
  - Collision
    - When two or more keys are mapped to the same hash value
  - Compression Function
    - Maps the hash code to an integer within range

**Graphs**:
- Adjacency List
  - Storage: O(|V| + |E|)
  - Add Vertex: O(1)
  - Add Edge: O(1)
  - Remove Vertex: O(|V| + |E|)
  - Remove Edge: O(|E|)
  - Query: O(|V|)
- Adjacency Matrix
  - Storage: O(|V| + |E|)
  - Add Vertex: O(1)
  - Add Edge: O(1)
  - Remove Vertex: O(|E|)
  - Remove Edge: O(|E|)
  - Query: O(|E|)
- Spanning Tree
  - Spanning sub-graph that is also a tree
- Forest
  - Graph with no cycles
- Tree
  - A connected forest

**ADT Data structures**: their operations, what types they store, complexities of the operations

**Algorithms**: complexities, inputs and outputs
- Sorting
  - Bubble Sort
    - DS: Array
    - Time Complexity: O(n^2)
    - Auxiliary Space Complexity: O(1)
  - Insertion Sort
    - DS: Array
    - Time Complexity: O(n^2)
    - Auxiliary Space Complexity: O(1)
  - Mergesort
    - DS: Array
    - Time Complexity: O(n log(n))
    - Auxiliary Space Complexity: O(n)
  - Quicksort
    - DS: Array
    - Time Complexity: O(n^2)
    - Auxiliary Space Complexity: O(n)
  - Selection Sort
    - DS: Array
    - Time Complexity: O(n^2)
    - Auxiliary Space Complexity: O(1)
  - Heapsort
    - DS: Array
    - Time Complexity: O(n log(n))
    - Auxiliary Space Complexity: O(1)
- Graphing
  - Binary Search
    - DS: Sorted array of n elements
    - Time Complexity: O(log(n))
    - Space Complexity: O(1)
  - BFS
    - DS: Graph of |V| vertices and |E| edges
    - Time Complexity: O(|V| + |E|)
    - Space Complexity: O(V)
    - **Dijkstra’s**
  - DFS
    - DS: Graph of |V| vertices and |E| edges
    - Time Complexity: O(|V| + |E|)
    - Space Complexity: O(V)
    - **Prim’s**
  - Shortest path by Dijkstra, using a Min-heap as priority queue
    - DS: Graph of |V| vertices and |E| edges
    - Time Complexity: O((|V| + |E|) log |V|)
    - Space Complexity: O(|V|)
  - Shortest path by Dijkstra, using an unsorted array as priority queue
    - DS: Graph of |V| vertices and |E| edges
    - Time Complexity: O(|V| ^2)
    - Space Complexity: O(|V|)
  - Shortest path by Bellman-Ford
    - DS: Graph of |V| vertices and |E| edges
    - Time Complexity: O(|V| |E|)
    - Space Complexity: O(|V|)
  - MST
    - Prim’s
    - Kruskal’s



**Problems**: NP-____
- Traveling Salesman Problem
- Euclid’s

**Patterns**:
- Singleton
- Abstract Factory
- Factory Method
- Facade
- Adapter
- Strategy
- Factory
- Visitor
- Builder
- Observer
- MVC
- Observer

To go over:
- generics

Implement:
- DFS
  - recursive
  - iterative
- BFS
  - iterative
- Fibonanacci
  - recursive
  - iterative
- Factorial
  - recursive
  - iterative