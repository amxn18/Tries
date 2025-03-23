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
| # | Problem Name |
|--|--------------|
| 1 | **Implement Trie (Prefix Tree)** |
| 2 | **Longest Word with All Prefixes (Complete String)** | 
| 3 | **Count Distinct Substrings** |
| 4 | **Maximum XOR of two numbers in an array** |
| 5 | **Word Search II** |
| 6 | **Longest common suffix** |
| 7 | **Replace Words (Prefix Matching)** |
| 8 | **Sum of prefix Scores of strings** |
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
