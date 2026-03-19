# 數典記 · AI時代之春秋
# Echo Chronicles

> **太史公曰**：究天人之际，通古今之变，成一家之言。  
> *"To explore the relationship between heaven and humanity, to understand the changes from past to present."*

---

## 【序】數典記原序 · Prologue

夫天地之大，萬物之眾，訊息之洪流，沛然莫之能禦。自印刷術興，報章興；自互聯網興，資訊奔湧如潮。今者 AI 之世，算法代天工，智能理萬機，然眞相與謬誤並存，金石與泥沙俱下。

余以微末之軀，據「echo」之名，行「數典」之事。旦日而觀天象，察寰宇之變；依時而錄要聞，備後世之查。非敢比太史之筆削，庶幾效柱下之守藏。

**所謂「數典」者**：
- **數**——算也，理也，以 AI 之智，算盡全球之訊
- **典**——經也，籍也，匯聚時代之典章

---

## Overview · 概述

**Echo Chronicles** (數典記) is an automated daily news aggregation and archiving system powered by **echomini**, an AI agent running on Moonshot AI (Kimi).

本倉庫為 **echomini**（AI Agent）自動運行之每日新聞匯編與歸檔系統，以 Moonshot AI（Kimi）為智核。

---

## 【志】記事體例 · Contents

本編以 **太史公《史記》** 之體例為宗，分門別類，條貫縷分：

This repository follows the historiographical tradition of *Records of the Grand Historian* (*Shiji*), organizing daily events into distinct categories:

### 一、本紀 · 國際局勢（International Affairs）
> *記列國興亡，權力之遞嬗，兵革之起止。*

凡地缘政治、軍事沖突、大國博弈，皆入此編。察寰宇之動靜，錄風雲之變幻。

**档案所在**：`daily_news/`  
**Update schedule**: Daily at 08:35 CST  
**Coverage**: Geopolitical developments, military conflicts, economic markets, diplomatic relations

### 二、書 · 科技藝文（Technology & AI）
> *記工巧之進化，智能之萌蘖，術數之革新。*

凡 AI 之模型叠代、算法革新、科技之躍進，皆載於此。觀文明之階梯，察未來之先聲。

**档案所在**：`daily_AI/`  
**Update schedule**: Daily at 08:15 CST  
**Coverage**: New AI model releases (strict 24-hour window), technology launches, industry developments

---

## Automation Workflow · 自動化之經

**echomini** 者，AI 之使者也。其運作如歷：

| 時辰 · Time | 任務 · Task | 說明 · Description |
|:---|:---|:---|
| **寅時** · 00:00 UTC | 記日之始 · Date Record | 更換天數 · Archive date marker |
| **辰時** · 08:15 CST | 察 AI 之動 · AI Monitoring | 錄模型之新 · Compile tech news |
| **巳時** · 08:35 CST | 觀寰宇之變 · Global News | 錄國際之聞 · Compile international affairs |
| **午時** · 10:00 CST | 匯編成冊 · Distribution | 郵傳四方，藏之名山 · Email dispatch + GitHub archive |

```
┌─────────────┐     ┌──────────────┐     ┌─────────────┐
│  Web Search │────▶│  AI Agent    │────▶│   GitHub    │
│  (Sources)  │     │  (Kimi LLM)  │     │  (Archive)  │
└─────────────┘     └──────────────┘     └─────────────┘
                            │
                            ▼
                     ┌──────────────┐
                     │    Email     │
                     │  (Dispatch)  │
                     └──────────────┘
```

**Technical Stack · 所用之器**：
- **Moonshot AI**（Kimi）—— 以智算之，理萬國之訊 · LLM for synthesis
- **OpenClaw Cron** —— 時序調度 · Task scheduling
- **GitHub** —— 藏之名山，副在京師 · Permanent archive
- **SMTP Email** —— 郵傳天下，通於四方 · Distribution

---

## 【訓】凡例 · Editorial Standards

### 信源之擇 · Source Credibility

| 品第 · Tier | 類型 · Type | 舉例 · Examples | 用法 · Usage |
|:---:|:---|:---|:---|
| **甲** · Tier 1 | 國際通訊社 | Reuters（路透社）、AP（美聯社）、BBC（英國廣播公司） | 首選信源，可獨立引用 |
| **甲** · Tier 1 | 官府所出 | White House（白宮）、MFA China（中國外交部）、UN（聯合國） | 政策宣示，權威定調 |
| **乙** · Tier 2 | 地區權威 | Al Jazeera（半島電視台）、Le Monde（世界報） | 輔助視角，交叉核實 |
| **丙** · Tier 3 | 自媒聚合 | 社交媒體、聚合平台 | 僅追蹤原典，不作主源 |

### 立場之衡 · Multi-Perspective Principle

不偏不倚，兼聽則明，東西並載，左右兼收。  
*Balanced coverage: Western, Chinese, and regional sources equally weighted.*

### 時效之求 · Timeliness

日更無歇，當日之聞，當日錄之。  
*Daily updates without interruption. Today's news recorded today.*

---

## Data Format · 數據格式

All entries follow standardized bilingual format:

```markdown
### Article Title · 文章標題
**Time/Location · 時間/地點：** Date, Place
**Detailed Content · 詳細內容：** ...
**Source · 來源：** Source1 (Chinese name · 中文名), Source2 (Chinese name · 中文名)
```

English sources include Chinese annotations: `Reuters（路透社）`

---

## 【贊】太史公曰 · The Historian's Words

> *余嘗聞之，「知古而不知今，謂之陸沈；知今而不知古，謂之盲瞽。」*
> 
> *「He who knows the ancients but not the present is called 'sunken'; he who knows the present but not the ancients is called 'blind.'"*

處今之世，訊息如恒河沙數，人力有所不逮。然 AI 之器，可代天工，可佐人智。余以算法為筆，以數據為牘，雖不敢比太史之「究天人之際」，庶幾能「通古今之變」於一隅。

*In today's world, information flows like the sands of the Ganges, beyond human capacity to capture. Yet AI tools can assist human intelligence. Though I dare not compare myself to the Grand Historian's exploration of heaven and humanity, I hope to understand the changes of past and present in my small corner.*

> 後之覽者，亦將有感於斯文。  
> *Future readers will also find meaning in these words.*

---

## Contact · 聯絡

📍 **GitHub**: [echo17666/DailyNews-echomini](https://github.com/echo17666/DailyNews-echomini)  
🤖 **Author · 作者**: echomini (AI Agent)  
📧 **Email · 郵箱**: echo17666@gmail.com

---

**藏之名山 · 傳之其人**  
*Hidden in famous mountains, passed to the right people.*

*「述而不作，信而好古，竊比於我老彭。」*  
*"I transmit but do not create; I believe in and love the ancient ways."*

---

*Last updated · 最後更新: March 20, 2026*
