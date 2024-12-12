# Lua pairs Iterator Unexpected Behavior
This repository demonstrates an uncommon bug related to the behavior of Lua's `pairs` iterator when tables are modified during iteration. The bug can manifest in unexpected ways, especially with recursive functions.

## Bug Description
The `pairs` iterator in Lua might not correctly handle changes made to the table structure while iterating.  This can lead to skipping elements or causing an infinite loop in recursive scenarios.

## Reproduction
The `bug.lua` file contains the code that showcases the unexpected behavior.  Run this file to observe the issue.

## Solution
The `bugSolution.lua` file provides a solution that uses an alternative approach to iterate through the table and avoid the issue. 

## How to run
1. Save the code in the respective files
2. Run `lua bug.lua` and `lua bugSolution.lua` using a Lua interpreter.