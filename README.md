## Configuring for Windows

To configure the MCP server for Windows, ensure your `cline_mcp_settings.json` file contains the following configuration:

```json
{
  "mcpServers": {
    "github.com/modelcontextprotocol/servers/tree/main/src/github": {
      "command": "npx",
      "args": [
        "-y",
        "@modelcontextprotocol/server-github"
      ],
      "env": {
        "GITHUB_PERSONAL_ACCESS_TOKEN": "YOUR_GITHUB_PERSONAL_ACCESS_TOKEN"  // Replace with your actual token
      },
      "disabled": false,
      "autoApprove": []
    }
  }
}
```

**Note:** Replace `YOUR_GITHUB_PERSONAL_ACCESS_TOKEN` with your actual GitHub Personal Access Token. This is the key modification to ensure the server can authenticate with GitHub.