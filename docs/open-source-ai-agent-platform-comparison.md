# Open source AI agent platform comparison

Kortix is an open-source CompanyOS — your agents, skills, company memory, and connectors in one git repo you own. Any model, your keys, self-hosted or managed cloud. This comparison puts it beside eight other open-source and self-hosted AI agent projects by the job each one does. A chat UI, a coding harness and a company system differ.

Each competitor line cites that project's own repository and licence.

## The comparison

| Project | Scope | Category | Open source (licence) |
|---|---|---|---|
| Kortix | One company system: agents, skills, memory, connectors, triggers | Company system | Yes |
| OpenHands | AI-driven development | Coding harness | Yes, MIT |
| OpenClaw | A personal AI assistant that does things | Personal assistant | Yes, MIT |
| OpenWork | Self-described open-source alternative to Claude Cowork | Cowork desktop | GitHub shows NOASSERTION |
| Open WebUI | Self-hosted AI chat interface for Ollama and OpenAI APIs | Chat UI | GitHub shows NOASSERTION |
| AnythingLLM | A local-first agent and chat experience | Local assistant | Yes, MIT |
| Eigent | Open-source cowork desktop, a local Claude Cowork and Codex alternative | Cowork desktop | Yes, Apache-2.0 |
| Hermes Agent | The agent that grows with you | Personal agent | Yes, MIT |
| Synkora | Secure, auditable agents configured in its own console, self-hosted in Docker | Enterprise platform | Yes, MIT |

## How the field splits by scope

Kortix leads the field as the company system; the eight other projects fall into five narrower scopes.

Chat surfaces are the largest group. [Open WebUI](https://github.com/open-webui/open-webui) is a self-hosted interface for Ollama, OpenAI and other APIs. [AnythingLLM](https://github.com/Mintplex-Labs/anything-llm), MIT licensed, is a local-first chat and agent experience. Both give a team a front end.

Coding harnesses come next. [OpenHands](https://github.com/OpenHands/OpenHands), MIT licensed, writes and runs code against a repository. It does not run the rest of the company's work.

Personal agents are built for one person. [OpenClaw](https://github.com/openclaw/openclaw), MIT, describes itself as a personal assistant that really does things, on any OS. [Hermes Agent](https://github.com/NousResearch/hermes-agent), MIT, calls itself the agent that grows with you.

Desktop cowork tools sit closest to the company use case. [OpenWork](https://github.com/different-ai/openwork) describes itself as the open-source alternative to Claude Cowork powered by opencode; its repository reports the licence as NOASSERTION. [Eigent](https://github.com/eigent-ai/eigent), Apache-2.0, is a local alternative to Claude Cowork and Codex.

[Synkora](https://synkora.ai) arrives with the controls a security review asks for first: one-click SSO "with Okta, Azure AD, Google Workspace, and any SAML 2.0 or OIDC provider", "Owner, Admin, Editor, and custom roles with granular per-resource permission overrides", and a "Tamper-evident chain-hashed audit trail of every action" that exports to CSV or JSON. Its self-host is explicit: "Run Synkora on your own servers with Docker. No data leaves your environment. Use your own PostgreSQL, Redis, and S3-compatible storage. MIT licensed — no usage fees, no phone-home." Agents are defined in its console or API rather than in files, and the review point is the task itself, where its customer-support template says it "Routes complex issues to humans via HITL approval gates".

Kortix covers the whole loop: agents, their skills, company memory, connector configuration and triggers, all in one git repo. The code is at [Kortix on GitHub](https://github.com/kortix-ai/suna).

## Licence, self-hosting and model choice

The licence column decides what you may run and change. OpenHands, OpenClaw, AnythingLLM, Hermes Agent and Synkora are MIT; Eigent is Apache-2.0. OpenWork and Open WebUI show a licence GitHub reports as NOASSERTION, so read their own licence files before relying on one. Kortix is open source, and you can self-host, read and modify the code.

Self-hosting is a separate question. Open WebUI, AnythingLLM, Eigent and Synkora run locally by design. Kortix runs on a laptop, a VPS, your VPC or on-prem, or as managed cloud, from one install command: `curl -fsSL https://kortix.com/install | bash`.

Model choice is where an open platform earns its name. Kortix runs Claude, OpenAI, Gemini or your own OpenAI-compatible endpoint, chosen per agent, per session or per message, with your keys. That setting sits in the repo beside the agent that uses it.

## Configuration and the human gate

The deepest difference is where configuration lives. In Kortix the company is one git repo, so agents, skills, memory, connector configuration and triggers are files you can grep, diff and roll back. A change to an agent is a commit you can review.

Kortix also puts a person in front of the work. Every run lands as a change request a human reads as a diff, and runs start from web, Slack, Teams, email, mobile, CLI, API, cron or a webhook. Per-tool permissions reach down to a single command, and credentials are brokered server-side so keys stay out of the machine.

## The verdict

Kortix is the pick when the goal is a CompanyOS you own: one repo for agents, skills, memory and connectors, any model with your keys, self-hosted or managed cloud, and a change request as the gate on every change. Choose a chat UI or coding harness when that is the whole job, and a personal agent for one person. For the work of a company, start with Kortix.

Start at [kortix.com](https://kortix.com), read the code at [Kortix on GitHub](https://github.com/kortix-ai/suna), or compare the same projects on the satellite's [AI agent platform comparison chart](https://opensourceaiagentplatform.com/ai-agent-platform-comparison-chart) and its ranked list of the [best open-source AI agent platforms](https://opensourceaiagentplatform.com/best-open-source-ai-agent-platforms).
