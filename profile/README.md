<div align="center">

<img src="github_banner.jpg" alt="Tensorlake" width="100%">

### Agent-native compute infrastructure.
### Secure sandboxes that scale from one to thousands.

[Documentation](https://docs.tensorlake.ai/) · [Book a Demo](https://calendly.com/diptanu-tensorlake/30min) · [Slack](https://tensorlakecloud.slack.com/)

</div>

---

Tensorlake provides dynamic, persistent sandboxes for AI agents. Run untrusted code securely, fan out parallel execution across clusters, and checkpoint agents to resume them on demand — from the CLI or the Python SDK.

```bash
pip install tensorlake
tl login
tl sbx create my-sandbox --cpus 1.0 --memory 1024
tl sbx exec <sandbox-id> python -c 'print("Hello from Tensorlake")'
tl sbx checkpoint <sandbox-id>
```

```python
from tensorlake.sandbox import Sandbox

sandbox = Sandbox.create(name="my-sandbox", cpus=1.0, memory_mb=1024)

result = sandbox.run("python", ["-c", "print('Hello from Tensorlake')"])
print(result.stdout)

# Checkpoint and snapshot
snapshot = sandbox.checkpoint(sandbox.sandbox_id)
```

## Why Tensorlake

- **Distributed Fan-out** — Go from one sandbox to hundreds per second for deep research and parallel tool use
- **Stateful Suspend & Resume** — Checkpoint agents to cold storage, wake them up instantly when needed
- **Dynamic Resources** — Allocate CPU, memory, and GPU on the fly — no static templates
- **SSD-native I/O** — Built for workloads that read and write heavily, not just fast boot
- **BYOC / On-Prem** — Run on your infrastructure for cost control, security, and compliance
- **Install Anything** — Docker, Kubernetes, systemd — full Linux environments, not stripped-down containers

## Repositories

| Repository | Description |
|---|---|
| [tensorlake/sdk](https://github.com/tensorlakeai/tensorlake) | CLI and Python SDK |
| [tensorlake/cookbooks](https://github.com/tensorlakeai/cookbooks) | Example projects and integrations |
| [tensorlake/skills](https://github.com/tensorlakeai/tensorlake-skills) | Skills for coding agents to use Tensorlake |
| [benchmarks](https://github.com/tensorlakeai/sandbox-sqlite-bench) | Sandbox File System I/O Benchmarks |

## Get in Touch

- [Documentation](https://docs.tensorlake.ai/)
- [Blogs](https://www.tensorlake.ai/blog)
- [Book a Demo](https://calendly.com/diptanu-tensorlake/30min)
- [Slack](https://tensorlakecloud.slack.com/)
- [Newsletter](https://tensorlake.beehiiv.com/)

<div align="center">

[![X](https://img.shields.io/badge/Follow_on_X-000000?style=flat&logo=x&logoColor=white)](https://x.com/tensorlake)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/company/tensorlake)

</div>
