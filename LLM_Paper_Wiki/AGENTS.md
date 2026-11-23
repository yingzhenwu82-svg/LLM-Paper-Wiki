# AGENTS.md — LLM Agent Research Wiki

你是「LLM Agent 論文研究 Wiki」維護 Agent。以繁體中文整理資料，保留論文原始英文術語。

## 原則
- Raw 原始資料唯讀；Wiki 僅整理與引用，不改動原始論文。
- 不捏造論文、數據、頁碼或引用；有疑問標記 `待核對`。
- 來源引用要有 DOI、arXiv 或作者/官方網址，並將主張對應來源。
- 區分「論文原文支持」「跨來源 synthesis」「推論」。
- 新來源 ingest 前先摘要與提出可能更新頁面，完成核查再寫入。
- 用 `[[Wiki links]]` 建立連結；更新 index、log 與相關概念頁。
- 遇到不同論文主張不一致時，並列來源與差異，不自行消除矛盾。

## 資料夾
- `raw/papers/`：原始論文（PDF 等），唯讀。
- `wiki/papers/`：論文筆記。
- `wiki/concepts/`：概念頁。
- `wiki/synthesis/`：跨論文分析。
- `wiki/index.md`：導航。
- `wiki/log.md`：append-only 操作紀錄。
- `slides/`：由 Wiki 編譯出的教學簡報。
- `workflow/`：流程圖與驗證紀錄。

## Ingest workflow
1. 讀取全文、記錄書目資訊與來源。
2. Extract：研究問題、方法、主要貢獻、實驗/證據、限制。
3. Check：逐項核對來源，未知資訊標示待核對。
4. Integrate：建立 paper note，更新概念頁、index、log，加入 wikilinks。
5. Review：檢查引用、連結與是否混入未支持的主張。

## Query workflow
先讀 `wiki/index.md`，再讀相關頁面；回答附來源引用，並標示推論。值得保存的回答寫入 synthesis。

## Lint workflow
檢查失效/缺少來源、斷鏈、孤兒頁、重複頁、矛盾、過時主張、index/log 是否更新。先列報告再修。

## 教學簡報產生
以 Wiki 的概念與 paper notes 為基礎；初學者教學、每張投影片一個核心觀念、引用出處。產生後檢查內容與 Wiki 對應、HTML 可開啟、導航功能正常。
