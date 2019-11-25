# Specification

本文件用于实验室代码文档规范化.

## 数据管理 Git

Git & GitHub 优秀的版本控制, 方便实现多人合作.

实现 SSH 认证, 链接请参考[link](https://help.github.com/cn/github/authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)

## Editor

- Visual Studio Code(VSCode) `优先推荐`, 支持对比算最全面, based on `electron`
- Sublime based on Python 速度比较快
- Atom, 相对于 vscode 相形见绌, based on `electron`
- Others

### VSCode plugins

如何安装插件请自行搜索, 善用`Ctrl+Shift+P`

以下是推荐插件, 语言方面不多推荐

- markdown

  1. Markdown Preview Enhanced
  2. Markdown PDF: convert markdown to PDF
  3. Markdown All in One

- git

  1. Git History

- Themes

  1. Material Icon Theme
  2. Material Theme

- Path Intellisense 找路径

- Linter 语法检查
  1. Prettier
  2. Markdownlint
  3. ESLint

### markdown 保存自动格式化

`Ctrl+Shift+P` 输入 setting 选择`open settings(JSON)`

```json
{
  // ...
  "[markdown]": {
    "editor.wordWrapColumn": 72,
    "editor.quickSuggestions": true,
    "editor.wrappingIndent": "none",
    "editor.defaultFormatter": "esbenp.prettier-vscode", //..需要安装 prettier formatter
    "editor.formatOnSave": true
  }

  // ...
}
```

## Coding IDE

推荐 JetBrians 系列, 现阶段的语言基本都支持, `学生free`, 支持也不错.

## Documents

`Markdown` 作为文档编写格式, GitHub 支持 markdown preview.

### Manual 参考目录

markdown [CheatSheet](CheatSheet)

[cheatsheet]: https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
