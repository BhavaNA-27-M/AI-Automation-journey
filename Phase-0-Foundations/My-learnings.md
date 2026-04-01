# 📖 Phase 0 — My Learnings

> What I understood, in my own words — with examples and real system designs.

---

## 💡 Key Concepts — In My Own Words

**AI vs ML vs Automation:**
- Automation follows rules I write — it does exactly what I tell it
- ML learns patterns from data — I don't hardcode the rules
- AI is the big umbrella — it can use both

**Workflow:**
- Every system is just Input → Process → Output
- Once I understood this, I started seeing systems everywhere

**API:**
- APIs are how two apps talk to each other
- Without APIs, no automation is possible — they are the bridges

**If/Then Logic:**
- This is the brain of every automation
- Every decision in a system is just: IF something happens → THEN do this

**Data Types:**
- Structured data = tables, easy to process
- Unstructured data = text, images — needs AI to understand

**Error Thinking:**
- Real systems break on edge cases
- Always ask: what if input is empty? What if API fails?

---

## 🏗️ My System Design — Resume Analyzer

> I applied every Phase 0 concept to design a real AI system from scratch.
+-------------------+
|   User Interface  |
|  Upload Resume    |
+-------------------+
|
v
+----------------------------+
| Receive Input              |  ← 0.3 Input
| User ID + Resume File      |
+----------------------------+
|
v
+----------------------------+
| Validate Input             |  ← 0.10 Edge Cases
| - User ID exists?          |
| - File uploaded?           |
| - File type valid?         |
| - File size OK?            |
+----------------------------+
|          |
Error      Valid
|          v
|   +----------------------------+
|   | Store Resume Temporarily  |
|   +----------------------------+
|             |
|             v
|   +----------------------------+
|   | Create API Request         |  ← 0.4 API
|   | Send Resume to AI          |
|   +----------------------------+
|             |
|             v
|   +----------------------------+
|   | Receive AI Response        |
|   | Skills, Experience,Summary |
|   +----------------------------+
|             |
|             v
|   +----------------------------+
|   | Validate AI Output         |  ← 0.5 IF Logic
|   | Skills detected?           |
|   | Summary empty?             |
|   +----------------------------+
|             |
|             v
|   +----------------------------+
|   | Store in Database          |  ← 0.6 Data Types
|   | Structured: ID, skills     |
|   | Unstructured: resume text  |
|   +----------------------------+
|             |
|             v
|   +----------------------------+
|   | Generate Feedback          |  ← 0.9 Intelligent Automation
|   | Send to User               |  ← 0.2 Output
|   +----------------------------+
---

## ✅ Concepts I Applied

| Concept | Where I Used It |
|---------|----------------|
| 0.2 Workflow | Full Input→Process→Output flow |
| 0.3 Input types | User ID + Resume file |
| 0.4 API | Sending resume to AI model |
| 0.5 IF Logic | Validating AI output |
| 0.6 Data types | Structured vs Unstructured storage |
| 0.9 Intelligent Automation | AI-generated feedback |
| 0.10 Edge Cases | File type, size, empty output checks |

---

*Phase 0 complete. Thinking like a system designer.* 🚀
