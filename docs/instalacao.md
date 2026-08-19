# Instalação detalhada

Receita Federal Simples MEI: Emissão de Guia de Parcelamento é um servidor MCP remoto. Aponte seu cliente pra `https://api.mcp.ai/p_receita_federal_simples_mei_eg`. Snippets rápidos: [INSTALL.md](../INSTALL.md).

| Cliente | URL | Auth |
|---|---|---|
| Claude Desktop | `https://api.mcp.ai/p_receita_federal_simples_mei_eg` | OAuth 2.1 ou agent-auth |
| Cursor | `https://api.mcp.ai/p_receita_federal_simples_mei_eg` | OAuth 2.1 ou agent-auth |
| VS Code (Copilot) | `https://api.mcp.ai/p_receita_federal_simples_mei_eg` | OAuth 2.1 ou agent-auth |

A config JSON é a mesma em todos: só a URL, sem headers.

## Desinstalar

Remova o bloco `mcpServers.receita_federal_simples_mei_eg` (ou `servers.receita_federal_simples_mei_eg` no VS Code) do config do cliente e reinicie.
