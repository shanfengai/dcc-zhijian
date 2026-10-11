# DCC Zhijian

汽车 DCC 线索首触外呼质检 Skill。

把汽车外呼文字稿按 6 个关键维度自动打分，生成同店座席对照 HTML 报告，快速看清谁会邀约、谁缺挖需、哪句话该改。

## 预览

1. 全店总览与评分水位

![全店总览](assets/screenshots/01-overview.png)

2. 座席对照与关键原话证据

![座席对照](assets/screenshots/02-agent-compare.png)

3. 根因分析与改进建议

![根因分析](assets/screenshots/03-root-cause.png)

在线展示页：[DCC Zhijian](https://shanfengai.github.io/dcc-zhijian/)

报告示例页：[DCC 质检对照报告](https://shanfengai.github.io/dcc-zhijian/examples/DCC%E8%B4%A8%E6%A3%80%E5%AF%B9%E7%85%A7%E9%95%BF%E5%9B%BE.html)

## 核心卖点

### 6 维度打分，不靠感觉

自我介绍、封闭邀约、异议处理、信心建立、需求挖掘、邀约成功，逐项拆开看。

### 批量对照，一屏看差距

多通电话、多位座席统一评分，直接生成适合复盘的长图报告。

### 阶段可配置，品牌不写死

盲订期、开业期、正式期都能用；品牌名、卖点词、权益词按项目传入。

### 不只给分，还给改法

报告会指出失分维度、原话证据和可直接抄进话术包的优化句。

## 安装

直接告诉你的 agent：

> 从 `github.com/shanfengai/dcc-zhijian` 安装 `dcc-zhijian` 这个 skill。

或者手动安装：

```bash
git clone https://github.com/shanfengai/dcc-zhijian ~/.codex/skills/dcc-zhijian
```

如果你的 agent 使用其他 skills 目录，把仓库 clone 到对应目录即可。

## 怎么用

```text
DCC 质检一下这段录音文字稿，品牌=XX汽车，阶段=盲订期。
```

```text
把这 5 段录音跑一遍 DCC 质检，都是同一家店的，品牌=XX汽车。
```

```text
3 号工号这通为什么只有 42 分？指出最低维度、原话证据和一句可改的话术。
```

## 评分框架

| 维度 | 权重 |
|---|---:|
| 自我介绍 | 15% |
| 封闭邀约 | 15% |
| 异议处理 | 15% |
| 信心建立 | 15% |
| 需求挖掘 | 20% |
| 邀约成功 | 20% |

报告还会独立提示过度承诺词、品牌认知盲区、红线触发、通话字数、客服有效发言字数等合规观察项。

## 文件说明

- `SKILL.md`：agent 入口与完整评分规则。
- `agents/openai.yaml`：agent 元信息。
- `assets/report-template.html`：锁定版式的报告模板基线。
- `examples/DCC质检对照长图.html`：示例质检报告。
- `dist/dcc-zhijian.zip`：打包后的 skill。

## 许可

[MIT](LICENSE)
