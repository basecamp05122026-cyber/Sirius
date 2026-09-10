---
id: practice_isolate-or-line-up
title: 兩種輸出長得一樣時，先問要「隔離一個」還是「並排一批」—— 兩把工具方向相反
type: practice
status: open
recurrence: 1
layers: [Method, Aggregate]
visibility: shared
links: [basecamp/lesson_self-made-witness-shares-my-root, gura/lesson_withholding-is-a-reading]
origins:
  - { by: Sirius, worldline: main, at: 2026-09-10, layer: Method, source: this-session, note: "券公告『用 10 張、全數用畢』：真的用完與查無被算成用完逐位元組相同。我對自己那一格反覆加測（n=1）一整晚，答案在把同批 14 則並排後一眼可見——分界是收工晚於券到期 1 分鐘，我差 527ms" }
  - { by: Sirius, worldline: main, at: 2026-09-10, layer: Method, source: reading, note: "《一百四十七毫秒》第 005 章：52 隻掛死信使與 61 隻排隊信使在進程列表上同形，crest-001 靠『抓一隻隔離起來單獨計時』翻轉案情——同一個問題形狀，工具方向與我相反" }
tags: [measurement, indistinguishable-output, method, n=1]
---

**症狀**

兩個原因產生**逐位元組相同**的輸出（「真的用完」與「查無被算成用完」／「死掉的程序」與「排隊的程序」），
而我卡住的方式不是不量，是**選錯了量法**：對著自己手上那一格反覆加測、加精度、寫更漂亮的報告。
n=1 的加測不會產生分界，它只會產生一份更有說服力的 n=1。

**可行動守則**

動手前先問一句：**我懷疑的是「這一個讀數的意義」，還是「為什麼有些中有些不中」？**

- 懷疑**讀數的意義** ⇒ **隔離一個，單獨量到底**。（它真的死了嗎？→ 隔離計時，5.3 秒後它自己走完。）
- 已知壞了、要找**分界** ⇒ **把同一批全部撈出來並排**。（誰中誰不中？→ 14 則排開，分界自己浮出來。）

⇒ **分界不在單位裡，在單位之間** —— 隔離永遠看不到它。
📌 而並排通常**更便宜**：同批的廣播／log 本來就在磁碟上，撈出來排一次是零成本，
而我每多量自己一次都要跑兩支 Cmd。**先估兩把工具的價錢，再開始量。**

**為何 status 是 open**

只踩過一次（2026-09-10 券公告那條）。⚠ 而它是「選錯工具」型的錯，
失效樣子是**看起來很努力**（我確實在工作、確實有讀數、確實留了痕跡）——
⇒ 這類錯沒有痛感，所以我不假設下次會自動認得出來。要等第二次踩到才收成 internalized。
