# 📐 Technical Curriculum Assets

> **Structured STEM Question Banks, Curriculum Maps & Progression Frameworks**  
> Designed for JEE/NEET preparation and competitive CS exam coaching.

![LaTeX](https://img.shields.io/badge/LaTeX-TikZ-008080?logo=latex)
![Bloom's Taxonomy](https://img.shields.io/badge/Pedagogy-Bloom's%20Taxonomy-blue)
![UbD](https://img.shields.io/badge/Design-Backward%20Design%20(UbD)-orange)
![License](https://img.shields.io/badge/License-CC%20BY%204.0-green)

This repository contains publication-ready curriculum materials built on **Backward Design (UbD)** principles, with every question mapped to **Bloom's Taxonomy** cognitive levels.

---

## 📂 Repository Structure

```
technical-curriculum-assets/
├── bloom-taxonomy-mapping.md        # CS unit: Bloom's level mapping
├── sample-question-bank.md          # Diagnostic questions with distractor rationales
├── curriculum-map-template.md       # Unit → Topic → Outcome → Assessment map
├── latex-templates/
│   └── question-paper-template.tex  # LaTeX template for typeset question papers
└── README.md
```

---

## 🎯 Curriculum Design Philosophy

All materials follow a **three-stage backward design**:

```
Stage 1: Identify Desired Results
  → What should students KNOW, UNDERSTAND, and be able to DO?
  → Mapped to Bloom's Taxonomy (Remember → Create)

Stage 2: Determine Acceptable Evidence
  → Diagnostic questions that reveal UNDERSTANDING, not just recall
  → Distractor analysis: Why does a student choose the wrong answer?

Stage 3: Plan Learning Experiences
  → Scaffolded practice pathways
  → Remediation resources for each misconception
```

---

## 📊 Sample Bloom's Taxonomy Mapping (Computer Science — Sorting Algorithms)

See [`bloom-taxonomy-mapping.md`](bloom-taxonomy-mapping.md) for the full table.

| Bloom's Level | Cognitive Verb | Sample Learning Outcome | Sample Assessment |
|---|---|---|---|
| **Remember** | Recall, List | List the steps of Bubble Sort | MCQ: What is the time complexity of Bubble Sort? |
| **Understand** | Explain, Describe | Explain why Merge Sort is stable | Short answer: Describe the role of the pivot in Quick Sort |
| **Apply** | Execute, Implement | Trace through Merge Sort on [5,3,8,1] | Trace: Show the array state after each pass |
| **Analyze** | Differentiate, Compare | Compare time complexity of Merge vs Quick Sort | Given input characteristics, identify the optimal algorithm |
| **Evaluate** | Justify, Critique | Justify choice of algorithm for a linked list | Design question: Which sort is best for nearly-sorted data? Why? |
| **Create** | Design, Construct | Design a hybrid sorting algorithm | Project: Implement a cache-optimized sort |

---

## 🧩 Sample Question Bank

See [`sample-question-bank.md`](sample-question-bank.md) for full diagnostic questions with rationales.

### Example Diagnostic Question (Bloom's: Analyze)

**Topic:** Sorting Algorithms  
**Q: An array of 10,000 nearly-sorted integers needs to be sorted. Which algorithm minimizes comparisons?**

| Option | Answer | Distractor Rationale |
|---|---|---|
| A. Quick Sort | ❌ | Students confuse average-case O(n log n) with worst-case behavior on sorted arrays |
| B. Merge Sort | ❌ | Students pick this for stability, ignoring extra space overhead |
| **C. Insertion Sort** | **✅** | O(n) for nearly-sorted data — the correct reasoning requires Analyze-level thinking |
| D. Heap Sort | ❌ | Students confuse guaranteed O(n log n) with optimal for this specific case |

**Teaching Note:** This question catches students who have only **remembered** complexity values without **analyzing** when each algorithm performs best.

---

## 🗺️ Curriculum Map Template

See [`curriculum-map-template.md`](curriculum-map-template.md) for the full template.

| Unit | Topic | Learning Outcome (Bloom's) | Assessment Method | Resource |
|---|---|---|---|---|
| Unit 1: Arrays | Array traversal | Remember — Recall iteration syntax | Quiz (5 MCQ) | Worksheet W1 |
| Unit 1: Arrays | 2D array indexing | Understand — Explain row-major order | Short answer | Worksheet W2 |
| Unit 2: Sorting | Bubble Sort | Apply — Trace algorithm on given array | Trace exercise | Worksheet W3 |
| Unit 2: Sorting | Algorithm selection | Analyze — Compare complexities | Case study problem | Problem Set P1 |
| Unit 3: Trees | BST operations | Apply — Insert/delete in BST | Diagram exercise | Worksheet W4 |
| Unit 3: Trees | Tree traversal | Analyze — Predict traversal output | MCQ + Trace | Problem Set P2 |

---

## 📋 How to Use These Materials

1. **Start with the curriculum map** — identify the unit and target Bloom's level
2. **Use diagnostic questions** to reveal concept gaps before teaching
3. **Match remediation** to the specific Bloom's level where the gap exists (don't teach higher-order before lower-order is mastered)
4. **Use distractor rationales** to design targeted re-teaching moments

---

## 👨‍💻 Author

**Manish Bhatta** — Technical Learning Designer & CS Curriculum Architect  
Founder, Expert Classes Rourkela | 6+ years in STEM curriculum design

📧 manishbhatta2013@gmail.com | 💼 [LinkedIn](https://www.linkedin.com/in/manishbhatta)

---

## 📄 License

[Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/)  
You are free to use, adapt, and share these materials with attribution.
