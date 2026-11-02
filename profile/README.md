<h1 align="center">Runelay</h1>

<p align="center">
  <b>The AI gateway for teams that ship with LLMs</b>: one endpoint between your tools and every model provider, with <b>usage tracking, spend limits and full control</b> over who calls what.
</p>

<p align="center">
  Made for devs who want <b>visibility, predictable costs and zero code changes</b>.
</p>

<p align="center">
  <img src="./assets/banner.png" alt="Runelay" width="100%" />
</p>

<p align="center">
  <a href="https://runelay.com">Website</a> ·
  <a href="https://x.com/userunelay">X (Twitter)</a>
</p>

<h2 align="center">Plug it into your stack</h2>

<p align="center">
  Runelay speaks the providers' own protocols. Swap the <b>base URL</b> and the <b>API key</b>, and your code stays the same.
</p>

```ts
import OpenAI from 'openai';

const client = new OpenAI({
	baseURL: 'https://api.runelay.com/v1',
	apiKey: process.env.RUNELAY_API_KEY, // rl_m_...
});

const response = await client.chat.completions.create({
	model: 'gpt-5',
	messages: [{ role: 'user', content: 'Hello from Runelay!' }],
});
```

<p align="center">
  Using Claude Code, Codex or Cursor? Point them at the gateway with two environment variables:
</p>

```bash
export ANTHROPIC_BASE_URL=https://api.runelay.com
export ANTHROPIC_API_KEY=rl_m_...
```

<h2 align="center">Why Runelay</h2>

<p align="center">
  <b>Bring your own keys</b>: connect Anthropic, OpenAI, Gemini and DeepSeek with your org's keys, encrypted at rest.<br />
  <b>Know where the money goes</b>: every request is metered with tokens, cache, latency and cost.<br />
  <b>Set the limits</b>: rate, token and concurrency limits per key and per organization.<br />
  <b>Stay up</b>: automatic failover between keys on 429s, 5xx and timeouts.<br />
  <b>Built for teams</b>: personal and service keys, roles, and per-seat billing.
</p>

<h2 align="center">Get started</h2>

<p align="center">
  Create your organization at <a href="https://runelay.com">runelay.com</a>, connect a provider key and generate a Runelay key. That's it.
</p>
