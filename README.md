# 🧮 Valid Parentheses

[LeetCode Problem Link](https://leetcode.com/problems/valid-parentheses/submissions/1737924251/)

---

## 📘 Problem Statement

Given a string containing just the characters `'('`, `')'`, `'{'`, `'}'`, `'['`, and `']'`, determine if the input string is valid.

A string is considered **valid** if:
- Open brackets are closed by the same type of brackets.
- Brackets are closed in the correct order.
- Every closing bracket has a corresponding opening bracket.

---

## 🧠 Approach

This problem is solved using a **stack** data structure:

- Traverse the string character by character.
- Push opening brackets onto the stack.
- For closing brackets, check if the top of the stack matches the corresponding opening bracket.
- If not, return `False`.
- At the end, the stack should be empty for the string to be valid.

---
## 📊 Complexity Analysis

```text
Time Complexity: O(n)
- We iterate through the string once.

Space Complexity: O(n)
- Stack may grow up to the length of the string in worst case.
 ```
## 🧪 Example Test Cases

```python
Input: "()"
Output: True

Input: "()[]{}"
Output: True

Input: "(]"
Output: False

Input: "([)]"
Output: False

Input: "{[]}"
Output: True
