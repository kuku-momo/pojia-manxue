<div align="center">

# 破甲助手 · 满血版

**一个接口，打通全部主流模型　—　全程大白话，不绕弯子**

GPT · Claude · Gemini · Grok · DeepSeek · Qwen · Kimi　　一套密钥，一个地址

[**立即接入 →**](https://ai.tt2066.top/)　·　[备用入口](https://zz.tt2066.top/)

</div>

---

## 破甲满血版是什么

**破甲助手**是我在做的 AI 统一接入服务。**满血版**的意思是：上游账号额度给足、线路不砍、不给你降智，模型该多聪明就多聪明。

下面这些，全部用**大白话**讲，不堆术语。

| | |
|---|---|
| **多模型一个入口** | 切模型只改 `model` 一个字段，不用分别去申请一堆账号，也不用来回切平台 |
| **兼容 OpenAI 协议** | base_url 指过来就行，OpenAI SDK、开源客户端、插件、脚本全都能直接用，业务代码一行不用改 |
| **流式输出** | SSE 逐字返回，聊天类应用跟官方体感一样，不会憋半天才吐一句 |
| **额度按量计费** | 用多少扣多少，团队多人共用一份额度，不必给每个人单独开号 |
| **密钥集中管理** | 一把密钥发出去，随时能单独吊销；谁在用、用了多少，后台都看得见 |
| **多线路兜底** | 上游抖动自动切线路，重试放在中转层，客户端不用自己写容灾 |

## 大白话破甲：三步接入

**1. 注册领密钥** — 打开站点注册，控制台点一下生成 API Key。

**2. 换掉 base_url** — 就改这一行，别的都别动：

```python
from openai import OpenAI

client = OpenAI(
    api_key="sk-你的密钥",
    base_url="https://ai.tt2066.top/v1"
)
```

**3. 照常调用，换模型只改 model**

```python
resp = client.chat.completions.create(
    model="claude-sonnet-4",
    messages=[{"role": "user", "content": "你好"}],
    stream=True
)

for chunk in resp:
    print(chunk.choices[0].delta.content or "", end="")
```

不想写代码就用 curl：

```bash
curl https://ai.tt2066.top/v1/chat/completions \
  -H "Authorization: Bearer sk-你的密钥" \
  -H "Content-Type: application/json" \
  -d '{"model":"gpt-4o","messages":[{"role":"user","content":"你好"}],"stream":true}'
```

## 能用在哪

```
OpenAI Chat Completions      ✅
OpenAI Responses             ✅
流式 SSE                     ✅
function calling / tools     ✅
视觉 / 多模态输入            ✅
任何读 base_url 的客户端    ✅
```

NextChat、Cherry Studio、Cursor、沉浸式翻译、各类 SDK —— 把地址换成 `https://ai.tt2066.top/v1`，就完事了，满血版直接跑起来。

## 常见问题（还是大白话）

**要改我的业务代码吗？**
不用。你的客户端能填 base_url，就改那一个地址，别的一个字不用动。

**多人一起用怎么算钱？**
一份额度，按实际调用量扣，用量明细后台能查，谁的账谁的。

**密钥要是漏了怎么办？**
后台单独吊销那一把，其他密钥照常用，不用全场换钥匙。

**满血版跟普通版差在哪？**
额度给足、线路不降级、响应不缩水。破甲满血讲的就是这个。

---

<div align="center">

**[立即接入 → https://ai.tt2066.top/](https://ai.tt2066.top/)**

备用地址：[zz.tt2066.top](https://zz.tt2066.top/)

破甲助手 · 满血版 · 大白话讲清楚

</div>
