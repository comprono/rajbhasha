# Security Policy

This repository is public documentation for Rajbhasha.net tools. It must not include secrets, private infrastructure details, server paths, credentials, database dumps, or deployment scripts.

## Reporting Security Issues

If you find a security issue involving Rajbhasha.net, please do not post exploit details publicly. Open a minimal GitHub issue that says a private security report is needed, or contact the site owner through the official website:

https://rajbhasha.net/

## Public-Safe Scope

Safe content for this repository:

- public tool links
- public API and MCP endpoint documentation
- non-sensitive examples
- user-facing usage notes
- search and discovery metadata

Unsafe content for this repository:

- passwords, tokens, keys, cookies, or session values
- SSH host details paired with credentials
- server deployment scripts
- WordPress admin details
- database exports
- private logs
- internal file paths that reveal operational details
- user-submitted text, images, or documents

## MCP Usage

The public MCP endpoint is intended for normal tool discovery and safe tool calls. Clients should avoid sending sensitive personal, legal, medical, or confidential text unless they understand the privacy implications of sending data to a web service.
