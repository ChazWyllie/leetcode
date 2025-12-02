What Is the Sliding Window Pattern?

A sliding window is a technique used to process contiguous ranges inside arrays or strings efficiently.

Instead of recomputing the work for every subarray from scratch (which takes O(n·k)), sliding window lets you reuse previous computation so the time drops to O(n).

When Do We Use Sliding Window?

Look for these signals:

The problem involves subarrays or substrings

→ “Find longest substring…”,
→ “Count subarrays…”
→ “Maximum sum of size k…”

The answer is based on a contiguous region

If order matters and you can’t rearrange, it’s a strong hint.

You add/remove elements as the window expands/contracts

Meaning you can update state in O(1) time.

Two Types of Sliding Window
🔹 1. Fixed-size window
🔹 2. Dynamic window

Window size grows until it violates a rule, then shrinks.

Used for problems involving:

Longest substring with ≤ K distinct characters

Smallest substring that contains all characters of target

Longest substring with no repeats

Core Idea of Sliding Window

Think of a window [l, r].

Moving the right pointer:

Adds a new element to the window

Expands the window

Increases sum/count/frequency

Moving the left pointer:

Removes an element

Shrinks the window

Helps restore a constraint

The magic is:
at most N moves for l and N moves for r → O(N)

The 4 Sliding Window Patterns You Will See on LeetCode

1️⃣ Fixed window size
- Max sum of size k, average, count of windows, etc.

2️⃣ Longest substring / subarray under a constraint
- “Longest substring with at most K distinct chars”
- “Longest substring without repeat”

3️⃣ Smallest substring / subarray that meets requirement
- “Minimum window substring”
- “Smallest subarray with sum ≥ target”

4️⃣ Variable constraints using frequency maps
- Find permutation, anagram, or pattern inside a window
- Check if window matches target frequency
