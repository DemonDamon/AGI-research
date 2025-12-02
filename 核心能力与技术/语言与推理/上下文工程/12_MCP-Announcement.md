# 12_MCP Announcement

**原始链接**: https://www.anthropic.com/news/model-context-protocol

---

# Introducing the Model Context Protocol \ Anthropic

原文链接: https://www.anthropic.com/news/model-context-protocol

Announcements

# Introducing the Model Context Protocol

Nov 25, 2024

Today, we're open-sourcing the [Model Context Protocol](https://modelcontextprotocol.io) (MCP), a new standard for connecting AI assistants to the systems where data lives, including content repositories, business tools, and development environments. Its aim is to help frontier models produce better, more relevant responses.

As AI assistants gain mainstream adoption, the industry has invested heavily in model capabilities, achieving rapid advances in reasoning and quality. Yet even the most sophisticated models are constrained by their isolation from data—trapped behind information silos and legacy systems. Every new data source requires its own custom implementation, making truly connected systems difficult to scale.

MCP addresses this challenge. It provides a universal, open standard for connecting AI systems with data sources, replacing fragmented integrations with a single protocol. The result is a simpler, more reliable way to give AI systems access to the data they need.

## Model Context Protocol

The Model Context Protocol is an open standard that enables developers to build secure, two-way connections between their data sources and AI-powered tools. The architecture is straightforward: developers can either expose their data through MCP servers or build AI applications (MCP clients) that connect to these servers.

Today, we're introducing three major components of the Model Context Protocol for developers:

* The Model Context Protocol [specification and SDKs](https://github.com/modelcontextprotocol)
* Local MCP server support in the [Claude Desktop apps](https://claude.ai/redirect/website.v1.d3918052-e3bf-4b01-ac7a-f7ef71383d8b/download)
* An [open-source repository](https://github.com/modelcontextprotocol/servers) of MCP servers

Claude 3.5 Sonnet is adept at quickly building MCP server implementations, making it easy for organizations and individuals to rapidly connect their most important datasets with a range of AI-powered tools. To help developers start exploring, we’re sharing pre-built MCP servers for popular enterprise systems like Google Drive, Slack, GitHub, Git, Postgres, and Puppeteer.

Early adopters like Block and Apollo have integrated MCP into their systems, while development tools companies including Zed, Replit, Codeium, and Sourcegraph are working with MCP to enhance their platforms—enabling AI agents to better retrieve relevant information to further understand the context around a coding task and produce more nuanced and functional code with fewer attempts.

"At Block, open source is more than a development model—it’s the foundation of our work and a commitment to creating technology that drives meaningful change and serves as a public good for all,” said Dhanji R. Prasanna, Chief Technology Officer at Block. “Open technologies like the Model Context Protocol are the bridges that connect AI to real-world applications, ensuring innovation is accessible, transparent, and rooted in collaboration. We are excited to partner on a protocol and use it to build agentic systems, which remove the burden of the mechanical so people can focus on the creative.”

Instead of maintaining separate connectors for each data source, developers can now build against a standard protocol. As the ecosystem matures, AI systems will maintain context as they move between different tools and datasets, replacing today's fragmented integrations with a more sustainable architecture.

## Getting started

Developers can start building and testing MCP connectors today. All [Claude.ai](http://claude.ai/redirect/website.v1.d3918052-e3bf-4b01-ac7a-f7ef71383d8b) plans support connecting MCP servers to the Claude Desktop app.

Claude for Work customers can begin testing MCP servers locally, connecting Claude to internal systems and datasets. We'll soon provide developer toolkits for deploying remote production MCP servers that can serve your entire Claude for Work organization.

To start building:

* Install pre-built MCP servers through the [Claude Desktop app](https://claude.ai/redirect/website.v1.d3918052-e3bf-4b01-ac7a-f7ef71383d8b/download)
* Follow our [quickstart guide](https://modelcontextprotocol.io/quickstart) to build your first MCP server
* Contribute to our [open-source repositories](https://github.com/modelcontextprotocol) of connectors and implementations

## An open community

We’re committed to building MCP as a collaborative, open-source project and ecosystem, and we’re eager to hear your feedback. Whether you’re an AI tool developer, an enterprise looking to leverage existing data, or an early adopter exploring the frontier, we invite you to build the future of context-aware AI together.

## Related content

### Introducing Claude Opus 4.5

The best model in the world for coding, agents, and computer use, with meaningful improvements to everyday tasks like slides and spreadsheets. Claude Opus 4.5 delivers frontier performance and dramatically improved token efficiency.

[Read more](/news/claude-opus-4-5)

### Claude now available in Microsoft Foundry and Microsoft 365 Copilot

[Read more](/news/claude-in-microsoft-foundry)

### Microsoft, NVIDIA, and Anthropic announce strategic partnerships

Microsoft, NVIDIA and Anthropic announced new strategic partnerships. Anthropic is scaling its rapidly-growing Claude AI model on Microsoft Azure, powered by NVIDIA, which will broaden access to Claude and provide Azure enterprise customers with expanded model choice and new capabilities. Anthropic has committed to purchase $30 billion of Azure compute capacity and to contract additional compute capacity up to one gigawatt.

[Read more](/news/microsoft-nvidia-anthropic-announce-strategic-partnerships)