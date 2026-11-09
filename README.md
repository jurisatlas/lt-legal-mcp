# Lithuania Legal Research MCP Server (`lt-legal-mcp`)

**[Lietuvių](#lang-lt) | [English Documentation](#english-documentation)**

---

<a id="lang-lt"></a>
## Teisinis MCP serveris Lietuvos teisės aktams ir teismų praktikai (`lt-legal-mcp`) — Lietuvių

### Apie šią saugyklą

Šioje saugykloje pateikiamas Model Context Protocol (MCP) serveris, sujungiantis jūsų AI programą (Claude Desktop, Cursor, Windsurf, VS Code / Copilot, Cline arba Antigravity) tiesiogiai su Teisės aktų registru (`e-tar.lt`) ir LITEKO teismų sprendimų paieška (`liteko.teismai.lt` — 12 apylinkės teismų, 5 apygardos teismai, Lietuvos apeliacinis teismas, LAT, LVAT ir Konstitucinis Teismas).

### Greitas diegimas (AI programos pasirinkimas)

1. **Atsisiuntimas:** Viršutiniame dešiniajame kampe spustelėkite **`<> Code` -> `Download ZIP`** ir išskleiskite aplanką kompiuteryje.
2. **Paleidimas:** Dukart spustelėkite **`Click_Here_To_Install_Windows.bat`** (Windows) arba **`Click_Here_To_Install_Mac.command`** (macOS).
3. **AI kliento pasirinkimas:** Pažymėkite naudojamas AI programas (Claude, Cursor, Windsurf, VS Code, Antigravity), spustelėkite diegti ir iš naujo paleiskite pasirinktą AI programą.

**Saugumo pastaba:** Diegimo įrankis veikia tik skaitymo režimu (read-only) ir neliečia jokių asmeninių failų jūsų kompiuteryje.

### Teismų pakopos ir oficialūs šaltiniai

| Teismų pakopa | Apimami teismai |
|:---|:---|
| **I pakopa (12 Apylinkės ir Regionų administraciniai teismai)** | 12 Apylinkės teismai (District Courts) & 2 Regionų administraciniai teismai |
| **II pakopa (5 Apygardos teismai ir Lietuvos apeliacinis teismas)** | 5 Apygardos teismai (Regional Courts: Vilnius, Kaunas, Klaipėda, Šiauliai, Panevėžys) & Lietuvos apeliacinis teismas (Court of Appeal of Lithuania) |
| **III pakopa (LAT, LVAT ir Konstitucinis Teismas)** | Lietuvos Aukščiausiasis Teismas (LAT), Lietuvos vyriausiasis administracinis teismas (LVAT) & Konstitucinis Teismas |

- **Teisės aktų registras (e-tar.lt Open API):** [https://www.e-tar.lt](https://www.e-tar.lt) (`e-tar.lt`, `lrs.lt`, `infolex.lt`)
- **LITEKO Vieša teismų sprendimų paieška (liteko.teismai.lt — All District, Regional, Appellate & Supreme Courts):** [https://liteko.teismai.lt/viesasprendimupaieska/](https://liteko.teismai.lt/viesasprendimupaieska/) (`teismai.lt`, `liteko.teismai.lt`, `lat.lt`, `lvat.lt`, `lrkt.lt`, `infolex.lt`)

---

<a id="english-documentation"></a>
## English Documentation

Model Context Protocol (MCP) server providing live, read-only access to **Lithuania (LT)** legislation, official gazettes, multi-tier judicial decisions (First Instance, Regional/Cantonal/Appellate, and Supreme/Constitutional courts, including HTML and PDF full-text extraction), and statutory citation verification across all major AI clients (**ChatGPT Desktop, OpenAI Codex CLI, Claude Desktop, Claude Code CLI, Cursor, Windsurf, VS Code / GitHub Copilot / Cline / Roo Code, Google Antigravity / Gemini CLI, Perplexity, and Continue.dev**).

---

### Interactive Desktop Setup (Select Your AI Assistant)

This package includes a graphical installer for legal practitioners and non-technical users that lets you select which AI application(s) you use:

1. **Download:** Click **`<> Code`** at the top right of this repository, select **`Download ZIP`**, and extract the folder to your computer.
2. **Run the Setup Utility:**
   - **Windows:** Double-click `Click_Here_To_Install_Windows.bat`
   - **macOS:** Double-click `Click_Here_To_Install_Mac.command`
3. **Select Your AI Client(s) & Connect:** Check the box(es) for the AI assistant(s) installed on your computer (**ChatGPT Desktop & OpenAI Codex CLI**, **Claude Desktop & Claude Code CLI**, **Cursor**, **Windsurf**, **VS Code / GitHub Copilot / Cline / Roo Code**, **Google Antigravity / Gemini CLI**, or **Perplexity / Continue.dev**), click **Install to Selected AI Clients**, and restart your selected AI application.

**System Integrity Note:** The setup utility operates strictly in read-only mode with respect to your personal files and documents. It installs an isolated Python runtime inside the extracted folder and registers the server entry only in the AI client configuration files you select.

---

### Multi-Tier Judicial Hierarchy & Live Indexed National Archives

This server performs live queries across the full judicial hierarchy and official legal archives of **Lithuania**, extracting full text from both HTML pages and official court/gazette PDF judgments:

| Judicial Tier | Covered Courts & Tribunals |
|:---|:---|
| **Tier 1 — First Instance** | 12 Apylinkės teismai (District Courts) & 2 Regionų administraciniai teismai |
| **Tier 2 — Regional / Cantonal / Appellate** | 5 Apygardos teismai (Regional Courts: Vilnius, Kaunas, Klaipėda, Šiauliai, Panevėžys) & Lietuvos apeliacinis teismas (Court of Appeal of Lithuania) |
| **Tier 3 — Supreme & Constitutional** | Lietuvos Aukščiausiasis Teismas (LAT), Lietuvos vyriausiasis administracinis teismas (LVAT) & Konstitucinis Teismas |

#### Official Portals & Live Indexed Domains

- **National Legislation & Official Gazette:** Teisės aktų registras (e-tar.lt Open API) — [https://www.e-tar.lt](https://www.e-tar.lt)
  - *Indexed Legislation Domains:* `e-tar.lt`, `lrs.lt`, `infolex.lt`
- **Court Decisions & Jurisprudence Archives:** LITEKO Vieša teismų sprendimų paieška (liteko.teismai.lt — All District, Regional, Appellate & Supreme Courts) — [https://liteko.teismai.lt/viesasprendimupaieska/](https://liteko.teismai.lt/viesasprendimupaieska/)
  - *Indexed Judicial & Open Case Law Domains:* `teismai.lt`, `liteko.teismai.lt`, `lat.lt`, `lvat.lt`, `lrkt.lt`, `infolex.lt`

---

### Available MCP Tools

| Tool | Description |
|:---|:---|
| `search_legislation` | Searches enacted statutes, codes, decrees, and official gazette publications in Lithuania. |
| `search_case_law` | Searches national jurisprudence and open judicial archives for Lithuania. |
| `search_tiered_court_decisions` | Filters case law specifically by judicial instance (`first_instance`, `appellate_regional`, `supreme_constitutional`) or specific regional/cantonal/district court. |
| `list_court_hierarchy` | Returns the complete 3-tier court structure and supported regional court filters for Lithuania. |
| `get_legal_document_markdown` | Retrieves full statutory or judicial texts (both HTML and official `.pdf` court judgments) and converts them into clean Markdown. |
| `verify_citation` | Validates statutory and case law citations against official registries. |

---

<details>
<summary><b>Manual Configuration for Developers (Optional)</b></summary>

```json
{
  "mcpServers": {
    "lt-legal-mcp": {
      "command": "uvx",
      "args": [
        "--from",
        "https://github.com/jurisatlas/lt-legal-mcp/archive/refs/heads/main.zip",
        "lt-legal-mcp"
      ]
    }
  }
}
```
</details>
