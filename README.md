# LRU Cache Visualization – Python GUI Project

An interactive implementation and visualization of an **LRU (Least Recently Used) Cache** using **Python** with **CustomTkinter** GUI. This project showcases how LRU cache works internally using a doubly linked list and a dictionary — suitable for educational demos, system design interviews, and algorithmic exploration.

---

## 📌 Project Overview

This project simulates and visualizes:
- Real-time **cache operations (get/put)**
- **Hit/miss tracking**
- Cache capacity handling with **eviction policy**
- Internal **doubly linked list updates**
- Terminal + optional GUI (CustomTkinter) feedback

It is built using clean **OOP design**, and demonstrates how LRU caches are built from scratch without using `OrderedDict` or `functools.lru_cache()`.

---

## ⚙️ How LRU Works in This Project

- Uses a **DoublyLinkedList** to track the order of access.
- Uses a **Python dictionary** for O(1) access to cache entries.
- On `get(key)`:
  - If hit: moves the node to the front (MRU position)
  - If miss: returns -1 and records a miss
- On `put(key, value)`:
  - If key exists: updates value and moves to front
  - If not:
    - Inserts at front
    - If capacity exceeded: evicts **tail node** (LRU)

---

## 🖥️ GUI & Terminal Output

- `CustomTkinter` can be used to visually show:
  - Cache hits/misses
  - Current cache state as a list
  - Stats (total access, miss rate)
- Console version prints cache states and logs in clear format

---

## 💻 Getting Started

### Run Locally

```python
https://github.com/Muhammad-Zunain/LRU-Cache-Project
cd LRU-Cache-Project
pip install customtkinter CTkMessagebox
python LRU.py
```
---
## 📸 Screenshots

#### LRU Cache
![image](https://github.com/user-attachments/assets/8418b29c-8a03-4d47-807d-a2b9439a47ce)

![image](https://github.com/user-attachments/assets/26d30ba0-8a30-428c-be7d-13f667903808)

#### Cache Miss
![image](https://github.com/user-attachments/assets/af74843b-6e5d-4688-bc6c-765a17836af6)

#### Cache Hit
![image](https://github.com/user-attachments/assets/17358d5f-be1b-452d-b5e2-516b14da03ba)


