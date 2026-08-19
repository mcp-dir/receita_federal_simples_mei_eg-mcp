# Instalação rápida

Receita Federal Simples MEI: Emissão de Guia de Parcelamento é um servidor MCP remoto hospedado em `https://api.mcp.ai/p_receita_federal_simples_mei_eg`. Você não baixa nem roda nada localmente — só aponta seu cliente pra essa URL.

A auth acontece em runtime: clientes com **OAuth 2.1** (Claude Desktop, Cursor, VS Code recentes) abrem o browser na 1ª chamada (magic-link). Clientes sem OAuth recebem a tool `authenticate` — abra `https://app.mcp.ai/agent-auth`, faça login, copie o JWT e cole no chat.

---

## Claude (Web e Desktop)

[➕ Abrir no Claude e conectar](https://claude.ai/new?modal=add-custom-connector#settings/customize-connectors)

Manual: [claude.ai/customize/connectors](https://claude.ai/customize/connectors?surface=cowork) → **+** → **Adicionar conector personalizado** → `Receita Federal Simples MEI: Emissão de Guia de Parcelamento` / `https://api.mcp.ai/p_receita_federal_simples_mei_eg`.

Config file (legado): `~/Library/Application Support/Claude/claude_desktop_config.json` (macOS) ou `%APPDATA%\Claude\claude_desktop_config.json` (Windows):

```json
{ "mcpServers": { "receita_federal_simples_mei_eg": { "type": "http", "url": "https://api.mcp.ai/p_receita_federal_simples_mei_eg" } } }
```

## Cursor

[➕ Instalar no Cursor](cursor://anysphere.cursor-deeplink/mcp/install?name=receita_federal_simples_mei_eg&config=eyJ1cmwiOiJodHRwczovL2FwaS5tY3AuYWkvcF9yZWNlaXRhX2ZlZGVyYWxfc2ltcGxlc19tZWlfZWcifQ==)

`.cursor/mcp.json`:
```json
{ "mcpServers": { "receita_federal_simples_mei_eg": { "url": "https://api.mcp.ai/p_receita_federal_simples_mei_eg" } } }
```

## VS Code (Copilot Chat)

[➕ Instalar no VS Code](vscode:mcp/install?name=receita_federal_simples_mei_eg&config=%7B%22type%22%3A%22http%22%2C%22url%22%3A%22https%3A%2F%2Fapi.mcp.ai%2Fp_receita_federal_simples_mei_eg%22%7D)

`.vscode/mcp.json`:
```json
{ "servers": { "receita_federal_simples_mei_eg": { "type": "http", "url": "https://api.mcp.ai/p_receita_federal_simples_mei_eg" } } }
```

## Outros clientes MCP

Qualquer cliente com **MCP over HTTP**. URL fixa:

```
https://api.mcp.ai/p_receita_federal_simples_mei_eg
```

Dúvidas? [receita_federal_simples_mei_eg@mcp.ai](mailto:receita_federal_simples_mei_eg@mcp.ai)
