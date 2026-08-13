# wit-combat-manager-archive — 项目技术文档

> 桌面战斗管理器的**归档 Python 快照**(历史版本,2026-06 起冻结);
> 活跃开发已迁移到 `wit-combat-manager`(PySide6)与 `wit-combat-manager-android`(Kotlin/Compose)。

## 1. 技术栈

| 类别 | 内容 |
|------|------|
| 语言/运行时 | Python(PySide6 桌面 GUI,历史快照) |
| 状态 | **归档**:不做新功能、不迁移架构/依赖;仅兼容性修复、安全修复与历史参考编辑 |

## 2. 架构概览

- 历史版本结构,与活跃项目不一致时以活跃项目为准;仅在明确要求回移植时与活跃 PySide6 项目对齐行为。

## 3. 目录结构

```
wit-combat-manager-archive/
├── main.py / models.py / combat.py / ui/ …   # 历史快照代码
├── AGENTS.md / CLAUDE.md                     # 本技术文档
└── (无活跃产物目录;发布物见活跃仓库)
```

## 4. 构建与测试

- 无持续集成;如需要,参考活跃仓库的 pytest 用法(本快照不保证全量通过)。

## 5. 运行与部署

- 不建议用于新环境;仅作为历史参考或紧急修复渠道。

## 6. 关键约束

- **归档纪律**:不做新功能;仅兼容性/安全修复与历史参考编辑;不迁移架构或依赖(除非用户要求刷新归档)。
- 与活跃项目行为对齐仅在明确要求回移植时进行。
- 探索优先 code-review-graph,回退 `rg`/读文件。

## 7. 开发约定

- 中文提交信息(fix/security/docs 前缀为主);改动前查 `git status`。
- 架构/结构变化时同步更新本文件与 `CLAUDE.md`。
