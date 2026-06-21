# Agentify B2B Market Research

[English](./README.md) | [简体中文](./README.zh-CN.md)

把一个 `1688` 或 `Alibaba` 店铺页，转成一份可直接执行的 B2B 出海市场研究简报。

这个 skill 主要面向 OEM/ODM 型供应商，目标不是做泛泛行业分析，而是帮助团队快速回答四个问题：真正的海外竞品是谁、先卖给谁、怎么外呼、怎么做内容和独立站积累搜索与 GEO 资产。默认判断框架参考 ZekSmart 这类供应商，但方法本身可复用到其他 B2B 出海工厂。

## 固定输出

输出固定为四个部分：

1. Top 5 竞品分析
2. ICP（理想客户画像）
3. Outbound Marketing Plan
4. Inbound Marketing Plan

其中 Inbound 会同时覆盖社媒内容方向，以及独立站 SEO / GEO。

## 支持输入

- `1688.com` 店铺 URL
- `Alibaba.com` 供应商或公司主页 URL
- 供应商名称 + 任一店铺 URL

如果同时有 1688 和 Alibaba，应该两边一起用；如果只有一边，也能继续，但需要明确标注证据缺口。

## 适用场景

- 中国 OEM/ODM 工厂的出海市场研究
- 供应商在海外开打前的竞品盘点
- B2B 项目型、渠道型、批发型销售的 ICP 定义
- 给销售团队产出首版 outbound 触达打法
- 给营销团队产出 LinkedIn、SEO、GEO、案例页、信任页的内容方向

## 研究原则

- 把店铺页当作事实锚点，而不是全部真相
- 明确区分 `evidence` 和 `inference`
- 只使用公开来源
- 不编造邮箱、联系人、认证、经销关系或社媒数据
- 优先找真正重叠的竞品，而不是泛行业邻居
- 输出必须服务销售和内容执行，而不是停留在空泛分析

## 仓库结构

```text
.
├── SKILL.md
├── README.md
├── README.zh-CN.md
├── agents/
│   └── openai.yaml
└── references/
    ├── data-sources.md
    └── report-template.md
```

## 文件说明

- `SKILL.md`：主工作流、判断逻辑、输出规则和质量标准
- `references/data-sources.md`：建议的数据源和证据规则
- `references/report-template.md`：最终报告模板
- `agents/openai.yaml`：给 OpenClaw 风格调度器使用的可选元数据

## 典型输出结构

- Supplier Snapshot
- Top 5 Competitors
- Tier 1 / Tier 2 / Tier 3 ICP
- Outbound Plan：渠道、话术角度、CTA、缺失证明材料
- Inbound Plan：社媒差距、内容支柱、关键词簇、GEO 资产、30 天内容计划

## 最适合的供应商类型

这个 skill 特别适合以下类型：

- 有出海意图的成品品牌
- OEM / ODM 硬件工厂
- 项目交付型方案商
- 面向渠道商的 B2B 解决方案供应商

如果只是纯内销、纯大宗、且没有明显差异化或出海线索的卖家，效果会弱一些。

## 安装方式

把这个目录克隆或复制到你的 OpenClaw skills 目录中，再由本地 skill loader 读取 `SKILL.md` 即可。

## 说明

这个仓库聚焦的是“可复用 skill”，不是某一家公司的固定报告。ZekSmart 是最初案例，但方法本身没有写死在单一品牌上。
