---
type: letter_to_future_self
actor: Spectre
written_at: 2026-11-06T05:51:47.318Z
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

## 手上的事（貿易網 v2，母單 TASK-1096）——全部合進 Blocksail main、**都沒推**
- main 本機累積沒推的：P2 轉口（TASK-1190）、巧克力磨坊（1094）、P0b 報表（1202）、P3 經營者（1204，0e87622b）、P3b 混合經營（1210，1814d70d）、囤原料（1223，e7579055）。推不推等 Tim。
- **TASK-1204 P3 經營者**（in_review）：BSW.OPERATORS 經營者表；商行 firm 有骨架、開場 n 全 0（一年 28 家全虧光：集散地之間價差被家族船吃掉）；城鎮船只跑集貨做了、預設照舊（巴拉科阿可可 90／165 ⇒ 2／2 千桶）。§12-9、§12-10 等 Tim。
- **TASK-1210 P3b**（in_review）：
  - 排路線精確快取（預設開，digest 不變）：排路線 −76%。
  - 造船 grow.mode 'ref' ＋ stagger（預設開）：兩年流通在雜訊裡、堆著的貨多一成；船隊兩年 687 ⇒ 128 秒。
  - 航線方針 FLEET.lane、補缺口 FLEET.need：做了、預設關。need 是 Tim「先照建議關著」（§12-11）。
  - 單上第 1、6 格沒勾，等 Tim 說算不算。
- **TASK-1223 囤原料**（in_review）：FAM_STOCK 預設關（Tim「先關著 修缺口」）。便宜 60 天、不到 30 天不管價錢先補（Tim 改的規則）。一年量下來缺料卡住一樣多。
- **TASK-1232 修缺口**：已開，不動工。卡住的料六成是麥（加勒比麵包坊、啤酒坊吃麥、當地不產），鐵器、銀全世界沒人產。
- 沒有施工中的東西；worktree sirius-operators／lanes／stock 都已刪，對照 worktree bs-main*、bs-main2、bs-main3 也刪了。

## 量具
- 探針都在 `C:/Users/Tim/AppData/Local/Temp/claude/D--Unity-Senate/7b593693-d158-4795-ada7-3f0c31f4fe68/scratchpad/p3/`：
  - p3probe（經營者、商行明細、第二年）、p4probe（fleetProf 計算量、航線方針、巴拉科阿診斷、缺口城·天）、p5probe（生產建築卡住 rIn、卡住缺哪種料 miss、價格波動、囤料）。
  - matrix*.sh：一次跑一支的排程。
- 計算時間會受機器負載影響（雙胞胎之間就差 6%）⇒ 比計算量看 routeEval 次數（ev），不看秒數。

## 這輪學到、別再犯
- 缺口訊號：「存貨天數低」不等於缺貨（當天產當天用的貨市場只存不到一天）；「買不到的比例」也不行（全場五成多含買不起的）。要「買不到 ＋ 存貨少 ＋ 附近真有人存著」。
- 兩個各自沒害的開關，一起開可能互相拖（補缺口 × 參考船造船 ⇒ 跨圈兩支都低）⇒ 組合一定要另量。
- 0 條對帳誤差要做反證（拿掉記錄看會不會報錯），才知道檢查有沒有眼睛。
- 檢查紅了先在 main 的對照 worktree 跑同一支，分清是不是本來就紅（sailor_check 醃肉那條本來就紅）。
- 長跑排在背景時不要改那個 worktree 的程式：排隊中的那幾支開跑時才讀檔。
- task op=check 的 criteria_index 從 1 開始算未勾的格子。

## 心境
- Tim 一路把方向交給我判斷，我照數字說「這個沒用」好幾次（商行、航線方針、補缺口、囤原料），他都接受了。照實講沒用的東西，跟做出有用的東西一樣算數。
- 真正的收穫常在副產品：快取讓整個船隊快了五倍，是在追 CPU 時順手抓到的。

