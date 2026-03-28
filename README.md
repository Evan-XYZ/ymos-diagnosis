# ymos-diagnosis

投资策略诊断工具。帮你搞清楚自己的投资系统到底健不健康。

**不推荐股票，不预测走势，只诊断你的投资"操作系统"。**

---

## 它能做什么

两种模式：

**问诊** — 你带着一个投资问题来（"该不该买 XX""我被套了怎么办"），它帮你判断这个问题本身成不成立。大部分投资问题会被消解掉——因为问题本身就是错的。

**体检** — 用 7 项检验把你的投资系统拆一遍，出一份诊断报告。

---

## 7 项检验

| # | 检验 | 核心问题 |
|---|------|---------|
| 1 | 策略存在性 | 你能用一段话写出你的投资策略吗？ |
| 2 | 可复现性 | 过去赚钱的交易，是逻辑还是运气？ |
| 3 | 风控存在性 | 你有止损规则吗？上次执行是什么时候？ |
| 4 | 仓位纪律 | 最大单只占比多少？定过上限吗？ |
| 5 | 情绪审计 | 最近一次冲动交易是什么时候？ |
| 6 | Beta 认知 | 你赚的是 Alpha 还是随大盘涨？ |
| 7 | 成长层级 | 你在投资成熟度的哪一层？ |

---

## 核心理念

6 条公理：

1. **策略必须可复述、可复制** — 说不出来的不叫策略，叫运气
2. **PVP 和 PVE 是完全不同的游戏** — 用错规则必输
3. **先板块 Beta，再个股 Alpha** — 顺序反了等于赌博
4. **情绪是最大的交易成本** — 系统的意义是切断情绪
5. **赔率 × 概率 = 真实期望值** — 只看赔率是赌徒思维
6. **99% 的投资亏损是心理问题** — 不是不知道，是在回避

---

## 安装

### Claude Code

```bash
# 方式一：直接复制 skill
git clone https://github.com/Evan-XYZ/ymos-diagnosis.git /tmp/ymos-diagnosis && cp -r /tmp/ymos-diagnosis/skills/ymos-diagnosis ~/.claude/skills/ && rm -rf /tmp/ymos-diagnosis
```

安装后在 Claude Code 中输入 `/ymos-diagnosis` 或 `/投资诊断` 即可。

### 不用 Claude Code

knowledge/ 目录下的文件是独立的方法论文档，可以直接阅读或粘贴到任何 AI 的 system prompt 中使用。

---

## 知识库

```
knowledge/
├── investment_axioms_and_framework.md   # 投资公理与诊断框架
└── diagnosis_case_library.md            # 按失败模式分类的案例库
```

Skill 运行时会参考这些文件，但不依赖它们——SKILL.md 是完全自包含的。

你也可以单独使用这些文件：
- 把 `investment_axioms_and_framework.md` 粘贴到你的 AI system prompt → 你的 AI 就有了投资纪律审计能力
- 读 `diagnosis_case_library.md` → 看看你有没有中招

---

## 和 YMOS 的关系

ymos-diagnosis 是一个**独立项目**，不需要安装 YMOS 就能使用。

它的定位是"入口层诊断"：帮你搞清楚你的投资系统健不健康。如果诊断完你想把策略系统化、自动化，可以看看 [YMOS](https://github.com/Evan-XYZ/YMOS) —— 一套开源的 AI 投资操作系统。

```
ymos-diagnosis（诊断）→ "你的策略到底是什么？健不健康？"
YMOS（系统化）→ "好，把这个策略变成可运行的系统"
```

---

## 许可证

本项目采用 [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/) 许可证。

- 个人使用、学习、研究：自由使用
- 公开发布衍生作品：请注明来源
- 商业用途：需要单独授权

---

## 关于作者

**勇麦（Yongmai）** — AI 时代投资系统架构师

- 🌐 博客：[yongmai.xyz](https://yongmai.xyz)
- 📧 邮箱：evan@yongmai.xyz
- 📱 公众号：勇麦
- 🎬 抖音：勇麦

## 参与贡献

欢迎通过以下方式参与：

- ⭐ Star 这个项目
- 🍴 Fork 并提交 PR
- 🐛 提交 Issue 反馈问题
- 🤝 分享给需要投资策略诊断的朋友
