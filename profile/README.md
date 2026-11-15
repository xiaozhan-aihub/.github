## 小战AIhub · XiaoZhan AIhub

多协议大模型 API 网关与 AI 创作平台。一把 `sk-gpushare-` 密钥，用 OpenAI / Anthropic / Google Gemini SDK 调用 120 多款对话、图像、视频、音乐与语音模型。

A multi-protocol AI model gateway and creation platform: one `sk-gpushare-` key lets the OpenAI, Anthropic and Google Gemini SDKs call 120+ chat, image, video, music and speech models.

| 类别 Category | 可调用的模型（部分）Models (selection) |
|---|---|
| 对话大模型 Chat | GPT-6 / GPT-6.1、Claude Opus / Sonnet / Haiku、Gemini 3.8 / 4、DeepSeek V4、Kimi K3、GLM-5.3、通义千问 Qwen3.8、Grok 4.7、MiniMax M2.7 |
| 图像生成 Image | GPT-Image 2 / 2.6、Seedream 5.0、Nano Banana Pro、Qwen Image 3.0、可灵图像 Kling 3.0、Grok Imagine |
| 视频生成 Video | Seedance 2.0 / 2.5、Veo 3.1、可灵 Kling 3.0 / 4.0、Vidu Q3、海螺 Hailuo H3、通义万相 Wan 3.0 |
| 音乐与语音 Audio | Suno V6、语音合成 TTS、声音克隆 voice cloning |

```python
from openai import OpenAI

client = OpenAI(base_url="https://api.dflop.top/v1", api_key="sk-gpushare-...")
resp = client.chat.completions.create(model="gpt-6-luna", messages=[{"role": "user", "content": "你好"}])
print(resp.choices[0].message.content)
```

- [api-examples](https://github.com/xiaozhan-aihub/api-examples)：接入示例（Python / Node.js / curl）：对话、工具调用、识图、生图、视频、音乐、语音合成。Runnable examples.
- [ai-model-api-pricing](https://github.com/xiaozhan-aihub/ai-model-api-pricing)：全部模型的 API 价格表，每日更新，按类别和厂商分页，CC BY 4.0 开放数据（[Hugging Face](https://huggingface.co/datasets/xiaozhan-aihub/ai-model-api-pricing)）。Daily AI model API pricing, open data.
- 官网 Website [model.dflop.top](https://model.dflop.top) · 文档 Docs [model.dflop.top/docs](https://model.dflop.top/docs) · 模型广场 [models](https://model.dflop.top/models) · 给大模型读的索引 [llms.txt](https://model.dflop.top/llms.txt)
