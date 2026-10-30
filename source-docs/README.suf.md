
## 知道某个重要信息，但repo中未列出？

欢迎贡献！请 [PR](https://github.com/ZenithalHourlyRate/thuservices/pulls)！

需要注意的是[本 repo](https://github.com/ZenithalHourlyRate/thuservices) 中使用了 [pre-commit hook](https://github.com/ZenithalHourlyRate/thuservices/blob/master/pre-commit)，请[安装](https://git-scm.com/book/zh/v2/%E8%87%AA%E5%AE%9A%E4%B9%89-Git-Git-%E9%92%A9%E5%AD%90)，并在有 bash 与 python3 的环境中进行 commit。

在 pre-commit hook 的作用下，README.md 是自动生成的，故如果需要在 README.md 中修改，请在 [source-docs 文件夹](https://github.com/xiaoshecode/thuservices/tree/master/source-docs)下进行。

本 Fork 将上游的 aux/ 改为 source-docs/，避免 Windows 保留目录名导致克隆失败；Git Bash 中仍可使用原来的生成流程。

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
