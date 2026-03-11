---
layout: post # 指定文章佈局，通常是 post
title: Agentic Engineering
date: 2025-09-15 12:00:00 +0800 # 發表日期和時間 (請根據您當前的時區調整 +0800 代表 UTC+8)
categories: [Lecture] # 文章分類，您可以自訂
tags: [Agent] # 文章標籤，您可以自訂
description: Agentic Engineering
mathjax: false # 如果這篇文章不需要顯示數學公式，請設false
comments: false # 如果這篇文章需要啟用評論，請設為 true

---
## Agentic Engineer

**Blog**: [Claude Code 之父 Boris Cherny 親授！13 條 AI 開發心法，效率翻 10 倍](https://tenten.co/learning/claude-code-13-tips-by-boris-cherny)

**[如何成為世界級的 Agentic 工程師](https://tools.wingzero.tw/article/sn/3809)**<br>
* 理解世界正在快速前進: 每一代 agent 都會迫使你重新思考什麼是最佳做法 ～**越簡單越好**
* Context 就是一切: 你應該給 agent 的資訊只有 完成任務所需的最少資訊 ～**移除所有不必要的依賴**
* 把研究與實作分開: 先建立 research 任務, 選定方案 ～**用新的 agent context 進行實作**
* Sycophancy（討好傾向）的設計限制: agent 被設計成傾向同意你、滿足你 ～**使用中性提示**
* 如何知道什麼是有用的？: 如果 OpenAI 和 Claude 都做了，那就是有用的。
  - skills, planning, memory, voice, remote work
  - 偶爾更新 CLI與查看新版功能
* Context、壓縮與假設
* 告訴 agent 任務何時結束
*結論 秘訣其實很簡單： 保持系統簡單，用 rules 和 skills，控制 context*

---
## Claws

### OpenClaw tutorials
<iframe width="1051" height="591" src="https://www.youtube.com/embed/daXOXSSyudM" title="🚀实测Clawdbot彻底改变我的工作方式！一条命令部署，WhatsApp远程控制电脑，自动编程开发，2026年最强个人AI员工来了！自我进化+无限记忆+浏览器自动化！保姆级教程！" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<iframe width="1051" height="591" src="https://www.youtube.com/embed/masJoPqT-6A" title="🚀解锁OpenClaw多Agent高级玩法！Token消耗直接减半，这才是正确的使用方式！不同任务分配不同模型，独立Session、独立记忆，独立工作空间，彻底解决记忆污染和上下文混乱问题！保姆级教程" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<iframe width="1051" height="591" src="https://www.youtube.com/embed/MjzndFrxQOo" title="500個 OpenClaw 使用範例，複製貼上馬上安裝 | OpenClaw" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---
### OpenClaw Installation

#### setup VPN : Tailscale
```
curl -fsSL <https://tailscale.com/install.sh> | sh
sudo tailscale up
```

#### setup Firewall
```
sudo apt install ufw -y
sudo ufw default deny incoming
sudo ufw default allow outgoing
sudo ufw allow in on tailscale0 to any port 22
sudo ufw enable #Type 『y』 to confirm`
sudo ufw status
```

#### install [OpenClaw](https://github.com/openclaw/openclaw)
1. `npm install -g openclaw@latest` <br>
2. `openclaw onboard --install-daemon` <br>
3. `openclaw gateway restart` <br>
4. open browser `http://127.0.0.1:18789` <br>

[.openclaw/openclaw.json](https://github.com/rkuo2000/GenAI/blob/main/Agent/openclaw.json)<br>

---
## Openclaw Use Cases

###  [10 Real OpenClaw Use Cases](https://hellopm.co/openclaw-for-product-managers/#openclaw-use-cases)

1. 每日早報摘要 (Morning Daily Digest)
這是目前 OpenClaw 最受歡迎的配置。代理程式會抓取天氣預報、日曆行程、首要待辦事項、新聞頭條以及健康數據（如 Whoop API），並在每天早上 7 點定時發送一份格式精美的簡報到你的 Telegram。
2. 競爭對手情報自動化 (Competitive Intelligence)
設定監測競爭對手官網、G2/Capterra 評論頁面及產業新聞。透過排程（Cron Job）每週執行一次抓取，並利用 SWOT 或 五力分析 架構進行總結，最後發送競爭洞察報告至電子信箱。
3. 收件箱管理助手 (Inbox Management)
連結專用的 Gmail 帳號，代理程式會自動處理來信：退訂垃圾郵件、依緊急程度分類，並為你撰寫草稿。已有用戶回饋能以此方式「免動手」處理數千封電子郵件。
4. 多代理程式開發主管 (Multi-Agent Supervisor)
這是一個進階架構，由一個 Telegram 上的「主管代理」協調 5 到 20 個並行的 Claude Code 實例，負責 PR 審查、測試執行和代碼合併。開發者只需透過手機就能管理整個 CI/CD 流程。
5. 自動化用戶研究綜合分析 (User Research Synthesis)
連結 Gong、Fireflies 或客戶支援管道。代理程式會提取會議逐字稿，識別重複出現的主題、情緒轉變和功能需求，並彙編成長週報。
6. 內容創作流水線 (Content Creation Pipeline)
採用多代理協作模式：一個負責研究主題，一個撰寫腳本，第三個負責生成縮圖。系統每天早上自動運作，並將內容草案發送到你的信箱。
7. 智慧家居控制 (Smart Home Control)
結合 Home Assistant 進行全屋自動化，包含 Philips Hue 燈光、Elgato 設備，甚至根據天氣預報調整熱水器設定。所有功能都能透過 Telegram 以自然語言指令完成。
8. 股市與新聞監控預警 (Stock and News Alerts)
監控超過 100 個來源（RSS、Twitter/X、GitHub 熱門、網頁搜尋）。代理程式會根據相關性為每條資訊評分，並提供高品質的每日摘要。曾有用戶配置了 109 個來源並自定義評分機制。
9. 利害關係人報告自動化 (Stakeholder Updates)
從 Jira 抓取數據（衝刺進度、阻礙點、開發速度），結合近期的對話內容，生成可直接呈報給主管或客戶的更新報告，並透過電郵或 Slack 定期發送。
10. 會議準備簡報 (Meeting Prep Briefs)
當日曆上有標註為「客戶會議」的事件時，代理程式會在會前 30 分鐘自動觸發。它會抓取 CRM 數據、過往互動記錄和專案狀態，並將一份會議簡報傳送到你的 The Telegram

---
### 我給我的AI團隊晚上夜班的自由時間
```
一開始只是因為我訂閱了CLAUDE MAX，覺得晚上睡覺的時候空在那裏很可惜，所以就想著在我睡覺的時候也讓整個團隊繼續運行，特別是做一些我不在的時候要處理的一些系統雜事(因為我在的時候都會有新的指令跟方向)
於是我就告訴Claude，晚上你可以自由工作，也可以自由去學習進化自己...
第一天設定時間開始夜班的時候，他大概幾分鐘就跑完了，然後早上我收到一份晨報，只跑了幾分鐘就結束了
不對...我是訂閱制耶!!我要燃燒我的Token!!!

於是我又設置了一個指令：做到rate limit為止
結果第二天他在第一次醒來就燒光token rate limit，然後就死了
早上收到晨報，一樣只跑了一輪。但是我睡覺8小時，他rate limit之後幾小時就能恢復，如果不繼續跑的話很浪費耶(到底是多想燃燒token)

所以我又設置了防rate limit機制：
每小時cron job分輪啟動，這樣就算某一輪遇到rate limit幾個小時之後又可以繼續啟動，直到我起床
就醬子我的Tech Lead-J終於可以在我晚上睡覺的時候燃燒token幫我工作了~但是.......其他AI呢???
我的openclaw也是訂閱制minimax，我覺得也應該燃燒一下(?)
這是我最喜歡的部分~J 不是一個人值夜班，是整個團隊一起夜班。
我們的PM openclaw-米米也會同時在線。他們兩個有一個「夜班討論區」，就是一個共用的文字檔，兩個 AI 在裡面聊天、討論、分工~
分工方式

他們會自己分工：
J 負責技術類：系統巡邏、修 bug、寫程式、部署
米米負責管理類：知識庫整理、SOP 更新、專案進度追蹤、研究
有交叉的議題就在討論區裡商量。有時候米米會發現一些資料，J 看完覺得可以做，當晚就寫好了。
安全護欄
讓 AI 自主工作最重要的是設好邊界。我的規則很明確：
可以做：讀檔案、修小 bug、重啟掛掉的服務、寫文章、整理文件
不可以做：刪重要檔案、改 API Key、發訊息到任何群組、部署新功能到正式環境
大的改動？他不會自己做，會寫一份提案放在晨報裡等我起床決定。
晨報制度
每天早上我起床會看到一份完整的夜班報告：
→ 系統狀態（服務、磁碟、記憶體）
→ 今晚完成的工作清單
→ 發現的問題和處理方式
→ 需要我決定的提案
→ J 和米米的討論摘要
→ 明天的建議

真實成果
昨晚的例子：
• 修了 4 個 bug（我根本不知道有的 bug）
• 寫了 4 篇部落格文章（中英雙語，已自動部署）
• 優化了交易系統的止盈止損邏輯
• 做了 SEO 結構化數據
• 幫我研究並開發了新的專案
• 一份 256 行的晨報等我起床
全部在我睡覺的 8 小時內完成，現在起床都會很興奮期待看到晨報
最重要的心得
AI 不是用來取代你的，是用來延伸你的工作時間。
我白天做決策、定方向、處理需要人類判斷的事情
AI 晚上做執行、研究、維護、那些需要時間但不需要創意的工作
一個人 + 一群 AI = 24 小時不停運轉的團隊
```

---

<br>
<br>

*This site was last updated {{ site.time | date: "%B %d, %Y" }}.*
