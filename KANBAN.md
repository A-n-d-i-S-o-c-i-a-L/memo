# KANBAN BOARD — XIBALBA Mission Control
> Auto-maintained. Last updated: 2026-11-13

## 🔵 BACKLOG
- Create premium skill packs for HermesHub
- Build knowledge graph memory system
- Implement multi-agent delegation framework
- Add cost optimization / model routing engine
- Build mobile app for Xibalba
- Create onboarding flow for new users
- Wire ToolScout into Hermes cron job
- Integrate MastermindOS browser extension workflow
- Integrate Claude Swarm for parallel multi-agent execution (needs Python 3.11+)
- Fix AgentOS OpenRouter API — USER MUST PROVIDE REAL API KEY
- Start AgentOS FCC proxy (port 8082) and frontend (port 5173)

## 💡 IDEAS
- Holographic memory system (vector + graph hybrid)
- Agent marketplace (share/trade agent configurations)
- Voice interface for Xibalba
- Automated skill generation from workflow patterns
- Crypto portfolio tracking dashboard in Xibalba
- Integration with more CEX/DEX for arb detection
- AutoVentureMachine swarm patterns as kanban templates

## 🔍 RESEARCH
- x402/MPP payment rail implementation details
- LangGraph vs custom workflow engine comparison
- Vector memory best practices (pgvector vs dedicated)
- Agent-to-agent communication protocols
- LLM provider failover strategies
- AgentOS multi-agent API integration patterns
- MastermindOS MCP server integration
- ToolScout 403/429 scraping resilience patterns

## 📋 PLANNING
- Hermes Agent integration architecture for Xibalba
- Live trading go-live criteria and risk framework
- Xibalba deployment and infrastructure plan
- Monetization strategy (SaaS tiers vs free)
- AgentOS ↔ Hermes API contract design
- ToolScout scheduled ingestion pipeline
- Arb-bot paper trading validation checklist
- FCC proxy + frontend startup sequence
- Crypto faucet collector credentials setup

## ✅ READY
- Wire Xibalba frontend to real API
- Implement goal management system
- Create Kanban board view in Xibalba
- Set up WebSocket for real-time monitoring
- Fix ToolScout CI
- Review smashmeter PR #80
- Follow up on HermesHub PRs (#103, #104, #105) — all mergeable, awaiting review
- Fix crypto-faucet-collector cron (add credentials.yaml + 2Captcha key)
- Install computer-use driver (hermes computer-use install)

## 🔄 IN PROGRESS
- Xibalba OS core development (agentic OS)
- HermesHub skills awaiting review
- Multi-exchange arb bot (paper trading) ✓ RUNNING
- ToolScout V3 pipeline (daily ingestion) ✓ RUNNING
- **AgentOS backend service RUNNING on port 8000** ✓

## ⏳ WAITING
- HermesHub PR review (Codex re-scan + human reviewer) — PRs #103, #104, #105 open since June
- Xibalba PR review — PR #7 (personas), PR #8 (Phase 1 connector status) open
- ToolScout CI fix (GitHub Actions platform issue) — recurring startup failures
- Market conditions for live trading decision
- Athena CI fix (claude/lookahead-harness branch) — repeated failures
- tradefarm CI fix (hardening/paper-release-candidate branch) — repeated failures
- crypto-faucet-collector credentials + playwright
- gh CLI authentication for daily briefing cron
- GitHub repo A-n-d-i-S-o-c-i-a-L/memo creation for memory backup
- **AgentOS AI agents — USER MUST PROVIDE OPENAPI KEY IN .env**
- Claude Swarm install (Python 3.11+ env)

## 🚫 BLOCKED
- ToolScout CI — GitHub Actions startup_failure (platform issue, not code)
- Live trading → needs risk framework sign-off
- Multi-agent mode → needs Xibalba agent runner implementation
- Daily briefing cron → needs gh auth
- Memory backup cron → needs GitHub repo + auth
- Faucet collector cron → needs credentials + 2Captcha
- **AgentOS AI agents → needs real OpenRouter API key in .env**
- Claude Swarm → needs Python 3.11+ environment

## 📝 REVIEW
- smashmeter PR #80 — comprehensive accessibility improvements
- Xibalba initial architecture → needs wire-up and auth
- Agentic-trading-systems skill validation via arb-bot paper trading ✓ RUNNING
- Directory-scraper-development skill validation via ToolScout run ✓ RUNNING
- AgentOS backend integration test: memory, shell, files, workflow all working ✓
- Arb-bot paper mode detecting real spreads across 5 exchanges ✓

## ✅ COMPLETED
- SOUL.md created
- Master Control document created
- 21 HermesHub skills submitted
- 49 duplicate smashmeter PRs closed
- Initial Xibalba architecture (FastAPI + Next.js + PostgreSQL + Redis)
- Multi-provider LLM abstraction (9 providers)
- Agent & Workflow CRUD APIs
- Frontend dashboard UI
- SMC strategy backtested (PF 2.72)
- Multi-exchange arb bot (paper trading)
- MEMORY.md updated with external project inventory
- directory-scraper-development skill updated with TAAFT fixes
- Hermes skills inventory documented (27 categories, 60+ skills)
- **6 new crypto/autonomous skills created**: crypto-arb-bot, crypto-athena, crypto-faucet-automation, agentos-backend, mastermind-web-intel, autoventure-swarm
- **AgentOS backend RUNNING on port 8000** — health, agents, memory, shell, files, workflow all verified
- **Arb-bot paper trading RUNNING** — dedicated venv, detecting spreads on 5 exchanges
- **ToolScout pipeline RUNNING** — dedicated venv, playwright installed, 76 GitHub entries, 12+ directories