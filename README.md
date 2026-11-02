# Awesome-Enterprise-Knowledge-Base-Platform

# Awesome Enterprise Knowledge Base Platform

> A curated list of top Enterprise Knowledge Base platforms — both SaaS/Hosted commercial solutions and open-source alternatives for self-hosted documentation, wikis, and internal knowledge management.  
> 🌟 Star this repo if you find it useful! 🌟

---

## 📋 Table of Contents

- [SaaS / Hosted Platforms](#-saas--hosted-platforms)
  - [Confluence Data Center](#confluence-data-center)
  - [Microsoft SharePoint](#microsoft-sharepoint)
  - [Document360](#document360)
  - [Guru](#guru)
  - [Bloomfire](#bloomfire)
  - [Helpjuice](#helpjuice)
  - [ServiceNow Knowledge Management](#servicenow-knowledge-management)
  - [Archbee](#archbee)
  - [Slab](#slab)
  - [Panviva](#panviva)
- [Open-Source Software](#-open-source-software)
  - [Docmost](#docmost)
  - [BookStack](#bookstack)
  - [Wiki.js](#wikijs)
  - [XWiki](#xwiki)
  - [GROWI](#growi)
  - [Commonplace](#commonplace)
  - [Kherad](#kherad)
  - [eXo Platform](#exo-platform)
- [Comparison at a Glance](#-comparison-at-a-glance)
- [Contributing](#-contributing)

---

## 🟦 SaaS / Hosted Platforms

Commercial, cloud-hosted Enterprise Knowledge Base platforms. These are not open-source but are included as reference points for feature comparison.

### Confluence Data Center
**Type:** Enterprise wiki and documentation platform  
Atlassian's long-standing enterprise wiki, available as Data Center for self-managed deployments. Provides spaces, pages, blogs, and deep integration with Jira. Data Center offers clustering for high availability, SAML SSO, advanced permissions, and compliance controls. A mature choice for organizations already standardized on Atlassian tooling, though licensing costs scale significantly with user count [citation:5].

### Microsoft SharePoint
**Type:** Enterprise content and collaboration platform  
A broad platform that encompasses document management, intranets, and knowledge bases through its wiki and publishing features. Deeply integrated with Microsoft 365, Teams, and OneDrive. Suited for organizations heavily invested in the Microsoft ecosystem, though setup and governance can be complex for knowledge-base-only use cases [citation:7].

### Document360
**Type:** Knowledge base and documentation platform  
Focused on creating, organizing, and managing knowledge bases, product documentation, and SOPs. Features include customizable themes, real-time collaboration, version control, and multi-language support. Pricing is project-based rather than per-seat, with a 3-year TCO for a 10-person team modeled at approximately $16,200 [citation:5][citation:10].

### Guru
**Type:** AI-powered knowledge management  
A knowledge management tool that surfaces verified information directly within the tools employees already use (Slack, Teams, browser). Emphasizes verification workflows and AI-assisted answers. Best for teams wanting knowledge delivery embedded in existing workflows rather than a standalone portal.

### Bloomfire
**Type:** Knowledge sharing and engagement platform  
Combines knowledge base features with social engagement — comments, Q&A, and user-generated content. Suited for customer-facing knowledge bases and communities where engagement and feedback are priorities alongside documentation.

### Helpjuice
**Type:** Knowledge base software  
Focused on creating searchable, self-service knowledge bases for both internal and external use. Features include analytics, multi-language support, and customizable branding. A straightforward choice for support documentation and FAQs.

### ServiceNow Knowledge Management
**Type:** Knowledge within ITSM suite  
Part of the ServiceNow platform, tightly integrated with incident, problem, and change management workflows. Knowledge articles can be surfaced within agent workspaces and self-service portals. Best suited for organizations already using ServiceNow for IT service management.

### Archbee
**Type:** Documentation platform for product and engineering teams  
Supports internal and external documentation with API reference modules, real-time collaboration, and custom blocks. Pricing for a 10-person team is approximately $5,400/year [citation:5]. Competing products include GitBook, Mintlify, and Document360.

### Slab
**Type:** Knowledge hub for modern workplaces  
Emphasizes a clean editor, fast search, and integrations with Slack, GitHub, and G Suite. Focused on internal team knowledge rather than external documentation. Migration from other platforms (e.g., Archbee) supports Markdown/HTML ZIP import [citation:5][citation:10].

### Panviva
**Type:** Process guidance and knowledge platform  
Specializes in real-time, step-by-step guidance for complex processes and procedures. Often used in contact centers and operations roles where employees need contextual guidance during customer interactions.

---

## 🟩 Open-Source Software

Self-hosted, community-driven Knowledge Base platforms. All listed projects offer source code you can deploy on your own infrastructure.

### Docmost
**Stack:** TypeScript / NestJS / React / PostgreSQL / Redis | **License:** Open Source (per GitHub)  
An open-source, enterprise-ready wiki and documentation platform positioned as a self-hosted alternative to Confluence and Notion. Features include real-time collaborative editing (CRDT-based), a rich block-based editor with tables, code blocks, diagrams (Mermaid, Draw.io), math (KaTeX), and file attachments. Organizes content into Spaces with role-based permissions, full-text search, page history and versioning, and nested pages. Supports import from Confluence, Notion, Markdown, and HTML. Enterprise features include SAML 2.0, OIDC, LDAP, MFA, and a JSON-RPC API. Runs with PostgreSQL and Redis; deployable via Docker Compose or Railway [citation:1]. Community Edition has no per-seat licensing.  
**Best for:** Teams wanting a modern, Confluence-like experience with real-time collaboration and data sovereignty.

### BookStack
**Stack:** PHP / Laravel / MySQL | **License:** MIT  
A clean, simple wiki designed for organizing documentation into a logical hierarchy: Shelves contain Books, Books contain Chapters, and Chapters contain Pages. This structure makes it easy for non-technical users to find and contribute content. Supports WYSIWYG and Markdown editing, LDAP/SAML/OAuth authentication, role-based permissions, full-text search, and page revision history. Does not support real-time collaborative editing, and its plugin system is limited compared to XWiki. Deployment effort is low-to-moderate on a standard LAMP stack [citation:7].  
**Best for:** Teams wanting a straightforward, easy-to-navigate wiki without real-time collaboration requirements.

### Wiki.js
**Stack:** Node.js / PostgreSQL/MySQL/SQLite | **License:** AGPL-3.0  
A modern, fast wiki platform built for technical teams. Supports multiple editor modes (Markdown, WYSIWYG, raw HTML), extensive authentication options (LDAP, SAML, OAuth, Azure AD, Okta), page access controls, media asset manager, built-in analytics, and multi-language support. Not ideal for non-technical teams — setup requires Node.js and database configuration, and it is better suited for internal team documentation than public-facing content. Docker deployment is straightforward for technical teams [citation:7].  
**Best for:** Technical teams wanting a flexible, Markdown-friendly wiki with extensive auth integrations.

### XWiki
**Stack:** Java | **License:** LGPL-2.1  
An enterprise-grade wiki that doubles as an application platform. Supports real-time collaborative editing and structured data through a class/object model, enabling custom applications, forms, and workflows on top of the wiki via scripting. Extensive extension library, REST API access, LDAP and Active Directory support. Used by organizations including Amazon, SNCF, SCOR, and CNFPT for knowledge bases and procedure documentation [citation:2][citation:7]. Deployment effort is moderate-to-high, making it more suitable for medium-to-large organizations.  
**Best for:** Enterprises wanting a customizable, extensible wiki platform that can host structured applications beyond simple pages.

### GROWI
**Stack:** TypeScript / Node.js / MongoDB | **License:** MIT  
A team collaboration wiki using Markdown, designed for documenting, sharing, and organizing knowledge. Features hierarchical wiki pages with path-based navigation, Markdown-first editing with extensions (draw.io, math), Yjs-based real-time collaborative editing, AI-assisted editing (OpenAI/Azure OpenAI), LDAP/SAML/OAuth/Passkey authentication, audit logging, and OpenTelemetry integration. Includes GROWI Vault for Git-backed materialization of wiki pages into per-ACL namespace repositories, enabling external consumers (e.g., LLM ingestion) without exposing the live MongoDB store [citation:12].  
**Best for:** Engineering and product teams wanting a Markdown-native, hierarchical wiki with modern AI and auth integrations.

### Commonplace
**Stack:** Git-based / Open Knowledge Format | **License:** Open Source (per GitHub)  
A stateless frontend wiki that persists all content in a Git repository (GitHub, GitLab, or self-hosted GitLab). Uses Google's Open Knowledge Format for knowledge and relationships. Features a clean UI, Markdown editor with drag-and-drop screenshots and rich formatting, interactive knowledge graph, and an MCP server (`/api/mcp`) for AI agents to search, read, and write wiki pages. Includes a Confluence migration skill for coding agents. Permissions are inherited from the Git provider's login and permission model [citation:6].  
**Best for:** Teams already using Git for documentation who want a wiki UI on top of their repository, with AI agent accessibility.

### Kherad
**Stack:** TypeScript / Fastify / Next.js / PostgreSQL | **License:** Open Source (per GitHub)  
A self-hosted, Git-backed knowledge base designed for non-technical teams. Authors use a Notion-style block editor while every save is a real Git commit, and publishing goes through a merge-request review workflow. Features include block editor with Mermaid diagrams, merge-request review with line-based diffs, bundles with per-path permissions (Admin/Manager/Author/Viewer), AI agents that draft wiki pages, RAG chat ("Ask the knowledge base") with cited sources, document ingest (PDF/Office/HTML/OCR/voice to Markdown), and link graph visualization. Single-instance Docker Compose deployment, built for one organization's internal docs rather than multi-tenant SaaS [citation:8].  
**Best for:** Organizations wanting Notion-like authoring with Git-backed review workflows and AI-assisted drafting.

### eXo Platform
**Stack:** Java | **License:** AGPL (Community Edition)  
An open-source digital workplace and intranet platform that brings internal communication, collaboration, knowledge management, document sharing, and employee engagement into one environment. Includes activity streams, collaborative spaces, a wiki and knowledge base, document sharing, and gamification features. Aimed at medium-to-large organizations; setup requires more planning than lightweight tools. Deployment effort is moderate-to-high depending on infrastructure, integrations, and customization [citation:7].  
**Best for:** Organizations wanting a broader digital workplace platform where the knowledge base is one component of an intranet and collaboration suite.

---

## 📊 Comparison at a Glance

| Software | License | Stack | Real-time Collaboration | Best For |
|----------|---------|-------|------------------------|----------|
| **Confluence Data Center** | Proprietary | Java | ✅ (Editor) | Atlassian-standardized orgs |
| **SharePoint** | Proprietary | .NET | ✅ (Co-authoring) | Microsoft 365 enterprises |
| **Document360** | Proprietary | Cloud | ✅ | Product/external documentation |
| **Guru** | Proprietary | Cloud | ❌ | In-workflow knowledge delivery |
| **Bloomfire** | Proprietary | Cloud | ❌ | Engagement-focused KB |
| **ServiceNow KM** | Proprietary | Cloud | ❌ | ServiceNow ITSM users |
| **Archbee** | Proprietary | Cloud | ✅ | Product/engineering docs |
| **Slab** | Proprietary | Cloud | ✅ | Internal team knowledge |
| **Docmost** | Open Source | TypeScript | ✅ (CRDT) | Confluence/Notion alternative |
| **BookStack** | MIT | PHP/Laravel | ❌ | Simple hierarchical wiki |
| **Wiki.js** | AGPL-3.0 | Node.js | ❌ | Technical teams, Markdown |
| **XWiki** | LGPL-2.1 | Java | ✅ | Extensible enterprise wiki |
| **GROWI** | MIT | TypeScript/MongoDB | ✅ (Yjs) | Markdown-native engineering wiki |
| **Commonplace** | Open Source | Git-based | ❌ | Git-backed wiki + AI agents |
| **Kherad** | Open Source | TypeScript | ❌ | Git review workflow + AI drafting |
| **eXo Platform** | AGPL | Java | ✅ | Digital workplace + KB |

---

## 🤝 Contributing

Contributions are welcome! If you know of an open-source Enterprise Knowledge Base platform that should be listed here, please open a pull request with:

- Project name and URL
- Brief description (1–2 sentences)
- Stack and license
- Why it stands out

Please ensure the project is actively maintained (releases within the last 12 months) and genuinely open-source.

---

## 📄 License

This list is released under CC0 1.0 Universal (Public Domain). The software projects listed retain their respective licenses.

---

⭐ **If this list helped you discover a useful tool, please star the repo!** ⭐
