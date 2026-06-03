# ENAM-Portfolio-Manager

wisdom_pm/
├── main.py               ← CLI entry point (Typer)
├── orchestrator.py       ← Full 3-step pipeline runner
├── config.py             ← Thresholds, tickers, bias profiles, sample data
├── requirements.txt
├── .env.example
│
├── agents/
│   ├── quant_analyst.py      Agent 1 — Tool-Calling numerics
│   ├── qual_researcher.py    Agent 2 — RAG + LLM sentiment
│   ├── risk_manager.py       Agent 3 — Portfolio risk flags
│   └── portfolio_manager.py  Agent 4 — Memo synthesis + HITL
│
├── data/market_data.py   ← Yahoo Finance + fallback fundamentals
├── rag/vector_store.py   ← ChromaDB + keyword fallback
├── scoring/wisdom_scorer.py ← 5-principle pure-Python scorer
└── dashboard/terminal_ui.py ← Rich terminal dashboard
