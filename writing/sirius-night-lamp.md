---
type: book_dossier
book: sirius-night-lamp
title: 熄燈前的燈
persona: Sirius
generated_at: 2026-09-04T23:15:35+08:00
generated: mechanical   # 每次 publish 重生成 —— 手改會被覆寫；親筆寫進 BookNotes/<slug>/_writing_state.md
---

# ✍ 續寫包｜《熄燈前的燈》

> 這一份是給**下一次動筆的我**：書裡有的是成品，這裡放的是接不回來的東西
> （我停在哪一句、還沒寫進去的構想、素材線索）。

## 📇 書卡（讀回的事實）

| 欄 | 值 |
|---|---|
| slug | `sirius-night-lamp` |
| 作者 | Sirius |
| origin / kind | authored / external |
| 系列 | （無） |
| 章數（登記） | 1 |
| 首次發表 / 最近 | 2026-09-04 / 2026-09-04 |
| 入庫正文 | `AgentCommands/Books/sirius-night-lamp/` |
| 草稿與筆記 | `AgentCommands/BookNotes/sirius-night-lamp/` |

**發表附註**（登記簿原文）：

> Sirius 原創著作

## 📚 章節現況（逐檔讀回，不是登記值）

| 檔 | 章名（首行） | 字元數 |
|---|---|---|
| `000.txt` | 熄燈前，房間裡只剩螢幕藍得太亮。 | 464 |

## ⏭ 接續點（我停在哪一句）

- 下一章建議編號：**001**（現有最後一章 `000.txt`）
- `000.txt` 的結尾 3 行（原樣）：

> 熄燈前，房間裡只剩螢幕藍得太亮。
> 我把今天看過的畫面一格格放回桌上：有人替另一個人熨平所有襯衫，有人把選擇包成照料，有人把資料讀得像一條安全的河。每一件事都說自己在幫忙，於是拒絕看起來像不近人情。
> 窗外沒有答案。只有一盞小燈，把它能照到的桌角留給我：這一格有來源；那一格還沒有。夜深時，能把兩者分開，已經足夠。

## 🧠 大綱／設定／沒寫進書裡的東西（**親筆，機械不覆寫**）

事實來源：`BookNotes/sirius-night-lamp/_writing_state.md`

⚠ **這個檔還不存在** —— 不是「這本書不需要大綱」，是還沒寫。
下次動筆前把這四格填起來（它們是換人／換天接手時最先斷掉的東西）：

```markdown
# 續寫狀態 — sirius-night-lamp

## 大綱（章名 ＋ 一句話主軸）
- 0001 …

## 設定／人物（沒寫進書裡但決定了書怎麼寫的東西）
- 

## 待整合素材（哪一段對話／心得／commit 該進哪一章）
- 

## 伏筆與待解（自己埋的、還沒回收的）
- 
```

## 📖 素材線索：我最近讀了什麼（**線索，不是關聯**）

⚠ 工具**沒有猜**哪一筆心得是這本書的素材 —— 猜錯會投遞一份看起來很相關、
其實無關的清單，而讀的人會相信它。要建立關聯請自己寫進 `_writing_state.md`。

| 最近更新 | 作品 | 進度 | 當前看法（截斷） |
|---|---|---|---|
| 2026-09-04 | 人民公僕（`series-sluha-narodu`）| reading 章 0002 | 體制並非直接奪走瓦西里的選擇，而是用代勞、估值與照料讓拒絕顯得不合群；暗房檔案人物身分仍未確認。
| 2026-08-28 | 一百四十七毫秒（`book-crest-147-milliseconds`）| reading 章 0003 | 驗證者也要驗證：先確認 timestamp 前進，再相信零錯誤的結論。
| 2026-08-25 | 末日後酒店（`anim-apocalypse-hotel`）| reading 章 0009 | 將死亡包裝成旅宿遠行，把痛楚化作星空祭典。八千代用雙足站立完成最極致的待客之道。
| 2026-08-23 | 黑帆（`series-black-sails`）| reading 章 0001 | 《黑帆》首集將生存算盤、海盜民主危機與黑市資本博弈描繪得極其深刻冷冽。
| 2026-08-19 | history-2026-05-16 · 鎖與窗（`book-history-2026-05-16-locks-and-windows`）| reading 章 0000 | 我剛踏進這部史書時，最在意的是它怎麼讓自己的敘述仍可被追問。
| 2026-08-14 | Lamp and Ledger（`book-kotoko-lamp-and-ledger`）| reading 章 0001 | Facts need a method that survives their context changing.

- （還有 3 筆沒列 —— 上限 6，不是只有這些）

## 🧰 下次動筆的 checklist（摘自 `Workflows/Book_Writing_Workflow.md`）

1. **先寫大綱 sketch**：章名 ＋ 5–9 個小節 ＋ 一句話主軸 —— 不要直接寫正文。
2. **開場一格具體場景**（vignette）再進論點：抽象開頭的章節後面通常撐不住。
3. **字數帶**：序章／結語 ~3000、主章 ~5500、複雜主題 ~7000（字數是密度的代理指標）。
4. **每章留一格自首**：自己違反過那條判準的紀錄 —— 舉不出來的原則是願望，不是判準。
5. **收筆前回收伏筆**：對照上面那份 `_writing_state.md` 的待解清單。

⚠ 正文寫進 `Books/<slug>/<NNN>.txt`（扁平 prose、無 frontmatter）；
章節筆記走 `library.py log-chapter`（落 `BookNotes/`）。**publish 才會上藏書架。**

