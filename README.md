<p align="center">
  <img src="./assets/banner.svg" alt="XXD Panel 030 项目横幅" width="1200">
</p>

<div align="center">

# 🦁 XXD Panel 030

### 用真实叶片、花瓣、枝条、果实、种子、草茎与树皮重构照片

[![Codex Skill](https://img.shields.io/badge/Codex-Skill-000000?style=flat-square)](./SKILL.md)
[![Four Modes](https://img.shields.io/badge/Modes-4-d75d32?style=flat-square)](#四种输出共享同一种自然材料拼合逻辑)
[![Raster Output](https://img.shields.io/badge/Output-PNG-3c6f67?style=flat-square)](#边界与信任)

<strong>简体中文</strong> · <a href="README.en.md">English</a> · <a href="README.ja.md">日本語</a> · <a href="README.ko.md">한국어</a> · <a href="README.ar.md">العربية</a>

</div>

> 真实自然材料 · 矩形色域 · 自然越界 · 极少黑线 · 编辑留白

XXD Panel 030 是一个面向 Codex 与兼容 Agent 的图像生成 Skill。它保留照片中真实的身份、比例、轮廓走势、姿态、方向、动作与关系，再用清晰可辨的真实叶片、花瓣、枝条、果实、种子、草茎、树皮或枯叶重构主体。

自然材料保留原本的形状、叶脉、纤维、透光、色差、卷曲、破损与不规则边缘。一块与当前源图协调的矩形色域建立秩序，但不画完整边框；主体大部分在内，只有真正具有方向感的一小段自然伸出。大量留白、不完全对称、极少黑线与轻量编辑文字，让自然材料的偶然性和版式纪律同时成立。

## 为什么需要 030

普通“树叶拼贴”很容易退化成儿童手工、现成花束、精准裁切的植物几何形，或把任意装饰误当成自然巧思。

030 的顺序完全相反：

```text
锁定身份／比例／走势／关系 → 选择能承担源图线索的真实自然形态 → 保留未经精准裁切的材质证据 → 建立一块无完整描边的源图协调矩形色域 → 主体大部分在内 → 只让真正有方向的一小段自然越界 → 平衡不完全对称与大量留白 → 只加入有功能的黑线和轻量编辑文字
```

如果换成一张无关照片，材料选择、主体轮廓、动作、矩形色域关系、自然越界、综合色彩和文字对齐仍然成立，这张图就不属于 030。

## 030 的视觉契约

- **源图身份：** 至少三个专属线索保住主体比例、轮廓走势、姿态、方向、动作、功能与关系。
- **真实自然形态：** 叶片、花瓣、枝条、果实、种子、草茎、树皮和枯叶必须看得出真实材质；它们原本的边缘与纹理直接建立主体，不是填进画好的轮廓。
- **一个矩形色域：** 色相、冷暖和明度与当前照片协调，以裁切或色差暗示边缘，不刻意画出完整四边。
- **源图决定越界：** 主体大部分在色域内部，只有原图动作或走势真正需要的一小段自然伸出。
- **黑线极少：** 细黑线只用于眼睛、表情、连接、动作暗示或短节奏，绝不为主体整体描边。
- **材料接触可信：** 真实叠压、尺度、卷曲和轻微接触影说明材料平放在承载面上，不变成贴纸或塑料假叶。
- **自然与编辑平衡：** 不完全对称、清晰重心、浅色背景和大量留白让画面鲜活但克制。
- **轻量文字：** 一个简短标题和必要的微型注释与色域边缘、留白或一根枝叶方向对齐。

## 样张 · 来自 X

> [小小东（@xiaoxiaodong01）](https://x.com/xiaoxiaodong01/status/2090464374188310979) · 2026-08-20<br>
> GPT2 x 植物 x 重构 x 美学提示词 x VOL.030

<table>
  <tr>
    <td width="50%"><a href="https://x.com/xiaoxiaodong01/status/2090464374188310979"><img src="./assets/examples/sample-01.jpg" alt="XXD Panel 030 样张 1"></a></td>
    <td width="50%"><a href="https://x.com/xiaoxiaodong01/status/2090464374188310979"><img src="./assets/examples/sample-02.jpg" alt="XXD Panel 030 样张 2"></a></td>
  </tr>
</table>

<p align="center"><a href="https://x.com/xiaoxiaodong01/status/2090464374188310979">查看原推文与完整提示词 →</a></p>

这些样张用于展示 030 的美学动机，不会把样张中的主体、构图、配色、文案或旧画幅变成生成参考或当前默认值。

## 四种可组合输出模式

可用 `1`、`1+3`、`1、2、4` 或 `全部` 选择一个或多个模式；`全部` 每张源图输出 7 个独立 PNG。模式确定后，Skill 会在生图前继续询问整张最终成品的画幅：`3:4` 原提示词画幅、明确跟随原图、常用比例，或自定义比例／准确像素。不会再静默套用源图尺寸。

| 模式 | 画幅逻辑 | 成品 |
| --- | --- | --- |
| `top-bottom` | 用户确认的整张成品画幅 | 一次生成完整画布：高保真原图在上，030 设计在下，约 50/50 |
| `left-right` | 用户确认的整张成品画幅 | 一次生成完整画布：高保真原图在左，030 设计在右，约 50/50 |
| `design-only` | 用户确认的整张成品画幅 | 030 设计铺满画布，不显示原照片 |
| `wallpaper-pack` | 逐设备确认 | 手机、iPad、电脑、儿童手表四张独立 PNG |

双联默认把原图作为高保真垫图／编辑参考，用一套完整提示词直接生成一张整体成品，让摄影、设计、色彩、光线、文字与含义自然呼应。只有完整画布针对性重试仍失败、用户要求原片逐像素不变、当前通道无法实现目标画幅，或需要无创像素校准时，才启用确定性拼合兜底。

壁纸可选连贯或独立。连贯套装先批准一张 iPad 定调图，另外三张分别参考原图＋同一定调图重新构图；独立套装的四张都只参考原图。两者都不会裁切其他设备成品或串联衍生图。

## 文字像轻量编辑注释一样进入画面

正式生图前，先选择自动文案、自定义文案或无文字。有文字时还要指定目标语言或地区。

自动文案从照片可见或有依据的身份、情绪、动作、关系或隐喻中提炼一个简短标题。它要与当前主体高度绑定，不用空泛诗句冒充高级。

默认只有一个简短标题；只有确有信息价值时才增加零至两个微型元素，不会编造植物种类、编号、年份、坐标或出处。文字使用目标文字系统中自然、轻量、精致的编辑排版，与色域边缘、留白或一根枝条、草茎、叶片方向对齐；文案仍需通过换图测试。

用户提供最终成稿时逐字保留。用户提供的是方向或可编辑草稿时，才会在保留受众、目的、必备词、语气和潜台词的前提下专业深化。

语言遵循目标受众，而不是用户下指令时使用的语言：

```text
目标市场或受众 > 指定成品语言 > 用户方向语言；都不明确时生图前询问
```

日本版使用自然日语，韩国受众使用自然韩语与正确空格，英国版使用英式英语，阿拉伯语版默认使用自然的现代标准阿拉伯语和真正的从右到左排版。排版会尊重各文字系统的比例、连接、方向与可读性。

## 完整画布优先与位图边界

图像模型负责整张成品的审美重构，双联也默认一次直出完整画布。`scripts/compose_panel.py` 只保留为条件明确的兜底、无创尺寸校准和只读审计工具，不再预先规划每次任务，也不评价审美是否成功。

全部交付为 PNG 位图。每次调用都在 `~/Desktop/xxd/` 下创建新任务；已配置图像通道只返回脱敏状态，不公开供应商、端点、凭据、请求头、提示词、响应或账户信息。SVG、HTML、Canvas、图表和程序绘图不能替代最终作品。

## 开始使用

```bash
git clone https://github.com/nevertoday/xxd-panel-030.git
mkdir -p ~/.codex/skills
ln -s "$(pwd)/xxd-panel-030" ~/.codex/skills/xxd-panel-030
```

Claude Code 用户可以把同一目录链接到 `~/.claude/skills/xxd-panel-030`。安装后重新启动 Agent 会话。

```text
$xxd-panel-030
把这张照片做成左右双联，文案由你根据照片内涵创作，使用自然韩语。
```

只上传照片也可以调用。Skill 会先用分行编号菜单询问一个或多个模式，再询问文字设置；选择壁纸时还会确认连贯或独立以及设备尺寸。

完整规范：

- [Skill 工作流](SKILL.md)
- [中文完整提示词](references/xxd-panel-030-prompt.zh-CN.md)
- [英文完整提示词](references/xxd-panel-030-prompt.en.md)
- [原始风格提示词](references/030-source.md)

## 边界与信任

- 每张照片只在自己的任务中使用，不借用其他输入、旧成品或样张里的主体、颜色、文案和构图。
- 每次调用都创建新的任务子文件夹；相同原图和参数也要重新生成，旧成品不能冒充当前任务。
- 最终交付为 PNG 位图，不是 SVG、HTML、Canvas 或程序绘图替代品。
- 已配置位图桥接只返回脱敏状态，不显示供应商、端点、请求头、凭据、提示词或服务器响应正文。
- 每个所选普通模式各返回一张；若选择 `wallpaper-pack`，再返回四张独立壁纸。选择 `全部` 时每张原图共返回 7 个 PNG，分处四个同级模式文件夹，绝不生成拼贴总览。

本地拼版需要 Python 3 和 Pillow。安全位图桥接使用 Python 3.11+ 的 `tomllib`。图像生成仍需要主机 Agent 的内置位图能力或已经配置好的兼容位图路径。

## 项目结构

```text
xxd-panel-030/
├── SKILL.md
├── README.md / README.en.md / README.ja.md / README.ko.md / README.ar.md
├── agents/openai.yaml
├── assets/
│   ├── banner.svg
│   └── examples/（未来本地样张占位）
├── scripts/
│   ├── compose_panel.py
│   └── configured_imagegen.py
└── references/
    ├── xxd-panel-030-prompt.zh-CN.md
    ├── xxd-panel-030-prompt.en.md
    └── 030-source.md
```

## 关于 XXD

XXD 是小小东的品牌名称缩写。项目由 [@xiaoxiaodong01](https://x.com/xiaoxiaodong01) 创建并维护。

## 服务与会员

### 深度咨询 · 299 元/小时

Skills 使用的一对一深度咨询按 299 元/小时收费。请通过下方微信二维码联系小小东预约。

### 小小东 Skills 用户交流群 · 入群 99 元

一次支付 99 元加入用户交流群，用于交流工作流、作品与互助；不包含按小时的一对一深度咨询。扫码后请备注“Skills 用户交流群”。

### 知识星球＋成员提示词库 · 699 元/年

[知识星球](https://wx.zsxq.com/group/15554814142882)与[小小东成员提示词库](https://vip.xiaoxiaodong.ai/)是同一份会员权益：**一次年费同时开通两边，无需重复付费。**

1. 在[知识星球](https://wx.zsxq.com/group/15554814142882)开通后，微信联系小小东领取成员提示词库兑换码。
2. 在[成员提示词库](https://vip.xiaoxiaodong.ai/)自助开通后，微信联系小小东邀请进入知识星球。

<p align="center">
  <a href="https://xiaoxiaodong.pages.dev/assets/wechat-qr.png"><img src="https://xiaoxiaodong.pages.dev/assets/wechat-qr.png" alt="小小东付费服务微信二维码" width="320"></a>
</p>

<div align="center">

**让自然提供形状，让版面提供巧思。**

</div>

---

<div align="center">
  <h2>☕ 为开源项目赞助算力</h2>
  <p>如果这个项目为你节省了时间，可以通过微信或支付宝赞助后续测试与生成算力。</p>
  <table>
    <tr>
      <td align="center" width="240">
        <a href="https://colors.xiaoxiaodong.ai/docs/images/wechat-reward-qr.png"><img src="https://colors.xiaoxiaodong.ai/docs/images/wechat-reward-qr.png" alt="小小东微信算力赞助二维码" width="180"></a><br>
        <strong>微信算力赞助</strong>
      </td>
      <td align="center" width="240">
        <a href="https://colors.xiaoxiaodong.ai/docs/images/alipay-reward-qr.png"><img src="https://colors.xiaoxiaodong.ai/docs/images/alipay-reward-qr.png" alt="小小东支付宝算力赞助二维码" width="180"></a><br>
        <strong>支付宝算力赞助</strong>
      </td>
    </tr>
  </table>
  <p><sub>赞助完全自愿，不会改变这个开源项目的使用权限。</sub></p>
</div>
