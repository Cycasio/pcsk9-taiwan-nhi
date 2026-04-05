# 🇹🇼 台灣 PCSK9 抑制劑健保給付 — 臨床 SOP 與工具

> **Taiwan NHI PCSK9 Inhibitor Reimbursement — Clinical SOP & Tools**

[![License: CC BY-SA 4.0](https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-sa/4.0/)
[![NHI Version](https://img.shields.io/badge/健保版本-114%2F9%2F1-blue.svg)](#)

台灣臨床醫師申請 PCSK9 抑制劑（Repatha / Praluent）健保事前審查的**實戰 SOP、計算工具、與快速參考指引**。

## 📋 目錄

| 檔案 | 說明 |
|------|------|
| [SOP — 事前審查申請流程](docs/sop-prior-auth.md) | 完整申請步驟、條件檢核、常見失敗原因 |
| [快速參考卡](docs/quick-reference.md) | 門診一頁式速查（可列印） |
| [藥品給付規定全文](docs/nhi-regulations.md) | 健保 2.6.4 PCSK9 給付條件整理 |
| [Statin 不耐受判定](docs/statin-intolerance.md) | 2019 台灣共識 + Myalgia Score |
| [FH 診斷標準計算機](tools/fh-calculator.html) | DLCN Score 互動計算（可離線使用） |

## 🔑 2025/9/1 重大修訂（114 年新制）

| 項目 | 修訂前 | 修訂後 |
|------|--------|--------|
| LDL-C 門檻 | ≥135 mg/dL | **≥100 mg/dL** |
| 核准期間 | 6 個月 | **12 個月** |
| Statin 觀察期 | 含 ezetimibe 共 6 個月 | **Statin ≥3 個月 → 再加 ezetimibe ≥3 個月** |
| 續用條件 | LDL-C 下降 ≥30% | 不變 |

## 🚦 誰可以申請？

```
ASCVD 事件（MI / 缺血性中風 / 血管再通術）
      │
      ├── 發病 1 年內開始最大耐受量 statin
      │
      ├── 路徑 A：高強度 statin ≥3 個月 → + ezetimibe ≥3 個月 → LDL-C 仍 ≥100
      ├── 路徑 B：Statin 禁忌 + ezetimibe ≥3 個月 → LDL-C 仍 ≥100
      └── 路徑 C：Statin 不耐受（2 種 statin）+ ezetimibe ≥3 個月 → LDL-C 仍 ≥100
              │
              └── ✅ 可申請 PCSK9 抑制劑
```

> ⚠️ **必要前提**：必須有 ASCVD 事件。單純 FH 高膽固醇**不符合** PCSK9 一般給付（HoFH 除外，見 Repatha 特殊路徑）。

## 🧬 FH 計算機

開啟 [`tools/fh-calculator.html`](tools/fh-calculator.html) 即可使用互動式 DLCN Score 計算機：

- ✅ 離線可用（純 HTML/CSS/JS）
- ✅ 手機友善 RWD 設計
- ✅ 自動判讀 Definite / Probable / Possible FH
- ✅ 顯示健保 Repatha HoFH 路徑適用性

## 📖 使用方式

1. **Clone 或下載**：
   ```bash
   git clone https://github.com/Cycasio/pcsk9-taiwan-nhi.git
   ```
2. **門診速查**：列印 [`docs/quick-reference.md`](docs/quick-reference.md) 放桌上
3. **FH 評估**：用瀏覽器開 `tools/fh-calculator.html`
4. **申請填表**：照 [`docs/sop-prior-auth.md`](docs/sop-prior-auth.md) 逐步執行

## ⚖️ 聲明

- 本資料整理自**衛福部健保署公開法規**，僅供臨床參考
- 給付規定以健保署最新公告為準
- 最後更新基準：114/9/1 修訂版

## 📝 授權

[CC BY-SA 4.0](LICENSE) — 歡迎轉載與改作，請註明出處。

## 🤝 貢獻

歡迎提 Issue 或 PR：
- 法規有更新？請回報
- 發現錯誤？請指正
- 有好用的臨床工具？歡迎貢獻

---

**維護者**：[陳昱彰醫師](https://drcyc.io) ｜ 義大醫院家庭暨社區醫學部
