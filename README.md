<p align="center">
  <b>O'zbekcha</b> · <a href="README.en.md">English</a> · <a href="README.ru.md">Русский</a>
</p>

<h1 align="center">
  <a href="https://github.com/Yaxyobek0877">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=28&duration=3000&pause=1000&color=00ADD8&center=true&vCenter=true&width=760&lines=Salom%2C+men+TexUz!;Backend+%26+Full-Stack+Developer;AI+Engineer+%2F+LLM+integratsiya;Python+%7C+Go+%7C+PostgreSQL;Qo%CA%BBqondan+salom%21" alt="Typing SVG" />
  </a>
</h1>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=Yaxyobek0877&label=Profil%20ko%27rishlar&color=00ADD8&style=for-the-badge" alt="Profile views" />
  <a href="https://github.com/Yaxyobek0877?tab=followers">
    <img src="https://img.shields.io/github/followers/Yaxyobek0877?label=Followers&style=for-the-badge&color=00ADD8&labelColor=0d1117" alt="GitHub followers" />
  </a>
  <img src="https://img.shields.io/badge/Focus-Backend%20%26%20AI-success?style=for-the-badge&labelColor=0d1117" alt="Focus" />
</p>

---

## Men haqimda

```yaml
ism:           TexUz
rol:           Backend / AI muhandis / jamoa rahbari
joylashuv:     Qo'qon, O'zbekiston
loyihalar:     [1Pro (AI Gateway), Gazer Max (aqlli kampus), Portal (P2P mesh), Enif]
open_source:   [github.com/Yaxyobek0877/portal_traffic]
texnologiyalar: [Django, FastAPI, PostgreSQL, pgvector, Redis, Docker, Cloudflare]
ai_stack:      [InsightFace, CUDA, LLM API, RAG, Vector search]
tarmoq:        [WebRTC, pion/webrtc, PCP-1 (Ed25519/X25519/XChaCha20)]
hozir_o'rgan:  [Model fine-tuning, Tizim markazlashtirish, MLOps]
shior:         "G'oyalarni o'ylab topib bo'lmaydi, ular asta-sekin shakllanadi."
```

- Hozir **1Pro AI Inference Gateway** (LLM API platforma), **Gazer Max** (yuz tanish asosidagi aqlli kampus) va **Portal** (P2P mesh tarmoq desktop dasturi, ochiq kodli) ustida ishlayapman; **Enif** ham mening loyihalarimdan biri.
- **AI muhandisligi**: LLM API'lar, **RAG**, **vector qidiruv** (`pgvector` HNSW), **yuz embedding** (`InsightFace` + CUDA) va **agentlar**.
- **Tarmoq va P2P**: WebRTC + `pion/webrtc`, NAT-traversal, mesh topologiya, **PCP-1** shifrlash (Ed25519 + X25519 + XChaCha20-Poly1305).
- **Backend va infra**: PostgreSQL optimallashtirish, real-time (WebSocket, mediamtx), **Hikvision ISAPI**, **Cloudflare Tunnel**, Docker.
- Bog'lanish: **yaxyobek877@gmail.com** yoki [Telegram](https://t.me/adhamov_yaxyobek) orqali.

---

## Asosiy loyihalarim

### 1Pro — AI Inference Gateway

<p>
  <a href="http://1pro.uz/">
    <img src="https://img.shields.io/badge/Sayt-1pro.uz-00ADD8?style=for-the-badge&logo=googlechrome&logoColor=white" alt="1pro.uz" />
  </a>
  <a href="https://1pro.uz/dashboard">
    <img src="https://img.shields.io/badge/Dashboard-1pro.uz%2Fdashboard-412991?style=for-the-badge&logo=vercel&logoColor=white" alt="Dashboard" />
  </a>
</p>

**Sayt:** [1pro.uz](http://1pro.uz/) &nbsp;·&nbsp; **Tur:** AI Inference Gateway &nbsp;·&nbsp; **Rolim:** Backend va AI integratsiya

**1Pro** — bu **kuchli sun'iy intellekt modellariga yagona API** orqali sodda kirish imkonini beruvchi platforma. Startaplar va dasturchilar uchun: ro'yxatdan o'tib, bepul foydalanishni boshlab, chat yoki API orqali darhol ishga tushirish mumkin.

**Asosiy g'oya**
> Biz infratuzilma murakkabligini o'z zimmamizga olamiz —
> shunda sizning startapingiz to'liq AI funksiyalarini yaratishga e'tibor qaratishi mumkin.

**Imkoniyatlar**
- **Yagona interfeys** — bitta API kaliti, bitta endpoint formati. 70B klassdagi modellardan tez foydalanish.
- **Bepul boshlash** — yangi foydalanuvchilar uchun bepul kvota. Dashboard orqali token sarfi, limitlar va umumiy foydalanishni aniq kuzating.
- **Korporativ xavfsizlik** — model darajasidagi qat'iy ruxsatnomalar. Ishlab chiqish, sinov va asosiy (production) kalitlar bir-biridan ajratilgan.
- **OpenAI-mos API** — standart `chat/completions` formati, mavjud SDK'lar ishlaydi.

**API misoli** (Python, Node.js va cURL'da qo'llab-quvvatlanadi)

```python
import requests

api_key = "sk-[Sizning-Kalitingiz]"
url = "https://1pro.uz/v1/chat/completions"

headers = {
    "Authorization": f"Bearer {api_key}",
    "Content-Type": "application/json"
}
data = {
    "model": "coder",
    "messages": [{"role": "user", "content": "Salom!"}]
}

response = requests.post(url, headers=headers, json=data)
print(response.json())
```

---

### Gazer Max — aqlli kampus tizimi

<p>
  <a href="https://gazer.1pro.uz/presentation.html">
    <img src="https://img.shields.io/badge/Prezentatsiya-gazer.1pro.uz%2Fpresentation.html-00ADD8?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Gazer Max prezentatsiya" />
  </a>
  <img src="https://img.shields.io/badge/%231-Aqlli%20kampus-success?style=for-the-badge&labelColor=0d1117" alt="#1 aqlli kampus" />
</p>

**Prezentatsiya:** [gazer.1pro.uz/presentation.html](https://gazer.1pro.uz/presentation.html) &nbsp;·&nbsp; **Tur:** Yuz tanish va aqlli kampus platformasi &nbsp;·&nbsp; **Rolim:** Backend / AI / jamoa rahbari

**Gazer Max** — universitet, maktab va tashkilotlar uchun **yagona AI platforma**. Yuz tanish, avtomatik davomat, turniket va kameralarni boshqarish, real-vaqt xavfsizlik — hammasi bitta tizimda. O'zbekistonda **20 000+ talabaga sinovdan o'tgan**.

**Tagline**
> Yuzni biroz ko'rsang — yetarli. Qolganini AI bajaradi.

**Real ko'rsatkichlar (universitet sinovi)**

| Ko'rsatkich | Qiymat |
|---|---|
| Faol talaba bazasi | **20 000+** |
| IP kameralar | **40+** |
| Turniketlar | **30+** |
| Yuz qidiruv vaqti | **< 10 ms** |
| Tanish aniqligi | **99.6%** |
| O'rnatish vaqti | **1 hafta** |
| Eshik ochilish | **~50 ms** |

**Modullar (12 ta, mustaqil ishlatish mumkin)**
- **Yuz tanish (AI)** — 512-o'lchovli embedding, pgvector HNSW indeks
- **Avtomatik davomat** — `on_time` / `late` / `absent` / `left_early` holatlari
- **Real-vaqt monitor** — 40+ kamera bitta ekranda, har frame'da AI tahlili
- **Turniket boshqaruvi** — Hikvision (DS-K1T341CMF) ISAPI orqali, offline'da ham
- **Bino va xona xaritasi** — Building / Floor / Classroom hierarchy
- **Yuz orqali qidiruv** — bitta rasm yuklang, to'liq tarix chiqadi (reverse search)
- **HEMIS sinxronizatsiyasi** — talaba/fakultet/guruh avtomatik
- **Dars jadvali** — davomat avtomatik shu jadval asosida
- **Hisobot va analitika** — live dashboard, Excel/PDF eksport
- **Granular kirish nazorati** — har foydalanuvchiga aniq kameralar/binolar/xonalar
- **Live audit jurnal** — har bir kirish, admin amali, urinish
- **Ochiq REST API** — Swagger, API key scope (read/write/full)

**Texnik stack**
- **AI:** InsightFace (buffalo_l) + NVIDIA CUDA — yuz embedding
- **Vector DB:** PostgreSQL + **pgvector HNSW** indeks
- **Backend:** Django 5 + Celery + Redis
- **Frontend:** React 19
- **Media:** mediamtx (HLS & WebRTC, 25 fps)
- **Qurilmalar:** Hikvision IP kameralar va turniketlar (ISAPI)
- **Infra:** Docker, **Cloudflare Tunnel** (outbound-only — server hech qanday port ochmaydi)
- **Real-time:** WebSocket

**7 qatlamli xavfsizlik**
1. Cloudflare Edge (WAF, DDoS, bot, GeoIP)
2. Cloudflare Access (2FA admin panel uchun)
3. nginx + TLS 1.3
4. Django + Argon2id (brute-force lock, CSRF, CSP)
5. Ma'lumotlar bazasi shifrlangan (Fernet AES-256)
6. JWT (15-daqiqalik token) + API kalitlar scope bilan
7. To'liq audit jurnal

**Foydalanuvchilar**
Universitetlar · maktablar va litseylar · korxonalar va ofislar · tibbiy muassasalar · davlat idoralari · zavod va omborlar

**Natijalar (1 oydan keyin)**
- −92% davomat vaqti (30 daqiqa → 0)
- +45% davomat aniqligi
- −68% xavfsizlik insidentlari
- 0 so'm ID-karta xarajati

---

### Portal — P2P mesh tarmoq dasturi (open-source)

<p>
  <a href="https://portal.1pro.uz/">
    <img src="https://img.shields.io/badge/Sayt-portal.1pro.uz-00ADD8?style=for-the-badge&logo=googlechrome&logoColor=white" alt="portal.1pro.uz" />
  </a>
  <a href="https://github.com/Yaxyobek0877/portal_traffic">
    <img src="https://img.shields.io/badge/GitHub-portal__traffic-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub repo" />
  </a>
  <a href="https://github.com/Yaxyobek0877/portal_traffic/releases/latest">
    <img src="https://img.shields.io/github/v/release/Yaxyobek0877/portal_traffic?style=for-the-badge&label=Reliz&color=00ADD8&labelColor=0d1117" alt="Latest release" />
  </a>
  <img src="https://img.shields.io/badge/Litsenziya-MIT-success?style=for-the-badge&labelColor=0d1117" alt="MIT license" />
</p>

**Sayt:** [portal.1pro.uz](https://portal.1pro.uz/) &nbsp;·&nbsp; **Kod:** [github.com/Yaxyobek0877/portal_traffic](https://github.com/Yaxyobek0877/portal_traffic) &nbsp;·&nbsp; **Rolim:** Muallif va asosiy ishlab chiquvchi

**Portal** — qurilmalar o'rtasida xususiy **peer-to-peer mesh tarmoq** quradigan desktop dastur. To'g'ridan-to'g'ri ulanish: orada hech qanday server yo'q (signaling server faqat handshake'da ishtirok etadi). Mahalliy hisob, bir nechta xona bir vaqtda, avtomatik qayta ulanish. Chat, fayl, kamera/NVR/o'yin serveri uchun port tunneli — hammasi P2P.

**Tagline**
> Server o'rtada yo'q. To'g'ridan-to'g'ri ulanish.

**Asosiy imkoniyatlar**
- **2 dan 16 qurilmagacha** mesh tarmoq — Portal ID + kod bilan ulashish (router/VPN/port forwarding kerak emas)
- **Chat va fayl uzatish** — drag-and-drop, uchidan-uchiga shifrlangan
- **TCP/UDP tunnel** — Minecraft serveri, Hikvision NVR, LAN kameralar va boshqa servislarni mesh orqali ulashish
- **Jonli mesh diagrammasi** — RTT, NAT-traversal indikatorlari (LAN / Internet / TURN), bandwidth probe
- **QR + portal kod** — yonidagi do'stga QR, masofadagiga ID + kod
- **Mahalliy hisob** — bcrypt parol, email yoki markaziy ro'yxatdan o'tish yo'q
- **Multi-portal** — oilaviy + ishxona + o'yin xonalari parallel
- **Avtomatik qayta ulanish** — tizim qayta yuklanganda oldingi sessiyalar tiklanadi
- **Per-service approval** — har bir ulanishni alohida tasdiqlash

**Shifrlash: PCP-1 protokoli**
WebRTC DTLS ostida ikkinchi qatlam shifrlash:
- **Ed25519** — identity kalitlar
- **X25519** — ephemeral key exchange
- **XChaCha20-Poly1305** — symmetric shifrlash
- **Per-pair forward secrecy** — har juftlik uchun alohida kalitlar

**Texnik stack**
- **Tarmoq:** `pion/webrtc` (Go), full mesh, multipleks data channel, heartbeat
- **Desktop UI:** Wails + React
- **Mobile:** Android (beta, manbadan)
- **Saqlash:** SQLite (mahalliy vault)
- **Signaling:** standart endpoint `wss://signaling.1pro.uz/ws` (yoki o'zingizniki)

**Platformalar**
macOS (Apple Silicon va Intel) · Windows 10/11 (64-bit) · Linux (Ubuntu 22.04+) · Android (beta)

**Holat:** **v0.5.x jonli reliz** · 8 ta bosqich tugadi · code signing jarayonda · MIT litsenziyali · ochiq kodli

```bash
# 1. reponi klonlang
git clone https://github.com/Yaxyobek0877/portal_traffic.git
cd portal_traffic/client

# 2. portal yarating (1-terminal)
go run ./cmd/portal-cli -mode create -nick alice

# 3. kodni boshqa terminalda joylang
go run ./cmd/portal-cli -mode join -nick bob \
    -portal <ID> -code <KOD>
```

---

### Enif — O'zbek AI yordamchi

<p>
  <a href="https://enif.uz/about">
    <img src="https://img.shields.io/badge/Sayt-enif.uz%2Fabout-00ADD8?style=for-the-badge&logo=googlechrome&logoColor=white" alt="enif.uz/about" />
  </a>
  <a href="https://t.me/enif_ai_bot">
    <img src="https://img.shields.io/badge/Telegram-@enif__ai__bot-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram bot" />
  </a>
  <img src="https://img.shields.io/badge/Platformalar-Web%20%C2%B7%20iOS%20%C2%B7%20Android-success?style=for-the-badge&labelColor=0d1117" alt="Platformalar" />
</p>

**Sayt:** [enif.uz/about](https://enif.uz/about) &nbsp;·&nbsp; **Telegram:** [@enif_ai_bot](https://t.me/enif_ai_bot) &nbsp;·&nbsp; **Rolim:** Backend va AI integratsiya

**Enif** — O'zbek tilidagi **ko'p qirrali sun'iy intellekt yordamchisi**. Chat, kod yozish, hujjat tahlili, ovozli muloqot, test yaratish, rasm tahlili va web qidiruv — hammasi bitta platformada. Web, iOS, Android hamda Telegram bot orqali ishlaydi.

**Asosiy imkoniyatlar**
- **Chat** — har qanday savolga matnli javob
- **Kod yozish va loyiha qurish** — React, Node.js, Python, FastAPI loyihalarini yaratish va to'g'ridan-to'g'ri publish qilish
- **Hujjat tahlili** — PDF, DOCX, TXT fayllarni o'qish va xulosalash
- **Ovozli muloqot** — TTS / STT, gapirib so'rang va ovozli javob oling
- **Test yaratish va yechish** — mavzu bo'yicha avtomatik test tuzish
- **Rasm tahlili (vision)** — multimodal, rasm haqida savol berish
- **Web qidiruv** — internetdan eng yangi ma'lumotlarni topish
- **Telegram bot** — [@enif_ai_bot](https://t.me/enif_ai_bot) orqali tezkor kirish

**Maxsus integratsiyalar**
- **HEMIS** — talabalar uchun universitet ma'lumotlari bilan ishlash
- **Custom AI API kalit** — kompaniyalar uchun

**Til qo'llab-quvvatlash**
O'zbekcha · Русский · English · Čeština

**Tariflar**

| Tarif | Narx | Workspace amali |
|---|---|---|
| **Free** | bepul | 3 / kun |
| **Pro** | 30 000 so'm / 30 kun | 10 / kun |
| **Ultra** | 100 000 so'm / 30 kun | 30 / kun |

**Holat:** **jonli reliz** · Web + iOS + Android + Telegram bot · 4 ta til

---

## Bog'lanish

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
  <i>"G'oyalarni o'ylab topib bo'lmaydi, ular asta-sekin shakllanadi."</i>
</p>

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=120&section=footer&animation=twinkling" />
</p>
