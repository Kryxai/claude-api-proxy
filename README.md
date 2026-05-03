# KryxAI — Cheap Claude & GPT API Gateway

[![Website](https://img.shields.io/badge/Website-kryxai.com-blue)](https://kryxai.com)
[![API](https://img.shields.io/badge/API-api.kryxai.com-green)](https://api.kryxai.com)

Access **Claude Opus 4.7, Sonnet 4.6, Haiku 4.5, GPT-5.4** and more at **up to 90% off** official pricing.

Drop-in replacement for Anthropic and OpenAI APIs. Works with Claude Code, Cursor, Cline, Codex CLI, and any OpenAI-compatible tool.

## Why KryxAI?

- **80-90% cheaper** than official API pricing
- **Same models, same quality** — requests go to the same Claude/GPT models
- **No subscription** — pay per token, starting from $10
- **No VPN needed** — works worldwide
- **OpenAI-compatible** — change one URL, everything works

## Pricing Comparison

| Model | Official Price (Input/Output per 1M tokens) | KryxAI Price | Savings |
|-------|---------------------------------------------|-------------|--------|
| Claude Opus 4.7 | $15.00 / $75.00 | $2.29 / $11.44 | **85%** |
| Claude Sonnet 4.6 | $3.00 / $15.00 | $1.38 / $6.86 | **54%** |
| Claude Haiku 4.5 | $1.00 / $5.00 | $0.46 / $2.29 | **54%** |
| GPT-5.4 | $3.00 / $10.00 | $0.58 / $3.44 | **81%** |

## Quick Start

### Claude Code (Mac/Linux)

\`\`\`bash
ANTHROPIC_AUTH_TOKEN="your-kryxai-key" \\
ANTHROPIC_BASE_URL="https://api.kryxai.com" \\
claude
\`\`\`

### Claude Code (Windows PowerShell)

\`\`\`powershell
$env:ANTHROPIC_AUTH_TOKEN="your-kryxai-key"
$env:ANTHROPIC_BASE_URL="https://api.kryxai.com"
claude
\`\`\`

### Python (OpenAI SDK)

\`\`\`python
from openai import OpenAI

client = OpenAI(
    api_key="your-kryxai-key",
    base_url="https://api.kryxai.com/v1"
)

response = client.chat.completions.create(
    model="claude-sonnet-4-6",
    messages=[{"role": "user", "content": "Hello!"}]
)
print(response.choices[0].message.content)
\`\`\`

### cURL

\`\`\`bash
curl https://api.kryxai.com/v1/chat/completions \\
  -H "Authorization: Bearer your-kryxai-key" \\
  -H "Content-Type: application/json" \\
  -d '{"model": "claude-sonnet-4-6", "messages": [{"role": "user", "content": "Hello!"}]}'
\`\`\`

## Supported Models

- Claude Opus 4.7 (Most Powerful)
- Claude Opus 4.6
- Claude Sonnet 4.6 (Best Value)
- Claude Haiku 4.5 (Fastest)
- GPT-5.5
- GPT-5.4
- GPT-5.3 Codex

## Features

- **OpenAI-compatible API** — same format as OpenAI/Anthropic
- **Multiple payment methods** — crypto & credit card
- **60 RPM** default rate limit per key
- **Dashboard** — manage keys, view usage, top up balance
- **No region restrictions** — works from anywhere

## API Documentation

Full docs at [kryxai.com/docs](https://kryxai.com/docs)

## Get Started

1. Sign up at [kryxai.com/register](https://kryxai.com/register)
2. Top up from $10
3. Copy your API key
4. Set base URL to \`api.kryxai.com\`
5. Start coding!

## Support

- Email: support@kryxai.com
- Telegram: [@cai85](https://t.me/cai85)
- Website: [kryxai.com](https://kryxai.com)

## License

MIT
