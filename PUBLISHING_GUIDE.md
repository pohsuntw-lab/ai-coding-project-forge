# EW AI Coding v0.8.1 發佈說明 / Publishing Guide

## 繁體中文

### v0.8.1 這次要驗證什麼

EW AI Coding v0.8.1 修正三張提示卡的語言一致性；每張卡都同時提供英文與繁體中文，並保持在 128 字元限制內。v0.8.0 的完整 AI 應用鍛造能力維持不變。

公開前至少完成以下驗證：

1. **一般想法模式**：使用者只說一句生活、學習或工作想法，系統能一次一題完成需求澄清，不強迫回答企業級問題。
2. **SOP／流程模式**：上傳 SOP、程序書、流程圖或工作描述後，先分析哪些任務適合做成應用，而不是直接把整份流程程式化。
3. **重複工作模式**：能辨識輸入、規則、輸出、人工判斷、例外與驗收方式，並指出最適合先做的第一版。
4. **雙語一致性**：繁體中文與英文都能完成同等品質的引導、摘要、五份文件與後續交接。
5. **五份規格一致性**：`PRODUCT.md`、`ARCHITECTURE.md`、`ACCEPTANCE.md`、`AGENTS.md`、`START_CODEX.md` 必須互相一致。
6. **交付平台**：Web、Windows、macOS、Linux、Android、iPhone/iPad 等交付目標不可由系統自行假定；會影響架構時必須先確認。
7. **Codex 後續流程**：Codex 完成後，EW AI Coding 應從 GitHub、測試、預覽、驗收、授權發布與價值驗證中第一個未完成階段繼續，而不是重新訪談。
8. **安全停止條件**：公開發布、付費服務、憑證、敏感資料、不可逆操作與高風險決策必須要求明確授權或人工確認。
9. **一般使用者優先**：個人、學習、旅行、生活與創作者用途都是一級場景；只有實際需要時才加入企業治理要求。

### 三張提示卡

ChatGPT 入口維持三張卡，不把所有功能塞進卡片。建議文案：

1. `I'm an individual user. I want to... / 我是一般用戶，我想要……`
2. `I'm a business user. I want to... / 我是企業用戶，我想要……`
3. `I've finished coding. What should I do next? / 我已完成 Coding，下一步該怎麼做？`

### 品牌與圖示

- 對外主名稱固定為 **EW AI Coding**。
- 副標可使用：`AI Application Project Forge / AI 應用專案鍛造工具`。
- v0.8.1 沿用銀色系 Embodied Worker 大象商標。
- GitHub `plugin.json` 與 ChatGPT 後台顯示名稱、版本、提示卡與圖示應保持一致。

### 建議發布順序

1. 確認 GitHub `SKILL.md` 與 `plugin.json` 已為 v0.8.1。
2. 將新版銀色 Embodied Worker 圖示替換 `assets/icon.png`。
3. 用至少三個真實案例測試：一般想法、SOP／流程分析、Codex 完工後續作。
4. 確認五份文件一致性及安全停止條件。
5. 在 ChatGPT 外掛後台同步最新 GitHub 版本與圖示。
6. 重新檢查三張提示卡與公開說明。
7. 提交審核；通過後再正式公開。

## English

### What v0.8.1 must validate

EW AI Coding v0.8.1 fixes language parity across the three starter cards. Every card now includes both English and Traditional Chinese and remains within the 128-character limit. The complete v0.8.0 application-forging workflow remains unchanged.

Before publication, validate at least these cases:

1. **Ordinary idea mode** — a user can start with one natural-language idea and proceed one question at a time without unnecessary enterprise governance.
2. **SOP/workflow mode** — the system analyzes which tasks are worth turning into applications instead of converting the whole procedure directly into software.
3. **Repetitive-task mode** — identify inputs, rules, outputs, human judgments, exceptions, and acceptance evidence, then recommend a practical first version.
4. **Bilingual parity** — Traditional Chinese and English provide equivalent guidance, summaries, five-file output, and handoff quality.
5. **Five-file consistency** — `PRODUCT.md`, `ARCHITECTURE.md`, `ACCEPTANCE.md`, `AGENTS.md`, and `START_CODEX.md` agree with each other.
6. **Delivery target** — Web, Windows, macOS, Linux, Android, iPhone/iPad, or other packaging must not be silently assumed when it changes implementation.
7. **Post-Codex continuation** — resume from the first incomplete stage among GitHub, testing, preview, acceptance, authorized release, and value verification instead of restarting the interview.
8. **Safety stops** — public release, paid services, credentials, sensitive data, irreversible actions, and high-risk decisions require explicit authorization or human approval.
9. **General-purpose positioning** — personal, learning, travel, lifestyle, and creator use cases remain first-class; enterprise controls are added only when required by the actual scope.

### Publishing sequence

1. Confirm GitHub `SKILL.md` and `plugin.json` are v0.8.1.
2. Replace `assets/icon.png` with the approved silver Embodied Worker elephant mark.
3. Test at least three real cases: ordinary idea, SOP/workflow analysis, and post-Codex continuation.
4. Verify five-file consistency and safety stop conditions.
5. Sync the latest GitHub version and icon in the ChatGPT plugin backend.
6. Recheck the three conversation starters and public description.
7. Submit for review and publish only after approval.
