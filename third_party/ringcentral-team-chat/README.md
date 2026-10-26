# RingCentral Team Chat

Cursor plugin that connects agents to [RingCentral](https://www.ringcentral.com) RingEX Team Chat through RingCentral's hosted [Model Context Protocol](https://modelcontextprotocol.io/) server.

RingEX Team Chat remote MCP server.

## Install

1. Open **Cursor Settings → Plugins**.
2. Search for **RingCentral Team Chat**.
3. Click **Install**, then complete the RingCentral sign-in prompt if one appears.

Or run `/add-plugin ringcentral-team-chat` in chat.

## MCP

```json
{
  "mcpServers": {
    "ringcentral-team-chat": {
      "type": "http",
      "url": "https://mcp.labs.ringcentral.com/ringex/v1.1.0/team-chat"
    }
  }
}
```

## Before you connect

You need a RingCentral account with team messaging.

## Notes

- The hosted runtime is the source of truth for tool names and schemas.
- Tool calls run under the RingCentral permissions of the user who authorizes the connection.
- RingEX Phone stays in the separate `ringcentral` plugin. Install both if you want phone and team chat.

## Docs

- RingCentral: https://www.ringcentral.com
- RingEX Team Chat MCP server: https://developers.ringcentral.com/mcp/servers/ringex-chat/
- Server URL: https://mcp.labs.ringcentral.com/ringex/v1.1.0/team-chat

Logo is RingCentral's mark from the `ringcentral` GitHub organization avatar (256×256). The submitted logo URL (`https://www.ringcentral.com`) is a web page, and ringcentral.com could not be reached when this plugin was added.

## License

MIT
