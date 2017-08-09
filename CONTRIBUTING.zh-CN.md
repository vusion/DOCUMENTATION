# 贡献指南
针对这个组织所有仓库的贡献指南。

Hi! 首先感谢你使用Vusion。

## Issue规范

- Issue仅用于提交Bug或Feature以及设计相关的内容，其它内容可能会被直接关闭。如果你在使用时产生了疑问，请到Slack或Gitter里咨询
- 在提交Issue之前，请搜索相关内容是否已被提出
- 请说明Vusion和Vue的版本号，并提供操作系统和浏览器信息。推荐使用JSFiddle生成在线demo，这能够更直观地重现问题

## Pull Request规范

- 请先fork一份到自己的项目下，不要直接在仓库下建分支
- 提交PR前请rebase，确保commit记录的整洁
- 确保PR是提交到dev分支，而不是master分支
- 如果是修复bug，请在PR中给出描述信息
- 合并代码需要两名维护人员参与：一人进行review后approve，另一人再次 review，通过后即可合并

## 提交信息规范

- 首字母必须大写（如"Fix a bug"，而不是"some bug"）
- 使用祈使句（如"Move cursor to..."，而不是"Moves cursor to..."）
- 使用一般现在时（如"Add feature"，而不是"Added feature"）
- 结束不需要用句号(.)
- 尽量限制在72个字符以内
- 尽量使用`#`关联Issue和Pull Request
- 使用`gitmoji`，选择一个适合的表情开头：
    - ✨ `:sparkles:` 当引入了新特性
    - 🐛 `:bug:` 当修复了一个bug
    - ⚡️ `:zap:` 当提高了性能
    - 🎨 `:art:` 当优化了代码结构或格式
    - 🔨 `:hammer:` 当重构了代码
    - 🚚 `:truck:` 当移动或重命名了文件
    - 🔥 `:fire:` 当删除了代码或文件
    - 📝 `:memo:` 当书写了文档
    - ✏️ `:pencil2` 当修复了错别字
    - 💄 `:lipstick:` 当更新了样式
    - ✅ `:white_check_mark:` 当添加了测试脚本
    - 🚧 `:construction:` 当仍在开发中
    - ⬆️ `:arrow_up:` 当更新了依赖包
    - 🔖 `:bookmark:` 当发布版本或打了标签
    - ... [更多](https://gitmoji.carloscuesta.me/)

### JavaScript代码规范

请在编辑器中配置ESLint。更多细节参见[eslint-config-vusion](https://github.com/vusion/eslint-config)。

### CSS代码规范

使用[REA规范](REA.md)。
