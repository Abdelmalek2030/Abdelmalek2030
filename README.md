# Abdelmalek

**Systems & Developer Tooling Engineer**  
Focused on low-overhead background daemon systems, zero-dependency POSIX CLI utilities, and developer productivity tooling across Linux and cloud infrastructure.

[![GitHub Sponsors](https://img.shields.io/badge/Sponsor-%E2%99%A5-ea4aaa?style=flat&logo=githubsponsors)](https://github.com/sponsors/Abdelmalek2030)
[![ShellCheck](https://img.shields.io/badge/Lint-ShellCheck%20Strict-brightgreen.svg)](#core-engineering-principles)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](./LICENSE)
[![GitHub Sponsors Target](https://img.shields.io/badge/Support-GitHub%20Sponsors-ea4aaa?style=flat&logo=githubsponsors&logoColor=white)](https://github.com/sponsors/Abdelmalek2030)

---

## ⚙️ Core Engineering Principles

- **Minimal Surface Area & Zero Bloat**: Prioritizing zero-dependency or strictly audited architectures to eliminate supply-chain risk and binary bloat.
- **Unix Philosophy & Portability**: Building composable, deterministic tools that strictly conform to standard POSIX `/bin/sh` specifications across Linux, macOS, and BSD.
- **Resource Predictability**: Bounded memory footprints, atomic kernel primitives (`mkdir(2)` mutexes), and deterministic teardown via signal-safe traps (`SIGTERM`/`SIGKILL`).

---

## 🛠️ Featured Open Source Infrastructure

### [devtools-hub](https://github.com/Abdelmalek2030/devtools-hub)
[![CI Pipeline](https://github.com/Abdelmalek2030/devtools-hub/actions/workflows/ci.yml/badge.svg)](https://github.com/Abdelmalek2030/devtools-hub/actions/workflows/ci.yml)
[![POSIX 100%](https://img.shields.io/badge/Language-Shell%20100%25-green.svg)](https://github.com/Abdelmalek2030/devtools-hub)

Reference-grade suite of zero-dependency POSIX developer utilities engineered with strict XDG Base Directory compliance:
- **`clean-ports`**: Port reclaimer with graceful `SIGTERM` teardown and deterministic `--dry-run` inspection.
- **`xdg-audit`**: Filesystem compliance auditor and storage footprint inspector with strict CI assertion modes.
- **`sys-doctor`**: Health diagnostics covering kernel architecture, load averages, disk pressure, and zombie processes.
- **`with-lock`**: Atomic concurrency mutex wrapper using POSIX `mkdir(2)` semantics for cron and CI/CD pipelines.
- *Infrastructure*: Complete section 1 UNIX manual pages (`man/`), AST markdownlinting, hermetic sandboxing, and execution latency benchmarking.

### [docker-prune-daemon](https://github.com/Abdelmalek2030/docker-prune-daemon)
[![CI Matrix & Quality Gate](https://github.com/Abdelmalek2030/docker-prune-daemon/actions/workflows/ci.yml/badge.svg)](https://github.com/Abdelmalek2030/docker-prune-daemon/actions/workflows/ci.yml)
[![GoReleaser](https://img.shields.io/badge/release-GoReleaser-blue?style=flat&logo=goreleaser)](https://github.com/goreleaser/goreleaser)
[![Go 100%](https://img.shields.io/badge/Language-Go%20100%25-blue.svg)](https://github.com/Abdelmalek2030/docker-prune-daemon)

Reference-grade, zero-dependency Go background daemon engineered for autonomous Docker disk space reclaim, kernel-level `syscall.Statfs` watermark auditing, systemd cgroups v2 (`MemoryMax=32M`) resource sandboxing, and cryptographic SLSA release provenance.

### [env-vault-cli](https://github.com/Abdelmalek2030/env-vault-cli)
Zero-dependency secure CLI utility built with native Node.js crypto modules for enterprise-grade AES-256-GCM environment file encryption and synchronization.

### [env-vault-action](https://github.com/Abdelmalek2030/env-vault-action)
Official GitHub Action companion for zero-dependency `.env.vault` decryption and direct injection of secrets into `$GITHUB_ENV` with automated CI log masking.

---

## 📈 Quality & Tooling Standards

```text
Static Analysis   ──► ShellCheck (Aggressive Rules: quote-safe-variables, check-unassigned-uppercase)
Testing Suite     ──► Zero-dependency behavioral assertions & isolated disposable mktemp sandboxes
Documentation     ──► Formal Architecture Specifications, Threat Models, and native roff man(1) pages
Distribution      ──► Standalone curl-to-sh bootstrap installer & standardized GNU Makefile
