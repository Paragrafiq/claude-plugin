# Paragrafiq pro Claude / Paragrafiq for Claude

> **Pracovní verze / Draft.** Konektor Paragrafiq v2 (`https://www.paragrafiq.cz/api/mcp/v2`) zatím není v produkci; tento repozitář je do té doby soukromý. / The Paragrafiq v2 connector is not in production yet; this repository stays private until it is.

## Česky

**Co to je.** Plugin pro Claude, který přidává skill `paragrafiq-legal-research`: návod, jak má Claude u otázek podle českého práva ověřovat znění zákonů a judikaturu pomocí nástrojů Paragrafiq, místo aby odpovídal z paměti. Součástí je i odkaz na konektor Paragrafiq (MCP).

**Co plugin obsahuje**
- `skills/paragrafiq-legal-research/`: skill (`SKILL.md`) a podklady (`references/hranice.md`, `nastroje.md`, `postupy.md`);
- `.mcp.json`: konfigurace konektoru na `https://www.paragrafiq.cz/api/mcp/v2`;
- `.claude-plugin/plugin.json` a `.claude-plugin/marketplace.json`.

**Jak plugin přidat (Claude Code)**
```
/plugin marketplace add Paragrafiq/claude-plugin
/plugin install paragrafiq@paragrafiq-plugins
```

**Konektor.** Postup připojení konektoru a popis nástrojů najdete na https://www.paragrafiq.cz/mcp.

**Upozornění.** Skill ani konektor nenahrazují právní poradenství. Odpověď Clauda je jeho výklad ověřených zdrojů za podmínek, které uživatel uvedl.

## English

**What it is.** A Claude plugin that adds the `paragrafiq-legal-research` skill: instructions that teach Claude to verify the text of Czech statutes and case law with the Paragrafiq tools instead of answering from memory. It also declares the Paragrafiq (MCP) connector.

**What is inside**
- `skills/paragrafiq-legal-research/`: the skill (`SKILL.md`) and its references (`references/hranice.md`, `nastroje.md`, `postupy.md`);
- `.mcp.json`: connector configuration pointing to `https://www.paragrafiq.cz/api/mcp/v2`;
- `.claude-plugin/plugin.json` and `.claude-plugin/marketplace.json`.

**Install (Claude Code)**
```
/plugin marketplace add Paragrafiq/claude-plugin
/plugin install paragrafiq@paragrafiq-plugins
```

**Connector.** Setup instructions and a description of the tools: https://www.paragrafiq.cz/mcp.

**Disclaimer.** Neither the skill nor the connector replaces legal advice. Claude's answer is its explanation of verified sources, conditional on the facts the user provided.

## Licence / License

MIT, see [LICENSE](LICENSE).
