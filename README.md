# Hi, I'm Yaser

**Full stack engineer · networking · distributed systems · ERP**

I currently build and run **VoidLag**, a gaming private network spanning 350+ PoPs in 50+ countries, and develop **NaderERP**, an ERP fork running in production across a group of companies. Main stack: C++, Go, Python and TypeScript.

<p>
  <a href="https://voidlag.com"><img src="https://img.shields.io/badge/VoidLag-voidlag.com-22c55e?style=flat-square" alt="VoidLag"></a>
  <a href="mailto:yassernaader@gmail.com"><img src="https://img.shields.io/badge/Email-yassernaader%40gmail.com-0ea5e9?style=flat-square&logo=gmail&logoColor=white" alt="Email"></a>
  <img src="https://img.shields.io/badge/Based%20in-Foz%20do%20Igua%C3%A7u%2C%20Brazil-64748b?style=flat-square" alt="Location">
  <img src="https://img.shields.io/badge/Speaks-PT%20%C2%B7%20AR%20%C2%B7%20EN-a855f7?style=flat-square" alt="Spoken languages">
</p>

<p>
  <img src="https://skillicons.dev/icons?i=cpp,go,py,ts,js,qt,nestjs,vue,nuxtjs,postgres,redis,docker,linux,aws,cloudflare,githubactions,grafana&perline=17" alt="Main stack">
</p>

---

## Featured work

### VoidLag — Gaming Private Network (GPN) · [voidlag.com](https://voidlag.com)
Gaming private network (GPN) SaaS that cuts jitter, packet loss and ping (**~35%** on Brazil–Europe routes). Worldwide coverage, **2,500+ users**, **2,458 games**.

```text
Windows client  (C++ · Qt 6)
├─ login ─────────> API  (NestJS) ──> picks best relay, registers WireGuard peer
└─ game traffic ──> Relay PoP  (Go · Linux) ──> NAT ──> Game server
   via WireGuard tunnel, only the game's packets
```

| Layer | Stack | Highlights |
|---|---|---|
| Desktop client | C++17, Qt 6 | Game process detection, live per-relay ping, licensing, auto-update, Authenticode-signed installer |
| Per-process tunnel | Go, wireguard-go, Windows Filtering Platform | Virtual TUN adapter capturing only the game's packets, no changes to the Windows routing table |
| Relays | Go, Linux, AWS, Hetzner, Vultr | WireGuard peer sync, NAT, UDP latency probes, on-demand traceroute, metrics, mTLS control API, cloud-init provisioning |
| Backend | NestJS, TypeScript, PostgreSQL, Prisma, Redis | Licenses, sessions, affiliates, Stripe/Asaas subscriptions, SSE over Redis pub/sub, cron jobs with distributed locks |
| Web & ops | Nuxt 4, Vue 3, Docker, Traefik, GitHub Actions | Customer area, admin and MRR dashboards, CI/CD with automated tests, multi-VPS deploys |

### NaderERP — ERP built on my own OpenERP/Odoo fork
Running in production across a business group and its partners, with 60+ users.

| Layer | Stack | Highlights |
|---|---|---|
| Core | Python, OpenERP ORM, PostgreSQL, JavaScript/OWL | 160+ maintained modules, core patches (ORM, web client, access control), i18n in PT/ES/EN/AR |
| Custom modules | Python, QWeb, OWL | Multi-currency finance with cash sessions, location-based stock picking, catalog and pricelist repricing, event-driven auto-printing, RBAC with 9 roles |
| NaderPrint | C++, Qt 6 | Tray agent that receives print jobs in real time and prints to local printers (raw ESC/POS and ZPL, PDF via QtPdf), token pairing, signed installer |
| Delivery | Docker Compose, PostgreSQL 16, Traefik, Make | Per-client deploy kit, SemVer-tagged DB migrations, staging validation, proxy-level maintenance mode |
| Infrastructure | Proxmox VE, PBS, Dell iDRAC, Grafana | On-prem virtualization, backups, server management and monitoring |

> Most of these repositories are private. Code walkthroughs are available on request.

---

## Stack

<details>
<summary>Full stack list</summary>

- **Languages:** C++17 · Go · Python · TypeScript · JavaScript · SQL · C# · Java · Delphi · Bash
- **Backend:** NestJS · REST · SSE · Redis · cron jobs · webhooks · OAuth 2.0 · Stripe · Asaas
- **Frontend:** Vue 3 · Nuxt 4 · Tailwind CSS · shadcn-vue · QWeb
- **Desktop:** Qt 6 · CMake · Inno Setup · Authenticode · ESC/POS and ZPL printing
- **ERP & data:** OpenERP/Odoo (ORM, modules, core) · Minerva · PostgreSQL · InterBase · Prisma
- **Networking:** TCP/IP · WireGuard · NAT · WFP packet interception · mTLS · LAN/Wi-Fi
- **Practices:** distributed systems · high availability · automated testing · CI/CD · observability (Grafana)
- **On-premises:** Proxmox VE · Proxmox Backup Server · Dell iDRAC
- **Cloud & DevOps:** AWS · Hetzner · Vultr · Cloudflare · Linux · Docker · Traefik · systemd · GitHub Actions

</details>

