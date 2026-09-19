# 免费大模型 API 指南

长期实测可用的免费 / 低价大模型 API 汇总，**全部兼容 OpenAI 接口格式**，可直连 Cherry Studio、LobeChat、NextChat、OneAPI、各类 Agent 工具。

> 更新：2026-09-19 ｜ 站点政策随时会变，福利没了不负责  
> 表格里的站名可直接点击跳转；部分链接含邀请码，可以的话支持一下弟弟

---

## 一、速查表

| 网站                                                          |  推荐指数 | 登录是否需要魔法 | 是否需要绑卡 |
| :---------------------------------------------------------- | :---: | :------: | :----: |
| [维云模型](https://vsllm.com/register?aff=Zn6v)                 | ★★★★☆ |     ✔    |    ✖   |
| [魔搭社区 ModelScope](https://modelscope.cn/)                   | ★★★★★ |     ✖    |    ✖   |
| [肖恩 AI](https://free.supxh.xin/register?code=3P8G4F)        | ★★★☆☆ |     ✖    |    ✖   |
| [幻城网安](https://api.hcnsec.cn/sign-up?aff=BUHW)              | ★★★★★ |     ✖    |    ✖   |
| [Agnes AI](https://platform.agnes-ai.cn/)                   | ★★★★★ |     ✖    |    ✖   |
| [商汤日日新 SenseNova](https://platform.sensenova.cn/)           | ★★★★☆ |     ✖    |    ✖   |
| [智谱 GLM 开放平台](https://open.bigmodel.cn/)                    | ★★★★★ |     ✖    |    ✖   |
| [OpenCode Zen](https://opencode.ai/zen)                     | ★★★★☆ |     ✖    |    ✖   |
| [蚂蚁百灵大模型](https://chat.ant-ling.com/open)                   | ★★★☆☆ |     ✖    |    ✔   |
| [硅基流动 SiliconFlow](https://cloud.siliconflow.cn/i/7PbesMGR) | ★★★☆☆ |     ✖    |    ✖   |

> ✔ = 需要 ｜ ✖ = 不需要（蚂蚁百灵需绑支付宝，但不扣款）

---

## 二、站点详解

### 1. 维云模型

- **网站**：<https://vsllm.com/register?aff=Zn6v>
- **Base URL**：`https://vsllm.cc/v1`
- **特点**：打开需科学上网，无需绑卡。站内有低价 GPT、Claude、DeepSeek 等主流模型。
- **福利模式**：
  1. **每日签到**可领一天额度（每 5 小时刷新一次，貌似该活动每月名额有限，建议当天要用时再签到）；
  2. **钱包额度**：通过每日抽卡获取。
- **推荐指数**：★★★★☆

### 2. 魔搭社区 ModelScope

- **网站**：<https://modelscope.cn/>
- **Base URL**：`https://api-inference.modelscope.cn/v1`
- **特点**：打开无需魔法、无需绑卡，全程没有任何付费入口。DeepSeek、Qwen 等国模齐全。
- **关键提醒**：务必先在**模型库**中筛选「支持体验 → 推理 API-Inference」，被选中的模型才能被调用。点进模型详情页可看到单次调用的大致额度消耗，整体响应快、比较耐用（生图类模型的 API 调用目前尚不稳定）。
- **福利模式**：每日登录领 250 积分（24 小时内有效）。
- **推荐指数**：★★★★★

### 3. 肖恩 AI

- **网站**：<https://free.supxh.xin/register?code=3P8G4F>
- **Base URL**：`https://speed1.toter.me/v1`（不通时换 `https://api.supxh.xin/v1`）
- **特点**：打开无需魔法、无需绑卡。免费档覆盖 Gemini、Claude、DeepSeek、Grok；付费套餐可选 GPT 等更先进的模型。
- **邀请码**：注册时填 `3P8G4F`，额外多得 2000 长期额度。
- **福利模式**：
  1. 注册初始赠送额度，偶尔会邮件补发额度；
  2. 每日签到领额度（仅限当天使用，记得用完）。
- **推荐指数**：★★★☆☆

### 4. 幻城网安

- **网站**：<https://api.hcnsec.cn/sign-up?aff=BUHW>
- **Base URL**：`https://api.hcnsec.cn/v1`
- **特点**：打开无需魔法、无需绑卡。以国内主流模型 Qwen、DeepSeek、Kimi 等为主，价格极低；目前 **Qwen3.8-Flash-Next 免费**。
- **彩蛋**：站主在魔搭开源了一个无限制的角色扮演模型 [SparkMuse-4B](https://modelscope.cn/models/hcnote/SparkMuse-4B)，能生成你弟弟喜欢的刘备文，有需要的可以自取。
- **福利模式**：每日领取额度（实测浮动较大，大概 1～500 之间）。
- **推荐指数**：★★★★★

### 5. Agnes AI

- **网站**：国内站 <https://platform.agnes-ai.cn/> ｜ 国际站 <https://platform.agnes-ai.com/>
- **Base URL**：`https://api.agnes-ai.cn/v1`
- **特点**：新加坡团队出品，**文本、图像、视频三模态全线免费**，无 Token 上限，邮箱注册即可，无需手机号。常用模型：`agnes-2.5-flash`、`agnes-3.0-flash`（文本，1M 上下文）、`agnes-image-2.1-flash`（文生图）、`agnes-video-v2.0`（文生视频）。国内站免魔法，直接访问。
- **福利模式**：2026 年 6 月起无限期免费开放，免费档约 20 RPM，日常写文档、跑 Agent 足够用。
- **小tip：**&#x7B80;单易申请企业账号，免费额度翻倍
- **注意**：视频模型稳定性一般；高峰期偶尔变慢。
- **推荐指数**：★★★★★

### 6. 商汤日日新 SenseNova

- **网站**：<https://platform.sensenova.cn/>
- **Base URL**：`https://token.sensenova.cn/v1`
- **特点**：手机号注册，无需绑卡、无需实名。主推 `sensenova-6.8-flash-lite`、`SenseNova U1.5 Fast`（专供信息图生成，其他生图容易“多手多脚”）。其他有ds、glm和kimi模型可调用（缺点是容易断）
- **福利模式**：**Token Plan 公测期完全免费**，5h和每周积分制，分通用积分池和商汤模型专属池。
- **注意**：模型名大小写敏感；公测结束后计费政策可能调整。
- **推荐指数**：★★★★☆

### 7. 智谱 GLM 开放平台

- **网站**：<https://open.bigmodel.cn/>
- **Base URL**：`https://open.bigmodel.cn/api/paas/v4/`
- **特点**：无需魔法、无需绑卡。
- **福利模式**：
  1. **GLM-4-Flash-250414 / GLM-Z1-Flash / GLM-4.7-Flash / GLM-4.6V-Flash**（可识图） **/ GLM-4.1V-Thinking-Flash**（可识图） **/ CogView-3-Flash**（生图） **/ CogVideoX-Flash**（生成视频）**永久免费**，不限 Token、限并发；（个人用下来4.7、4.6模型经常429限额，不过简单文本模型4就够用了）
  2. 新用户注册另送 2000 万 Token 额度。
- **推荐指数**：★★★★★

### 8. OpenCode Zen

- **网站**：<https://opencode.ai/zen>
- **Base URL**：`https://opencode.ai/zen/v1`
- **特点**：无需魔法，注册免费模型不产生费用。免费档包含MiMo-V2.5 Free、Nemotron 3 Ultra Free 等带 `-free` 后缀的模型和官方的Big Pickle模型。
- **福利模式**：免费模型不限额度，平台整体限速约 30 RPM / 500 RPD，模型列表见 <https://opencode.ai/zen/v1/models>。
- **推荐指数**：★★★★☆

### 9. 蚂蚁百灵大模型

- **网站**：<https://chat.ant-ling.com/open>
- **Base URL**：`https://api.ant-ling.com/v1`
- **特点**：**每天 50 万 Token 免费额度**，次日2点刷新。
- **注意**：这是本清单里**唯一需要绑定支付宝**的站点——注册后必须完成支付宝绑定才能创建 API Key，但不会扣款。
- **模型名**：可选 Ring-2.6-1T、Ling-2.6-1T、Ling-3.0-flash-VL 等。
- **推荐指数**：★★★☆☆

### 10. 硅基流动 SiliconFlow

- **网站**：<https://cloud.siliconflow.cn/i/7PbesMGR>
- **Base URL**：`https://api.siliconflow.cn/v1`
- **特点**：打开无需魔法、无需绑卡，国内节点、高并发、新模型上架最快。
- **邀请码**：注册时填 `7PbesMGR`，谢谢支持一下✿。
- **福利模式**：
  1. 一批 10B 以下的对话模型完全免费（输入输出价格均为 0，例如 `THUDM/GLM-Z1-9B-0414`）；
  2. 我本人更常用它的 **ASR 语音识别模型**：`FunAudioLLM/SenseVoiceSmall`、`XingChenAGI/XingChenASR-V3.2`，免费且效果好。
- **推荐指数**：★★★☆☆

### 11. 其他

英伟达（限流严重，经常调用不了）、书生（额度消耗太快）、Hermes（需绑卡）、groq（需魔法）、cf（链接麻烦）、hugging face（魔法）、讯飞lite（8k上下文，只能chat，tool用不了一点）等因为这样那样问题就不在我常用的模型范围，因此未列出。

---

## 三、通用接入提示

- 本清单所有站点均为 **OpenAI 兼容格式**，配置三项即可：`Base URL` + `API Key` + `模型名`。
- 想统一管理多家 Key，建议用 OneAPI / NewAPI 做中转，或直接在 Cherry Studio 里逐个填。
- 免费站点普遍有 **RPM（每分钟请求）与 RPD（每日请求）限制**，超限报 429，重试或换站即可。
- 上下文长度、模型名大小写、Base URL 结尾斜杠都可能踩坑，报错优先检查这三项。

## 四、免责声明

- 以上均为个人实测记录，站点政策、免费额度、可用模型随时可能变动，请以各站最新公告为准。
- 本文不构成任何推荐或背书，请勿在其中提交敏感数据。
- 邀请码为自愿填写，可自行删除链接后缀直接访问。
