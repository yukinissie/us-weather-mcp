# us-weather-mcp-server

I created an MCP server based on the tutorial.

https://modelcontextprotocol.io/quickstart/server

## Usage

Edit `claude_desktop_config.json`.

If you are using the Claude Desktop app with MacOS or Linux, you can find the configuration file at:

`~/Library/Application\ Support/Claude/claude_desktop_config.json`

You can use the following configuration to run the MCP server for `claude_desktop_config.json`. (Required Java 21.0.2 or
higher)

```json
{
  "mcpServers": {
    "weather": {
      "command": "/path/to/java/21.0.2/bin/java",
      "args": [
        "-jar",
        "/path/to/us-weather-mcp/build/libs/us-weather-mcp-1.0-SNAPSHOT-all.jar"
      ]
    }
  }
}
```

And then, you can run the MCP server at the Claude Desktop app.
