# PowerTokens

**One OpenAI-compatible API for Chinese AI models — video, image, audio and LLMs (Seedance · Wan · Kling · Qwen · GLM · MiniMax · DeepSeek V3.2). No Chinese account required.**

## 🎬 Video Studio 1.12 — free & open source

<a href="https://github.com/PowerTokens/video-studio"><img src="https://raw.githubusercontent.com/PowerTokens/video-studio/main/docs/images/showcase-locker.gif" width="480" alt="Clip generated with Wan 3.0 in PowerTokens Video Studio"></a>

Batch, compare and storyboard videos with Wan · Seedance · Kling and more.

**[▶ Open the web app](https://powertokens.github.io/video-studio-web/)** · **[⬇ Windows desktop app](https://github.com/PowerTokens/video-studio/releases/latest)** · **[Sign up](https://www.powertokens.ai/?utm_source=github&utm_medium=profile&utm_campaign=org)**

## Repositories

| Repo | What it is |
|------|------------|
| [video-studio](https://github.com/PowerTokens/video-studio) | Free Windows desktop + MCP Video Studio (batch / compare / storyboard) |
| [video-studio-web](https://github.com/PowerTokens/video-studio-web) | Web UI companion — runs in the browser |
| [python-examples](https://github.com/PowerTokens/python-examples) | Python + OpenAI SDK quickstart |
| [typescript-examples](https://github.com/PowerTokens/typescript-examples) | Node / TypeScript + OpenAI SDK quickstart |
| [pt-usage-dashboard](https://github.com/PowerTokens/pt-usage-dashboard) | Offline usage & cost dashboard (single HTML file, EN/中文) |
| [awesome-chinese-model-apis](https://github.com/PowerTokens/awesome-chinese-model-apis) | Curated list of Chinese model APIs and gateways |

## Quickstart

Base URL for OpenAI-compatible SDKs: `https://api.powertokens.ai/v1`

```python
import os
from openai import OpenAI

client = OpenAI(
    api_key=os.environ["POWERTOKENS_API_KEY"],
    base_url="https://api.powertokens.ai/v1",
)
resp = client.chat.completions.create(
    model="MiniMax-M3",
    messages=[{"role": "user", "content": "Describe Paris in one sentence."}],
)
print(resp.choices[0].message.content)
```

**Links:** [Website](https://www.powertokens.ai/?utm_source=github&utm_medium=profile&utm_campaign=org) · [Docs](https://docs.powertokens.ai/en/guides/powertokens-quickstart?utm_source=github&utm_medium=profile&utm_campaign=org) · [Models](https://www.powertokens.ai/en/models?utm_source=github&utm_medium=profile&utm_campaign=org) · [Discord](https://discord.gg/JtgtRdhJVS)

---

中文：PowerTokens 一个接口调用国产视频 / 图像 / 大模型，无需国内账号 · [网页版 Video Studio](https://powertokens.github.io/video-studio-web/) · [文档](https://docs.powertokens.ai/)
