
## 知道某个重要信息，但repo中未列出？

欢迎贡献！请 [PR](https://github.com/ZenithalHourlyRate/thuservices/pulls)！

本 Fork 使用自己的 [pre-commit hook](https://github.com/xiaoshecode/thuservices/blob/master/pre-commit)，需要 Bash 与 Python 3。请安装本仓库的版本；上游 hook 的模板路径与本 Fork 不同。

在 pre-commit hook 的作用下，README.md 是自动生成的，故如果需要在 README.md 中修改，请在 [source-docs 文件夹](https://github.com/xiaoshecode/thuservices/tree/master/source-docs)下进行。

本 Fork 将上游的 aux/ 改为 source-docs/，避免 Windows 保留目录名导致克隆失败。已经复制到 `.git/hooks/pre-commit` 的旧 hook 不会随代码更新，升级后必须重新安装，否则它仍会读取已移除的 `aux/`，可能清空或生成不完整的 README。

在仓库根目录的 Bash / Git Bash 中安装或升级 hook。若现有 hook 包含其他检查，请先保留并合并那些逻辑，再执行安装：

```sh
cp pre-commit "$(git rev-parse --git-path hooks/pre-commit)"
chmod +x "$(git rev-parse --git-path hooks/pre-commit)"
```

### 编译

```
python3 -m pip install --user -r requirements.txt # 安装 Python 依赖包
mkdocs serve # 直接在本地 serve，或者：
mkdocs build --clean # 生成于 site/ 文件夹中
```

## LICENSE

本站的文本遵循 CC BY-NC 4.0

本项目内的存放的代码遵循代码文件内自带的 LICENSE。若代码文件中未附带 LICENSE，则认为该文件暂无 LICENSE，有需求者可以联系相应 committer。

## 维护与在线文档

本仓库 Fork 自 [https://github.com/thuservices/thuservices](https://github.com/thuservices/thuservices)，保留上游来源与许可证。

- [在线维护文档](https://xiaoshecode.github.io/xiaoshecode/repos/thuservices/)
- [仓库维护说明](https://github.com/xiaoshecode/thuservices/blob/master/MAINTENANCE.md)：用途、目录、检查结果与未验证范围。
