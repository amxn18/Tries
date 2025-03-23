# Tries
# 🔠 Tries (Prefix Tree) - DSA

This repository contains the complete implementation and problems related to **Trie Data Structure**, also known as **Prefix Tree**. Tries are an efficient information retrieval data structure used for handling strings, especially in problems involving **search, autocomplete, prefix matching**, and **dictionary-based operations**.

---

## 📌 Contents

### ✅ Trie Implementation (Basic)
- Custom `Node` class using an array of 26 pointers to represent lowercase English letters ('a' to 'z').
- Efficient Trie structure for prefix-based operations.
- Functions:
  - insert(word)        → Inserts a word into the trie.
  - search(word)        → Checks if a word exists in the trie.
  - startsWith(prefix)  → Checks if any word in the trie starts with the given prefix.

### ✅ Implement Trie II (With Count & Erase)
- Extended Trie with frequency tracking for each word and prefix.
- Custom `Node` class maintains:
  - ew → Number of times a word ends at this node.
  - cp → Number of times a prefix passes through this node.
- Functions:
  - insert(word)                  → Inserts a word and updates prefix + end counts.
  - countWordsEqualTo(word)      → Returns how many times the exact word was inserted.
  - countWordsStartingWith(pre)  → Returns how many words start with the given prefix.
  - erase(word)                  → Deletes one occurrence of the word from the trie.


### ✅ Trie Problems Included
| # | Problem Name | Description |
|--|--------------|-------------|
| 1 | **Implement Trie (Prefix Tree)** | Standard problem to implement the core Trie operations (LC/CodingNinjas). |
| 2 | **Longest Word with All Prefixes** | Find the longest word such that all its prefixes also exist in the trie. |
| 3 | **Insert and Search in Trie** | Basic insertion and searching functionality of trie. |
| 4 | **Word Dictionary / Add and Search Word** | Word search with `.` wildcard support. |
| 5 | **Number of Distinct Substrings** | Count the number of distinct substrings using trie. |
| 6 | **Implement Phone Directory** | Return all matching contacts from a dictionary for a given prefix. |
| 7 | **Word Break using Trie** | Solve word break problem using dictionary in a Trie. |
| 8 | **Word Search II (Leetcode Hard)** | Use backtracking with Trie to find all words in a 2D board. |
| 9 | **Replace Words (Prefix Matching)** | Replace words in a sentence using shortest prefix from a dictionary. |

---

## 🧠 Why Tries?

Tries are essential for:
- Fast prefix-based operations (autocomplete, spell checkers)
- Solving string problems in optimal time complexity
- Applications in IP routing, pattern matching, and more

---

## 🛠️ Language & Tools

- Language: C++
- IDE: VS Code / CodeStudio / LeetCode
- Compiled with: GCC (MinGW) / Online Judges

---

## 🚀 How to Use

```cpp
Trie* obj = new Trie();
obj->insert("apple");
bool isWordPresent = obj->search("apple");       // true
bool isPrefixPresent = obj->startsWith("app");   // true
