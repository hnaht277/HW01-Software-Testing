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

- **Gemini** (Google) — used to generate explanations for 20 software defects (2022–2026) from source URLs.
- **ChatGPT** (OpenAI) — used to generate 15 test cases for a physical fan product.
- **Claude** (Anthropic) — used to generate an ISTQB QA/QC Role mindmap.

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

**Prompt #1 Gemini (07/06/2026, 16:00)**
> "tôi có 20 link về Software Defects 2022–2026 như sau, hãy giải thích từng cái cho tôi và nguyên nhân, hậu quả, giải pháp trong từng bài: [20 URLs including Air Canada chatbot, Replit DB deletion, Google Gemini image bias, Auto-GPT crypto drainer, Mata v. Avianca, CrowdStrike BSOD, Ford EV recall, MOVEit SQL injection, TanStack supply chain, Atlassian Confluence, NBC outage, Toyota data leak, Cloudflare DNS, iOS zombie photos, LastPass breach, Log4Shell, Microsoft Exchange Online, Tesla FSD rolling stop, X rate limit, M365 Admin outage]"

*Impact:* Generated all 20 defect explanations and 20 AI explanation screenshots. Output required extensive review, hallucinations identified in Defects 1, 2, 9, 10 and corrected in the final report.

---

**Prompt #2 ChatGPT (08/06/2026, 00:38)**
> "viết cho tôi 15 test case cho 1 chiếc máy quạt phổ thông, bao gồm đủ các thông tin (Objective / Input / Steps / Expected / Actual / Verdict). Máy quạt không có remote, bật bằng núm vặn 4 mức 0 (tắt), 1, 2, 3. có nút nhấn xuống/kéo lên để bật tắt chế độ quay trái phải. có thể chỉnh đầu quạt gập lên, xuống, có thể điều chỉnh độ cao của quạt."

*Impact:* Generated 15 structured test cases with all required columns. Three critical edge cases were missing (TC10, TC15, TC16) and were added manually based on ISTQB Boundary Value Analysis and Equivalence Partitioning principles.

---

**Prompt #3 Claude (08/06/2026, 04:08)**
> "tạo 1 file md và vẽ cho tôi 1 ISTQB QA/QC role mindmap. đặt file ở HW01-Software-Testing"

*Impact:* Generated a hierarchical mindmap of ISTQB roles. Three factual errors were identified and corrected: (1) "QA/QC" are not ISTQB role names; (2) UAT belongs under Validation, not Verification; (3) Test Process Improvement is not a CTAL Test Analyst primary focus. Corrected mindmap produced separately.

---

**4. Specific parts of the work AI contributed to**

- **§Requirement 2 (20 Software Defects):** Gemini generated the initial 20 defect explanations, severity ratings, and AI explanation screenshots. I reviewed each against primary source articles and appended an "AI Bias/Hallucination in explanation" column identifying fabricated details (e.g., Defect 1: fabricated passenger name; Defect 9: wrong attack vector for TanStack supply chain incident; Defect 10: conflated Confluence vulnerability with a separate hardcoded-password vulnerability). I also corrected severity levels where AI was inconsistent with source evidence.

- **§Requirement 3 (Test Cases for Physical Product):** ChatGPT generated 15 test cases for a standing fan with all required columns (Objective / Input / Steps / Expected / Actual / Verdict). I identified and added 3 missing edge cases (TC10: oscillation activated while fan is OFF; TC15: tilt angle exceeds mechanical safe limit; TC16: sudden power interruption during operation). I also renamed all Objective statements to assertive format per ISTQB FL §4.

- **§ISTQB QA/QC Role Mindmap:** Claude generated the initial mindmap. I identified 3 factual errors per ISTQB FL Syllabus §2.2 and CTAL syllabus and produced a corrected version using only ISTQB-accurate role taxonomy.

- **AI did NOT contribute to:** §Requirement 1 (job postings search, screenshots, analysis), execution videos, device photos, AI Critique paragraph, AI Audit Report, or this Disclosure Form.

&nbsp;

---

**5. How I reviewed, revised, or verified the AI output**

My verification strategy combined **source triangulation**, **ISTQB principle cross-checking**, and **systematic gap analysis**:

- **For defect explanations (Gemini):** I read every primary source article cited in each defect entry and compared them against Gemini's output. Any detail present in the AI output but absent from the source article was flagged as a potential hallucination and documented in the "AI Bias/Hallucination in explanation" column. For example, Gemini fabricated "Jake Moffatt" (Defect 1) and mischaracterized the TanStack attack as a credential compromise rather than a GitHub Actions + cache poisoning attack (Defect 9).

- **For test cases (ChatGPT):** I applied ISTQB FL §4.3 (Boundary Value Analysis) and §4.4.1 (Equivalence Partitioning) to identify missing invalid partitions. Specifically, I identified three missing edge cases: TC10 (oscillation at speed 0), TC15 (tilt beyond safe limit), and TC16 (power interruption mid-operation). I also verified each Objective column against the fan's physical specifications to ensure test names were in assertive format.

- **For the mindmap (Claude):** I cross-referenced Claude's output against ISTQB FL Syllabus §2.2 (Test Management Role and Testing Role) and the CTAL Test Analyst syllabus. Any non-ISTQB terminology (e.g., "QA," "QC") or misplaced concepts (e.g., UAT under Verification) was identified and corrected in the final version.

&nbsp;

---

**6. Citation (if required by course style guide)**

Software Testing uses **IEEE style**:

- Anthropic. (2026). *Claude* [Large language model]. https://claude.ai
- Google. (2026). *Gemini* [Large language model]. https://gemini.google.com
- OpenAI. (2026). *ChatGPT* [Large language model]. https://chat.openai.com

&nbsp;

---

## 3. Statement of Honesty

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