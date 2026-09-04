# Data Structures & Algorithms (DSA) in C++

A comprehensive, production-ready repository dedicated to mastering core Data Structures and Algorithms implemented in C++. Designed for computer science students, competitive programmers, and engineers preparing for technical coding interviews.

---

## 📌 Repository Features

- **Modern C++ Standards:** Written using clean C++17/C++20 practices, standard template library (STL) interoperability, and RAII principles for memory management.
- **Generic & Modular Implementations:** Class templates (`template <typename T>`) allow data structures to work seamlessly with arbitrary data types.
- **Complexity Annotations:** Every implementation includes explicit **Big-O** Time and Space complexity analysis in the docstrings.
- **Exception Safety & Memory Cleanliness:** Utilizes smart pointers (`std::unique_ptr`, `std::shared_ptr`) where appropriate to prevent memory leaks and dangling references.

---

## 🗂️ Table of Contents

1. [Data Structures](#-data-structures)
2. [Algorithmic Paradigms](#-algorithmic-paradigms)
3. [Repository Layout](#-repository-layout)
4. [Getting Started & Compilation](#-getting-started--compilation)
5. [Complexity Quick Reference](#-complexity-quick-reference)
6. [Contributing](#-contributing)
7. [License](#-license)

---

## 🧱 Data Structures

### 1. Linear Data Structures
- **Vectors & Dynamic Arrays:** Custom implementation of a dynamically resizing vector class (`Vector<T>`).
- **Linked Lists:**
  - Singly Linked List (`SinglyLinkedList<T>`) — Insertion, Deletion, Reversal, Cycle Detection (Floyd's algorithm).
  - Doubly Linked List (`DoublyLinkedList<T>`).
- **Stacks & Queues:**
  - Stack (`Stack<T>`) & Queue (`Queue<T>`) via Array & Linked List backings.
  - Circular Queue & Deque (`Deque<T>`).
  - Priority Queue built on custom Min/Max Binary Heaps.

### 2. Non-Linear Data Structures
- **Trees:**
  - Binary Search Tree (`BST<T>`) — Insertion, Deletion, Traversals (In-order, Pre-order, Post-order, Level-order).
  - Self-Balancing Trees: AVL Tree (`AVLTree<T>`) & Red-Black Tree (`RedBlackTree<T>`).
- **Heaps:** Min-Heap & Max-Heap (`heapify`, `extractTop`, `decreaseKey`).
- **Graphs:**
  - Graph representations using Adjacency List (`std::unordered_map<T, std::vector<T>>`) and Adjacency Matrix.
  - Traversals: Breadth-First Search (BFS) and Depth-First Search (DFS).
- **Advanced Structures:** Trie (`Trie`), Segment Tree (`SegmentTree`), Disjoint Set Union (`DSU` / Union-Find).

---

## ⚙️ Algorithmic Paradigms

- **Sorting Algorithms:**
  - Quick Sort, Merge Sort, Heap Sort, Radix Sort, Tim Sort.
- **Searching & Binary Search:**
  - Lower bound, Upper bound, Searching in rotated sorted arrays, Binary search on answer space.
- **Two Pointers & Sliding Window:**
  - Subarray problems, maximum sum windows, container with most water.
- **Dynamic Programming (DP):**
  - 1D/2D DP: 0/1 Knapsack, Unbounded Knapsack, Longest Common Subsequence (LCS), Edit Distance, Matrix Chain Multiplication.
- **Graph Algorithms:**
  - Shortest Path: Dijkstra, Bellman-Ford, Floyd-Warshall.
  - Minimum Spanning Tree (MST): Kruskal's (DSU) and Prim's algorithm.
  - Topological Sort (Kahn's Algorithm & DFS).

---

## 📂 Repository Layout

```text
dsa-in-cpp/
├── data_structures/
│   ├── linear/           # Arrays, Vectors, Linked Lists, Stacks, Queues
│   ├── trees/            # BST, AVL Tree, Segment Tree, Trie
│   ├── heaps/            # MinHeap, MaxHeap
│   └── graphs/           # Graph representations, DSU
├── algorithms/
│   ├── sorting/          # QuickSort, MergeSort, HeapSort
│   ├── searching/        # Binary Search variants
│   ├── dynamic_programming/
│   └── graph_algorithms/ # Dijkstra, MST, Topological Sort
├── include/              # Shared header template definitions (.hpp)
├── tests/                # Unit test drivers (`assert` or GoogleTest)
└── README.md
