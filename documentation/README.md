# Solution Pattern: AI-Powered Application Integration Platform

This solution pattern demonstrates how to build a unified platform that combines:
- Secure data ingestion across environments (Service Interconnect)
- Event-driven messaging architecture (Kafka)
- AI-assisted workflow automation (Agentic Apache Camel + MaaS)
- LLM governance and rate limiting (Connectivity Link)

## Building the documentation

Install Antora CLI:
```bash
npm i -g @antora/cli @antora/site-generator
```

Build the site from project root:
```bash
antora playbook.yml
```

Output: `build/site/solution-pattern-app-connect-ai/index.html`

## Structure

```
documentation/
├── antora.yml                    # Antora component configuration
├── modules/ROOT/
│   ├── nav.adoc                  # Navigation menu
│   ├── pages/
│   │   ├── index.adoc            # Landing page
│   │   ├── 01-pattern.adoc       # Use cases, business story, solution overview
│   │   ├── 02-architecture.adoc  # Technical deep dive
│   │   ├── 03-demo.adoc          # Demo walkthrough
│   │   └── 04-devresources.adoc  # Developer resources
│   └── assets/images/            # SVG icons and diagrams
```

## Related Resources

- Hands-on workshop: [showroom/](../showroom/)
- Reference pattern: [solution-pattern-multi-channel-messaging-platform/](../solution-pattern-multi-channel-messaging-platform/)

## Contributors

Bruno Meseguer (Red Hat)
