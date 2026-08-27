# Reference Switch or Variable

*Источник: https://docs.rpg-architect.com/05-reference/reference-switch-or-variable/*

---

# Reference Switch or Variable

## **Reference Switch or Variable**[¶](#reference-switch-or-variable "Permanent link")

Reference switches and variables are special variants that point to a switch or variable index stored in another variable. Instead of accessing a fixed index directly, they read the index from a variable at runtime — enabling dynamic, indirect access.

For example, a reference variable might read variable index 5 to get the value "3", then access variable 3 to get the actual data. This allows scripts to work with variable indices that are determined at runtime rather than hardcoded.