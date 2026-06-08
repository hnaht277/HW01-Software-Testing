# AI Use Disclosure Form

**Faculty of Information Technology (FIT)** — Ho Chi Minh City University of Science (HCMUS)  
**CS423 / CSC13003** — Software Testing (AI-augmented · 2026)

---

> **AI POLICY · TEMPLATES — 2026 v1.0**  
> AI Use Disclosure Form  
> Attach to assignments where AI was used in any permitted capacity.  
> Adapted from Med Kharbach, PhD (2026) — *AI Use Policy Templates for Higher Education*. CC BY-NC-SA 4.0.  
> This adaptation is prepared for FIT@HCMUS – CS423 / CSC15003 Software Testing course.

---

## 1. Course & Student Info

| Field              | Value |
| :----------------- | :---- |
| Course            | CS423 / CSC13003 – Software Testing |
| Assignment ID      | HW#01 |
| Assignment Title   | QA/QC Jobs · 20 Defects · Test a Physical Product |
| AI Use Category (1–5) | Category 2 (AI used for brainstorming, drafting, and revision) |
| Date               | 6/8/2026 |
| Student name       | Ngô Hồng Thanh |
| Student ID         | 23127475 |

---

## 2. Disclosure Questions

**1. AI tool(s) used**

- **Gemini** (Google) used to find 10 QA/QC job postings (all links returned 404; manually re-searched); and to generate explanations for 20 software defects (2022–2026) from source URLs.
- **ChatGPT** (OpenAI) used to generate 15 test cases for a physical fan product.
- **Claude** (Anthropic) used to generate an ISTQB QA/QC Role mindmap.
- **ChatGPT** (OpenAI) used to identify 3 factual mistakes in the ISTQB QA/QC Role Mindmap.

---

**2. Stage(s) of the assignment where AI was used**

Tick all that apply:

- [x] Brainstorming
- [x] Outlining
- [x] Drafting
- [ ] Feedback
- [x] Revision
- [ ] Coding
- [ ] Data analysis
- [ ] Visual design
- [ ] Other (specify): \_\_\_\_\_\_\_\_\_\_

&nbsp;

---

**3. Main prompts or tasks given to the AI**

**Prompt #0 — Gemini (07/06/2026, 00:27)**
> "Requirement 1 QA/QC Job Market 2026+ (40 pts): Find 10 QA/QC job postings PUBLISHED WITHIN 60 DAYS of the submission date. Mandatory: ≥ 3 positions REQUIRING AI/LLM/automation-AI skills. Each posting: link, dated screenshot, job description, required skills, salary. Write 1–2 sentences of 'AI Impact Analysis' per posting. tôi có yêu cầu như trên, tìm và đưa link cho tôi"

*Impact:* Generated 10 job listing summaries with links. All 10 links returned 404/not found when accessed, the output was entirely unusable and discarded. I manually searched LinkedIn and company career pages to locate the actual active postings.

---

**Prompt #1a — Gemini (07/06/2026, 01:30)**
> "với yêu cầu: Requirement 2 – 20 Software Defects 2022–2026 (20 pts): Find 20 software defects publicized between 2022 and 2026. Mandatory: ≥ 5 defects related to AI/LLM (hallucination, prompt injection, bias). Each defect: source link, description, severity, consequences, solution. NEW: find 1 place where the AI is biased or hallucinates when explaining the defect. Clarification: this applies to EVERY defect, each of the 20 entries must include 1 identified instance of AI bias or hallucination (20 instances total). tôi chưa hiểu lắm, giải thích yêu cầu lại cho tôi, ý đề kêu tìm lỗi hả, nhưng tìm lỗi của phần mềm gì?"

*Impact:* Gemini correctly clarified that "AI bias/hallucination" refers to the AI *itself* hallucinating false details when explaining each software defect not about finding bugs in AI. The answer helped the student understand that for each of the 20 defects, they must identify where the AI's explanation contained fabricated or biased information vs. what the source article actually states. Output accepted as-is; no correction needed.

---

**Prompt #1 — Gemini (07/06/2026, 16:00)**
> "tôi có 20 link về Software Defects 2022–2026 như sau, hãy giải thích từng cái cho tôi và nguyên nhân, hậu quả, giải pháp trong từng bài: [20 URLs including Air Canada chatbot, Replit DB deletion, Google Gemini image bias, Auto-GPT crypto drainer, Mata v. Avianca, CrowdStrike BSOD, Ford EV recall, MOVEit SQL injection, TanStack supply chain, Atlassian Confluence, NBC outage, Toyota data leak, Cloudflare DNS, iOS zombie photos, LastPass breach, Log4Shell, Microsoft Exchange Online, Tesla FSD rolling stop, X rate limit, M365 Admin outage]"

*Impact:* Generated all 20 defect explanations and 20 AI explanation screenshots. Output required extensive review, hallucinations identified in Defects 1, 2, 9, 10 and corrected in the final report.

---

**Prompt #2 — ChatGPT (08/06/2026, 00:38)**
> "viết cho tôi 15 test case cho 1 chiếc máy quạt phổ thông, bao gồm đủ các thông tin (Objective / Input / Steps / Expected / Actual / Verdict). Máy quạt không có remote, bật bằng núm vặn 4 mức 0 (tắt), 1, 2, 3. có nút nhấn xuống/kéo lên để bật tắt chế độ quay trái phải. có thể chỉnh đầu quạt gập lên, xuống, có thể điều chỉnh độ cao của quạt."

*Impact:* Generated 15 structured test cases with all required columns. Three critical edge cases were missing (TC10, TC15, TC16) and were added manually based on ISTQB Boundary Value Analysis and Equivalence Partitioning principles.

---

**Prompt #3 Claude (08/06/2026, 04:08)**
> "tạo 1 file md và vẽ cho tôi 1 ISTQB QA/QC role mindmap. đặt file ở HW01-Software-Testing"

*Impact:* Generated a hierarchical mindmap of ISTQB roles. Three factual errors were identified and corrected: (1) "QA/QC" are not ISTQB role names; (2) UAT belongs under Validation, not Verification; (3) Test Process Improvement is not a CTAL Test Analyst primary focus. Corrected mindmap produced separately.

---

**Prompt #4 — ChatGPT (08/06/2026, 04:32)**

> "tìm 3 mistake trong ISTQB QA/QC Role Mindmap sau: [mermaid code]"

*Impact:* ChatGPT correctly identified 3 factual mistakes in the Claude-generated mindmap: (1) QA/QC presented as ISTQB roles instead of organizational umbrella terms per FL Syllabus §2.2; (2) UAT placed under Verification instead of Validation per FL Syllabus §1.3; (3) Test Process Improvement misplaced in CTAL Test Analyst Track. All three mistakes cited against ISTQB CTFL 4.0. Output accepted as-is; no corrections needed.

---

**5. Specific parts of the work AI contributed to**

- **§Requirement 1 (Job Postings):** Gemini generated initial 10 job listing summaries with links. All links returned 404/not found — output was entirely unusable. I manually searched LinkedIn and company career pages to locate and verify 10 actual active postings meeting the ≥3 AI/LLM-skill requirement. Screenshots were retaken with my account name visible.

- **§Requirement 2 (20 Software Defects):** Gemini generated the initial 20 defect explanations, severity ratings, and AI explanation screenshots. I reviewed each against primary source articles and appended an "AI Bias/Hallucination in explanation" column identifying fabricated details (e.g., Defect 1: fabricated passenger name; Defect 9: wrong attack vector for TanStack supply chain incident; Defect 10: conflated Confluence vulnerability with a separate hardcoded-password vulnerability). I also corrected severity levels where AI was inconsistent with source evidence.

- **§Requirement 3 (Test Cases for Physical Product):** ChatGPT generated 15 test cases for a standing fan with all required columns (Objective / Input / Steps / Expected / Actual / Verdict). I identified and added 3 missing edge cases (TC10: oscillation activated while fan is OFF; TC15: tilt angle exceeds mechanical safe limit; TC16: sudden power interruption during operation). I also renamed all Objective statements to assertive format per ISTQB FL §4.

- **§ISTQB QA/QC Role Mindmap:** Claude generated the initial mindmap. I identified 3 factual errors per ISTQB FL Syllabus §2.2 and CTAL syllabus and produced a corrected version using only ISTQB-accurate role taxonomy.

- **§Mistake Analysis (Mindmap Review):** ChatGPT correctly identified 3 factual mistakes in the Claude-generated mindmap (find_mistake1.png → find_mistake3.png). All 3 mistakes were cited against ISTQB CTFL 4.0. No corrections needed; output accepted as-is.

- **AI did NOT contribute to:** §Requirement 1 (job postings search, screenshots, analysis), execution videos, device photos, AI Critique paragraph, AI Audit Report, or this Disclosure Form.

&nbsp;

---

**6. How I reviewed, revised, or verified the AI output**

My verification strategy combined **source triangulation**, **ISTQB principle cross-checking**, and **systematic gap analysis**:

- **For job postings (Gemini):** I attempted to access every URL provided by Gemini. All 10 returned 404/not found errors. Per ISTQB FL §2.1 (Test Planning), test artifacts must be traceable to authoritative, live sources — since no link survived validation, the entire output was discarded and replaced with manual search results.

- **For defect explanations (Gemini):** I read every primary source article cited in each defect entry and compared them against Gemini's output. Any detail present in the AI output but absent from the source article was flagged as a potential hallucination and documented in the "AI Bias/Hallucination in explanation" column. For example, Gemini fabricated "Jake Moffatt" (Defect 1) and mischaracterized the TanStack attack as a credential compromise rather than a GitHub Actions + cache poisoning attack (Defect 9).

- **For test cases (ChatGPT):** I applied ISTQB FL §4.3 (Boundary Value Analysis) and §4.4.1 (Equivalence Partitioning) to identify missing invalid partitions. Specifically, I identified three missing edge cases: TC10 (oscillation at speed 0), TC15 (tilt beyond safe limit), and TC16 (power interruption mid-operation). I also verified each Objective column against the fan's physical specifications to ensure test names were in assertive format.

- **For the mindmap (Claude):** I cross-referenced Claude's output against ISTQB FL Syllabus §2.2 (Test Management Role and Testing Role) and the CTAL Test Analyst syllabus. Any non-ISTQB terminology (e.g., "QA," "QC") or misplaced concepts (e.g., UAT under Verification) was identified and corrected in the final version.

&nbsp;

---

**7. Citation (if required by course style guide)**

Software Testing uses **IEEE style**:

- Anthropic. (2026). *Claude* [Large language model]. https://claude.ai
- Google. (2026). *Gemini* [Large language model]. https://gemini.google.com
- OpenAI. (2026). *ChatGPT* [Large language model]. https://chat.openai.com

&nbsp;

---

## 4. Statement of Honesty

> By signing below, I confirm that the disclosure above is accurate and complete. I understand that **undisclosed or false disclosure of AI use is treated as academic misconduct** and may result in a **0 grade** for the assignment and disciplinary referral.

---

## Signature

| Field                  | Value |
| :--------------------- | :---- |
| Student name (printed) | Ngô Hồng Thanh |
| Student ID             | 23127475 |
| Class / Cohort         | CSC13003B |
| Course                 | CS423 / CSC13003 – Software Testing |
| Instructor             | MSc. Trần Thị Bích Hạnh, MSc. Hồ Tuấn Thanh |
| Date                   | 6/8/2026 |
| **Signature**          | Ngô Hồng Thanh |

---

## References

- Kharbach, M. (2026). *AI Use Policy Templates for Higher Education*. CC BY-NC-SA 4.0.
- ISTQB Foundation Level Syllabus (latest version).
- Hardman, P. (2025). A Post-AI Learning Taxonomy.
- Fuster Rabella, M. (2025). *OECD Education Working Paper No. 338*.
- Perkins, M., Roe, J., & Furze, L. (2025). AI Assessment Scale.
- Anthropic (2025). *Building reliable AI test agents* — engineering blog.
- DeepEval & Promptfoo documentation — testing frameworks for LLM systems.