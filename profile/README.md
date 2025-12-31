# LokiMCPUniverse

**Open-Source Enterprise Model Context Protocol Servers**

<div align="center">

![Focus](https://img.shields.io/badge/Focus-Enterprise%20MCP%20Servers-DC143C?style=for-the-badge&labelColor=2B2B2B)
![Status](https://img.shields.io/badge/Status-16%20Live%20on%20Registry-696969?style=for-the-badge&labelColor=2B2B2B)
![License](https://img.shields.io/badge/License-MIT-DC143C?style=for-the-badge&labelColor=2B2B2B)

**[Official MCP Registry](https://registry.modelcontextprotocol.io/) • [GitHub Repos](https://github.com/asklokesh) • [Install Guide](#quick-start)**

</div>

---

## Mission

Building open-source Model Context Protocol (MCP) servers for enterprise tools. 16 servers live on the official registry, enabling AI agents to seamlessly integrate with critical business platforms.

**No vendor lock-in. No enterprise agreements. Just open-source tools you can trust.**

## Live Servers (16/19 on Official Registry)

### GitOps & Infrastructure
- **ArgoCD** - GitOps continuous delivery
- **Rancher** - Kubernetes management
- **Azure** - Microsoft cloud platform

### CI/CD & Automation
- **Harness** - CI/CD platform
- **Rundeck** - Runbook automation
- **UiPath** - RPA automation

### ITSM & Service Management
- **ServiceNow** - ITSM platform

### CRM & Sales
- **HubSpot** - CRM and marketing automation
- **Zoho CRM** - Customer relationship management

### Finance & Accounting
- **QuickBooks** - Financial management
- **FreshBooks** - Accounting and invoicing
- **Xero** - Cloud accounting

### Analytics & Business Intelligence
- **PowerBI** - Business analytics
- **Tableau** - Data visualization

### Marketing & Communication
- **Mailchimp** - Email marketing
- **Hootsuite** - Social media management
- **Chanty** - Team communication

## Why Open Source MCP Servers?

### No Vendor Lock-In
Some tools have official MCP implementations (Azure, ArgoCD, HubSpot). Many don't. These open-source alternatives give you:

- **MIT Licensed** - Audit the code, know what it does
- **Free Forever** - No licensing fees, no enterprise requirements
- **Fully Customizable** - Fork it, modify it, deploy your way
- **Community Driven** - Features based on real user needs

### Production Ready
- Async/await throughout for high performance
- Retry logic with exponential backoff
- Rate limit handling
- Structured JSON logging
- Comprehensive error handling
- Environment-based configuration

## Quick Start

### Installation

```bash
# Install via uvx (recommended)
uvx servicenow-mcp-server
uvx argocd-mcp-server
uvx azure-mcp-server

# Or via pip
pip install servicenow-mcp-server
```

### Claude Desktop Configuration

```json
{
  "mcpServers": {
    "servicenow": {
      "command": "uvx",
      "args": ["servicenow-mcp-server"],
      "env": {
        "SERVICENOW_INSTANCE": "your-instance.service-now.com",
        "SERVICENOW_USERNAME": "your-username",
        "SERVICENOW_PASSWORD": "your-password"
      }
    }
  }
}
```

### Browse All Servers

Visit the official MCP Registry: **https://registry.modelcontextprotocol.io/**

Search for: **asklokesh**

## Server Status

**Live on Registry:** 16 servers ✅
- All production-ready
- All open source (MIT license)
- All installable via `uvx` or `pip`

**Pending:** 1 server ⏳
- HubSpot (awaiting PyPI README indexing)

**Blocked:** 2 servers ⚠️
- GCP, GitLab (PyPI ownership conflicts)

## Architecture

Every server follows a consistent architecture:

```
server-name-mcp-server/
├── src/
│   ├── server.py          # MCP protocol implementation
│   ├── client.py          # Platform API client
│   ├── auth.py            # Authentication
│   └── config.py          # Configuration
├── tests/                 # Test suite
├── examples/              # Usage examples
└── README.md             # Documentation
```

**Stack:**
- Python 3.8+
- MCP SDK
- Hatchling build system
- PyPI + uvx distribution

## Use Cases

### For SRE Teams
```
"Check if we have any critical ServiceNow incidents"
"Show me failed ArgoCD deployments in the last hour"
"Deploy staging branch to ArgoCD"
```

### For Platform Engineers
```
"List all Azure VMs in production"
"Create a P1 incident in ServiceNow for database outage"
"Run Rundeck job for production deployment"
```

### For Finance Teams
```
"What's our revenue this quarter?" (QuickBooks)
"Show me unpaid invoices" (FreshBooks)
"List all active subscriptions" (Xero)
```

## Contributing

PRs welcome! These are community-driven projects.

1. **Report Issues** - Found a bug? Open an issue
2. **Request Features** - Need something? Let us know
3. **Submit PRs** - Code contributions appreciated
4. **Improve Docs** - Help make our docs better

```bash
# Development setup
git clone https://github.com/asklokesh/[server-name]
cd [server-name]
pip install -e ".[dev]"
pytest
```

## Community & Support

- **GitHub Issues**: Report bugs and request features
- **Pull Requests**: Contribute improvements
- **MCP Registry**: Find all published servers
- **Documentation**: Each repo has detailed README

## Official vs Community Implementations

Some tools have official MCP servers from vendors:
- **Azure** - Microsoft (GA)
- **ArgoCD** - argoproj-labs (Official)
- **HubSpot** - HubSpot (Beta)
- **QuickBooks** - Intuit (Preview, sandbox only)
- **UiPath** - Native platform support
- **Rancher** - SUSE (Tech Preview)

**Why use community versions?**
- Open source vs proprietary
- MIT license vs vendor agreements
- Free vs potential licensing costs
- Customizable vs vendor-controlled
- Community features vs vendor roadmap

Most tools (ServiceNow, Tableau, Zoho, PowerBI, etc.) have **no official MCP servers** - these community implementations fill that gap.

## Current Status (December 2025)

**Accomplishment:** 16 enterprise MCP servers published to official registry

**Built during:** Christmas/New Year holidays 2024-2025

**Impact:** Enterprise teams can now integrate AI with critical business tools using standardized, open-source MCP servers

**Next:** Continue adding servers as community needs them

---

<div align="center">

**Open Source • Production Ready • No Vendor Lock-In**

[Browse Servers](https://registry.modelcontextprotocol.io/) • [Install Guide](#quick-start) • [GitHub](https://github.com/asklokesh)

![Founded](https://img.shields.io/badge/Founded-2024-DC143C?style=flat-square&labelColor=2B2B2B)
![Servers Live](https://img.shields.io/badge/Registry-16%20Live-696969?style=flat-square&labelColor=2B2B2B)
![Open Source](https://img.shields.io/badge/License-MIT-DC143C?style=flat-square&labelColor=2B2B2B)

Built by [@asklokesh](https://github.com/asklokesh) during the holidays 🎄

</div>
