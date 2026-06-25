# 中文文档风格与排版规范

[![License: MIT](https://img.shields.io/badge/License-MIT-2ea44f.svg)](LICENSE)
[![Language](https://img.shields.io/badge/Language-简体中文-d73a49.svg)](README.md)
[![Documentation](https://img.shields.io/badge/Documentation-Style%20Guide-0969da.svg)](docs/style-guide.md)

## 摘要

本项目是一套面向简体中文文章、产品文案与技术文档的写作和排版规范，内容涵盖空格、标点、数字、单位、专有名词、中西文混排、标题、段落、列表、表格、链接、代码、图片、语言风格与审校流程。

项目以公开中文写作规范为基础，对不同来源中的规则进行归类、去重和交叉比较。对于存在分歧的规则，本项目不直接采用单一来源的结论，而是结合国家标准、技术文档实践和使用场景，区分强制规则、推荐规则与团队可选规则。

本项目重点参考以下三个项目与文章：

1. [sparanoid/chinese-copywriting-guidelines：中文文案排版指北](https://github.com/sparanoid/chinese-copywriting-guidelines)
2. [yikeke/zh-style-guide：中文技术文档写作风格指南](https://github.com/yikeke/zh-style-guide)
3. [Hindy Hong：写给大家看的中文排版指南](https://zhuanlan.zhihu.com/p/20506092)

本项目不是上述资料的合并转载，而是基于逐条阅读、规则比较和重新表述形成的综合性规范。各来源的具体贡献、差异和版权信息见 [NOTICE.md](NOTICE.md)。

## 编制目的

中文文档常见问题包括：

- 中英文和数字之间缺少必要空格；
- 中文语境中混用半角与全角标点；
- 数字、单位、日期和范围符号的格式不统一；
- 专有名词、产品名称和英文缩略语大小写错误；
- 标题层级、段落长度和列表结构缺乏一致性；
- 技术文档中的链接、代码、提示信息和操作步骤不规范；
- 团队将个人审美偏好误写为强制规则。

本项目旨在建立一套可解释、可执行、可审校的规范体系，以降低文档协作成本，提高中文文档的准确性、一致性、可读性和可维护性。

## 规范体系

本项目将规则分为三个层级：

- **强制规则**：涉及语言文字正确性、格式一致性或基本可读性，原则上必须遵守。
- **推荐规则**：适用于多数场景，但可依据媒介、受众和项目要求进行调整。
- **可选规则**：存在地域、机构或审美差异，团队应选择一种方案并保持一致。

当不同规则发生冲突时，建议按照以下优先级处理：

1. 法律法规、国家标准、行业标准和交付机构的明确要求；
2. 品牌、产品、协议和专有名词的官方写法；
3. 项目或机构已经发布的内部规范；
4. 本项目提出的通用规范；
5. 作者个人习惯。

## 内容结构

- [完整规范](docs/style-guide.md)：规则正文、适用条件、例外和示例
- [规范速查表](docs/quick-reference.md)：常用规则的简表
- [技术文档专项规范](docs/technical-writing.md)：README、API 文档、操作手册和故障排查
- [发布前审校清单](docs/editorial-checklist.md)：适用于编辑与评审流程的检查表
- [贡献指南](CONTRIBUTING.md)：规则新增、修订与争议处理要求
- [来源与版权说明](NOTICE.md)：参考资料、规则取舍和许可边界

## 配套 AI Skills

本项目的规则体系已经转化为可复用的 Codex Skill 与 Claude Code Skill，集中维护在 [hachiwar/codex-skills](https://github.com/hachiwar/codex-skills) 仓库中。

- Codex Skill：[`chinese-document-style`](https://github.com/hachiwar/codex-skills/tree/main/chinese-document-style)
- Claude Code Skill：[`claude-chinese-document-style`](https://github.com/hachiwar/codex-skills/tree/main/claude-chinese-document-style)
- 安装方法、适用场景与调用示例：[中文文档风格与排版技能介绍](https://github.com/hachiwar/codex-skills/blob/main/docs/chinese-document-style.md)

两个 Skill 将本项目的详细规范拆分为核心工作流与按需加载的参考资料，可用于审校学术报告、技术文档、README 和其他简体中文文档。Skill 的维护与版本更新在 `codex-skills` 仓库进行，本项目继续作为规范正文和规则依据。

## 核心规则示例

| 类别 | 规范写法 | 不规范写法 |
| --- | --- | --- |
| 中文与英文 | 使用 GitHub 登录 | 使用GitHub登录 |
| 中文与数字 | 共处理 12 个任务 | 共处理12个任务 |
| 数字与单位 | 10 GB、8 km | 10GB、8km |
| 百分比与角度 | 15%、90° | 15 %、90 ° |
| 中文标点 | 你好，世界！ | 你好, 世界! |
| 标点与空格 | 使用 Python，很简单。 | 使用 Python ，很简单。 |
| 专有名词 | GitHub、JavaScript、MySQL | Github、Javascript、mysql |
| 省略号 | 事情尚未结束…… | 事情尚未结束... |
| 破折号 | 基本原则——保持一致。 | 基本原则 - 保持一致。 |
| 数值范围 | 10～20 GB | 10-20GB |

上述规则存在例外。例如，URL、代码、命令、文件路径、产品型号、数学公式和品牌官方名称不应通过机械替换增加空格或修改字符。

## 适用范围

本规范适用于：

- 项目 README、博客、教程和知识库；
- 产品界面、帮助中心和一般产品文案；
- API 文档、开发者文档、操作手册和技术方案；
- 团队内部编辑规范与内容评审流程；
- 非特定格式约束下的一般中文说明文档。

学术论文、法律文书、新闻稿、出版物、政府公文和标准文件通常具有专门规范，应优先遵循相关机构和文种的要求。

## 编制原则

### 正确性

文档中的事实、数据、日期、名称、引用和链接应准确。排版规范不能替代事实核验，也不能以视觉统一为由修改代码、协议或官方名称。

### 一致性

同一文档或同一文档体系中的术语、人称、引号、括号、日期和编号形式应保持一致。对于不存在唯一结论的排版问题，一致性通常比个人偏好更重要。

### 可读性

排版规则应服务于信息理解。规则的使用不得破坏代码、URL、文件名、数学表达式或其他具有固定语法的内容。

### 可执行性

规则应明确说明适用范围、例外和示例。无法通过人工或工具稳定执行的规则，不宜规定为强制要求。

### 可追溯性

重要规则应尽量说明依据。存在来源冲突时，应记录取舍理由，而不是隐藏分歧。

## 规则差异的处理

三个主要来源在部分问题上存在不同主张。例如：

- 简体中文使用弯引号还是直角引号；
- 纯英文括注使用全角括号还是半角括号；
- 中文与链接之间是否增加空格；
- 数值范围使用一字线还是浪纹线。

本项目将此类问题列为可选规则或按使用场景分别规定，并在 [NOTICE.md](NOTICE.md) 中记录具体取舍。具有国家标准或机构规范约束的场景，应优先服从相应要求。

## 工具与人工审校

Markdownlint、Vale、AutoCorrect 和 pangu.js 等工具可以辅助发现空格、标点和格式问题，但不能可靠判断事实错误、逻辑关系、术语歧义和语气是否适当。

建议将自动检查与人工审校结合：

1. 使用工具检查可形式化的格式规则；
2. 由作者检查事实、结构和示例；
3. 由非作者检查可读性与歧义；
4. 对操作型文档进行可用性测试。

## 贡献

欢迎通过 Issue 或 Pull Request 提交以下内容：

- 新的规范依据或标准资料；
- 规则冲突与适用边界；
- 可验证的正误示例；
- 无障碍、国际化或特定文档类型的补充规范；
- 错别字、失效链接和表述问题。

新增规则应说明规则层级、适用范围、例外和参考依据。具体要求见 [CONTRIBUTING.md](CONTRIBUTING.md)。

## 致谢与参考来源

本项目明确参考并感谢以下三个项目与文章：

1. [sparanoid/chinese-copywriting-guidelines](https://github.com/sparanoid/chinese-copywriting-guidelines)：提供了中英文空格、全角标点、数字与单位、专有名词大小写等基础规则；
2. [yikeke/zh-style-guide](https://github.com/yikeke/zh-style-guide)：提供了技术文档语言风格、结构、标点、数字、列表、表格、链接、代码和命名等系统内容；
3. Hindy Hong 的《[写给大家看的中文排版指南](https://zhuanlan.zhihu.com/p/20506092)》：提供了引号、省略号、破折号、行首行尾禁则、西文排版和中西文混排等内容。

详细来源说明见 [NOTICE.md](NOTICE.md)。

## 许可证

本项目原创内容采用 [MIT License](LICENSE) 发布。第三方内容、商标、标准文本和引用材料仍受其原始许可与权利声明约束。
