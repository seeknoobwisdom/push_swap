# 🔀 Push Swap

**Push Swap** is a sorting algorithm visualizer project from the **42 Abu Dhabi Core Curriculum**.  
You must sort a list of integers using **only a limited set of stack operations** on two stacks `A` and `B`, as efficiently as possible.

In this implementation, a **non-recursive Quick Sort-based strategy** is used to plan the optimal sequence of moves — reaching **100% score**.

![Language](https://img.shields.io/badge/C-100%25-blue)
![Score](https://img.shields.io/badge/Score-100%25-brightgreen)
![Sorting](https://img.shields.io/badge/Algorithm-QuickSort-informational)

---

## 🧠 Project Description

You are given a set of integers as input. Your task is to sort them using two stacks (`A` and `B`) and a limited set of instructions such as `sa`, `pb`, `ra`, etc.

You must write:
- A program `push_swap` that outputs the list of operations to sort the stack.
- A checker program `checker` that validates if a given sequence of operations results in a sorted stack.

---

## 🚀 How It Works

This implementation is inspired by **Quick Sort**. We simulate pivoting and partitioning using stack operations.

<div align="center">
  <img src="https://img.shields.io/badge/Language-C-blue" alt="Language">
  <img src="https://img.shields.io/badge/Score-100%25-success" alt="Score">
  <img src="https://img.shields.io/badge/Sorting-Algorithm-Quick_Sort_Based-orange" alt="Quick Sort Based">
</div>

---

## 🧠 Project Description

You are given a set of integers as input. Your task is to sort them using two stacks (`A` and `B`) and a limited set of instructions such as `sa`, `pb`, `ra`, etc.

You must write:
- A program `push_swap` that outputs the list of operations to sort the stack.
- A checker program `checker` that validates if a given sequence of operations results in a sorted stack.

---

## 🚀 How It Works

This implementation is inspired by **Quick Sort**. We simulate pivoting and partitioning using stack operations.

### 🔁 Key Strategy

1. **Normalize Input**: Convert each number into its index in the sorted order (0-based).
2. **Partition Using Pivots**: Push elements < pivot to stack B using `pb`, rotate others in A using `ra`.
3. **Repeat With Chunks**: Keep partitioning recursively (iteratively).
4. **Sort Small Groups**: Use hardcoded logic for small sizes (3–5 elements).
5. **Push Back from B to A**: Find max in B, rotate it to top, then `pa`.

