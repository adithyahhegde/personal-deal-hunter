# Personal Deal Hunter

Personal-use, free-first deal discovery for Bengaluru **560073**.

## Status

- v0.4 exists as a local project archive in the original ChatGPT conversation, but **its full source has not yet been uploaded to GitHub**.
- 33 offline tests using synthetic data were reported as passing; no live DesiDime authentication, product retrieval or Telegram alert has been verified.
- Intended source: the official DesiDime OAuth MCP at `https://mcp.desidime.com/mcp`.
- ₹1–₹10 community deals are **unverified leads**, not confirmed 560073 checkout prices.
- Inflated-MRP claims alone are insufficient proof of a genuine bargain.

## Safe setup

Upload the **extracted v0.4 project source files** from the archive in this conversation. Exclude `config.json`, `.env`, OAuth/session tokens, databases, caches, and output records. Replace this README with the longer README shipped in the archive if desired.

Once source files are present:

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
python -m unittest discover -s tests -v
python community_hunter.py --inspect-tools
python community_hunter.py
```

The first live OAuth login must be performed securely by the repository owner. Do not add credentials to GitHub.

GitHub Actions currently runs offline tests only. **Do not turn on 5-minute unattended polling** until DesiDime authentication persistence, usage limits and the platform's access terms are validated. An authenticated local browser session is not automatically available on ephemeral GitHub runners.

This repository is **public**. Do not commit credentials, identifying delivery addresses, or raw deal response logs.