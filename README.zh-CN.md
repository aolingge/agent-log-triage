<p align="center">
  <img src="assets/readme-banner.svg" alt="Agent Log Triage banner" width="100%">
</p>

<h1 align="center">Agent Log Triage</h1>

<p align="center">检查 AI Agent 失败日志是否包含错误、命令、文件、环境和下一步信号。</p>

<p align="center"><a href="README.md">English</a> · <a href="#快速开始">快速开始</a> · <a href="#检查项">检查项</a></p>

<p align="center">
  <img alt="Node.js" src="https://img.shields.io/badge/node-%3E%3D18-2563EB">
  <img alt="dependencies" src="https://img.shields.io/badge/dependencies-0-111827">
  <img alt="license" src="https://img.shields.io/badge/license-MIT-16A34A">
</p>

<p align="center">
  <img src="assets/cli-preview.svg" alt="Agent Log Triage CLI preview" width="88%">
</p>

## 为什么做这个

AI Agent 工具链继续快速增长，但很多仓库缺少小而清晰的本地检查器。这个工具保持零依赖、可接 CI、可双端镜像。

## 快速开始

```bash
npx github:aolingge/agent-log-triage --path failure.log
```

Generate Markdown:

```bash
npx github:aolingge/agent-log-triage --path failure.log --markdown > report.md
```

Generate SARIF:

```bash
npx github:aolingge/agent-log-triage --path failure.log --sarif > results.sarif
```

## 检查项

| Check | What it looks for |
| --- | --- |
| error | Contains error signal. |
| command | Contains command context. |
| file | Contains file or line context. |
| next | Contains next-step hint. |

## CI Usage

See [docs/github-actions.md](docs/github-actions.md).

## Mirrors

- GitHub: https://github.com/aolingge/agent-log-triage
- Gitee: https://gitee.com/aolingge/agent-log-triage

## Visual Identity

The banner and CLI preview are SVG assets committed in `assets/`, so the README renders cleanly on GitHub and Gitee without external image hosting.

## 参与贡献

Good first PRs: add checks, add fixtures, improve docs, or add GitHub Actions examples.

## License

MIT
