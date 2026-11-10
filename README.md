# weekly-report-skill ⛱️

一个 [CodeBuddy Code](https://www.codebuddy.cn) 技能插件：**一键生成结构化工作周报**。

它会让 AI 助手在你说「写周报 / 生成周报 / 本周总结」时，自动收集你的工作素材（口述内容、笔记文件、git 提交记录），按标准模板整理成一份重点突出的周报。

## ✨ 功能

- **自动收集素材**：支持从对话、工作笔记、git 提交记录三种来源收集本周工作
- **四象限归纳**：本周完成 / 进行中 / 问题与风险 / 下周计划
- **标准模板输出**：统一格式，条目精炼（每条「动作 + 结果/数据」）
- **不编造内容**：素材缺失的信息以 `[待补充]` 占位，绝不瞎编

## 📦 安装

### 方式一：手动复制（推荐新手）

1. 下载本仓库（Code → Download ZIP，或 `git clone`）
2. 把 `skills/weekly-report` 整个文件夹复制到：
   ```
   ~/.codebuddy/skills/weekly-report
   ```
3. 重启 CodeBuddy Code，然后输入 `/weekly-report` 或直接说「帮我写周报」即可使用

### 方式二：git clone

```bash
git clone https://github.com/<你的用户名>/weekly-report-skill.git
cp -r weekly-report-skill/skills/weekly-report ~/.codebuddy/skills/
```

## 🚀 使用示例

> 你：帮我把这周的工作写成周报，我周一修了登录 bug，周三上线了新搜索功能，还在做数据看板。

AI 助手会输出：

```markdown
# 周报（2026-11-02 ~ 2026-11-06）

## 本周完成
1. 修复登录模块 bug，恢复正常登录流程
2. 新搜索功能上线

## 进行中
1. 数据看板开发中 [待补充：当前进度]

## 下周计划
[待补充]
```

## 📁 目录结构

```
weekly-report-skill/
├── README.md                                # 本文件
├── LICENSE                                  # MIT 开源协议
└── skills/
    └── weekly-report/                       # 技能本体
        ├── SKILL.md                         # 技能定义（核心）
        └── assets/
            └── weekly-report-template.md    # 周报模板
```

## 🛠️ 自定义

- 想改周报格式？编辑 `skills/weekly-report/assets/weekly-report-template.md`
- 想改生成规则？编辑 `skills/weekly-report/SKILL.md` 中的「第 3 步」

## 📄 License

[MIT](./LICENSE)
