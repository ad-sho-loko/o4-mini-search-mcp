# o4-mini-search-mcp

An MCP (Model Context Protocol) server that provides web search capabilities using OpenAI's o4-mini model. The `o3-search` tool accepts text queries and returns AI-powered search results.

## Installation

### Using npx (Recommended)

Claude Code:

```
$ claude mcp add o4-mini -s user \
	-e OPENAI_API_KEY=your-api-key \
	-e SEARCH_CONTEXT_SIZE=medium \
	-e REASONING_EFFORT=medium \
	-- npx o4-mini-search-mcp
```

json:

```json
{
  "mcpServers": {
    "o4-mini": {
      "command": "npx",
      "args": ["o4-mini-search-mcp"],
      "env": {
        "OPENAI_API_KEY": "your-api-key",
        // Optional: low, medium, high (default: medium)
        "SEARCH_CONTEXT_SIZE": "medium",
        "REASONING_EFFORT": "medium"
      }
    }
  }
}
```
