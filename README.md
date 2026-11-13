# Copilot Studio – LOB SharePoint HTML Reports

Reference design for generating one HTML report per line of business (LOB) from a large, frequently updated SharePoint library, built with Copilot Studio workflows (Microsoft Copilot harness) and Dataverse.

| Document | What it covers |
| --- | --- |
| [architecture.html](architecture.html) | Start here: plain-language overview of how the system works, with a glossary |
| [rebuild-spec.html](rebuild-spec.html) | Step-by-step build guide: tables, six workflows in build order, tests and troubleshooting |

Core idea: process only changed files per LOB, summarize each file once into Dataverse, and render each report from stored summaries with a fixed template. No retrieval (RAG) and no AI-written HTML.
