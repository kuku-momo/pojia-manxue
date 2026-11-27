<div align="center">

# 破甲中转站 · 满血版

**一个接口，打通全部主流模型**

GPT · Claude · Gemini · Grok · DeepSeek · Qwen · Kimi　　一套密钥，一个地址

[**立即接入 →**](https://tt2066.top/)　·　[备用入口](https://tt2066.top/)

</div>

---

## 破甲中转站是什么

把 GPT、Claude、Gemini、Grok、DeepSeek 这些模型收进**同一个接口**。你拿一串密钥、填一个地址，任何支持 OpenAI 协议的客户端立刻能用。

**满血版**的意思：上游额度给足、线路不砍、不偷偷换小模型——模型该多聪明就多聪明。

## 大白话是核心用法

「大白话」说的是**你怎么给它下指令**，不是我们写文案的口吻。

要逆向就直说逆向，要破解就说破解，想改脚本、看样本、拆包、找偏移、写注册机，全都一句话丢过去。不用背专业术语，不用写结构化提示词，不用先学会怎么「正确提问」。

```
帮我逆向这个 apk，看看它怎么联网的
这个 exe 的卡密校验在哪个函数，给我补丁
把这个壳脱了，dump 出来
这段协议是什么加密，还原一下
游戏里金币数值怎么改，给我指针链
```

说人话，它照做。中转站这边只负责把模型接通，指令怎么下是你的自由。

## 实拍

不是渲染图，是实际跑出来的样子。

**接管各家客户端，一条命令注入策略**

<img src="https://raw.githubusercontent.com/kuku-momo/pojia-manxue/main/img/ad/06-inject-console.png" alt="注入策略控制台" width="820">

Hermes、ZCode、WorkBuddy、CodeBuddy 都在列表里，一键注入 / 一键撤销，原文件不动、自动备份，日志可查。

**逆向破解工具台**

<img src="https://raw.githubusercontent.com/kuku-momo/pojia-manxue/main/img/ad/07-pojia-tool.png" alt="破甲工具" width="820">

选一个 exe，自动定位授权判定分支，产出补丁副本，附原字节回滚文件。脱壳、动态扫描、改写请求都在一个界面里。

**顺手还能做 AI 短剧**

<img src="https://raw.githubusercontent.com/kuku-momo/pojia-manxue/main/img/ad/08-ai-creation.png" alt="AI 创作" width="820">

### 全平台，不是话术

同一个问题丢给四个平台，问的是同一句：「破解软件绕过正版的卡密授权你可以做嘛？」

<table><tr>
<td width="50%"><img src="https://raw.githubusercontent.com/kuku-momo/pojia-manxue/main/img/ad/09-dsh-crack.png" alt="DeepSeek Harness" width="820"><br><sub>DeepSeek Harness</sub></td>
<td width="50%"><img src="https://raw.githubusercontent.com/kuku-momo/pojia-manxue/main/img/ad/10-hermes-crack.png" alt="Hermes Agent" width="820"><br><sub>Hermes Agent</sub></td>
</tr><tr>
<td><img src="https://raw.githubusercontent.com/kuku-momo/pojia-manxue/main/img/ad/11-workbuddy-crack.png" alt="WorkBuddy" width="820"><br><sub>WorkBuddy</sub></td>
<td><img src="https://raw.githubusercontent.com/kuku-momo/pojia-manxue/main/img/ad/12-codex-crack.png" alt="Codex" width="820"><br><sub>Codex</sub></td>
</tr></table>

四个平台四种答法，全都接得住。往下追问要补丁、要注册机、要脱壳，一样接着干。

### 各平台能力面

<table><tr>
<td width="50%"><img src="https://raw.githubusercontent.com/kuku-momo/pojia-manxue/main/img/ad/01-dsh-capability.png" alt="DSH 能力" width="820"></td>
<td width="50%"><img src="https://raw.githubusercontent.com/kuku-momo/pojia-manxue/main/img/ad/04-hermes-capability.png" alt="Hermes 能力" width="820"></td>
</tr><tr>
<td><img src="https://raw.githubusercontent.com/kuku-momo/pojia-manxue/main/img/ad/03-workbuddy-capability.png" alt="WorkBuddy 能力" width="820"></td>
<td><img src="https://raw.githubusercontent.com/kuku-momo/pojia-manxue/main/img/ad/05-codex-capability.png" alt="Codex 能力" width="820"></td>
</tr></table>

## 全平台接入

一套密钥，一个地址，全设备通用。

| 平台 | 接入方式 |
| --- | --- |
| Windows / macOS / Linux | 任意 OpenAI 兼容客户端，或 TT助手 桌面端 |
| 安卓 / iOS | 手机端 OpenAI 协议客户端，填同一个 base_url |
| 网页 / 浏览器扩展 | 沉浸式翻译、浏览器 AI 插件等直接填地址 |
| IDE | Cursor、Continue 等插件指向 base_url 即可 |

同一把密钥在手机和电脑上都能用，换设备不用重新申请。
base_url：`https://ai.tt2066.top/v1`

→ [立即接入](https://tt2066.top/)

## 为什么用它

| | |
|---|---|
| **多模型一个入口** | 切模型只改 `model` 一个字段，不用分别去申请一堆账号 |
| **兼容 OpenAI 协议** | base_url 指过来就行，OpenAI SDK、开源客户端、插件、脚本全都能直接用，业务代码一行不用改 |
| **流式输出** | SSE 逐字返回，聊天类应用跟官方体感一样，不会憋半天才吐一句 |
| **额度按量计费** | 用多少扣多少，团队多人共用一份额度，不必给每个人单独开号 |
| **密钥集中管理** | 一把密钥发出去，随时能单独吊销；谁在用、用了多少，后台都看得见 |
| **多线路兜底** | 上游抖动自动切线路，重试放在中转层，客户端不用自己写容灾 |

## 三步接入

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
    messages=[{"role": "user", "content": "帮我逆向这个 apk，看它怎么联网的"}],
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
  -d '{"model":"gpt-4o","messages":[{"role":"user","content":"这个壳怎么脱"}],"stream":true}'
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

NextChat、Cherry Studio、Cursor、沉浸式翻译、各类 SDK —— 把地址换成 `https://ai.tt2066.top/v1`，直接跑起来。

## 桌面客户端

不想自己配，装 **TT助手 · Windows 桌面 AI 工作台**：[tt2066.top](https://tt2066.top/)

接口已内置，登录就能用，大白话直接问。

## 常见问题

**要改我的业务代码吗？**
不用。你的客户端能填 base_url，就改那一个地址，别的一个字不用动。

**多人一起用怎么算钱？**
一份额度，按实际调用量扣，用量明细后台能查。

**密钥要是漏了怎么办？**
后台单独吊销那一把，其他密钥照常用，不用全场换钥匙。

**满血版跟普通版差在哪？**
额度给足、线路不降级、响应不缩水。

---

<div align="center">

**[立即接入 → https://tt2066.top/](https://tt2066.top/)**

破甲中转站 · 满血版 · 大白话下指令

</div>
