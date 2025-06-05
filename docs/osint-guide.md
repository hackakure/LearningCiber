# 🔍 OSINT Guide - Intelligence Gathering Masterclass

> **"La información es poder, pero saber dónde encontrarla es sabiduría"**

## 🎯 Filosofía OSINT Hackakure

**OSINT (Open Source Intelligence)** bajo filosofía Hackakure combina **precisión técnica** con **ética inquebrantable**. Recopilamos intelligence para **proteger**, nunca para **dañar**.

*"El verdadero ninja digital no deja rastro mientras descubre todos los rastros."*

---

## 📚 Fundamentos OSINT

### 🔑 Principios Core

#### 1. **Metodología Sistemática**
- **Planificación**: Define objetivos claros
- **Recopilación**: Fuentes diversificadas
- **Análisis**: Correlación y verificación
- **Disseminación**: Reporting profesional

#### 2. **Ética Inquebrantable**
- **Legalidad**: Solo fuentes públicas
- **Proporcionalidad**: Mínimo necesario
- **Confidencialidad**: Protección de datos sensibles
- **Responsabilidad**: Uso ético de la información

#### 3. **Seguridad Operacional (OPSEC)**
- **Anonimización**: VPN + Tor cuando necesario
- **Compartimentalización**: Separar investigaciones
- **Attribution avoidance**: No dejar rastros
- **Data security**: Cifrado y almacenamiento seguro

---

## 🛠️ Arsenal OSINT Hackakure

### 🌐 Reconnaissance General

#### **Domain Intelligence**
```bash
# Subdomain enumeration
amass enum -d target.com
subfinder -d target.com
assetfinder target.com

# DNS analysis
dig +short target.com
dnsrecon -d target.com
fierce --domain target.com
```

#### **Network Intelligence**
```bash
# Shodan searches
shodan search "hostname:target.com"
shodan search "org:Target Company"

# Certificate transparency
crt.sh query
censys.io searches
```

### 👤 People Intelligence (HUMINT)

#### **Social Networks**
- **LinkedIn**: Professional profiles y connections
- **Twitter**: Real-time intelligence y sentiment
- **Facebook**: Personal information y relationships
- **Instagram**: Geolocation y lifestyle patterns
- **GitHub**: Technical skills y code repositories

#### **Professional Platforms**
- **Crunchbase**: Company intelligence
- **AngelList**: Startup ecosystem
- **Glassdoor**: Internal company culture
- **Stack Overflow**: Technical community

#### **Specialized Tools**
```bash
# Social media intelligence
sherlock username  # Username enumeration
socialscan username email  # Account discovery
holehe email@target.com  # Email service check

# Email intelligence
theHarvester -d target.com -b all
hunter.io API queries
breach databases (legal sources only)
```

### 🌍 Geospatial Intelligence (GEOINT)

#### **Imagery Analysis**
- **Google Earth**: Historical imagery comparison
- **Bing Maps**: Different perspective angles
- **Yandex Maps**: Enhanced Eastern European coverage
- **Satellite imagery**: Commercial providers

#### **Metadata Extraction**
```bash
# Image metadata
exiftool image.jpg
foca document_analysis.pdf

# Geolocation tools
geoSpy image_location
PlaNet neural networks
```

### 📱 Technical Intelligence (TECHINT)

#### **Mobile Intelligence**
```bash
# Phone number intelligence
truecaller API
numverify validation
phoneinfoga +1234567890

# Mobile app analysis
MARA framework
APK analysis tools
```

#### **Infrastructure Analysis**
```bash
# Web technology stack
builtwith.com analysis
wappalyzer browser extension
whatweb target.com

# Historical analysis
wayback machine queries
archive.today snapshots
```

---

## 🎯 Metodologías Avanzadas

### 🔄 OSINT Cycle Hackakure

#### **Phase 1: Requirements (要求)**
```
┌─ Intelligence Requirements ─┐
│ • What information needed?  │
│ • Why is it needed?         │
│ • When is it needed by?     │
│ • How will it be used?      │
└─────────────────────────────┘
```

#### **Phase 2: Collection (収集)**
```
┌─ Source Diversification ────┐
│ • Primary sources          │
│ • Secondary sources        │
│ • Cross-reference sources  │
│ • Validation sources       │
└─────────────────────────────┘
```

#### **Phase 3: Processing (処理)**
```
┌─ Data Processing ───────────┐
│ • Data normalization       │
│ • Correlation analysis     │
│ • Pattern recognition      │
│ • Timeline construction    │
└─────────────────────────────┘
```

#### **Phase 4: Analysis (分析)**
```
┌─ Intelligence Analysis ─────┐
│ • Hypothesis testing       │
│ • Confidence assessment    │
│ • Gap identification       │
│ • Risk evaluation          │
└─────────────────────────────┘
```

#### **Phase 5: Dissemination (普及)**
```
┌─ Intelligence Delivery ─────┐
│ • Executive summary        │
│ • Detailed findings        │
│ • Actionable recommendations│
│ • Follow-up requirements    │
└─────────────────────────────┘
```

### 🥷 Advanced Techniques

#### **Passive Reconnaissance Matrix**
| Target Type | Primary Sources | Secondary Sources | Validation |
|-------------|----------------|-------------------|------------|
| **Domain** | DNS, Certificates | Archive, WHOIS | Multiple DNS |
| **Email** | Search engines | Breach databases | Email validation |
| **Person** | Social media | Professional sites | Cross-platform |
| **Company** | Official sites | News, filings | Financial data |
| **IP Range** | Shodan, Censys | BGP data | Network scanning |

#### **Temporal Analysis**
```bash
# Timeline construction
wayback_machine_downloader target.com
photon -u target.com --wayback

# Change detection
visualping.io monitoring
distill.io page monitoring
```

---

## 🔧 Herramientas por Categoría

### 🌟 Essential Toolkit

#### **Multi-Source Frameworks**
- **[Maltego](https://www.maltego.com/)** - Visual link analysis platform
- **[SpiderFoot](https://spiderfoot.net/)** - Automated OSINT collection
- **[OSINT Framework](https://osintframework.com/)** - Resource directory
- **[Recon-ng](https://github.com/lanmaster53/recon-ng)** - Modular reconnaissance

#### **Specialized Tools**
```bash
# Domain/Subdomain
amass, subfinder, assetfinder, knockpy

# Social Media
sherlock, socialscan, twint, instalooter

# Email/Phone
theHarvester, hunter.io, phoneinfoga, numverify

# Images/Documents
exiftool, foca, ghiro, reveye

# Dark Web
OnionScan, tor-crawler, ahmia.fi
```

### 🎨 Custom Scripts & Automation

#### **Python OSINT Automation**
```python
#!/usr/bin/env python3
"""
Hackakure OSINT Automation Framework
Ethical reconnaissance with integrated OPSEC
"""

import requests
import json
from bs4 import BeautifulSoup
import subprocess

class HackakureOSINT:
    def __init__(self, target):
        self.target = target
        self.results = {}
        
    def subdomain_enum(self):
        """Automated subdomain enumeration"""
        tools = ['amass', 'subfinder', 'assetfinder']
        # Implementation with error handling
        
    def social_footprint(self):
        """Social media footprint analysis"""
        # Sherlock integration
        # Cross-platform correlation
        
    def breach_check(self):
        """Ethical breach database checking"""
        # HaveIBeenPwned API integration
        # Legal compliance checks
```

---

## 📊 OSINT Labs & Practice

### 🎯 Beginner Challenges

#### **Lab 1: Basic Domain Intelligence**
```
Target: hackakure.com
Tasks:
1. Enumerate subdomains
2. Identify web technologies
3. Map network infrastructure
4. Timeline historical changes
5. Report findings professionally
```

#### **Lab 2: Social Engineering Prep**
```
Target: Fictional company "CyberCorp"
Tasks:
1. Employee enumeration via LinkedIn
2. Technology stack identification
3. Physical location mapping
4. Communication channels analysis
5. Attack surface summary
```

### ⚡ Intermediate Challenges

#### **Lab 3: APT-style Reconnaissance**
```
Scenario: Nation-state level intelligence gathering
Target: Government contractor
Tasks:
1. Multi-source intelligence fusion
2. Supply chain analysis
3. Personnel background checks
4. Infrastructure correlation
5. Threat modeling
```

### 🔥 Advanced Scenarios

#### **Lab 4: Real-world Investigation**
```
Scenario: Incident response support
Context: Suspected data breach
Tasks:
1. Threat actor attribution
2. TTP (Tactics, Techniques, Procedures) analysis
3. Infrastructure overlap detection
4. Campaign timeline reconstruction
5. Predictive intelligence
```

---

## 🛡️ OPSEC para OSINT

### 🔒 Operational Security

#### **Network Anonymization**
```bash
# VPN + Tor setup
openvpn --config provider.ovpn
systemctl start tor
proxychains firefox

# DNS over HTTPS
cloudflared proxy-dns

# Burner infrastructure
Digital Ocean droplets
AWS temporary instances
```

#### **Identity Compartmentalization**
- **Separate browser profiles** for different investigations
- **Disposable email addresses** via ProtonMail, Guerrilla Mail
- **Temporary phone numbers** for verification
- **Virtual machines** for isolation

#### **Data Protection**
```bash
# Encrypted storage
cryptsetup luksFormat /dev/sdX
veracrypt containers

# Secure communication
Signal for team coordination
ProtonMail for external communication
```

---

## 📈 Professional OSINT Reporting

### 📋 Report Structure Hackakure

#### **Executive Summary**
- **Scope** and **objectives**
- **Key findings** summary
- **Risk assessment** overview
- **Recommendations** prioritized

#### **Technical Findings**
- **Methodology** detailed
- **Sources** cited with confidence levels
- **Evidence** with timestamps and provenance
- **Analysis** with supporting data

#### **Actionable Intelligence**
- **Immediate actions** required
- **Long-term recommendations**
- **Monitoring** suggestions
- **Follow-up** intelligence requirements

### 🎨 Visualization Techniques

#### **Maltego Graphs**
- **Entity relationships** mapping
- **Timeline visualizations**
- **Geospatial correlations**
- **Network topologies**

#### **Custom Dashboards**
```python
# Intelligence dashboard with Plotly
import plotly.graph_objects as go
import plotly.express as px

# Geographic distribution
# Timeline analysis
# Risk heat maps
# Correlation matrices
```

---

## 🌟 Advanced OSINT Specializations

### 🕸️ Dark Web Intelligence
- **Tor hidden services** enumeration
- **Criminal marketplace** monitoring (legal/ethical only)
- **Leak site** tracking
- **Attribution** analysis

### 📱 Mobile Intelligence
- **App store** intelligence
- **Mobile device** fingerprinting
- **Location** tracking analysis
- **Communication app** intelligence

### 🏢 Corporate Intelligence
- **Financial intelligence** gathering
- **Supply chain** analysis
- **Executive** background research
- **Competitive intelligence**

### 🌍 Geopolitical Intelligence
- **Nation-state** activity monitoring
- **Critical infrastructure** analysis
- **Disinformation** campaign detection
- **Influence operation** tracking

---

## 📚 Recursos de Aprendizaje

### 📖 Libros Esenciales
- **"Open Source Intelligence Techniques"** - Michael Bazzell
- **"OSINT Techniques: Resources for Uncovering Online Information"** - Ric Messier
- **"Social Media Intelligence"** - Wendy Walker

### 🎓 Cursos Especializados
- **[SANS SEC487](https://www.sans.org/cyber-security-courses/open-source-intelligence-gathering/)** - Open Source Intelligence Gathering
- **[Bellingcat's Online Investigation Toolkit](https://www.bellingcat.com/resources/how-tos/)**
- **[Intelligence Studies on Coursera](https://www.coursera.org/specializations/intelligence)**

### 🏆 Certificaciones OSINT
- **GIAC Open Source Intelligence (GOSI)**
- **Certified OSINT Professional (COP)**
- **OSINT Curious Training**

---

## 🤝 Comunidad OSINT

### 🌐 Comunidades Online
- **[OSINT Curious](https://osintcurio.us/)** - Community y resources
- **[Bellingcat](https://www.bellingcat.com/)** - Investigative journalism
- **[Reddit r/OSINT](https://www.reddit.com/r/OSINT/)**

### 🎪 Eventos y CTFs
- **TraceLabs** - Missing person CTFs
- **OSINT Summit** - Annual conference
- **BSides OSINT** tracks

---

**🥷 Hackakure OSINT Mastery**: *"El verdadero maestro OSINT ve lo invisible, conecta lo desconectado, y protege mientras descubre."*

**🔍 Próximo paso**: Aplica estos conocimientos en [🏆 CTF Labs](ctf-labs.md) para scenarios prácticos.