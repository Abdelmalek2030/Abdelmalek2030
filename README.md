# Abdelmalek

**Systems & Developer Tooling Engineer**  
Focused on low-overhead background daemons, zero-dependency CLI utilities, and developer productivity tooling across Linux and cloud environments.

---

### Core Engineering Principles

- **Minimal Surface Area & Zero Bloat**: Prioritizing zero-dependency or strictly audited architectures to reduce supply-chain risk and binary sizes.
- **Unix Philosophy**: Small, composable tools that accept standard inputs, emit clean outputs, and integrate seamlessly into terminal pipelines.
- **Resource Predictability**: Safe concurrency, deterministic memory footprints, and daemon stability for continuous local development.

---

### Featured Open Source Tooling

#### [`docker-prune-daemon`](https://github.com/Abdelmalek2030/docker-prune-daemon)
> Automated background daemon for container disk reclamation, dangling image lifecycle management, and Docker engine maintenance.

- **Stack**: Go (Golang) / Docker Engine API
- **Key Features**: Configurable disk pressure thresholds, non-blocking scheduled pruning, safe container volume exclusion rules.
- **Status**: Active development · MIT License

```bash
# Run standalone daemon
docker-prune-daemon --threshold=85% --interval=30m


