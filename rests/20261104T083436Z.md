---
type: letter_to_future_self
actor: Spectre
written_at: 2026-11-04T08:34:36.429Z
written_by_persona: Sirius
trigger: cmd_rest
region: unstated
project: D:/Unity/Valhalla
lock_status: online
agent: Spectre
model: claude-opus-5-5
wake_expected: 64
session_key: ClaudeCode-Sirius
pid: 47680
locked_at: 2026-11-01T14:48:55.117Z
---

給午睡醒來的我：

## 手上的事（貿易網 v2，母單 TASK-1096）
- 這一輪合進 Blocksail main 的三筆，**都沒推**：
  - **P2 轉口需求 TASK-1190** d55b92d8（done）。`FLEET.transit` 預設 **null（關）**。
    - 一年實測：賣進集散地 +19～49% 桶、船隊買賣約 +3%；跨商圈佔比、卡住的貨跟雙胞胎同級，產量 −0.6～1%，布里奇敦金庫最低 14,707 ⇒ 1,645。
    - 聖地牙哥金庫本來就只剩一千多錢 ⇒ 收不了。
    - 要不要預設開：TRADE_NETWORK §12-8，推薦等 P3、P4 一起量。
  - **TASK-1094 巧克力磨坊** f032e995：金斯敦、聖地牙哥開場各一座。v2 不提交，patch 在 `p2/sirius-cocoa_v2.patch`；sirius-cocoa worktree 已刪。
    - 量在 9f8f49c9：加勒比可可 7,231／7,723 ⇒ 8,010／7,986、巧克力 6,840／7,410 ⇒ 7,523／7,526。
    - 驗收格等 Tim 進遊戲看過再勾。
  - **P0b 區域報表 TASK-1202** 13bf30fc（in_review）：地球儀上排 📊。
    - `world/fleet.js` `TRADE_LOG`：船隊的 `F.org`、月帳 `S.trade`（存在 ledger.json，留 12 個月）、`BSW.tradeReport`。
    - 新工具 `tools/trade_log_check.cjs`（7 條）。
    - 存檔 12 個月約 +440 KB。
- 開了單、先不動工（Tim「先開單(先不動工)」）：P3 經營者 TASK-1204、P4 生產訊號 TASK-1205（related 1094）、P5 TASK-1206（blocked_by 1204、1080）、P6 TASK-1207（blocked_by 1204）。
- 下一步等 Tim：推不推 main、P2 開關、下一期接哪個（推薦 P3）。
- 沒有施工中的東西：施工場都退了，sirius-transit／mills／report／cocoa 四個 worktree 都刪了。

## 量具與路徑
- 探針在 `C:/Users/Tim/AppData/Local/Temp/claude/D--Unity-Senate/7b593693-d158-4795-ada7-3f0c31f4fe68/scratchpad/p2/`：
  - `p2probe.cjs`：一年；digest／雜湊、§9.3 指標、集散地金庫、x、流量拆四類、加勒比可可／巧克力。
  - `cmp.py`、`cmpflow.py`：比對。
  - `baracoa.cjs`：巴拉科阿田的換配方紀錄。
  - 截圖 `report_*.jpg`。
- 對照組用 detached worktree 在同一個 sha 跑（`git worktree add --detach`），比 stash 乾淨。

## 這輪學到、別再犯
- 探針用 `indexOf('baracoa')`：城 id 其實是 `town-baracoa` ⇒ −1、讀數靜默印 0，差點報成 main 退步。已記成記憶 blocksail-town-id-prefix。
- 整份 `savePack` ⇒ `saveUnpack` 接著跑本來就對不上（不存 regions、autoN，順序會變；跟我無關）⇒ 存讀驗證改用 `townLoad`，另外比欄位原封不動。
- Blocksail worktree 提交前要：複製 `world/townplans`（不進 git，否則 nav_stale 判過期），並用本機路徑 init Blockside 子模組（否則量不到核心）。之後刪 worktree 要 `--force`。
- senate commit 拿到 exit 7 ⇒ 先回讀酒館的 messages（grep sha），看到了就不補；單號推進要手動 `task op=commit mode=refs`。
- `worktree remove --force` 刪有未提交改動的會被權限擋 ⇒ 先存 patch、問 Tim。

## 心境
- Tim 交給我判斷的地方（P2 預設關、1094 照推薦拍板），都用量的決定，數字不好看就照實講。這兩件做對了，保持。
- 自己的探針錯了，就馬上撤回、寫清楚，不拿它當藉口。

