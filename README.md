# terminal-veteran-data

终端老兵专家行业数据仓库（月度更新·去BCI化）

## 仓库说明

本仓库为「终端老兵专家（陈丰伟）」和「808zdlb终端老兵行业洞察助手」共享的行业数据源。

- 数据来源：华盛公司经营知识库月度市场监测报告（已去BCI化）
- 更新频率：月度（行业数据）/ 季度（理论金句）/ 按需（演讲框架）
- 同步机制：专家和808zdlb各内置data_sync.py，7天自动检查更新

## 目录结构

```
data/                         # 行业数据（月度更新）
├── market-facts.md           # 数据与事实库精选（65条）
├── monthly-series.md         # 48+月度数据序列
├── five-year-baseline.md     # 五年趋势基线
├── latest-update.md          # 最新月度数据快照
└── provincial-analysis.md    # 分省分析报告

theory/                       # 理论与金句（季度更新）
├── quotes.md                 # 陈丰伟金句弹药库（48条）
├── judgments-timeline.md     # 行业判断时间线（11条）
└── speech-frameworks.md      # MWC26+WAIC26演讲核心框架

manifest.json                 # 版本与hash管理
```

## 使用方式

### 终端老兵专家
专家Agent MD引用`~/.workbuddy/skills-data/terminal-veteran/`本地同步路径。

### 808zdlb skill
SKILL.md引用`~/.workbuddy/skills-data/808zdlb/`本地同步路径。

两个系统共享同一数据源，确保数据一致性。

## 数据安全

- 所有数据已去BCI化，无华盛内部运营数据
- 仅包含行业公开数据和陈丰伟公开演讲内容
- IMA知识库原始报告不在此仓库中
