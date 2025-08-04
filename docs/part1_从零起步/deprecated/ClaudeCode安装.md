### Claude Code是一个CLI (命令行界面) 工具, 它是我们的高效的代码生成助手

---

**传统浏览器上的AI问答不能帮助我们直接修改代码文件, 也不能直接阅读我们的整个代码库**
- 但Claude Code可以直接修改文件和阅读代码库, 只需要在代码库的root directory(根目录)用命令### Claude唤起Claude Code即可.

**且浏览器AI问答无法打断AI的生成进度并补充信息, 可能出现生成到一半就已经踏上了错误的方向**
- 而Claude Code会在做出修改前允许我们打断它, 并为它提供重要的指示和补充信息

### 安装Claude Code

---

**安装Node.js**
- https://nodejs.org/dist/v22.17.1/node-v22.17.1-x64.msi
- 在VS Code内呼出bash, 并运行以下三行命令来确认安装成功, 报错代表失败
```
which node
which npm
node -v       # → v22.x.x
```

**安装Claude Code**
- 运行sudo npm install -g @anthropic-ai/claude-code
- 此后, 在VScode连接到wsl后, Claude Code的logo会自动出现在右上角, 点击即可呼出Claude Code

**使用Claude Code**
- Claude Code可以像Chatgpt, Claude一样对话, 但是它修改代码的时候会有3个选项, 选项1是允许它的修改, 选项2是允许它的修改并之后不再询问, 选项3是拒绝当前修改, 并提供额外信息
- 用/init可以让Claude Code分析当前代码, 并创建一个叫CLAUDE.md的文档, 这个文档可以在为未来的Claude Code提供项目背景信息
- 用/to memorize可以让Claude Code更新CLAUDE.md
- 用\ + enter可以空行
