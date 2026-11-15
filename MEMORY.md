Andre preferences (2026-06-12): EXECUTION > design. Honest assessment first. Direct answers. Australia markets. High risk tolerance. End-to-end ownership. Clear status. Wants code/files built not blueprints.

Key files: property-lead-gen-blueprint.md | master-opportunity-database.md | online-money-prompts-framework.md | ultimate-business-discovery-framework.md | C:\Users\andre\property-lead-gen\ (16 files, 146KB code).

To make Hermes powerful: persistent memory, cron jobs for intelligence, feed actual data, use for execution, add tools, feedback loops, multi-step delegation, session search, agent-to-agent workflows, specific outcomes.
§
ENV: Windows host (237GB C: drive, currently full). MSYS bash — forward-slash paths in terminal(). execute_code sandbox uses native Windows paths (r"C:\..."), NOT /c/ paths. PowerShell syntax does NOT work in terminal(). GitHub: A-n-d-i-S-o-c-i-a-L. Hermes skills: 27+ categories, 60+ skills. Cron: 3 jobs. Memory: MEMORY.md + USER.md + MASTER_CONTROL.md in hermes/memories/. Config: max_turns=120, reasoning_effort=ultra, openrouter/nvidia/nemotron-3-ultra-550b-a55b:free model. HERMES X: Fable-class autonomous intelligence system installed 2026-11-13. Windows pitfall: du and find commands HANG on large directories (AppData, PROGRAMS, node_modules). Always use Python os.scandir with depth limiting for disk scans.
§
User asked about making Hermes Agent as powerful as possible. Key insight: the user wants to maximise agent effectiveness, not just get a list. This is a meta-request about agent optimisation.
§
Crypto Faucet Collector built 2026-06-28 at H:\DEV\tools\crypto-faucet-collector\. Supports FreeBitco.in, Cointiply, BonusBitcoin, FireFaucet. Uses Playwright + 2Captcha. Cron job "crypto-faucet-collector" runs hourly. Needs credentials.yaml and 2Captcha API key to go live.
§
Project ToolsRus (ToolScout): Path C:/Users/andre/DEV/ToolsRus. Core intelligence in ToolScout_V3_complete/Toolscout/ai_tool_intelligence/. Uses a CSV database at backups/toolscout_db.csv. Scheduler runs in scheduler/cron_job.py. UI backend runs from web_ui/main.py on port 8081.
§
Updated directory-scraper-development skill with TAAFT/WSJ URL filtering pitfall and TAAFT tool-page enrichment patterns.
§
=== EXTERNAL DRIVE PROJECTS (H:\) — INTEGRATION READY ===

AGENTOS (H:\DEV\ai-tools\AgentOS\):
- Full multi-agent OS: FastAPI backend + React dashboard + free-claude-code proxy (port 8082)
- 6 specialist agents: supervisor, planner, researcher, coder, automation, memory
- Obsidian vault memory at H:\DEV\ai-tools\AgentOS\obsidian_vault\
- Start: .\scripts\start-agentos.ps1 → API:8000, Dashboard:5173, FCC:8082
- Skills: autonomous-ai-agents/hermes-agent, software-development/agentic-trading-systems
- Integrates with: Hermes via HTTP API, kanban-orchestrator for task routing
- **STATUS (2026-11-13): FULLY OPERATIONAL** ✓
  - Health check: OK — model = nvidia/nemotron-3-ultra-550b-a55b:free
  - All 6 agents listed: supervisor, planner, research, coding, automation, memory
  - **ALL AI AGENTS WORKING**: research, coding, planner, supervisor, automation, memory
  - Memory agent: WORKING (local vault)
  - Shell tool: WORKING
  - File operations: WORKING
  - Workflow (deterministic): WORKING
  - Memory listing: WORKING
  - FCC proxy (port 8082): **RUNNING** ✓
  - Frontend (port 5173): **RUNNING** ✓
  - Fixed: .env path resolution bug in main.py + router.py (parent.parent → parent, parents[2])
  - Fixed: load_dotenv(override=True) for hot reload

MASTERMINDOS (H:\DEV\mastermindOS\):
- Web Intelligence OS: Next.js 16 + PostgreSQL + pgvector + Chromium MV3 extension + MCP server
- Stack: pnpm/Turborepo, Better Auth, PostgreSQL direct connections
- Extension API key from web Settings page
- Provider-neutral AI (OpenAI-compatible endpoint for embeddings/reasoning)
- Start: pnpm install → pnpm db:migrate → pnpm auth:migrate → pnpm dev:web
- Build extension: pnpm build:extension → load apps/extension/dist as unpacked

CLAUDE SWARM (H:\DEV\claude-swarm\):
- Multi-agent orchestration PyPI package: pip install claude-swarm
- Dependency-aware scheduling, file conflict detection, Opus quality gate, budget enforcement
- Demo mode: claude-swarm --demo (no API key)
- Real usage: export ANTHROPIC_API_KEY → claude-swarm "task"
- Config: swarm.yaml for custom agent topologies
- Integrates with: kanban-orchestrator (spawn swarm as kanban task), terminal skill
- **STATUS**: Requires Python 3.11+ — available Python 3.10/3.14 have env issues

ATHENA QUANT TRADING (H:\DEV\trading\Athena\):
- Multiple versions: Athena/, AthenaV2/, athena-work/, athena.zip, athenafiles.zip
- Core quant strategies for agentic-trading-systems skill
- Integrates with: agentic-trading-systems skill as additional engine
- **STATUS**: SMC backtested (PF 2.72, 24 trades/year), walk-forward validation needed

ARB-BOT MULTI-EXCHANGE ARBITRAGE (H:\DEV\trading\arb-bot\):
- 18 exchanges, 4 arb types (cross-spot, spot-perp, funding rate, triangular)
- Paper→live progression with risk chassis (daily loss limit, kill switch, engine lock)
- SQLite dashboard: trades, opportunities, spread_history, balance_snapshots
- Config: arb_bot_v2.py with ExchangeConfig per exchange
- MEXC 0% fees = primary arb venue
- Start paper: python arb_bot_v2.py (mode=BotMode.PAPER)
- Skills: software-development/agentic-trading-systems (documents this exact architecture)
- **STATUS (2026-11-13): PAPER TRADING RUNNING** ✓
  - Dedicated venv created at H:\DEV\trading\arb-bot\.venv\
  - Dependencies installed: aiohttp, numpy
  - Detecting live spreads: APTUSDT (0.5%), DOGEUSDT (0.4%), ADAUSDT (0.6%), MATICUSDT (1.0%), BTCUSDT (0.8-1.8%), LINKUSDT (1.2-1.4%)
  - Exchanges active: OKX, MEXC, Bybit, Kraken, Binance
  - Net profits simulated (paper mode)
  - Running in background (pid 13456)

TOOLSCOUT V3 (H:\DEV\ToolsRus\ToolScout_V3_complete\Toolscout\ai_tool_intelligence\):
- Scrapers: FuturePedia, TAAFT, GitHub, Product Hunt, Startup directories
- Processors: cleaning, deduplication, enrichment, funding detection, trend analytics
- Export: Google Sheets with CSV fallback
- Scheduler: daily_job.py with concurrent source collection
- Trend scoring: GitHub stars, PH votes, directory mentions, recency, funding signal
- Skills: software-development/directory-scraper-development (updated with TAAFT fixes)
- Run: .venv\Scripts\activate && python main.py
- **STATUS (2026-11-13): PIPELINE RUNNING** ✓
  - Dedicated venv at .venv with all deps (playwright, pandas, gspread, openai, etc.)
  - Playwright chromium installed
  - Collected 76 entries from GitHub
  - Scraping 12+ directories (TAAFT, FuturePedia, TopAI.tools, FutureTools, etc.)
  - Some blocked by 403/429 (expected — needs web-scraping-resilience skill)
  - Running in background (pid 22232)

CRYPTO FAUCET COLLECTOR (H:\DEV\tools\crypto-faucet-collector\):
- Already configured as Hermes cron job "crypto-faucet-collector" (hourly)
- Playwright + 2Captcha, 4 faucets
- Needs: config/credentials.yaml + 2Captcha API key
- Logs: logs/ directory
- **STATUS**: Credentials.yaml exists but has placeholders; playwright not installed; 27 cron failures

AUTOVENTURE MACHINE (H:\DEV\AutoVentureMachine\):
- Agent swarm framework with YAML configs: scout.yaml, factory.yaml, council.yaml, allocate.yaml
- Swarm orchestration patterns for kanban-orchestrator integration

FREQTRADE (H:\DEV\ai-tools\Freqtrade\):
- Full-featured crypto trading framework (alternative trading engine)
- Install: pip install -e .

=== HERMES X ARCHITECTURE (Installed 2026-11-13) ===

**SOUL.md** — HERMES X Identity (Fable-class autonomous intelligence)
**Operating System** (operating-system/):
- MASTER_OPERATING_DOCTRINE.md — Planning, prioritisation, autonomy, execution
- AUTONOMY_RULES.md — Delegation, approval boundaries, escalation
- DECISION_FRAMEWORK.md — Evidence-based decision methodology
- RESEARCH_STANDARDS.md — Intelligence gathering and validation
- ENGINEERING_STANDARDS.md — Code quality, testing, deployment
- AGENT_ORCHESTRATION.md — Specialist department coordination
- QUALITY_CONTROL.md — Independent verification and audit
- CONTINUOUS_IMPROVEMENT.md — Self-improvement cycle and skill evolution

**Specialist Departments** (skills/hermes-x/):
- exec-intel — Executive Intelligence (strategy, governance)
- research-discovery — Research & Discovery (deep research, CI)
- software-engineering — Software Engineering (architecture, coding, deploy)
- ai-agents — AI & Agent Development (AgentOS, Claude Swarm, AutoVenture)
- business-monetisation — Business & Monetisation (ventures, revenue)
- quant-research — Quantitative Research (trading, arb, risk)
- creative-production — Creative Production (AI media, pipelines)
- quality-security — Quality & Security (independent audit, gates)
- operations — Operations (infra, deploy, monitoring, cron)

**Project Continuity** (projects/):
- XIBALBA, ATHENA, ARB_BOT, TOOLSCOUT, MASTERMIND, AI_MEDIA_FACTORY, VENTURE_STUDIO

=== HERMES SKILLS INSTALLED (27 categories, 60+ skills) ===
Key ready-to-use:
- autonomous-ai-agents: claude-code, codex, computer-use, hermes-agent, kanban-codex-lane, opencode, agentos-backend, autoventure-swarm
- software-development: agentic-trading-systems, directory-scraper-development, web-app-scaffolding, monorepo-scaffolding, subagent-driven-development, test-driven-development
- devops: kanban-orchestrator, kanban-worker, webhook-subscriptions
- research: arxiv, blogwatcher, competitor-news-monitor, grounded-citations, polymarket, mastermind-web-intel
- productivity: notion, linear, google-workspace, airtable, pdf, xlsx, weekly-review-planning
- creative: architecture-diagram, manim-video, comfyui, excalidraw, p5js
- email: himalaya, email-inbox-triage
- github: github-auth, github-code-review, github-issues, github-pr-workflow, github-repo-management
- web: blocked-page-recovery, web-scraping-resilience
- mlops: huggingface-hub, weights-and-biases, llama-cpp, evaluation, vector-databases
- crypto: crypto-arb-bot, crypto-athena, crypto-faucet-automation
- **hermes-x:** exec-intel, research-discovery, software-engineering, ai-agents, business-monetisation, quant-research, creative-production, quality-security, operations

=== CRON JOBS STATUS ===
- Daily Mission Control Briefing (0 9 * * *): ERROR (interrupted) — needs gh CLI auth
- Daily Memory Backup (0 23 * * *): ERROR (connection) — needs GitHub repo A-n-d-i-S-o-c-i-a-L/memo + push auth
- crypto-faucet-collector (0 * * * *): ERROR (27 failures) — needs credentials.yaml + 2Captcha key + playwright install

=== INTEGRATION PRIORITIES ===
1. ~~Start AgentOS backend (local multi-agent API server)~~ ✓ DONE - running on port 8000
2. ~~Fix AgentOS AI agents~~ ✓ DONE - all 6 agents working with nvidia/nemotron-3-ultra
3. Fix crypto-faucet-collector cron (add credentials)
4. Run ToolScout pipeline (integrates with directory-scraper-development skill) ✓ RUNNING
5. Paper-trade arb-bot (validates agentic-trading-systems skill) ✓ RUNNING
6. Install claude-swarm (parallel multi-agent via terminal) — blocked by Python version
7. Create crypto skill category (arb-bot, Athena, faucet) ✓ DONE - 3 skills created
8. Wire ToolScout into Hermes cron
9. Set up Kanban tasks for trading system development
10. ~~Start AgentOS FCC proxy (port 8082) and frontend (port 5173)~~ ✓ DONE
11. **Execute first HERMES X improvement cycle** (7-day target per CONTINUOUS_IMPROVEMENT.md)
12. **Validate department skills** via live workstream delegation