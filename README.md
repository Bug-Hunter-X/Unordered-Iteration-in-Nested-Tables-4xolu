# Lua Nested Table Iteration Bug

This repository demonstrates a common issue in Lua when iterating over nested tables using `pairs`. The `pairs` iterator does not guarantee any specific order, which can lead to unexpected behavior and subtle bugs if the table is modified during iteration. 

The `bug.lua` file contains code that recursively traverses a nested table.  The `bugSolution.lua` shows how to solve this by creating a copy of the table before iterating to avoid modifying the original data during traversal.