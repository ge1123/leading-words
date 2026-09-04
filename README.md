# leading-words

| Leading word | 它暗示 agent 要怎麼做 |
|---|---|
| `vertical slice` | 先做一個端到端可跑的小功能，不要分層鋪太大 |
| `single source of truth` | 不要重複定義同一件事，資料或規則只保留一份權威來源 |
| `human-in-the-loop` | 關鍵步驟要讓人確認，不要 agent 自己一路做到底 |
| `deletion test` | 測試某段文字刪掉後行為有沒有變，沒變就是 no-op |
| `context pointer` | 主文件不要塞滿內容，只放指向外部 reference 的提示 |
| `leg work` | 在某個步驟上多做探索、確認、查證，不要草草帶過 |
| `thin slice` | 做最小但完整的一小段功能 |
| `branch-specific reference` | 只有某個分支才用到的資料，不要放在主 skill 裡 |
| `pruning` | 修剪 skill，刪掉重複、過時、無效內容 |
| `no-op` | 看起來有指令，但實際不影響 agent 行為的內容 |
| `minimal diff` | 只做必要修改，避免不相關的大改或重構 |
| `local patterns first` | 先看現有專案慣例，照既有風格與架構實作 |

# Lightweight prompt

表達方式使用 ascii 加上少量文字，依內容選用表格、卡片、決策樹、類比、時間軸，不需要全部使用，降低抽象形容詞與副詞，優先使用具體名詞、動作與例子，避免過度簡短造成句子破碎，保持完整語意
