# Claude Code 配置目录

此目录存放 Claude Code 的项目级配置。

## 文件说明

- `settings.json` - 项目级设置
- `commands/` - 自定义斜杠命令
- `memory/` - 持久化记忆文件

## 配置说明

### settings.json

项目级 Claude Code 设置，包括：
- 项目名称
- 权限配置 (permissions)
- 钩子配置 (hooks)

### commands/

存放自定义斜杠命令，每个 `.md` 文件对应一个命令。

### memory/

存放持久化记忆，用于跨会话保存重要信息。