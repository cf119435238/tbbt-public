# tbbt-public

Public repository for projects and notes.

## Local-only directories

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
