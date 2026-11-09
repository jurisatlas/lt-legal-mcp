---
name: lt-legal-mcp-skill
description: Official Lithuania (LT) legislation, multi-tier court precedent research, and citation verification skill.
version: 2.0.0
author: JurisAtlas
license: MIT
---

# Lithuania Legal Research & Multi-Tier Case Law Skill (`lt-legal-mcp`)

Use this skill whenever the user asks a legal question, drafts a pleading or contract, or researches case law across any judicial instance in **Lithuania (LT)**.

## Verification & Research Rules

1. **Citation Verification:** Never fabricate a statutory provision or case citation. Query `search_legislation`, `search_case_law`, `search_tiered_court_decisions`, or `verify_citation` before citing any authority (e.g., `ECLI:LT:LAT:2024:e3K300124 or TAR`).
2. **Multi-Tier Judicial Coverage:**
   - **First Instance (Trial / Municipal / District):** 12 Apylinkės teismai (District Courts) & 2 Regionų administraciniai teismai
   - **Second Instance (Cantonal / Regional / Appellate):** 5 Apygardos teismai (Regional Courts: Vilnius, Kaunas, Klaipėda, Šiauliai, Panevėžys) & Lietuvos apeliacinis teismas (Court of Appeal of Lithuania)
   - **Supreme & Constitutional Instance:** Lietuvos Aukščiausiasis Teismas (LAT), Lietuvos vyriausiasis administracinis teismas (LVAT) & Konstitucinis Teismas
   - **Primary Tiered Database:** LITEKO Vieša teismų sprendimų paieška (liteko.teismai.lt — All District, Regional, Appellate & Supreme Courts) (`https://liteko.teismai.lt/viesasprendimupaieska/`)
