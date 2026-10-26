# RingCentral

Cursor plugin that connects agents to [RingCentral](https://www.ringcentral.com) RingEX Phone and RingEX Team Chat through RingCentral's hosted [Model Context Protocol](https://modelcontextprotocol.io/) servers.

RingEX Phone and Team Chat remote MCP servers.

## Install

1. Open **Cursor Settings → Plugins**.
2. Search for **RingCentral**.
3. Click **Install**, then complete the RingCentral sign-in prompt if one appears.

Or run `/add-plugin ringcentral` in chat.

## MCP

```json
{
  "mcpServers": {
    "ringcentral": {
      "type": "http",
      "url": "https://mcp.labs.ringcentral.com/ringex/phone"
    },
    "ringcentral-team-chat": {
      "type": "http",
      "url": "https://mcp.labs.ringcentral.com/ringex/v1.1.0/team-chat"
    }
  }
}
```

## Before you connect

You need a RingCentral account with RingEX phone service and team messaging.

## Notes

- The hosted runtime is the source of truth for tool names and schemas.
- Tool calls run under the RingCentral permissions of the user who authorizes the connection.

## Docs

- RingCentral: https://www.ringcentral.com
- RingEX Phone MCP server: https://developers.ringcentral.com/mcp/servers/ringex-phone/
- RingEX Team Chat MCP server: https://developers.ringcentral.com/mcp/servers/ringex-chat/
- Phone server URL: https://mcp.labs.ringcentral.com/ringex/phone
- Team Chat server URL: https://mcp.labs.ringcentral.com/ringex/v1.1.0/team-chat

Logo is RingCentral's mark from the `ringcentral` GitHub organization avatar (256×256). The submitted logo URLs were web pages rather than images, and ringcentral.com could not be reached when this plugin was built.

## License

MIT
