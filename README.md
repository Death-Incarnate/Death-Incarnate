```
 ____             _   _       ___                                  _
|  _ \  ___  __ _| |_| |__   |_ _|_ __   ___ __ _ _ __ _ __   __ _| |_ ___
| | | |/ _ \/ _` | __| '_ \   | || '_ \ / __/ _` | '__| '_ \ / _` | __/ _ \
| |_| |  __/ (_| | |_| | | |  | || | | | (_| (_| | |  | | | | (_| | ||  __/
|____/ \___|\__,_|\__|_| |_| |___|_| |_|\___\__,_|_|  |_| |_|\__,_|\__\___|
```

**Chris Schwieters** — U.S. Army Veteran

Infrastructure engineer. Security operator. Building autonomous systems that monitor, defend, and optimize themselves.

---

### What I Run

```
Machine    Death-Incarnate
CPU        AMD Ryzen 9 9950X3D — 16C/32T, 144MB L3
GPU        NVIDIA RTX 5070 Ti — PCIe Gen5 x16
Memory     64GB DDR5
Storage    Dual NVMe (930GB + 3.7TB)
Network    10GbE (Aquantia AQC113CS)
OS         CachyOS (Arch) — Kernel 6.19, PREEMPT_DYNAMIC
Scheduler  scx_bpfland (sched-ext BPF)
```

### What I Build

**Self-Monitoring Infrastructure** — Health checks, thermal monitoring, network surveillance, automated alerting, system profiling. One ecosystem repo runs everything. 5-minute monitoring cycles. NASA-grade fault detection with tiered recovery.

**MCP Server Ecosystem** — Custom Model Context Protocol servers giving AI agents direct control over system telemetry, home devices, network infrastructure, and cloud services. 8 servers, 50+ tools.

**Edge Computing** — Cloudflare Workers with AI inference (12 endpoints), Durable Objects, D1 storage, Zero Trust networking, and automated deployment pipelines.

**Security Operations** — Credential validation, vulnerability research, attack surface mapping. Offensive security with defensive infrastructure.

### Stack

```
Systems    Bash, Python, systemd, BPF
Cloud      Cloudflare (Workers, Pages, D1, Tunnel, AI)
AI/Agents  Claude Code, MCP, FastMCP
Infra      Vercel, AWS, Cloudflare Zero Trust
Monitors   Custom (health-check.sh, 5 subsystem monitors)
Profiling  perf, FlameGraph, custom benchmark suite
Network    ASUS GT-BE98 Pro (WiFi 7), 10GbE backbone
```

### Philosophy

Build it right or don't build it. Zero bloat, zero dead code, zero orphan configs. Every component traces to a requirement. If it doesn't serve a purpose, it gets deleted.

Smallest viable change. Abstract only at rule of three. Optimize only after profiling.

---

<sub>Purpose-built from Idaho.</sub>


---

## OpenClaw Content Studio Blueprint

A full architecture and implementation blueprint for an autonomous content studio (OpenClaw + Remotion + Nano Banana 2 + multi-platform publishing) is available under:

- `docs/openclaw-content-studio/README.md`
