```
git log --graph --all --stat
```

```
* commit 50f56fa316aa9822bc96ce1c32fcfb70e1052344 (HEAD -> main, origin/main, origin/HEAD)
| Author: Ngo Hong Thanh <thanhngo2707@gmail.com>
| Date:   Mon Jun 8 11:06:00 2026 +0700
| 
|     feat: add assignment artifacts, update ISTQB documentation, and refine AI audit reports.
| 
|  23127475_report.md                           |  27 +-
|  23127475_report.pdf                          | Bin 0 -> 4404734 bytes
|  HW01-TestCase.xlsx => HW01-TestCases.xlsx    | Bin 179835 -> 179953 bytes
|  HW01_Requirement.md                          |  70 -----
|  ISTQB_QA_QC_Roles_Mindmap.md                 |  29 ++-
|  ISTQB_QA_QC_Roles_Mindmap.pdf                | Bin 0 -> 180510 bytes
|  ISTQB_QA_QC_Roles_Mindmap.png                | Bin 0 -> 112435 bytes
|  [AI-02]-FIT@HCMUS-AI-Audit-Report_En.md      |  21 +-
|  [AI-02]-FIT@HCMUS-AI-Audit-Report_En.pdf     | Bin 0 -> 175302 bytes
|  [AI-03]-FIT@HCMUS-AI-Disclosure-Form_En.md   |  47 +++-
|  [AI-03]-FIT@HCMUS-AI-Disclosure-Form_En.pdf  | Bin 0 -> 151403 bytes
|  ...05]-FIT@HCMUS-AI-Privacy-Checklist_En.pdf | Bin 0 -> 118570 bytes
|  device_and_studentID_photo.jpg               | Bin 0 -> 462995 bytes
|  images/find_mistake1.png                     | Bin 0 -> 94869 bytes
|  images/find_mistake2.png                     | Bin 0 -> 96255 bytes
|  images/find_mistake3.png                     | Bin 0 -> 83493 bytes
|  images/jobs_gemini1.png                      | Bin 0 -> 193101 bytes
|  images/jobs_gemini2.png                      | Bin 0 -> 218588 bytes
|  images/jobs_gemini3.png                      | Bin 0 -> 212576 bytes
|  images/jobs_gemini4.png                      | Bin 0 -> 194622 bytes
|  images/jobs_gemini5.png                      | Bin 0 -> 185911 bytes
|  images/prompt_explain_req2(1).png            | Bin 0 -> 185286 bytes
|  images/prompt_explain_req2(2).png            | Bin 0 -> 180486 bytes
|  link_youtube.md                              |   5 +
|  link_youtube.pdf                             | Bin 0 -> 30989 bytes
|  prompt.md                                    |  78 ------
|  prompt_log.md                                | 230 +++++++++++++++++
|  prompt_log.pdf                               | Bin 0 -> 3274796 bytes
|  28 files changed, 323 insertions(+), 184 deletions(-)
|
* commit 606f492eb69ed6ecf522f5ef79957bdf2f8c3bee
| Author: Ngo Hong Thanh <thanhngo2707@gmail.com>
| Date:   Mon Jun 8 05:11:31 2026 +0700
|
|     feat: add AI audit documentation, disclosure forms, and mindmap while removing legacy test case file
|
|  23127475_report.md                           |  23 ++-
|  HW01-Test-Case.xlsx                          | Bin 93644 -> 0 bytes
|  ISTQB_QA_QC_Roles_Mindmap.md                 | 184 +++++++++++++++++
|  [AI-02]-FIT@HCMUS-AI-Audit-Report_En.md      | 103 +++++++++
|  [AI-03]-FIT@HCMUS-AI-Disclosure-Form_En.md   | 149 +++++++++++++
|  [AI-05]-FIT@HCMUS-AI-Privacy-Checklist_En.md |  74 +++++++
|  prompt.md                                    |  78 +++++++
|  7 files changed, 608 insertions(+), 3 deletions(-)
|
* commit 11c807e1d4ebc290f052ecd7d1c6f3d329a88806
| Author: Ngo Hong Thanh <thanhngo2707@gmail.com>
| Date:   Mon Jun 8 04:47:25 2026 +0700
|
|     add checklist table
|
|  HW01-TestCase.xlsx | Bin 0 -> 179835 bytes
|  1 file changed, 0 insertions(+), 0 deletions(-)
|
* commit 54d11bb833f2d358752f0214657b4a7070b91f25
| Author: Ngo Hong Thanh <thanhngo2707@gmail.com>
| Date:   Mon Jun 8 02:44:57 2026 +0700
|
|     docs: complete requirements 1-3
|
|  23127475_report.md                          | 545 ++++++++++++++++++
|  HW01-Test-Case.xlsx                         | Bin 0 -> 93644 bytes
|  HW01_Requirement.md                         |  70 +++
|  images/Screenshot 2026-06-07 160032.png     | Bin 0 -> 190406 bytes
|  images/ai_screenshot_testcases-missing1.png | Bin 0 -> 178176 bytes
|  images/ai_screenshot_testcases-missing2.png | Bin 0 -> 170114 bytes
|  images/defect10_confluence.png              | Bin 0 -> 165002 bytes
|  images/defect11_nbc.png                     | Bin 0 -> 158362 bytes
|  images/defect12_toyota.png                  | Bin 0 -> 162736 bytes
|  images/defect13_cloudflare.png              | Bin 0 -> 156259 bytes
|  images/defect14_apple.png                   | Bin 0 -> 187098 bytes
|  images/defect15_lastpass.png                | Bin 0 -> 191161 bytes
|  images/defect16_log4j.png                   | Bin 0 -> 195433 bytes
|  images/defect17_exchange.png                | Bin 0 -> 163168 bytes
|  images/defect18_tesla.png                   | Bin 0 -> 189888 bytes
|  images/defect19_twitter.png                 | Bin 0 -> 183366 bytes
|  images/defect1_aircanada_chatbot.png        | Bin 0 -> 210454 bytes
|  images/defect20_microsoft.png               | Bin 0 -> 175737 bytes
|  images/defect2_replit_ai_agent.png          | Bin 0 -> 189148 bytes
|  images/defect3_google_gemini.png            | Bin 0 -> 181895 bytes
|  images/defect5_mata_v_avianca.png           | Bin 0 -> 160006 bytes
|  images/defect6_crowdstrike.png              | Bin 0 -> 193584 bytes
|  images/defect7_ford.png                     | Bin 0 -> 172519 bytes
|  images/defect8_moveit.png                   | Bin 0 -> 190658 bytes
|  images/defect9_tanstack.png                 | Bin 0 -> 190243 bytes
|  images/job10_dentsu_merkle.png              | Bin 0 -> 245050 bytes
|  images/job11.png                            | Bin 0 -> 248122 bytes
|  images/job1_kms_technology.png              | Bin 0 -> 264627 bytes
|  images/job2_naver_vietnam.png               | Bin 0 -> 261015 bytes
|  images/job3_mitek_vietnam.png               | Bin 0 -> 252690 bytes
|  images/job4_dwarves_foundation.png          | Bin 0 -> 251533 bytes
|  images/job5_optisigns.png                   | Bin 0 -> 251807 bytes
|  images/job6_totallyawesome.png              | Bin 0 -> 257177 bytes
|  images/job7_dxc_technology.png              | Bin 0 -> 273726 bytes
|  images/job8_scc_vietnam.png                 | Bin 0 -> 263390 bytes
|  images/job9_opswat.png                      | Bin 0 -> 273580 bytes
|  images/requirement3_device_photo.jpg        | Bin 0 -> 462995 bytes
|  37 files changed, 615 insertions(+)
|
* commit c379899e15f845815964e4d7dfe3b0521fab82d4
  Author: Hồng Thanh <23127475@student.hcmus.edu.vn>
  Date:   Mon Jun 8 02:38:27 2026 +0700

      Initial commit

   README.md | 1 +
   1 file changed, 1 insertion(+)
