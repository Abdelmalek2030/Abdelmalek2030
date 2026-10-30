<div align="center">

# Abdelmalek
### Systems & Developer Tooling Architect

<p align="center">
  <img src="https://img.shields.io/badge/Focus-Systems_%26_Low_Overhead_Daemons-000000?style=for-the-badge&logo=gnu-bash&logoColor=white" />
  <img src="https://img.shields.io/badge/Architecture-Zero_Dependency_%2F_POSIX-101010?style=for-the-badge&logo=linux&logoColor=white" />
  <img src="https://img.shields.io/badge/Security-Reference_Grade_Cryptosystems-020202?style=for-the-badge&logo=securityscorecard&logoColor=white" />
</p>

*Engineering low-overhead daemon systems, zero-dependency POSIX CLI utilities, and deterministic developer productivity infrastructure across Linux and cloud environments.*

[<img src="https://img.shields.io/badge/GitHub-devtools--hub-181717?style=flat-square&logo=github">](https://github.com/Abdelmalek2030/devtools-hub)
[<img src="https://img.shields.io/badge/SecOps-env--vault--cli-007EC6?style=flat-square&logo=gnupg">](https://github.com/Abdelmalek2030/env-vault-cli)
[<img src="https://img.shields.io/badge/CI%2FCD-env--vault--action-2088FF?style=flat-square&logo=githubactions">](https://github.com/Abdelmalek2030/env-vault-action)
[<img src="https://img.shields.io/badge/Systems-docker--prune--daemon-00ADD8?style=flat-square&logo=go">](https://github.com/Abdelmalek2030/docker-prune-daemon)

</div>

---

### 🏛️ Core Engineering Principles

* **Minimal Surface Area & Zero Bloat:** Prioritizing zero-dependency or strictly audited architectures to eliminate supply-chain risk and binary bloat.
* **Unix Philosophy & Portability:** Building composable, deterministic tools that strictly conform to standard POSIX interface specifications across Linux, macOS, and BSD.
* **Resource Predictability:** Bounded memory footprints, atomic kernel primitives (`flock(2)` mutexes), and deterministic teardown via signal-safe traps (`SIGTERM`/`SIGKILL`).
* **Cryptographic Rigor:** Enforcing authenticated encryption (`AES-256-GCM`), memory hygiene (`buf.fill(0)` explicit wiping), and memory-hard key derivation (`scrypt` per RFC 7914).

---

### 🚀 Flagship Developer Tooling Infrastructure

| Repository | Stack | Architecture & Security Philosophy |
| :--- | :---: | :--- |
| **[`env-vault-cli`](https://github.com/Abdelmalek2030/env-vault-cli)** | `JavaScript` `Node.js` | Reference-grade zero-dependency CLI utilizing native `node:crypto` primitives for enterprise AES-256-GCM `.env` secret encryption, scrypt key rotation, and atomic persistence. |
| **[`env-vault-action`](https://github.com/Abdelmalek2030/env-vault-action)** | `GitHub Actions` `Node.js` | Official zero-dependency companion action for secure in-memory decryption and secret injection into `$GITHUB_ENV` with automated log redaction (`::add-mask::`). |
| **[`docker-prune-daemon`](https://github.com/Abdelmalek2030/docker-prune-daemon)** | `Go` `Systemd` | Low-overhead Docker pruning daemon engineered with integrated security auditing, signal-safe execution traps, and automated release pipelines. |
| **[`devtools-hub`](https://github.com/Abdelmalek2030/devtools-hub)** | `Infrastructure` | Centralized developer tooling hub enforcing strict XDG Base Directory compliance and hermetic CI/CD quality gates. |

---

### 🛠️ Technical Competency Matrix

* **Systems & Languages:** Go, Native JavaScript (Node.js runtime primitives), POSIX Shell Scripting, GNU Make.
* **Cryptography & SecOps:** AES-256-GCM (AEAD), scrypt (RFC 7914), HMAC-SHA256, CSPRNG stream generation, CSPRNG heredoc isolation.
* **Infrastructure & CI/CD:** Docker containerization, systemd daemons, GitHub Actions CI/CD matrix optimization, CodeQL security auditing, OpenSSF scorecard compliance.
* **Code Quality & Governance:** Strict zero external runtime dependencies, explicit memory hygiene, atomic filesystem operations, POSIX 0600 permission enforcement.

---

<div align="center">
  <i>"Simplicity is prerequisite for reliability. Zero dependencies mean zero supply-chain attack vectors."</i>
</div>
