<div align="center">

# 破甲助手 · AI 统一接入

**一个接口，打通全部主流模型**

GPT · Claude · Gemini · Grok · DeepSeek · Qwen · Kimi　　一套密钥，一个地址

[**立即接入 →**](https://ai.tt2066.top/)　·　[备用入口](https://zz.tt2066.top/)

</div>

---

## 为什么用它

| | |
|---|---|
| **多模型一个入口** | 切模型只改 `model` 字段，不用分别申请一堆账号 |
| **兼容 OpenAI 协议** | base_url 指过来即可，OpenAI SDK、开源客户端、插件、脚本全部直接可用，业务代码零改动 |
| **流式输出** | SSE 逐字返回，聊天类应用体感与官方一致 |
| **额度按量计费** | 用多少扣多少，团队多人共用一份额度，不必给每人单独开号 |
| **密钥集中管理** | 一把密钥分发出去，可随时单独吊销；用量与调用方看得见 |
| **多线路兜底** | 上游抖动自动切换线路，重试放在中转层，客户端不用重写容灾 |

## 接入三步

**1. 注册领密钥** — 打开站点完成注册，在控制台生成 API Key。

**2. 换掉 base_url** — 其余参数保持原样：

```python
from openai import OpenAI

client = OpenAI(
    api_key="sk-你的密钥",
    base_url="https://ai.tt2066.top/v1"
)
```

**3. 照常调用，切模型只改 model**

```python
resp = client.chat.completions.create(
    model="claude-sonnet-4",
    messages=[{"role": "user", "content": "你好"}],
    stream=True
)

for chunk in resp:
    print(chunk.choices[0].delta.content or "", end="")
```

curl 版：

```bash
curl https://ai.tt2066.top/v1/chat/completions \
  -H "Authorization: Bearer sk-你的密钥" \
  -H "Content-Type: application/json" \
  -d '{"model":"gpt-4o","messages":[{"role":"user","content":"你好"}],"stream":true}'
```

## 兼容范围

```
OpenAI Chat Completions      ✅
OpenAI Responses             ✅
流式 SSE                     ✅
function calling / tools     ✅
视觉 / 多模态输入            ✅
任何读取 base_url 的客户端   ✅
```

现有的 NextChat、Cherry Studio、Cursor、沉浸式翻译、各类 SDK，把地址换成 `https://ai.tt2066.top/v1` 即可。

## 常见问题

**要改业务代码吗？**
不用。只要客户端支持自定义 base_url，改一个地址就完成迁移。

**多人共用怎么算？**
一份额度，按实际调用量扣减，用量明细在控制台可查。

**密钥泄露怎么办？**
控制台可单独吊销该密钥，不影响其他密钥。

---

<div align="center">

**[立即接入 → https://ai.tt2066.top/](https://ai.tt2066.top/)**

备用地址：[zz.tt2066.top](https://zz.tt2066.top/)

</div>
