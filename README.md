# Horizon Insights MCP

Horizon Insights MCP is a remote MCP server for investment research workflows.

It provides access to market data, financial statements, valuation data, macro indicators, charts, company transcripts, research materials, market news, and stock screening capabilities through MCP-compatible AI clients and platforms.

## Capabilities

Horizon Insights MCP can help users access and analyze:

- A-share, US stock, and Hong Kong stock market data
- Index data and index constituents
- Financial statements and key financial metrics
- Valuation data such as PE, PB, dividend yield, and valuation percentiles
- Macro indicators
- Market news
- Company transcripts and research materials
- Charts and structured financial datasets
- Stock screening and strategy research workflows

## Remote MCP Server

```text
https://vmcp.hzinsights.com/mcp/
```

Transport:

```text
streamable-http
```

## Authentication

This MCP server requires a Bearer Token.

Header format:

```text
Authorization: Bearer <USER_TOKEN>
```

Users can create a token in the user center:

```text
https://vmcp.hzinsights.com/dashboard
```

## Example MCP Configuration

```json
{
  "mcpServers": {
    "horizon-insights": {
      "url": "https://vmcp.hzinsights.com/mcp/",
      "headers": {
        "Authorization": "Bearer <USER_TOKEN>"
      }
    }
  }
}
```

Replace `<USER_TOKEN>` with your own token.

## Usage Examples

After connecting the server, users can ask questions such as:

```text
Show me recent market data and valuation metrics for Kweichow Moutai.
```

```text
Compare Apple and Microsoft using their latest financial statements and valuation data.
```

```text
Find A-share companies with stable ROE, low valuation, and high dividend yield.
```

```text
Summarize recent market news related to AI infrastructure and semiconductors.
```

## Quota Notice

If your account quota is used up, the service may return a quota notice.

You can check your quota or recharge in the user center:

```text
https://vmcp.hzinsights.com/dashboard
```

## Registry

Official MCP Registry name:

```text
io.github.shentao12022-cmyk/horizon-insights-mcp
```

## Repository Metadata

This repository contains metadata and integration documentation for the Horizon Insights MCP server.
