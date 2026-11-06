# Neko-AI Public

Release artifacts for [Neko-AI](https://github.com/Neko-Inference/Neko-AI).

Every `cli-v*` tag here carries the `nekocode` terminal client:

| asset | what it is |
| --- | --- |
| `nekocode-linux-amd64` | the static musl build — Ubuntu, Fedora, Arch, Debian, RHEL, openSUSE, Alpine, WSL2 |
| `nekocode-macos-arm64` | Apple Silicon macOS build, ad-hoc signed |
| `nekocode-macos-amd64` | Intel macOS build, ad-hoc signed |
| `*.sha256` | the checksum for the matching binary |
| `release.json` | the manifest the CLI's update check reads |

Install:

```sh
curl -fsSL https://panel-ai.neko-build.tech/install.sh | bash
```

The installer verifies the checksum before it writes anything. It is Linux
x86_64; on macOS, download the matching `nekocode-macos-*` asset and its
`.sha256`, verify the checksum, and place the binary at
`~/.local/bin/nekocode`.

This repository holds binaries only; the source lives in the private monorepo.
