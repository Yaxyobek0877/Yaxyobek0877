<p align="center">
  <a href="README.md">O'zbekcha</a> · <b>English</b> · <a href="README.ru.md">Русский</a>
</p>

<h1 align="center">
  <a href="https://github.com/Yaxyobek0877">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=28&duration=3000&pause=1000&color=00ADD8&center=true&vCenter=true&width=760&lines=Hi%2C+I%27m+TexUz%21;Backend+%26+Full-Stack+Developer;AI+Engineer+%2F+LLM+integration;Python+%7C+Go+%7C+PostgreSQL;Hello+from+Kokand%21" alt="Typing SVG" />
  </a>
</h1>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=Yaxyobek0877&label=Profile%20views&color=00ADD8&style=for-the-badge" alt="Profile views" />
  <a href="https://github.com/Yaxyobek0877?tab=followers">
    <img src="https://img.shields.io/github/followers/Yaxyobek0877?label=Followers&style=for-the-badge&color=00ADD8&labelColor=0d1117" alt="GitHub followers" />
  </a>
  <img src="https://img.shields.io/badge/Focus-Backend%20%26%20AI-success?style=for-the-badge&labelColor=0d1117" alt="Focus" />
</p>

---

## About me

```yaml
name:           TexUz
role:           Backend / AI engineer / team lead
location:      Kokand, Uzbekistan
projects:      [1Pro (AI Gateway), Gazer Max (smart campus), Portal (P2P mesh), Enif]
open_source:   [github.com/Yaxyobek0877/portal_traffic]
technologies:  [Django, FastAPI, PostgreSQL, pgvector, Redis, Docker, Cloudflare]
ai_stack:      [InsightFace, CUDA, LLM API, RAG, Vector search]
networking:    [WebRTC, pion/webrtc, PCP-1 (Ed25519/X25519/XChaCha20)]
learning_now:  [Model fine-tuning, System centralization, MLOps]
motto:         "Ideas can't be invented on demand — they take shape gradually."
```

- Currently building **1Pro AI Inference Gateway** (LLM API platform), **Gazer Max** (face-recognition smart campus) and **Portal** (open-source P2P mesh desktop app); **Enif** is also one of my projects.
- **AI engineering**: LLM APIs, **RAG**, **vector search** (`pgvector` HNSW), **face embeddings** (`InsightFace` + CUDA) and **agents**.
- **Networking & P2P**: WebRTC + `pion/webrtc`, NAT-traversal, mesh topology, **PCP-1** encryption (Ed25519 + X25519 + XChaCha20-Poly1305).
- **Backend & infra**: PostgreSQL optimization, real-time (WebSocket, mediamtx), **Hikvision ISAPI**, **Cloudflare Tunnel**, Docker.
- Contact: **yaxyobek877@gmail.com** or via [Telegram](https://t.me/adhamov_yaxyobek).

---

## Main projects

### 1Pro — AI Inference Gateway

<p>
  <a href="http://1pro.uz/">
    <img src="https://img.shields.io/badge/Site-1pro.uz-00ADD8?style=for-the-badge&logo=googlechrome&logoColor=white" alt="1pro.uz" />
  </a>
  <a href="https://1pro.uz/dashboard">
    <img src="https://img.shields.io/badge/Dashboard-1pro.uz%2Fdashboard-412991?style=for-the-badge&logo=vercel&logoColor=white" alt="Dashboard" />
  </a>
</p>

**Site:** [1pro.uz](http://1pro.uz/) &nbsp;·&nbsp; **Type:** AI Inference Gateway &nbsp;·&nbsp; **My role:** Backend & AI integration

**1Pro** is a platform offering **simple access to powerful AI models through a single API**. For startups and developers: sign up, start on the free tier, and launch instantly via chat or API.

**Core idea**
> We take on the infrastructure complexity —
> so your startup can focus entirely on building AI features.

**Capabilities**
- **Unified interface** — one API key, one endpoint format. Quick access to 70B-class models.
- **Free to start** — free quota for new users. Track token spend, limits and overall usage clearly via the dashboard.
- **Enterprise security** — strict per-model permissions. Development, staging and production keys are isolated.
- **OpenAI-compatible API** — standard `chat/completions` format, existing SDKs just work.

**API example** (supported in Python, Node.js and cURL)

```python
import requests

api_key = "sk-[Your-Key]"
url = "https://1pro.uz/v1/chat/completions"

headers = {
    "Authorization": f"Bearer {api_key}",
    "Content-Type": "application/json"
}
data = {
    "model": "coder",
    "messages": [{"role": "user", "content": "Hello!"}]
}

response = requests.post(url, headers=headers, json=data)
print(response.json())
```

---

### Gazer Max — smart campus system

<p>
  <a href="https://gazer.1pro.uz/presentation.html">
    <img src="https://img.shields.io/badge/Presentation-gazer.1pro.uz%2Fpresentation.html-00ADD8?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Gazer Max presentation" />
  </a>
  <img src="https://img.shields.io/badge/%231-Smart%20campus-success?style=for-the-badge&labelColor=0d1117" alt="#1 smart campus" />
</p>

**Presentation:** [gazer.1pro.uz/presentation.html](https://gazer.1pro.uz/presentation.html) &nbsp;·&nbsp; **Type:** Face recognition & smart campus platform &nbsp;·&nbsp; **My role:** Backend / AI / team lead

**Gazer Max** is a **unified AI platform** for universities, schools and organizations. Face recognition, automatic attendance, turnstile and camera management, real-time security — all in one system. **Battle-tested on 20,000+ students** in Uzbekistan.

**Tagline**
> A glance is enough. AI handles the rest.

**Real metrics (university deployment)**

| Metric | Value |
|---|---|
| Active student base | **20,000+** |
| IP cameras | **40+** |
| Turnstiles | **30+** |
| Face search time | **< 10 ms** |
| Recognition accuracy | **99.6%** |
| Deployment time | **1 week** |
| Door open latency | **~50 ms** |

**Modules (12, usable independently)**
- **Face recognition (AI)** — 512-dim embedding, pgvector HNSW index
- **Automatic attendance** — `on_time` / `late` / `absent` / `left_early` states
- **Real-time monitor** — 40+ cameras on one screen, AI analysis on every frame
- **Turnstile control** — Hikvision (DS-K1T341CMF) via ISAPI, works offline too
- **Building & room map** — Building / Floor / Classroom hierarchy
- **Search by face** — upload one image, get full history (reverse search)
- **HEMIS sync** — student/faculty/group automatically
- **Class schedule** — attendance computed automatically from the schedule
- **Reports & analytics** — live dashboard, Excel/PDF export
- **Granular access control** — exact cameras/buildings/rooms per user
- **Live audit log** — every access, admin action, attempt
- **Open REST API** — Swagger, API key scope (read/write/full)

**Tech stack**
- **AI:** InsightFace (buffalo_l) + NVIDIA CUDA — face embeddings
- **Vector DB:** PostgreSQL + **pgvector HNSW** index
- **Backend:** Django 5 + Celery + Redis
- **Frontend:** React 19
- **Media:** mediamtx (HLS & WebRTC, 25 fps)
- **Devices:** Hikvision IP cameras and turnstiles (ISAPI)
- **Infra:** Docker, **Cloudflare Tunnel** (outbound-only — the server opens no ports)
- **Real-time:** WebSocket

**7-layer security**
1. Cloudflare Edge (WAF, DDoS, bot, GeoIP)
2. Cloudflare Access (2FA for the admin panel)
3. nginx + TLS 1.3
4. Django + Argon2id (brute-force lock, CSRF, CSP)
5. Database encrypted (Fernet AES-256)
6. JWT (15-minute token) + API keys with scope
7. Full audit log

**Users**
Universities · schools and lyceums · companies and offices · medical institutions · government agencies · factories and warehouses

**Results (after 1 month)**
- −92% attendance time (30 minutes → 0)
- +45% attendance accuracy
- −68% security incidents
- 0 UZS spent on ID cards

---

### Portal — P2P mesh networking app (open-source)

<p>
  <a href="https://portal.1pro.uz/">
    <img src="https://img.shields.io/badge/Site-portal.1pro.uz-00ADD8?style=for-the-badge&logo=googlechrome&logoColor=white" alt="portal.1pro.uz" />
  </a>
  <a href="https://github.com/Yaxyobek0877/portal_traffic">
    <img src="https://img.shields.io/badge/GitHub-portal__traffic-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub repo" />
  </a>
  <a href="https://github.com/Yaxyobek0877/portal_traffic/releases/latest">
    <img src="https://img.shields.io/github/v/release/Yaxyobek0877/portal_traffic?style=for-the-badge&label=Release&color=00ADD8&labelColor=0d1117" alt="Latest release" />
  </a>
  <img src="https://img.shields.io/badge/License-MIT-success?style=for-the-badge&labelColor=0d1117" alt="MIT license" />
</p>

**Site:** [portal.1pro.uz](https://portal.1pro.uz/) &nbsp;·&nbsp; **Code:** [github.com/Yaxyobek0877/portal_traffic](https://github.com/Yaxyobek0877/portal_traffic) &nbsp;·&nbsp; **My role:** Author & lead developer

**Portal** is a desktop app that builds a private **peer-to-peer mesh network** between devices. Direct connections, no server in the middle (the signaling server only participates in the handshake). Local account, multiple rooms in parallel, automatic reconnection. Chat, files, port tunneling for cameras/NVR/game servers — all P2P.

**Tagline**
> No server in the middle. Direct connections.

**Key features**
- **2 to 16 devices** in a mesh — share via Portal ID + code (no router/VPN/port forwarding required)
- **Chat and file transfer** — drag-and-drop, end-to-end encrypted
- **TCP/UDP tunneling** — share a Minecraft server, Hikvision NVR, LAN cameras and other services over the mesh
- **Live mesh diagram** — RTT, NAT-traversal indicators (LAN / Internet / TURN), bandwidth probe
- **QR + portal code** — QR for someone next to you, ID + code for someone remote
- **Local account** — bcrypt password, no email or central registration
- **Multi-portal** — family + work + game rooms in parallel
- **Automatic reconnection** — previous sessions restored after a system reboot
- **Per-service approval** — every connection confirmed individually

**Encryption: PCP-1 protocol**
A second encryption layer under WebRTC DTLS:
- **Ed25519** — identity keys
- **X25519** — ephemeral key exchange
- **XChaCha20-Poly1305** — symmetric encryption
- **Per-pair forward secrecy** — separate keys per pair

**Tech stack**
- **Networking:** `pion/webrtc` (Go), full mesh, multiplexed data channel, heartbeat
- **Desktop UI:** Wails + React
- **Mobile:** Android (beta, from source)
- **Storage:** SQLite (local vault)
- **Signaling:** default endpoint `wss://signaling.1pro.uz/ws` (or your own)

**Platforms**
macOS (Apple Silicon and Intel) · Windows 10/11 (64-bit) · Linux (Ubuntu 22.04+) · Android (beta)

**Status:** **v0.5.x live release** · 8 phases done · code signing in progress · MIT licensed · open source

```bash
# 1. clone the repo
git clone https://github.com/Yaxyobek0877/portal_traffic.git
cd portal_traffic/client

# 2. create a portal (terminal 1)
go run ./cmd/portal-cli -mode create -nick alice

# 3. join with the code (another terminal)
go run ./cmd/portal-cli -mode join -nick bob \
    -portal <ID> -code <CODE>
```

---

### Enif — Uzbek AI assistant

<p>
  <a href="https://enif.uz/about">
    <img src="https://img.shields.io/badge/Site-enif.uz%2Fabout-00ADD8?style=for-the-badge&logo=googlechrome&logoColor=white" alt="enif.uz/about" />
  </a>
  <a href="https://t.me/enif_ai_bot">
    <img src="https://img.shields.io/badge/Telegram-@enif__ai__bot-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram bot" />
  </a>
  <img src="https://img.shields.io/badge/Platforms-Web%20%C2%B7%20iOS%20%C2%B7%20Android-success?style=for-the-badge&labelColor=0d1117" alt="Platforms" />
</p>

**Site:** [enif.uz/about](https://enif.uz/about) &nbsp;·&nbsp; **Telegram:** [@enif_ai_bot](https://t.me/enif_ai_bot) &nbsp;·&nbsp; **My role:** Backend & AI integration

**Enif** is a **multi-purpose AI assistant for the Uzbek language**. Chat, code generation, document analysis, voice interaction, test creation, image analysis and web search — all on a single platform. Available on Web, iOS, Android and as a Telegram bot.

**Key features**
- **Chat** — text answers to any question
- **Code & project building** — generate and directly publish React, Node.js, Python, FastAPI projects
- **Document analysis** — read and summarize PDF, DOCX, TXT files
- **Voice interaction** — TTS / STT, speak your question and get a spoken answer
- **Test creation and solving** — auto-generate topic-based quizzes
- **Image analysis (vision)** — multimodal, ask questions about an image
- **Web search** — pull the latest information from the internet
- **Telegram bot** — quick access via [@enif_ai_bot](https://t.me/enif_ai_bot)

**Special integrations**
- **HEMIS** — works with university data for students
- **Custom AI API key** — for companies

**Supported languages**
O'zbekcha · Русский · English · Čeština

**Pricing**

| Tier | Price | Workspace actions |
|---|---|---|
| **Free** | free | 3 / day |
| **Pro** | 30,000 UZS / 30 days | 10 / day |
| **Ultra** | 100,000 UZS / 30 days | 30 / day |

**Status:** **live release** · Web + iOS + Android + Telegram bot · 4 languages

---

## What I'm learning now

- **Training and shipping models** — training, fine-tuning, evaluating and shipping ML and LLM models on real datasets
- **Centralizing whole systems** — merging separate services into one unified platform, managing data flow from a single hub
- **Digitizing processes** — moving paper-based and manual business processes onto fully automated digital systems
- **MLOps & data pipelines** — data collection, cleaning, model versioning and monitoring
- **AI agents** — tool use, function calling, multi-step reasoning and RAG architectures

---

## 2026 plans

- [ ] Move several services in the 1Pro ecosystem to microservices
- [ ] Release an open-source Go library
- [ ] Start a technical blog (Go, PostgreSQL, AI)
- [ ] Mentor junior developers
- [ ] Write a case study on performance optimization

---

## Contact

<p align="center">
  <a href="https://t.me/adhamov_yaxyobek">
    <img src="https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white" />
  </a>
  <a href="mailto:yaxyobek877@gmail.com">
    <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" />
  </a>
  <a href="https://github.com/Yaxyobek0877">
    <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" />
  </a>
  <a href="http://1pro.uz/">
    <img src="https://img.shields.io/badge/1Pro-00ADD8?style=for-the-badge&logo=googlechrome&logoColor=white" />
  </a>
</p>

---

<p align="center">
  <i>"Ideas can't be invented on demand — they take shape gradually."</i>
</p>

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=120&section=footer&animation=twinkling" />
</p>
