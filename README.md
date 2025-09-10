# Circuit Cinema Model Context Protocol (MCP) API Documentation

This repository provides the official documentation and resources for integrating your AI agents and applications with Circuit Cinema's streaming service via the **Model Context Protocol (MCP)**.

Circuit Cinema embraces the "Bring Your Own AI" (BYOAI) model, offering an open, model-agnostic API that allows your personal AI agents to seamlessly interact with our platform for search, watchlist management, and future features like subscription management.

## Getting Started

### 1. Key Discovery Endpoints

Your MCP-compliant AI agent can automatically discover our service and its capabilities by looking for our `mcp.json` manifest:

* **MCP Discovery File:** `https://circuitcinema.com/.well-known/mcp.json`
* **MCP Server Endpoint:** `https://mcp.circuitcinema.com`

For platforms utilizing the OpenAPI standard, our `ai-plugin.json` and `openapi.yaml` are also available:

* **Plugin Manifest:** `https://circuitcinema.com/.well-known/ai-plugin.json`
* **OpenAPI Specification:** `https://data.circuitcinema.com/openapi.yaml`

### 2. Dynamic Client Registration (RFC 7591)

Our MCP implementation supports secure, on-the-fly client registration as per RFC 7591. Your AI agent will use this endpoint to register itself with our authorization server before initiating an OAuth 2.1 flow.

* **Registration Endpoint:** `https://oauth.circuitcinema.com/v1/oauth2/register`

### 3. Authorization Server Metadata (RFC 8414)

Discover our authorization server's capabilities and endpoints:

* **OAuth Authorization Server Metadata:** `https://oauth.circuitcinema.com/.well-known/oauth-authorization-server`

---

## Code Samples & Client Examples

_Coming Soon! We'll be adding client libraries, code snippets, and example implementations in various languages to help you get started quickly._

## Support

If you have questions or encounter issues, please:

* Open an issue in this GitHub repository.
* Visit our community forum (if you have one).
* Contact our developer support team at [dev-support@circuitcinema.com](mailto:dev-support@circuitcinema.com).

## Contributing

We welcome feedback and suggestions for improving our documentation. Please feel free to open issues or submit pull requests.

---

**Circuit Cinema** | [Website](https://circuitcinema.com) | [LinkedIn](https://www.linkedin.com/company/circuit-cinema)
