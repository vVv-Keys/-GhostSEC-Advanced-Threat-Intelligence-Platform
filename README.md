<p align="center">
  <img src="https://github.com/vVv-Keys/GhostSEC-Advanced-Threat-Intelligence-Platform/blob/main/ghostbanner.png" alt="GhostSEC Banner" width="100%" height="50%" />
</p>

# 👻 GhostSEC - Advanced Threat Intelligence Platform

GhostSEC is an enterprise-ready, AI-enhanced Threat Intelligence Platform (TIP) designed for real-time IOC ingestion, ML-based prioritization, campaign detection, and threat visualization — all integrated with Discord, MISP, and your enterprise SIEMs.

## 🔥 Key Features

### 🛰️ Multi-Source Threat Ingestion

* Ingests live CTI from 15+ open sources (ThreatFox, URLhaus, SANS ISC, CIRCL, etc.)
* Real-time honeypot integration via Cowrie, Dionaea, DShield, and generic sensor webhook support

### 🧠 ML Threat Prioritization

* Random Forest model scoring IOC severity using enriched feature sets
* Confidence-based deduplication and alert filtering

### 🧬 Campaign Detection

* IOC correlation via shared infrastructure, malware family, ASN clustering
* Named campaigns tracked over time with evolution snapshots

### 📊 Interactive Dashboard

* Dash/Plotly UI with:

  * Global threat heatmaps
  * Campaign tracking views
  * IOC database with TTL, filters, tags
  * Export center (PDF, CSV, STIX, MISP, YARA)

### 🤖 Discord Bot (GhostSEC Bot)

* 15+ commands (`!ghost help`, `!ghost status`, `!ghost update`, etc.)
* Role-protected command execution
* Live threat alerts, bot uptime, and feed sync

### 📤 Enterprise Integration

* Custom webhook routing to: Splunk, QRadar, Sentinel, Teams, Slack, SMS
* Export format support: STIX 2.1, TAXII 2.0, MISP JSON, CSV, PDF, YARA

---

## 📦 Installation

```bash
git clone https://github.com/your-org/ghostsec.git
cd ghostsec
pip install -r requirements.txt
```

Create a `.env` file based on `.env.example` and configure:

```env
DISCORD_TOKEN=your_discord_bot_token
CHANNEL_ID=123456789
THREATFOX_URL=https://threatfox.abuse.ch/api/
```

---

## 🚀 Running

### Launch the bot:

```bash
python start_ghostsec.py
```

### Launch the dashboard:

```bash
python start_dashboard.py
```

Visit: [http://localhost:5000](http://localhost:5000)

---

## 📚 Documentation

* `SETUP_GUIDE.md` - Full system setup
* `DISCORD_SETUP.md` - Discord permissions and roles
* `enterprise_setup.md` - SIEM/webhook integrations
* `API_GUIDE.md` - Feed structure, ML scoring pipeline

---

## 🧪 Example Commands

```bash
!ghost help
!ghost update
!ghost status
!ghost test critical
!ghost sources
```

---


---

## 💀 Credits

Built by GhostSec Labs. For defenders, red teams, and cyber intel professionals.
