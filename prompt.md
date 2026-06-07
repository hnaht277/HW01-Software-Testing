# prompt giải thích các defect trong requirement 2
thời gian: 16:00 07/06/2026
tool: gemini

tôi có 20 link về Software Defects 2022–2026 như sau, hãy giải thích từng cái cho tôi và nguyên nhân, hậu quả, giải pháp trong từng bài:
https://www.cbc.ca/news/canada/british-columbia/air-canada-chatbot-lawsuit-1.7116416

https://www.theregister.com/software/2025/07/21/vibe-coding-service-replit-deleted-production-database/719783

https://edition.cnn.com/2024/02/22/tech/google-gemini-ai-image-generator

https://gist.github.com/rain-1/a1ed1116c6da4d2b195e562c8d3f9482

https://www.theguardian.com/technology/2023/jun/23/two-us-lawyers-fined-submitting-fake-court-citations-chatgpt

https://www.eccouncil.org/cybersecurity-exchange/incident-handling/crowdstrike-incident/

https://www.wardsauto.com/news/ford-motor-recalls-4M-trucks-suvs-trailer-module-fseries-nhtsa/814204/

https://cloud.google.com/blog/topics/threat-intelligence/zero-day-moveit-data-theft

https://tanstack.com/blog/npm-supply-chain-compromise-postmortem

https://www.cybersecuritydive.com/news/atlassian-confluence-password-leaked/627941/

https://www.bleepingcomputer.com/news/technology/national-bank-of-canada-online-systems-down-due-to-technical-issue/

https://cloudsecurityalliance.org/blog/2025/07/21/reflecting-on-the-2023-toyota-data-breach

https://blog.cloudflare.com/cloudflare-1-1-1-1-incident-on-july-14-2025/

https://9to5mac.com/2024/05/23/apple-deleted-photos-resurfacing-explanation/

https://blog.lastpass.com/posts/notice-of-recent-security-incident

https://www.cisa.gov/news-events/news/cisa-issues-emergency-directive-mitigate-log4j-vulnerability

https://techjacksolutions.com/scc-intel/microsoft-exchange-online-suffers-recurring-global-mail-flow-failures-pattern-points-to-systemic-infrastructure-instability/

https://globalnews.ca/news/8585468/tesla-recall-self-driving-cars-rolling-stop/

https://waxy.org/2023/07/twitter-bug-causes-self-ddos-possibly-causing-elon-musks-emergency-blocks-and-rate-limits-its-amateur-hour/

https://cybersecuritynews.com/microsoft-365-admin-center-outag/

# output giải thích các defect trong requirement 2:
các hình trong HW01-Software-Testing\images có tên dạng defect1_...png đến defect20_...png

INCOMPLETE do có nhiều chỗ bị hallucination chi tiết trong phần AI Bias/Hallucination in explanation của các defect trong requirement 2 (cần trình bày ra).

# prompt test các case trong requirement 3
thời gian: 12:38 AM 08/06/2026
tool: chatgpt
viết cho tôi 15 test case cho 1 chiếc máy quạt phổ thông, bao gồm đủ các thông tin (Objective / Input / Steps / Expected / Actual / Verdict). Máy quạt không có remote, bật bằng núm vặn 4 mức 0 (tắt), 1, 2, 3. có nút nhấn xuống/kéo lên để bật tắt chế độ quay trái phải. có thể chỉnh đầu quạt gập lên, xuống, có thể điều chỉnh độ cao của quạt.

# output test các case trong requirement 3:
hình HW01-Software-Testing\images\ai_screenshot_testcases-missing1.png và HW01-Software-Testing\images\ai_screenshot_testcases-missing2.png

INCOMPLETE do các test case tạo ra chưa bao gồm các edge case được thêm vào (TC10, TC15, TC16) và cột Test case name/Objective tên chưa ở dạng khẳng định.

student fix: sửa các cột Test case name/Objective, thêm 3 edge case Test case (TC10, TC15, TC16)

# prompt vẽ mindmap:
thời gian: 4:08 AM 08/06/2026
tool: claude

tạo 1 file md và vẽ cho tôi 1 ISTQB QA/QC role mindmap. đặt file ở HW01-Software-Testing

# output vẽ mindmap:
HW01-Software-Testing\ISTQB QA_QC Role mindmap.md

INCOMPLETE vì:

| # | Mistake                                                    | Lý do                                                                                                    |
| - | ---------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- |
| 1 | QA và QC được coi là ISTQB Roles                           | ISTQB định nghĩa Test Management Role và Testing Role, không phải QA/QC role. (syllabus ISTQB CTFL)     |
| 2 | UAT nằm trong Verification Focus                           | UAT chủ yếu là Validation, không phải Verification.                                                      |
| 3 | Test Process Improvement nằm trong CTAL Test Analyst Track | Đây không phải trọng tâm chính của Test Analyst theo CTAL. (syllabus ISTQB CTAL Test Analyst)           |
