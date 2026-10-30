# thuservices 维护说明

清华大学校园服务和工具索引，含 MkDocs 站点。

- 上游：https://github.com/thuservices/thuservices
- 在线文档：https://xiaoshecode.github.io/xiaoshecode/repos/thuservices/
- 检查日期：2026-10-30

## 环境与使用

- python -m pip install -r requirements.txt

使用/检查入口（需先满足依赖条件）：

- `python gen.readme.py  # 输出目录到终端`
- `python -m mkdocs serve`

## 目录职责

- docs/ — 分类服务文档
- source-docs/ — README 模板与辅助工具（原 aux/）
- gen.readme.py — 汇总 README
- mkdocs.yml — 站点配置

## 本次整理

- 新增维护文档和在线文档入口，补全用途、目录、使用路径及验证边界。
- 修复 Windows 无法检出的文件/目录名，并同步相关引用。
- 同步 pre-commit、README 模板和工具文档路径；生成器显式使用 UTF-8。

## 检查记录

- **仓库目录与入口盘点**（passed）：检查 Git 索引中的 38 个路径、README 和项目配置；不等于功能验收。
- **完整构建与端到端运行**（not_run）：辅助脚本涉及校园账号、网络或费用查询，本次不执行这些外部操作；未验证服务链接当前可用性。
- **README 生成器**（passed）：python -X utf8 gen.readme.py 运行成功，合并前后模板后同步根目录和 docs/README.md。

## 验证边界与待办

- 辅助脚本涉及校园账号、网络或费用查询，本次不执行这些外部操作；未验证服务链接当前可用性。

## 后续维护约定

保留上游许可证与作者信息。沿用现有模块边界和格式配置；修复功能时同步最小回归验证。依赖或接口变更需写明迁移步骤，避免仅为目录美观搬动公开入口。
