# Sample Diagnostic Question Bank

## Subject: Computer Science — Data Structures  
## Design Standard: Bloom's Taxonomy + Distractor Rationale Framework

---

### Q1 — Bloom's Level: Remember

**Topic:** Time Complexity Basics  
**Question:** What is the time complexity of searching for an element in an **unsorted array** of n elements?

| Option | Verdict | Distractor Rationale |
|---|---|---|
| A. O(1) | ❌ | Confusing with hash table lookup; students remember "arrays are fast" |
| B. O(log n) | ❌ | Confusing with **binary search** — which requires a **sorted** array |
| **C. O(n)** | **✅** | Linear scan required; no structure to exploit |
| D. O(n log n) | ❌ | Confusing search complexity with sort complexity |

**Teaching Note:** Students choosing B have learned Binary Search in isolation without the pre-condition (sorted input). Address with: "Binary Search requires sorted data — why?"

---

### Q2 — Bloom's Level: Understand

**Topic:** Recursion  
**Question:** What is the **base case** of a recursive function, and why is it essential?

**Model Answer:** The base case is the condition that stops recursion — without it, the function calls itself infinitely, causing a stack overflow. It defines the simplest sub-problem that can be solved directly without further recursion.

**Common Gap Indicators:**
- Student defines base case correctly but cannot explain why it matters → **Understand gap** (can recall, not explain)
- Student cannot state base case → **Remember gap** → Remediate with factorial/Fibonacci tracing

**Diagnostic Probe:** "Write a recursive function for factorial without a base case. What happens? Why?"

---

### Q3 — Bloom's Level: Apply

**Topic:** Bubble Sort  
**Question:** Trace Bubble Sort on the array `[7, 3, 5, 1]`. Show the array state after each complete pass.

**Expected Output:**
```
Pass 1: [3, 5, 1, 7]   ← 7 bubbles to end
Pass 2: [3, 1, 5, 7]   ← 5 bubbles to position
Pass 3: [1, 3, 5, 7]   ← sorted
```

**Common Errors:**
| Error Pattern | Bloom's Level Missed | Remediation |
|---|---|---|
| Only shows final result, not passes | Apply (can't execute procedure) | Step-by-step trace worksheet |
| Confuses pass count with swap count | Understand (procedure confusion) | Define "pass" explicitly with animation |
| Correct output, wrong order of swaps | Apply (procedural error) | Pair-trace with a partner |

---

### Q4 — Bloom's Level: Analyze

**Topic:** Algorithm Selection  
**Question:** You have an array of 50,000 student names, already **95% sorted** (only a few elements out of place). Which sorting algorithm minimizes the number of comparisons?

| Option | Verdict | Distractor Rationale |
|---|---|---|
| A. Merge Sort | ❌ | Students pick "best" algorithm without considering input characteristics |
| B. Quick Sort | ❌ | Confusing average-case with best-case; Quick Sort is O(n²) on nearly-sorted with bad pivot |
| **C. Insertion Sort** | **✅** | O(n + k) where k = inversions; optimal for nearly-sorted data |
| D. Heap Sort | ❌ | O(n log n) guaranteed, but higher constant; not optimal here |

**Why this is an Analyze question:** Students must decompose the problem (input characteristics) and relate it to algorithm behavior — not just recall complexity tables.

---

### Q5 — Bloom's Level: Evaluate

**Topic:** Data Structure Selection  
**Question:** A mobile app needs to store a dictionary where users frequently look up word definitions and occasionally add new words. Justify your choice: **Hash Table** vs **Binary Search Tree**.

**Strong Answer Criteria:**
- Identifies that O(1) average lookup makes Hash Table favorable for this use case ✅
- Acknowledges BST advantage: alphabetical ordering (relevant for "suggest next word" feature) ✅
- Considers mobile constraints: Hash Table may have worse cache performance on small datasets ✅
- Gives a justified recommendation, not just lists pros/cons ✅

**Weak Answer Pattern:** "Hash tables are faster" — Evaluate-level failure; student cannot weigh trade-offs.

**Remediation:** Trade-off matrix exercise: Given 5 scenarios, justify data structure choice with at least 2 criteria per answer.
