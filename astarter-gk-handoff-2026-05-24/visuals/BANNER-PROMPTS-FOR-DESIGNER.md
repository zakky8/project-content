# 海报生成提示词 — 用于 GPT Image 2 / DALL-E 3 / Designer Brief

**参考基准：** Cointime 文章正在使用的 Astarter 主海报（左侧文案，右侧 3D 等距立方体 + 浮动 HUD 信息卡 + Cointime 标识，深紫色背景 + 青色光效，1180×480px）。

**两张新海报需要保持与该参考海报相同的视觉语言、构图、字体、配色、立方体风格、HUD 信息卡布局、底部 Cointime 标识位置——只更换文案内容。**

---

## 📁 文件夹中我用 Pillow 生成的 banner-investors-1180x480.png 和 banner-roadmap-1180x480.png

⚠️ **这两张是占位 / 规格预览（spec mockup），不是最终成稿。**

它们传达了构图意图（左文案 + 右几何元素 + 1180×480 + Quiet Substrate 配色），但程序化绘制无法达到参考海报的 3D 渲染质量。

**最终成稿请按下方任一方案产出。**

---

## 方案 A — GPT Image 2 / DALL-E 3 提示词（最快路径）

### Banner 1：投资者阵容（OKX Ventures × EMURGO 共同领投）

```
A premium horizontal Chinese Web3 promotional banner, dimensions 1180×480 pixels,
3D isometric illustration style, EXACT STYLE MATCH to Astarter's existing brand
poster series.

LEFT SIDE (40% of canvas):
  Headline 1 (large, bold, white, Source Han Sans / 思源黑体 Heavy):
    "ASTARTER 战略融资"
  Headline 2 (large, cyan-blue gradient, slightly smaller):
    "OKX Ventures × EMURGO 共同领投"
  Sub-text (medium, white, spaced letters):
    "W e b 4 . 0   A I   A g e n t   基 础 设 施"
  Tagline (small, light gray):
    "构建覆盖风险投资、交易所生态与战略合作伙伴的多层资本结构"
  CTA pill (rounded outline, white text):
    "MH Ventures · Adaverse 跟投"
  Top-left corner: clean space for real Astarter logo (will be composited in Figma)

RIGHT SIDE (60% of canvas):
  Hero element: isometric cubic AI core box, glowing purple/violet faces,
  central face showing "AI" text in cyan-blue with subtle glow,
  another face showing the Astarter "CO" infinity logo (placeholder — will be
  replaced in Figma post-process).
  4-6 small "CO" branded coin tokens floating around the cube with motion blur.
  Underneath cube: glowing hexagonal podium/platform with cyan light rays.
  Far right edge: 4 floating glassmorphism HUD info cards stacked vertically:
    1. Icon (briefcase) + "OKX Ventures · 战略领投"
    2. Icon (network) + "EMURGO · 持续支持"
    3. Icon (handshake) + "MH Ventures · 机构跟投"
    4. Icon (globe) + "Adaverse · 生态伙伴"
  Bottom-right corner: small "FEATURED ON Cointime" badge

BACKGROUND:
  Deep violet gradient (#0F0820 to #6F00FF), hexagonal grid pattern overlay
  with focal alpha falloff toward the cube. Subtle cyan particle field.
  Subtle vignette.

STYLE REFERENCES:
  Cinema 4D / Octane render aesthetic. Premium / editorial / tech-forward.
  Pentagram + Stripe gradient hero banner energy.

DO NOT:
  - Generate a fake Astarter logo (leave clean space top-left)
  - Use round podium template (use hexagonal)
  - Stack emojis
  - Use Cardano / Crypto cliché imagery (no coins flying, no rockets)
  - Use Y2K aesthetics
```

### Banner 2：6-12 个月路线图（ABox 节点 + AI 应用市场）

```
A premium horizontal Chinese Web3 promotional banner, dimensions 1180×480 pixels,
3D isometric illustration style, EXACT STYLE MATCH to Astarter's existing brand
poster series.

LEFT SIDE (40% of canvas):
  Headline 1 (large, bold, white, Source Han Sans / 思源黑体 Heavy):
    "未来 6-12 个月"
  Headline 2 (large, cyan-blue gradient, slightly smaller):
    "ABox 节点全球部署 + AI 应用市场"
  Sub-text (medium, white, spaced letters):
    "W e b 4 . 0   自 主 智 能 代 理 基 础 设 施"
  Tagline (small, light gray):
    "为 Web4 自主智能代理生态提供更坚实的底层支撑"
  CTA pill (rounded outline, white text):
    "ASTARTER · 全球生态版图"
  Top-left corner: clean space for real Astarter logo

RIGHT SIDE (60% of canvas):
  Hero element: same isometric cubic AI core box, this time surrounded by
  a network of glowing dotted lines radiating outward to small "node" spheres
  positioned in 4-5 directions (representing global node deployment).
  Each node sphere is small, glowing cyan with subtle motion blur.
  Underneath cube: glowing hexagonal podium with cyan light rays.
  Far right edge: 4 floating glassmorphism HUD info cards stacked vertically:
    1. Icon (globe network) + "ABox 节点 · 全球部署加速"
    2. Icon (app store) + "AI 应用市场 · 即将推出"
    3. Icon (gear) + "AI Agents · 基础设施能力强化"
    4. Icon (chain link) + "DeFAI · 真实落地中"
  Bottom-right corner: small "FEATURED ON Cointime" badge

BACKGROUND:
  Same deep violet gradient + hex grid + cyan particles + vignette as Banner 1.

STYLE REFERENCES:
  Cinema 4D / Octane render aesthetic. Same visual family as the existing
  Astarter Cointime banner.

DO NOT:
  Same restrictions as Banner 1.
```

---

## 方案 B — Figma 模板（最实用，5 分钟可完成）

**前提：** 你（GK / 设计同事）有 Cointime 上线的那张 Astarter 主海报源文件（Figma / PSD / AI）。

**步骤：**

1. **打开源海报文件** — 现在挂在 Cointime 文章上的那张
2. **复制为新文件** × 2
3. **Banner 1（投资者）**：
   - 左侧文案改成：
     - 主标题：「ASTARTER 战略融资」
     - 副标题：「OKX Ventures × EMURGO 共同领投」
     - 第三行：「Web4.0 AI Agent 基础设施」
     - 底部 tagline：「构建覆盖风险投资、交易所生态与战略合作伙伴的多层资本结构」
     - CTA pill：「MH Ventures · Adaverse 跟投」
   - 右侧 4 个 HUD 卡片替换为：
     - OKX Ventures · 战略领投
     - EMURGO · 持续支持
     - MH Ventures · 机构跟投
     - Adaverse · 生态伙伴
   - 其他（立方体、podium、Cointime 标识、配色）**全部保留不变**
4. **Banner 2（路线图）**：
   - 左侧文案改成：
     - 主标题：「未来 6-12 个月」
     - 副标题：「ABox 节点全球部署 + AI 应用市场」
     - 第三行：「Web4.0 自主智能代理基础设施」
     - 底部 tagline：「为 Web4 自主智能代理生态提供更坚实的底层支撑」
     - CTA pill：「ASTARTER · 全球生态版图」
   - 右侧 4 个 HUD 卡片替换为：
     - ABox 节点 · 全球部署加速
     - AI 应用市场 · 即将推出
     - AI Agents · 基础设施能力强化
     - DeFAI · 真实落地中
   - 其他全部保留不变
5. **导出 1180×480 PNG** × 2

**预计时间：** Banner 1 = 5 分钟 · Banner 2 = 5 分钟 · 共 10 分钟

---

## 方案 C — 委托真实设计师（如果时间允许）

- 把参考海报 + 上面方案 A 的提示词 + 方案 B 的文案变化清单全部发给设计师
- 设计师按相同视觉语言重新渲染 2 张
- 预计时间：1-2 个工作日
- 预计成本：可接受范围（如果有内部设计师）

---

## ⚠️ 关于我（Zakky / AI）的 Pillow 生成版本

`banner-investors-1180x480.png` 和 `banner-roadmap-1180x480.png` 是 Pillow 程序化绘制的。

**优点：**
- 配色、构图比例、字体层级与参考保持一致
- 可以作为媒体临时占位（紧急情况下）
- 给设计师 / GPT Image 2 一个明确的"构图意图"参考

**缺点：**
- 没有真实 3D 渲染
- 没有立方体的 AI 字面 + CO logo 面
- 没有 4 个 HUD 信息卡
- 没有浮动 CO 代币
- 没有 podium 光效
- 没有 Cointime 角标

**结论：** 媒体投放请用方案 A / B / C 之一产出的最终成稿，不要直接用 Pillow 版本。

---

## 📐 技术规格清单（任何方案都要遵守）

| 项目 | 规格 |
|---|---|
| 尺寸 | 1180 × 480 px |
| 格式 | PNG（透明背景可选）/ JPG（小文件） |
| DPI | 72 |
| 文件大小目标 | <500 KB |
| 颜色模式 | RGB（不是 CMYK） |
| 主色 | `#0F0820` 深紫 · `#6F00FF` 紫 · `#00E5FF` 青 · `#FFFFFF` 白 |
| 字体 | 思源黑体 Heavy（CN）· Druk Wide Bold（EN headline）· GT America Mono（spec） |
| Logo | 真实 Astarter logo（top-left）+ "FEATURED ON Cointime" 角标（bottom-right） |
| 比例参考 | 与现有 Cointime 主海报完全一致 |
