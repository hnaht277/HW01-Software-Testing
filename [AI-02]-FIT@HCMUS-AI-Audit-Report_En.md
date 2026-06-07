# AI Audit Report

**Faculty of Information Technology (FIT)** — Ho Chi Minh City University of Science (HCMUS)  
**CS423 / CSC13003** — Software Testing (AI-augmented · 2026)

---

> **AI POLICY · TEMPLATES — 2026 v1.0**  
> AI Audit Report — 5-section Template per Artifact  
> Mandatory appendix for every AI-assisted homework (HW#01–HW#06, and Seminar).  
> Adapted from Med Kharbach, PhD (2026) — *AI Use Policy Templates for Higher Education*. CC BY-NC-SA 4.0.  
> This adaptation is prepared for FIT@HCMUS – CS423 / CSC15003 Software Testing course.

---

## 1. Student Information

| Field                      | Value |
| :------------------------- | :---- |
| Student name (printed)     | Ngô Hồng Thanh |
| Student ID                 | 23127475 |
| Class / Cohort            | CSC13003B    |
| Assignment ID (e.g. HW#00) | HW#01 |
| Assignment date            | 6/8/2026 |
| AI tool(s) used           | ChatGPT, Gemini, Claude |

- **AI tool used?**  [X] Yes  [ ] No

---

## 2. Instructions (read before filling)

- Add **one row per AI-generated artifact** (test case, script, checklist, OpenAPI spec, JMeter plan, etc.).
- Paste the **verbatim prompt** — DO NOT paraphrase.
- Paste the **verbatim AI output** (or include a labelled screenshot in the report).
- Tag the verdict: **VALID / INVALID / INCOMPLETE**.
- Reasoning must cite a **course slide, ISTQB section, or technical RFC**.
- Show the **corrected artifact** with the change highlighted.

> Sample row is in *italic* — replace it before submission.

---

## 3. Audit Table

| # | (1) Prompt + Tool | (2) AI Output | (3) Verdict | (4) Reasoning (ISTQB) | (5) Student Fix |
| :--- | :--- | :--- | :--- | :--- | :--- |
| #1 | **Tool:** Gemini  <br> **Time:** 16:00 07/06/2026  <br> **Prompt:** `"tôi có 20 link về Software Defects 2022–2026 như sau, hãy giải thích từng cái cho tôi và nguyên nhân, hậu quả, giải pháp trong từng bài: [20 URLs]"` | 20 defect explanations (defect1_aircanada_chatbot.png → defect20_microsoft.png) covering AI/LLM defects (1–5) and general system defects (6–20). | `INCOMPLETE` | Per ISTQB FL §4.4.2 (Error Guessing), AI-generated content must be validated against authoritative sources. AI hallucinated specific details not present in source articles (e.g., Defect 1: fabricated passenger name "Jake Moffatt" and "buy-then-refund" instruction; Defect 2: fabricated transfer_funds() function; Defect 9: mischaracterized supply chain attack as credential compromise instead of GitHub Actions + cache poisoning; Defect 10: conflated Confluence vulnerability with Questions-for-Confluence hardcoded password). ISTQB FL §2.1 requires testers to verify traceability between test evidence and requirements a principle that extends to verifying AI output against primary sources. | Each defect entry in §Requirement 2 was corrected with an **AI Bias/Hallucination in explanation** column appended, citing which specific details were fabricated or overstated vs. what the source article actually states. Example fix for Defect 1: removed fabricated "buy-then-refund" instruction; noted that the article only states chatbot offered a post-flight refund claim, not a purchase-first workflow. |
| #2 | **Tool:** ChatGPT  <br> **Time:** 12:38 AM 08/06/2026  <br> **Prompt:** `"viết cho tôi 15 test case cho 1 chiếc máy quạt phổ thông, bao gồm đủ các thông tin (Objective / Input / Steps / Expected / Actual / Verdict). Máy quạt không có remote, bật bằng núm vặn 4 mức 0 (tắt), 1, 2, 3. có nút nhấn xuống/kéo lên để bật tắt chế độ quay trái phải. có thể chỉnh đầu quạt gập lên, xuống, có thể điều chỉnh độ cao của quạt."` | 15 test cases with columns: Objective / Input / Steps / Expected / Actual / Verdict (screenshots: ai_screenshot_testcases-missing1.png, ai_screenshot_testcases-missing2.png). | `INCOMPLETE` | ISTQB FL §4.3 (Boundary Value Analysis) and §4.4.1 (Equivalence Partitioning) require coverage of edge and corner cases. AI generated 15 TCs covering nominal paths but missed ≥3 edge cases: (a) TC10 – oscillation switch activated while fan is OFF (unpowered motor); (b) TC15 – tilt angle beyond safe mechanical limit causing tip-over; (c) TC16 – power interruption mid-operation followed by restore. Per ISTQB FL §2.2, test conditions must include both valid and invalid partitions AI only explored the valid partition. | Added TC10: Oscillation ON while fan speed = 0 (OFF) → Expected: oscillation motor does not activate. Added TC15: Tilt head to maximum tilt angle → Expected: fan should not tip over; verify mechanical stop works. Added TC16: Simulate sudden power loss during operation → Expected: fan stops safely with no unexpected restart. Also renamed all Objective fields to assertive statements (e.g., "Verify fan oscillates when oscillation button is pressed at speed ≥ 1" instead of "Testing oscillation"). |
| #3 | **Tool:** Claude  <br> **Time:** 4:08 AM 08/06/2026  <br> **Prompt:** `"tạo 1 file md và vẽ cho tôi 1 ISTQB QA/QC role mindmap. đặt file ở HW01-Software-Testing"` | ISTQB QA_QC Role mindmap.md — a hierarchical mindmap categorizing ISTQB roles, QA vs QC responsibilities, verification/validation focus areas, and CTAL tracks. | `INCOMPLETE` | ISTQB Foundation Level Syllabus explicitly defines only two role clusters: **Test Management Role** and **Testing Role** (FL Syllabus §2.2). "QA" and "QC" are not ISTQB role names they are organizational umbrella terms. This is a fundamental terminology error. Additionally, ISTQB CTAL Test Analyst syllabus does not make "Test Process Improvement" a primary focus, and UAT belongs under **Validation** (V-Model), not Verification contradicting ISTQB FL §1.3 (Verification vs. Validation distinction). AI conflated industry colloquialisms with ISTQB taxonomy. | Replaced the mindmap with a corrected version using only ISTQB-accurate role terminology: Test Manager (Test Management Role) and Test Analyst / Test Automation Engineer / Test Consultant (Testing Role). Moved UAT from Verification to Validation. Removed Test Process Improvement from CTAL Test Analyst track and relocated it to Test Manager track. Verified against ISTQB FL Syllabus §2.2 and CTAL syllabus. |

---

## 4. Summary of AI Accuracy

| Metric                              | Count | Percentage |
| :---------------------------------- | :---- | :--------- |
| Total AI-generated artifacts audited |   3   | 100 %      |
| **VALID** (correct, accepted as-is) |   0   |   0 %      |
| **INVALID** (wrong; rejected)       |   0   |   0 %      |
| **INCOMPLETE** (acceptable after edits) |  3   |  100 %     |

> **Note:** All 3 artifacts were tagged `INCOMPLETE`. All required student corrections before acceptance.

---

## 5. Conclusion — When should AI be used (or not)?

AI proved highly effective as a **brainstorming accelerator** for generating initial content (defect explanations, test case templates, structural outlines), allowing students to reach a first draft quickly. However, every artifact audited contained at least one factual error or structural gap that required manual correction. The most persistent failure mode was **AI hallucination** fabricating specific details (names, dates, code snippets, technical mechanisms) not present in source articles combined with **terminology imprecision** (e.g., using "QA/QC" instead of ISTQB role taxonomy). AI also systematically missed **edge/corner cases** when generating test cases, focusing on nominal paths and valid partitions while ignoring invalid ones. **Recommendation:** Use AI for ideation and scaffolding, but always validate output against primary sources and apply ISTQB techniques (boundary value analysis, equivalence partitioning, error guessing) manually to cover gaps. AI should never replace the tester's critical judgment or traceability verification step.

&nbsp;

---

## 6. Mandatory Disclosure *(paste verbatim)*

> "Report sections §Requirement 2 (20 Software Defects), §Requirement 3 (Test Cases for Physical Product), and §ISTQB QA/QC Role Mindmap were initially generated by AI tools (Gemini, ChatGPT, Claude); I reviewed and corrected each artifact. For §Requirement 2, I appended an 'AI Bias/Hallucination in explanation' column to each defect entry, identifying fabricated or overstated details against primary source articles. For §Requirement 3, I added 3 missing edge cases (TC10, TC15, TC16) and renamed all Test Case Objectives to assertive statements. For the Mindmap, I identified 3 factual mistakes per ISTQB FL Syllabus §2.2 and CTAL syllabus and replaced the mindmap with a corrected version. The detailed AI Audit Report is attached as Appendix A. I confirm I did not use AI to generate any artifact listed in the prohibited category."

---

## Signature

| Field                  | Value |
| :--------------------- | :---- |
| Student name (printed) | Ngô Hồng Thanh |
| Student ID             | 23127475 |
| Class / Cohort         | CSC13003B |
| Course                | CS423 / CSC13003 – Software Testing |
| Instructor            | MSc. Trần Thị Bích Hạnh, MSc. Hồ Tuấn Thanh |
| Date                  | 6/8/2026 |
| **Signature**         | Ngô Hồng Thanh |

---

## References

- Kharbach, M. (2026). *AI Use Policy Templates for Higher Education*. CC BY-NC-SA 4.0.
- ISTQB Foundation Level Syllabus (latest version).
- Hardman, P. (2025). A Post-AI Learning Taxonomy.
- Fuster Rabella, M. (2025). *OECD Education Working Paper No. 338*.
- Perkins, M., Roe, J., & Furze, L. (2025). AI Assessment Scale.
- Anthropic (2025). *Building reliable AI test agents* — engineering blog.
- DeepEval & Promptfoo documentation — testing frameworks for LLM systems.