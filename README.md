# Neko-AI Public

Release artifacts for [Neko-AI](https://github.com/Neko-Inference/Neko-AI).

Every `cli-v*` tag here carries the `neko` terminal client:

| asset | what it is |
| --- | --- |
| `neko-linux-amd64` | the static musl build — Ubuntu, Fedora, Arch, Debian, RHEL, openSUSE, Alpine, WSL2 |
| `neko-linux-amd64.sha256` | its checksum |
| `release.json` | the manifest the CLI's update check reads |

Install:

```sh
curl -fsSL https://panel-ai.neko-build.tech/install.sh | bash
```

The installer verifies the checksum before it writes anything. This repository
holds binaries only; the source lives in the private monorepo.
