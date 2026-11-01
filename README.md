<div align="center">

<img width="100%" src="assets/hero.svg" alt="Abdelouahid Kherchache" />

<a href="https://git.io/typing-svg">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=24&duration=3000&pause=800&color=FF1E1E&center=true&vCenter=true&width=650&lines=Final-Year+CS+Student+%40+USTHB;Next.js+%7C+TypeScript+%7C+Nest.js+Developer;Docker+%7C+Dokploy+%7C+Production+Deployments;Exploring+Web+Security+%26+Pentesting;" alt="Typing SVG" />
</a>

<br/>

<img src="https://img.shields.io/badge/USTHB-L3%20ACAD%20Software%20Engineering-B22222?style=for-the-badge&logo=googlescholar&logoColor=white" />
<img src="https://img.shields.io/badge/Location-Algiers,%20Algeria-8B0000?style=for-the-badge&logo=googlemaps&logoColor=white" />

<br/><br/>

<a href="https://portfolio-ouahid.vercel.app"><img src="https://img.shields.io/badge/Portfolio-CC0000?style=for-the-badge&logo=vercel&logoColor=white" /></a>
<a href="https://linkedin.com/in/abdelouahid-kherchache"><img src="https://img.shields.io/badge/LinkedIn-990000?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
<a href="mailto:wahidkherchache@gmail.com"><img src="https://img.shields.io/badge/Email-8B0000?style=for-the-badge&logo=gmail&logoColor=white" /></a>
<!-- <a href="https://github.com/wahidkherchache"><img src="https://img.shields.io/badge/GitHub-660000?style=for-the-badge&logo=github&logoColor=white" /></a> -->

<br/><br/>

<img src="https://komarev.com/ghpvc/?username=wahidkherchache&style=for-the-badge&color=CC0000&label=PROFILE+VIEWS" />
<img src="https://img.shields.io/github/followers/wahidkherchache?style=for-the-badge&color=B22222&label=FOLLOWERS&logo=github" />
<img src="https://img.shields.io/github/stars/wahidkherchache?style=for-the-badge&color=8B0000&label=STARS" />

</div>

<br/>

---

## 🔴 About Me

```yaml
name: "Abdelouahid Kherchache"
role: "Junior Computer Engineer"
university: "USTHB — University of Science and Technology Houari Boumediene"
location: "Baba Hassen, Algiers, Algeria"
```

Full-Stack Developer and final-year Computer Science student at USTHB (Algiers), specializing in software engineering. Ive been working as a Junior Software Engineer at Black and Yellow since August 2026, building production web applications end to end. On the front end, I work with Next.js, React, and TypeScript. On the back end, I build APIs with Nest.js and Node.js, backed by PostgreSQL (with Prisma ORM) and MongoDB.



 
## 🔴 Tech Stack

**Languages**
<p> <img src="https://skillicons.dev/icons?i=java,c,js,ts,python" /> </p>

**Front-End**
<p> <img src="https://skillicons.dev/icons?i=react,nextjs,html,css,tailwind,vite" /> </p>

**Back-End & Databases**
<p> <img src="https://skillicons.dev/icons?i=nodejs,nestjs,express,mongodb,postgres,prisma,redis,supabase" /> </p>

**Cloud, DevOps & Tooling**
<p> <img src="https://skillicons.dev/icons?i=linux,docker,git,github,githubactions,vscode,vercel" /> </p>

<p>
<img src="https://img.shields.io/badge/Dokploy-CC0000?style=for-the-badge&logoColor=white" />
<img src="https://img.shields.io/badge/Traefik-8B0000?style=for-the-badge&logo=traefikproxy&logoColor=white" />
<img src="https://img.shields.io/badge/MinIO-B22222?style=for-the-badge&logo=minio&logoColor=white" />
<img src="https://img.shields.io/badge/WireGuard-990000?style=for-the-badge&logo=wireguard&logoColor=white" />
</p>

**Design**
<p> <img src="https://skillicons.dev/icons?i=figma" /> </p>

---

## 🔴 Security & Networking Focus

<div align="center">

| Domain | Proficiency | Details |
|---|:---:|---|
| Web Application Security | 🔴🔴🔴⚪⚪ | OWASP Top 10, XSS, CSRF, SQL Injection, security headers |
| Networking Fundamentals | 🔴🔴🔴🔴⚪ | Core networking concepts, Linux/CMD comparative administration |
| Web Pentesting | 🔴🔴⚪⚪⚪ | Building toward bug bounty participation |
| Databases & SQL | 🔴🔴🔴⚪⚪ | Oracle SQL, relational design |

</div>

---




## 🔴 Featured Work

<details open>
<summary><b>🎨 E-Learning Platform — System Design in Figma</b> · <i>Delivered</i></summary>
<br/>

Complete design of an e-learning platform: the whole website, all pages, delivered in Figma and handed over to the client.

| | |
|---|---|
| **Scope** | Full website — every page, user flows and component system |
| **Tool** | Figma |
| **Status** | ✅ Delivered |

</details>

<details>
<summary><b>🚀 Production CMS Deployment on a Client VPS</b></summary>
<br/>

Took a multi-service headless CMS from local development to a real production VPS owned by the client, using Docker Swarm and Dokploy.

| | |
|---|---|
| **Frontend / Admin** | Next.js (standalone Docker output) |
| **API** | NestJS |
| **Database** | MongoDB as a replica set (transactions required) |
| **Cache / Rate limiting** | Redis |
| **File storage** | MinIO (S3-compatible) behind a File Manager service |
| **Proxy + TLS** | Traefik + Let's Encrypt |
| **Access** | WireGuard VPN, SSH |

```text
Visitor --HTTPS--> Traefik --> Website | Dashboard | API | MinIO (signed links)
                                              API --> MongoDB, File Manager --> MinIO, Redis
```

Only Traefik is exposed. Databases, Redis and internal services stay on the internal Docker network.

</details>

---

## 🔴 What I Learned — Deployment & DevOps

<details>
<summary><b>🐳 Docker & Networking</b></summary>
<br/>

- Services talk to each other by **service name**, never `localhost`; services on different networks cannot see each other.
- Debugged a container-only `Connection reset by peer` caused by an **MTU mismatch** (1442 vs 1500). Fixed with TCP **MSS clamping** (`iptables`), persisted with `netfilter-persistent`.
- Swarm `host`-mode published ports bypass the `DOCKER-USER` chain — always verify firewall rules with packet counters instead of assuming they work.

</details>

<details>
<summary><b>🔐 Configuration & Secrets</b></summary>
<br/>

- `NEXT_PUBLIC_*` variables are baked at build time: changing them needs a **rebuild**, not a restart.
- Runtime secrets never go into an image; secrets shared by two services must be byte-identical, all others unique per environment and per client.
- Anything that appears in a screenshot or log is exposed and must be rotated.

</details>

<details>
<summary><b>🔎 Debugging Method</b></summary>
<br/>

- Read the exact log line — each error points at one layer: `WRONGPASS` (Redis), `ENOTFOUND` (DNS/network), `InvalidAccessKeyId` (storage key), `self-signed certificate` (TLS not issued yet), `Not authenticated` (service token / allowed IP).
- Split the system into layers and test each alone: DNS → port → TLS → proxy → app → database.
- Prove it before blaming someone else's network: packet counters and `tcpdump`.

</details>

<details>
<summary><b>🗄️ Data, Storage, TLS & DNS</b></summary>
<br/>

- MongoDB **replica set** is mandatory when the API uses transactions.
- S3-style storage serves downloads through **presigned URLs**: the storage service needs a public domain with a valid certificate, and the signed hostname can't change afterwards.
- Let's Encrypt (HTTP-01) needs port 80 open and correct DNS; mind the per-domain rate limits.

</details>

<details>
<summary><b>⚙️ Build Resources & Operations</b></summary>
<br/>

- Building Next.js/Nest images on a small machine: one build at a time, with swap; measure the real minimum heap before lowering `NODE_OPTIONS`.
- Traefik JSON access logs + `logrotate` (30+ days); daily backups (`mongodump` + storage volume), 7-day retention, plus an **off-server copy** and a tested restore.
- Admin ports (SSH, platform panel) reachable only through a VPN.

</details>

---

## 🔴 Contribution Snake

<div align="center">
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/wahidkherchache/wahidkherchache/output/github-contribution-grid-snake-dark.svg" />
  <img alt="Contribution snake" src="https://raw.githubusercontent.com/wahidkherchache/wahidkherchache/output/github-contribution-grid-snake.svg" width="100%" />
</picture>
</div>

---

## 🔴 Connect With Me

<div align="center">

<a href="mailto:wahidkherchache@gmail.com"><img src="https://img.shields.io/badge/Gmail-CC0000?style=for-the-badge&logo=gmail&logoColor=white" /></a>
<a href="https://linkedin.com/in/abdelouahid-kherchache"><img src="https://img.shields.io/badge/LinkedIn-8B0000?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
<!-- <a href="https://github.com/wahidkherchache"><img src="https://img.shields.io/badge/GitHub-660000?style=for-the-badge&logo=github&logoColor=white" /></a> -->
<a href="https://wahidkherchache.github.io/Portfo/"><img src="https://img.shields.io/badge/Portfolio-B22222?style=for-the-badge&logo=vercel&logoColor=white" /></a>

</div>

---

<div align="center">

*"Code with purpose, secure with intent."*

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:1a1a1a,50:8B0000,100:0d0d0d&height=120&section=footer" />

</div>
