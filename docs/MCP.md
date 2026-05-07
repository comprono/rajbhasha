# Rajbhasha MCP

Rajbhasha exposes a public MCP-style JSON-RPC endpoint at:

https://rajbhasha.net/mcp

Discovery files:

- https://rajbhasha.net/.well-known/mcp.json
- https://rajbhasha.net/mcp/openapi.yaml
- https://rajbhasha.net/api/openapi.json

## List Tools

```bash
curl -X POST https://rajbhasha.net/mcp \
  -H "Content-Type: application/json" \
  -d '{"jsonrpc":"2.0","id":1,"method":"tools/list"}'
```

## Initialize

```bash
curl -X POST https://rajbhasha.net/mcp \
  -H "Content-Type: application/json" \
  -d '{"jsonrpc":"2.0","id":2,"method":"initialize","params":{}}'
```

## Call a Tool

```bash
curl -X POST https://rajbhasha.net/mcp \
  -H "Content-Type: application/json" \
  -d '{
    "jsonrpc": "2.0",
    "id": 3,
    "method": "tools/call",
    "params": {
      "name": "official_phrase_search",
      "arguments": {
        "query": "approval"
      }
    }
  }'
```

## Security Notes

Do not send secrets, private documents, or sensitive personal data to public endpoints unless you understand and accept the privacy implications. Public tool calls should be limited to normal Hindi conversion, OCR, typing, and phrase-search usage.
