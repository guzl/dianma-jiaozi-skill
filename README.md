# 点妈手工饺子店 AI Skill

![Version](https://img.shields.io/badge/dynamic/json?url=https://raw.githubusercontent.com/guzl/dianma-jiaozi-skill/main/skill.json&query=$.version&label=version&color=blue) ![License](https://img.shields.io/badge/license-MIT-green) ![MCP](https://img.shields.io/badge/protocol-MCP-purple) ![Transport](https://img.shields.io/badge/transport-Streamable%20HTTP-orange)

这是一个 AI Skill——安装后，你的 AI 助手就能查询点妈手工饺子店的信息：在哪吃、几点开门、能不能外卖、是否有生饺子售卖、生饺子如何煮、Wi-Fi密码是什么。

店主大学学的是计算机科学专业，专业荒废多年，现在尝试做一个自己门店的AI服务，请大家多多支持。

## 关于点妈手工饺子店

电子科技大学旁边的饺子馆，2019年开始营业，本店宗旨：好吃不贵，量大实惠，做电科学子的碳水补给中心。不光有饺子，还有河南的胡辣汤、卤面，河北的炒饼丝，自研的鸡丝拌面。欢迎大家多多光顾。

| 项目 | 内容 |
|------|------|
| 餐厅名称 | 点妈手工饺子店 |
| 营业时间 | 9:00 - 21:00（以实际查询为准） |
| 门店地址 | 成都龙湖时代天街19栋 |

## 这个 Skill 能做什么

点妈手工饺子店的官方信息服务，包含多项 MCP 查询（完整工具列表以 `tools/list` 返回为准）：

| 能力 | 你可以问 | 来源 |
|------|----------|------|
| 餐厅信息 | "点妈手工饺子店在哪？""几点开门？" | MCP |
| 外卖服务 | "能送外卖吗？""怎么点外卖？" | MCP |
| 生饺子打包 | "能打包吗？""生饺子怎么煮？" | MCP |
| 店内WiFi | "WiFi密码多少？" | MCP |
| 最新消息 | "有什么新活动？" | MCP |


## 目录结构

```
dianma-dumpling-skill/
├── SKILL.md                 # 核心文件：元数据 + Agent 指令
├── skill.json               # 机器可读配置（MCP 端点、工具定义）
├── scripts/                 # 预留目录
├── README.md
└── LICENSE
```

## 安装

### 最简单的方式：告诉你的 AI 助手

直接拷贝下面这句话发给你的 AI 助手：

> 帮我安装点妈手工饺子店 Skill，仓库地址：https://github.com/guzl/dianma-jiaozi-skill

Agent 会自动克隆仓库并安装到对应的 Skill 目录。

### 其他安装方式

**手动克隆到 Skill 目录：**

将本仓库克隆到你项目下的 Skill 目录，不同 IDE 对应的路径：

| IDE | Skill 目录 |
|-----|-------------|
| Qoder | `.qoder/skills/dianma-jiaozi-skill/` |
| Cursor | `.cursor/skills/dianma-jiaozi-skill/` |
| Trae | `.trae/skills/dianma-jiaozi-skill/` |
| Windsurf | `.windsurf/skills/dianma-jiaozi-skill/` |
| Claude Code | `.claude/skills/dianma-jiaozi-skill/` |
| 通用 | `.agents/skills/dianma-jiaozi-skill/` |

```bash
# 示例：安装到 Qoder
git clone https://github.com/guzl/dianma-jiaozi-skill \
  .qoder/skills/dianma-jiaozi-skill
```

只要目录下有 `SKILL.md`，Agent 下次启动就会自动加载这个 Skill。

## 发布平台

- GitHub：https://github.com/guzl/dianma-jiaozi-skill

## 技术协议

| 项目 | 说明 |
|------|------|
| 协议 | MCP (Model Context Protocol) |
| 传输 | Streamable HTTP |
| MCP 端点 |  |
| 部署 | 阿里云服务器 |

## 版本

版本号见顶部徽章，以 [`skill.json`](./skill.json) 为准。

> 说明：本 Skill 参考借鉴北邮金谷园饺子馆的skill，如有侵权，请联系guzl86@qq.com。

## License

[MIT](LICENSE)
