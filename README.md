# Hyperresearch Answers for Cursor

Every web search provider has gaps. Each one indexes different pages, misses different sources, and none of them reach the structured data behind most real questions.

Hyperresearch Answers layers four web search engines with about 45 structured sources, including company filings, government statistics, public registers, scholarly indexes and books. Your agent gets one search tool with the gaps filled in.

Every answer is checked word for word against quotes from the pages it cites. If the sources don't back it up, it says "not found" instead of guessing. Your agent gets the answer and its proof, not whole web pages, so its context stays on your code.

## Tools

- **ask**: one question, one verified answer with its quotes and links.
- **search**: ranked sources with only the relevant passages, for when your agent should read the evidence itself.

## Setup

1. Install the plugin from the Cursor Marketplace.
2. The first time the agent calls a tool, Cursor opens a sign-in window. Sign in with your Hyperresearch account.
3. Ask your agent something that needs a sourced fact, for example: "What's the current rate limit for the GitHub REST API for authenticated users? Use Hyperresearch Answers and show the source."

Calls are paid from the prepaid credit in your Hyperresearch account, and every result shows what it cost and the balance left. New accounts get free credit to try it. More: https://hyperresearch.ai/answers

## Manual setup (without the plugin)

Add this to `.cursor/mcp.json`:

```json
{
  "mcpServers": {
    "hyperresearch-answers": {
      "url": "https://answers.hyperresearch.ai/mcp"
    }
  }
}
```

## Support

jordan@hyperresearch.ai
