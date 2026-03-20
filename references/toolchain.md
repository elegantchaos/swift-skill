# Toolchain And Platform Expectations

Use this file when deciding which Swift language and platform conventions should apply.

- Follow the project's current Swift and platform targets.
- For new Swift projects, prefer modern Swift 6 patterns when they are compatible with project constraints.
- For mixed or legacy codebases, implement changes in a migration-friendly style.
- Do not assume all targets in a multi-target workspace use identical build settings; verify toolchain and deployment expectations before applying broad migrations.
