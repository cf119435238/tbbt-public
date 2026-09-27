# tbbt-public

## 中文说明

用于分享项目和笔记的公开仓库，上传的内容可被他人查看。

### 仅保存在本地的目录

- `local-private/`：存放 Token、密码、私人笔记和本地连接配置。
- `third-party/`：存放本地下载的第三方库。

这两个目录及其内容均由 Git 忽略，不会通过正常提交上传到 GitHub。
重新克隆仓库后，请在本地创建这两个目录，并分别放置一个内容为 `*` 的 `.gitignore` 文件。
仓库根目录的 `.gitignore` 是随仓库共享的排除规则，应保留并提交。

### 依赖与配置

- 依赖清单和锁定文件应提交到 Git，以便恢复项目依赖。
- 第三方库的安装和调用方式需要根据各项目单独配置；创建目录不会自动完成配置。
- 只提交已去除敏感信息的示例配置，不要提交真实密码、Token 或连接凭据。

### 使用注意

忽略规则不会加密本地文件，也不会移除已跟踪的文件或清理历史提交。
不要强制添加本地私密文件，每次提交前请检查暂存内容。

---

## English

Public repository for projects and notes.

### Local-only directories

- local-private/: tokens, passwords, private notes, and local connection settings.
- third-party/: locally downloaded third-party libraries.

These directories and their contents are excluded from Git. After cloning, create
both directories locally and place a .gitignore containing a single * in each.
The root .gitignore remains the shared source of exclusion rules.

Keep dependency manifests and lockfiles in Git so dependencies can be restored.
Library loading and installation must be configured for each project separately.
Only commit sanitized example configuration files, never real secrets.

Ignore rules do not encrypt files, remove tracked files, or clean commit history.
Do not force-add local-only files. Review staged changes before every commit.
