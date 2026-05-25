# Career Experience Translator

> 🎯 根据 JD 匹配简历，挖出非垂直经历里的岗位价值。  
> 🔁 把校园项目、竞赛、社团、兼职和研究经历，转化成简历能写、面试能说的能力证据。

Career Experience Translator 是一组面向求职场景的 AI Skills，专门解决一个常见问题：

**我想投这个岗位，但我的经历好像没有那么对口。**

它会从目标 JD 出发，分析简历里的直接匹配和可迁移匹配，尤其帮助没有完全垂直工作/实习经历的用户，找到自己已有经历中可以支撑岗位要求的能力证据。

最终，它不是只告诉你“匹不匹配”，而是继续帮你把这些经历改成：

- 📝 简历上更贴近 JD 的表达
- 🎙️ 面试中更自然、有细节的口语回答
- 🗂️ 之后可以复用的 experience notes

它尤其适合这些情况：

- 🎓 想投某个岗位，但没有非常垂直的实习或工作经历
- 🧩 简历里多是校园项目、竞赛、社团、兼职、课设、研究或个人作品
- 🔍 不知道简历里哪些经历可以支撑目标 JD
- 📝 简历写得像流水账
- 🎙️ 面试时讲经历像背稿，缺少真实细节
- 🛡️ 想用 AI 准备求职，但不想被 AI 编造经历

这组 Skills 的核心不是“包装一个更厉害的人”，而是：

**把真实经历翻译成岗位能听懂、简历能呈现、面试能说出口的表达。**

## 🧭 这组 Skills 能做什么

它覆盖一条完整的求职表达流程：

```text
story-doctor
挖出普通经历里的故事素材

role-fit-check
判断简历和 JD 的直接匹配与可迁移匹配

resume-refiner
基于已有简历做贴岗润色

experience-translator
把一段经历转译成面试口语表达

mock-interview
围绕真实经历进行追问训练

experience-bank
保存、检索和复用经历笔记
```

## 🧰 Skills 列表

| Skill | 作用 |
| --- | --- |
| 🧠 `experience-translator` | 核心引擎：把一段真实经历翻译成岗位语言和面试口语表达 |
| 🔎 `role-fit-check` | 入口判断：分析简历和 JD 的直接匹配、可迁移匹配与缺口 |
| 📝 `resume-refiner` | 简历润色：基于已有简历和目标 JD 做修改建议与 bullet 优化 |
| 🩺 `story-doctor` | 经历挖掘：当用户觉得经历普通时，问出冲突、选择、变化和影响 |
| 🎙️ `mock-interview` | 模拟面试：围绕一段真实经历做追问训练 |
| 🗂️ `experience-bank` | 经历资产库：保存、列出、检索和复用 experience notes |

## 🚪 快速入口

| 你现在卡在 | 建议使用 |
| --- | --- |
| 有 JD，但不确定自己能不能投 | `$role-fit-check` |
| 有简历，想针对某个 JD 润色 | `$resume-refiner` |
| 有一段经历，但不知道面试时怎么讲 | `$experience-translator` |
| 觉得自己的经历太普通，没什么可说 | `$story-doctor` |
| 已经准备好回答，想练习面试追问 | `$mock-interview` |
| 想把整理过的经历保存下来，下次复用 | `$experience-bank` |

## 🧷 共同原则

- ✅ 不虚构经历、数据、岗位、工具或成果。
- 📏 允许使用有依据的近似事实，但必须保留不确定性。
- 🕊️ 如果用户只记得大概范围，可以写成“约”“大概”“needs confirmation”，不能改成精确数据。
- 🔦 优先挖掘真实细节、决策、约束、变化和取舍。
- 🚫 避免空泛表达，例如“具备良好沟通能力”“负责推进项目落地”。
- 🌱 重点不是把经历说大，而是把经历讲清楚。

## 📦 仓库结构

```text
career-experience-translator/
|-- README.md
|-- docs/
|   |-- suite-guide.md
|-- skills/
|   |-- experience-translator/
|   |-- role-fit-check/
|   |-- resume-refiner/
|   |-- story-doctor/
|   |-- mock-interview/
|   |-- experience-bank/
```

每个 skill 目录都包含：

```text
SKILL.md
README.md
agents/openai.yaml
```

## 💬 一句话总结

```text
把普通经历，翻译成岗位能理解的能力证据。
```
