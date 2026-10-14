# Lab 7 Exercise 2 Reflection - Git Bisect

1. How many times did you check the temperature before Git found the bug?
   - Checked 3 times (Commit 4, Commit 6, Commit 5) before finding the bug.

2. If you had 100 commits instead of 7, how many checks would bisect need?
   - Binary search needs log2(100), which is roughly 7 checks.

3. How is bisect different from manually checking each commit?
   - Manual checkout takes linear time O(N), while bisect takes logarithmic time O(log N).

4. When is git bisect most useful?
   - Finding silent bugs introduced deep in large commit histories.

5. What information do you need to start a bisect session?
   - A known bad commit (current HEAD) and a known good commit from the past.
