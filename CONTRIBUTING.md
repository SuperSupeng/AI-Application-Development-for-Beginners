# 贡献指南

感谢您对 AI-Application-Development-for-Beginners 项目的关注！我们欢迎所有形式的贡献，包括但不限于：

- 🐛 报告 Bug
- 💡 提出新功能建议
- 📝 改进文档
- 🔧 提交代码修复
- 🌟 分享使用经验

## 贡献流程

### 1. Fork 项目

1. 在 GitHub 上 Fork 本仓库
2. 克隆您的 Fork 到本地：
   ```bash
   git clone https://github.com/您的用户名/AI-Application-Development-for-Beginners.git
   cd AI-Application-Development-for-Beginners
   ```

### 2. 创建分支

为您的贡献创建一个新的分支：

```bash
git checkout -b feature/您的功能名称
# 或者
git checkout -b fix/您要修复的问题
```

### 3. 提交更改

1. 进行您的修改
2. 确保遵循本指南的格式规范
3. 提交您的更改：
   ```bash
   git add .
   git commit -m "feat: 添加新功能描述"
   ```

### 4. 推送并创建 Pull Request

```bash
git push origin feature/您的功能名称
```

然后在 GitHub 上创建 Pull Request。

## 格式规范

### Markdown 格式规范

#### 1. 标题层级

- 使用 `#` 表示一级标题（页面主标题）
- 使用 `##` 表示二级标题（主要章节）
- 使用 `###` 表示三级标题（子章节）
- 使用 `####` 表示四级标题（小节）
- 避免使用超过四级的标题

```markdown
# 主标题
## 主要章节
### 子章节
#### 小节
```

#### 2. 代码块

- 使用三个反引号包裹代码块
- 指定语言类型以获得语法高亮
- 代码块前后要有空行

```markdown
```javascript
function example() {
    console.log("Hello World");
}
```
```

#### 3. 行内代码

- 使用单个反引号包裹行内代码
- 用于标记文件名、函数名、变量名等

```markdown
请运行 `npm install` 命令安装依赖。
```

#### 4. 列表格式

- 无序列表使用 `-` 或 `*`
- 有序列表使用数字加点
- 列表项之间保持一致的缩进

```markdown
- 第一项
- 第二项
  - 子项 1
  - 子项 2

1. 第一步
2. 第二步
```

#### 5. 链接和图片

- 链接使用 `[描述](URL)` 格式
- 图片使用 `![alt文本](图片URL)` 格式

```markdown
[项目主页](https://github.com/SuperSupeng/AI-Application-Development-for-Beginners)
![项目横幅](assets/banner.png)
```

#### 6. 强调和引用

- 粗体使用 `**文本**`
- 斜体使用 `*文本*`
- 引用使用 `>`

```markdown
**重要提示**：请确保遵循规范。
*注意*：这是注意事项。
> 这是一段引用文字。
```

### 专有名词规范

#### 1. AI 相关术语

| 正确用法 | 错误用法 | 说明 |
|---------|---------|------|
| AI 辅助开发 | AI 辅助开发 | 保持空格 |
| vibe-coding | vibe coding, vibe_coding | 使用连字符 |
| Cursor | cursor, CURSOR | 首字母大写 |
| ChatGPT | chatgpt, Chat GPT | 保持官方命名 |
| Claude | claude | 首字母大写 |
| GitHub Copilot | GitHub copilot, github copilot | 保持官方命名 |
| 大语言模型 | 大语言模型(LLM) | 中文优先，英文缩写可加括号 |
| 提示工程 | Prompt Engineering | 中文优先 |
| 微调 | Fine-tuning | 中文优先 |

#### 2. 技术术语

| 正确用法 | 错误用法 | 说明 |
|---------|---------|------|
| 前端 | 前端端 | 避免重复 |
| 后端 | 后端端 | 避免重复 |
| API | api, Api | 全大写 |
| REST API | RESTapi, rest api | 保持官方命名 |
| JSON | json, Json | 全大写 |
| HTTP | http, Http | 全大写 |
| HTTPS | https, Https | 全大写 |
| URL | url, Url | 全大写 |
| 数据库 | 数据数据库 | 避免重复 |
| 服务器 | 服务服务器 | 避免重复 |

#### 3. 开发工具和框架

| 正确用法 | 错误用法 | 说明 |
|---------|---------|------|
| Node.js | nodejs, NodeJS | 保持官方命名 |
| React | react | 首字母大写 |
| Vue.js | vuejs, VueJS | 保持官方命名 |
| TypeScript | typescript, TS | 保持官方命名 |
| JavaScript | javascript, JS | 保持官方命名 |
| npm | NPM, Npm | 全小写 |
| yarn | Yarn, YARN | 全小写 |
| Git | git | 首字母大写 |
| GitHub | github, Github | 保持官方命名 |

#### 4. 项目相关术语

| 正确用法 | 错误用法 | 说明 |
|---------|---------|------|
| AI-Application-Development-for-Beginners | AI 应用开发教程 | 使用项目全名 |
| ChatPDF | Chat PDF, chatpdf | 保持项目命名 |
| 端到端 | 端到端端 | 避免重复 |
| 实战教程 | 实战教程教程 | 避免重复 |

### 文档结构规范

#### 1. 文件命名

- 使用小写字母和连字符
- 避免使用空格和特殊字符
- 文件名应具有描述性

```
✅ 正确：getting-started.md, api-reference.md
❌ 错误：Getting Started.md, API Reference.md
```

#### 2. 章节组织

- 每个文档应有清晰的层级结构
- 使用目录导航（适用于长文档）
- 保持逻辑顺序

```markdown
# 文档标题

## 目录
- [简介](#简介)
- [快速开始](#快速开始)
- [详细说明](#详细说明)

## 简介
...

## 快速开始
...

## 详细说明
...
```

### 提交信息规范

使用 [Conventional Commits](https://www.conventionalcommits.org/) 规范：

```bash
# 格式
<type>[optional scope]: <description>

# 示例
feat: 添加用户认证功能
fix: 修复登录页面样式问题
docs: 更新 README 文档
style: 格式化代码
refactor: 重构用户管理模块
test: 添加用户认证测试
chore: 更新依赖包
```

类型说明：
- `feat`: 新功能
- `fix`: 修复 Bug
- `docs`: 文档更新
- `style`: 代码格式调整
- `refactor`: 代码重构
- `test`: 测试相关
- `chore`: 构建过程或辅助工具的变动

### 代码规范

#### 1. 代码注释

- 使用中文注释
- 重要函数和复杂逻辑必须有注释
- 注释要简洁明了

```javascript
/**
 * 用户登录函数
 * @param {string} username - 用户名
 * @param {string} password - 密码
 * @returns {Promise<Object>} 登录结果
 */
async function login(username, password) {
    // 验证输入参数
    if (!username || !password) {
        throw new Error('用户名和密码不能为空');
    }
    
    // 调用登录 API
    const response = await fetch('/api/login', {
        method: 'POST',
        body: JSON.stringify({ username, password })
    });
    
    return response.json();
}
```

#### 2. 变量命名

- 使用有意义的变量名
- 遵循驼峰命名法
- 避免使用缩写（除非是通用缩写）

```javascript
// ✅ 正确
const userProfile = {};
const isAuthenticated = false;
const apiEndpoint = '/api/users';

// ❌ 错误
const up = {};
const auth = false;
const api = '/api/users';
```

### 审查标准

您的贡献需要满足以下标准：

1. **格式正确**：遵循 Markdown 格式规范
2. **术语统一**：使用规范的专有名词
3. **内容准确**：技术信息正确无误
4. **逻辑清晰**：文档结构合理，易于理解
5. **中文优先**：优先使用中文，必要时可添加英文对照

### 联系方式

如果您在贡献过程中遇到任何问题，可以通过以下方式联系我们：

- 在 GitHub 上创建 Issue
- 发送邮件至项目维护者
- 参与项目讨论

感谢您的贡献！🎉 