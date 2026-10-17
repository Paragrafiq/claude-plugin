# Paragrafiq pro Claude / Paragrafiq for Claude

## Česky

**Co to je.** Plugin pro Claude, který přidává skill `paragrafiq-legal-research`: návod, jak má Claude u otázek podle českého práva ověřovat znění zákonů a judikaturu pomocí nástrojů Paragrafiq, místo aby odpovídal z paměti. Součástí je i konfigurace konektoru Paragrafiq (MCP).

**Co plugin obsahuje**
- `skills/paragrafiq-legal-research/`: skill (`SKILL.md`) a podklady (`references/hranice.md`, `nastroje.md`, `postupy.md`);
- `.mcp.json`: konfigurace konektoru Paragrafiq;
- `.claude-plugin/plugin.json` a `.claude-plugin/marketplace.json`.

**Jak plugin přidat (Claude Code)**
```
/plugin marketplace add Paragrafiq/claude-plugin
/plugin install paragrafiq@paragrafiq-plugins
```

**Konektor a nejlepší výsledky.** Postup připojení konektoru, nahrání skillu a větu do profilu najdete na https://www.paragrafiq.cz/mcp. Skill i konektor se nastavují zvlášť: skill se nepřidá sám s konektorem.

**Upozornění.** Skill ani konektor nenahrazují právní poradenství. Odpověď Clauda je jeho výklad ověřených zdrojů za podmínek, které uživatel uvedl.

## English

**What it is.** A Claude plugin that adds the `paragrafiq-legal-research` skill: instructions that teach Claude to verify the text of Czech statutes and case law with the Paragrafiq tools instead of answering from memory. It also carries the Paragrafiq (MCP) connector configuration.

**What is inside**
- `skills/paragrafiq-legal-research/`: the skill (`SKILL.md`) and its references (`references/hranice.md`, `nastroje.md`, `postupy.md`);
- `.mcp.json`: Paragrafiq connector configuration;
- `.claude-plugin/plugin.json` and `.claude-plugin/marketplace.json`.

**Install (Claude Code)**
```
/plugin marketplace add Paragrafiq/claude-plugin
/plugin install paragrafiq@paragrafiq-plugins
```

**Connector and best results.** How to connect the connector, upload the skill and use the profile sentence: https://www.paragrafiq.cz/mcp. The skill and the connector are set up separately: the skill is not added automatically with the connector.

**Disclaimer.** Neither the skill nor the connector replaces legal advice. Claude's answer is its explanation of verified sources, conditional on the facts the user provided.

## Licence / License

MIT, see [LICENSE](LICENSE).
