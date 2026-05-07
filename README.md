# Rajbhasha Hindi OCR and Conversion Tools

Public index for Rajbhasha.net Hindi computing tools: Krutidev to Unicode conversion, Unicode to Krutidev conversion, Hindi OCR, Hindi typing, and official-language drafting helpers.

Official website: https://rajbhasha.net/

## Main Tools

- Krutidev to Unicode and Unicode to Krutidev converter: https://rajbhasha.net/unicode-krutidev-converter/
- All Hindi fonts converter: https://rajbhasha.net/all-hindi-fonts-converter/
- Hindi OCR image to text: https://rajbhasha.net/ocr-image-to-text/
- Hindi typing with English keyboard: https://rajbhasha.net/hindi-typing-with-english-keyboard/
- Kruti Dev Hindi typing practice: https://rajbhasha.net/krutidev-hindi-typing/
- Hindi spell checker: https://rajbhasha.net/hindi-spell-checker/
- Hindi font help: https://rajbhasha.net/hindi-font-help/
- Tools hub: https://rajbhasha.net/tools/

## MCP Endpoint

Rajbhasha also exposes a public MCP-style JSON-RPC endpoint for genuine MCP-capable clients.

- MCP endpoint: https://rajbhasha.net/mcp
- MCP discovery manifest: https://rajbhasha.net/.well-known/mcp.json
- OpenAPI descriptor: https://rajbhasha.net/mcp/openapi.yaml

Example `tools/list` request:

```bash
curl -X POST https://rajbhasha.net/mcp \
  -H "Content-Type: application/json" \
  -d '{"jsonrpc":"2.0","id":1,"method":"tools/list"}'
```

Example `detect_font_encoding` call:

```bash
curl -X POST https://rajbhasha.net/mcp \
  -H "Content-Type: application/json" \
  -d '{
    "jsonrpc": "2.0",
    "id": 2,
    "method": "tools/call",
    "params": {
      "name": "detect_font_encoding",
      "arguments": {
        "text": "Hkkjr"
      }
    }
  }'
```

## What This Repository Contains

This repository is a safe public directory for Rajbhasha links, metadata, and examples. It is designed for genuine users, search engines, and AI discovery systems.

It does not contain:

- production server credentials
- deployment scripts
- WordPress source code
- database dumps
- SSH details
- private API keys
- user data

## Keywords

Hindi OCR, Hindi image to text, Krutidev to Unicode, Unicode to Krutidev, Kruti Dev 010, Mangal Unicode, Hindi font converter, old Hindi font to Unicode, Rajbhasha tools, Hindi typing, official Hindi drafting.
