# WIT Combat Manager (Python Backup)

## 知识图谱（code-review-graph）

**本项目已配备代码知识图谱。探索代码时优先使用 MCP 工具。**

| 需求 | 使用 |
|------|------|
| 理解整体架构 | `get_architecture_overview` |
| 查找函数/类 | `semantic_search_nodes` |
| 追踪调用关系 | `query_graph` (callers_of / callees_of) |
| 代码审查 | `detect_changes` + `get_review_context` |
| 影响分析 | `get_impact_radius` + `get_affected_flows` |

图谱覆盖：10 文件 / 116 节点 / 948 边 / 22 执行流。仅在图谱未覆盖时才回退到 Grep/Glob/Read。

## 项目说明

WIT 战斗管理器的 Python 版快照，已不再新增功能。主动开发在 `trpg_manager/`（PySide6）和 `wit-combat-manager-android/`（Kotlin/Compose）。
