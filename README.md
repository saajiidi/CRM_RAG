# ShopAI CRM — Streamlit Dashboard

Everything that runs 100% on Streamlit Cloud — no backend needed.

## What's Inside

| Tab | What it does |
|-----|-------------|
| 📊 Dashboard | Live metrics, platform breakdown, AI tool usage |
| 💬 Conversations | Monitor WhatsApp/Instagram/Messenger threads, human takeover |
| 🤖 Test Agent | Chat with the real Claude agent using mock WooCommerce tools |
| 📦 WooCommerce | Browse products, search orders, trigger RAG sync |

## Deploy to Streamlit Cloud

1. Push this folder to a GitHub repo
2. Go to share.streamlit.io
3. Connect your repo → set `app.py` as main file
4. Done!

## Add Your API Key (for Test Agent tab)

Option A — Enter it in the sidebar when the app loads (not saved)

Option B — Add to Streamlit Secrets:
Go to App Settings → Secrets → add:
```
ANTHROPIC_API_KEY = "sk-ant-..."
```

## What This Does NOT Do (needs a backend)
- Receive real WhatsApp/Instagram/Messenger webhooks
- Actually call your WooCommerce store (live data)
- Persist conversations between sessions

For those, deploy a FastAPI backend on Render.com (free tier).
