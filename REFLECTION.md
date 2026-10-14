# Lab 7 Exercise 2 Reflection - Git Bisect

### 1. How many times did you have to check the temperature before Git found the bug?
- I checked the temperature 3 times (Commit 4, Commit 6, and Commit 5) before Git pinpointed the exact commit.

### 2. If you had 100 commits instead of 7, about how many checks would bisect need?
- Binary search uses log2(N). For 100 commits, Git bisect would only need about 7 checks (2^7 = 128).

### 3. How is bisect different from manually checking each commit with git checkout?
- Manual checking requires reviewing commits one by one sequentially. `git bisect` cuts the search area in half at every step, saving significant time.

### 4. When would git bisect be most useful in real projects?
- It is most useful in large codebases with long commit histories where a bug or regression was introduced silently at an unknown time.

### 5. What information do you need to start a bisect session?
- You need a known bad state (usually current HEAD) and at least one known good commit in the past where the bug did not exist.
