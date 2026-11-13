# Copilot Studio – LOB SharePoint HTML Reports

Reference design for generating one HTML report per line of business (LOB) from a large, frequently updated SharePoint library, built with Copilot Studio workflows (Microsoft Copilot harness) and Dataverse.

| Document | What it covers |
| --- | --- |
| [architecture.html](architecture.html) | One-page architecture: components, data model, design rules |
| [rebuild-spec.html](rebuild-spec.html) | Node-by-node build spec for all six workflows, expressions, prompts and HTML template |

Core idea: process only changed files per LOB, summarize each file once into Dataverse, and render each report from stored summaries with a fixed template. No retrieval (RAG) and no AI-written HTML.
