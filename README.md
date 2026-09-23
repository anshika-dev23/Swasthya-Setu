<div align="center">

<img src="assets/swasthya-setu-hero.svg"
     width="100%"
     alt="SwasthyaSetu - Smart Voice-First Rural Healthcare Platform">

<br>

<a href="#-the-problem">
<img src="https://img.shields.io/badge/PROBLEM-0B1F2A?style=for-the-badge&logoColor=white">
</a>

<a href="#-the-solution">
<img src="https://img.shields.io/badge/SOLUTION-00C878?style=for-the-badge&logoColor=white">
</a>

<a href="#-how-it-works">
<img src="https://img.shields.io/badge/WORKFLOW-008CFF?style=for-the-badge&logoColor=white">
</a>

<a href="#-architecture">
<img src="https://img.shields.io/badge/ARCHITECTURE-7C3AED?style=for-the-badge&logoColor=white">
</a>

<a href="#-roadmap">
<img src="https://img.shields.io/badge/ROADMAP-F59E0B?style=for-the-badge&logoColor=white">
</a>

<br><br>

<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white">
<img src="https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white">
<img src="https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white">
<img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black">
<img src="https://img.shields.io/badge/AI-Assisted-7C3AED?style=flat-square">

</div>

<br>

---

<div align="center">

> **Healthcare communication should be accessible before it can be digital.**

</div>

<br>

# 🌾 About SwasthyaSetu

**SwasthyaSetu** is a **Smart Voice-First Rural Healthcare Platform** designed around one simple idea:

> **Let people communicate about their healthcare in a way that feels natural to them.**

The platform explores voice-first interaction for rural communities where typing, complicated interfaces, medical terminology, language differences, and unreliable connectivity can become barriers to digital healthcare.

Instead of making the patient adapt completely to the application, SwasthyaSetu aims to make the interaction **simpler, more accessible, and more human.**

---

# 🚨 The Problem

Rural healthcare access is not only about the physical availability of hospitals.

The **communication layer** itself can become a barrier.

### Common challenges include:

| Challenge | Impact |
|---|---|
| 🏥 Limited access to doctors | Difficult access to timely professional guidance |
| 🛣️ Long travel distances | Additional effort and cost |
| 📶 Unstable connectivity | Difficulty using continuously online systems |
| ⌨️ Typing dependency | Patients may struggle to describe symptoms |
| 📖 Low digital literacy | Complex interfaces can become difficult to navigate |
| 🗣️ Language differences | Formal language may not match everyday communication |
| 🎙️ Accent variations | Speech systems may need regional adaptation |
| 📋 Fragmented information | Patient history may become difficult to organize |
| 💊 Prescription complexity | Instructions may be misunderstood |
| ⏰ Missed follow-ups | Important healthcare interactions may be missed |

---

# 💡 The Solution

SwasthyaSetu introduces a **voice-first communication layer** between rural patients and healthcare professionals.

Instead of asking a user to navigate a long form:

```text
OPEN FORM
    ↓
TYPE INFORMATION
    ↓
SELECT OPTIONS
    ↓
SUBMIT
```

the interaction can move toward:

```text
PRESS 🎙️
    ↓
SPEAK NATURALLY
    ↓
UNDERSTAND
    ↓
STRUCTURE
    ↓
CONFIRM
    ↓
CONNECT
```

### Core principle

<div align="center">

## 🎙️ Listen → 🧠 Understand → 📋 Structure → 👨‍⚕️ Connect → 🔊 Respond

</div>

---

# 🧭 The User Journey

```mermaid
flowchart LR

P["👤 Patient"]

P --> V["🎙️ Speak Naturally"]

V --> S["📝 Speech-to-Text"]

S --> AI["🧠 AI / NLP"]

AI --> C{"Information<br/>Clear?"}

C -->|No| Q["❓ Ask for Confirmation"]

Q --> V

C -->|Yes| R["📋 Structured Record"]

R --> D["👨‍⚕️ Healthcare Professional"]

D --> G["💬 Healthcare Guidance"]

G --> L["🌐 Language Processing"]

L --> T["🔊 Text-to-Speech"]

T --> P
```

---

# 🎙️ Voice-Based Registration

Instead of filling a long registration form, the user can communicate naturally.

### Example

> **"Mera naam Ram Kumar hai, meri age 52 saal hai aur main Barabanki ke ek gaon mein rehta hoon."**

The system can process relevant information such as:

```text
Name
   ↓
Ram Kumar

Age
   ↓
52

Location
   ↓
Barabanki
```

The extracted information can then be shown to the user for confirmation before being stored.

### Design rule

> **When important information is uncertain, ask for confirmation instead of silently assuming.**

---

# 🩺 Voice-Based Health Complaint

A patient can describe their problem naturally.

### Example

> **"Mujhe teen din se bukhar hai aur raat mein bahut zyada thand lagti hai."**

The system can organize the information into a structured representation:

```yaml
complaint: fever

duration:
  value: 3
  unit: days

additional_information:
  - chills at night
```

The goal is to **improve communication and information organization**.

It is not intended to independently diagnose a patient.

---

# 🌐 Regional Language & Accent Awareness

Healthcare communication does not always happen in standardized language.

SwasthyaSetu is designed with future support for:

- Hindi
- Regional languages
- Local accents
- Mixed-language speech
- Everyday vocabulary
- Pronunciation variations

For example:

```text
Dawai
Dawa
Medicine
```

may represent the same general concept depending on context.

Similarly:

```text
Sugar
Shugar
Suggar
```

may represent speech variations that need contextual interpretation.

The important design principle is:

```text
Uncertain
   ↓
Ask
   ↓
Confirm
   ↓
Store
```

---

# 🧠 AI-Assisted Information Processing

AI is positioned as an **assistive layer**, helping transform natural communication into structured information.

```mermaid
flowchart LR

A["🎙️ Natural Speech"]
--> B["📝 Speech Recognition"]

B --> C["🧠 NLP"]

C --> D["🔎 Entity Extraction"]

D --> E["🎯 Intent Recognition"]

E --> F["📋 Structured Information"]

F --> G["👨‍⚕️ Human Review"]
```

### Potential information categories

- Patient details
- Symptoms
- Duration
- Basic health information
- Medicines
- Follow-up requirements
- Appointment information
- Vitals

---

# 👨‍⚕️ Human-in-the-Loop Healthcare

SwasthyaSetu is designed around a **human-in-the-loop approach**.

AI can assist with:

- Speech processing
- Information extraction
- Language processing
- Structuring patient-reported information

Healthcare professionals remain involved in healthcare decision-making.

```mermaid
flowchart LR

P["👤 Patient"]
--> AI["🧠 AI-Assisted Processing"]

AI --> H["👨‍⚕️ Healthcare Professional"]

H --> G["💬 Guidance"]

G --> T["🌐 Language Processing"]

T --> V["🔊 Voice Response"]

V --> P
```

---

# 🔊 Voice Response

The communication loop can work in both directions.

```text
PATIENT
   │
   │ speaks
   ▼
🎙️ VOICE
   │
   ▼
🧠 PROCESSING
   │
   ▼
👨‍⚕️ HEALTHCARE PROFESSIONAL
   │
   │ guidance
   ▼
🌐 LANGUAGE PROCESSING
   │
   ▼
🔊 VOICE RESPONSE
   │
   ▼
PATIENT
```

Potential use cases include communicating:

- Medicine instructions
- Dosage information
- Precautions
- Follow-up instructions
- Appointment information

---

# ❤️ Vitals & Health Timeline

The platform can organize basic patient information over time.

### Example

```text
┌──────────────────────────────────────┐
│          PATIENT HEALTH TIMELINE     │
├──────────────────────────────────────┤
│                                      │
│ 👤 Registration                      │
│       │                              │
│       ▼                              │
│ 🎙️ Health Complaint                  │
│       │                              │
│       ▼                              │
│ ❤️ Vitals                            │
│       │                              │
│       ▼                              │
│ 👨‍⚕️ Healthcare Review                 │
│       │                              │
│       ▼                              │
│ 💬 Guidance                          │
│       │                              │
│       ▼                              │
│ 🔁 Follow-up                         │
│                                      │
└──────────────────────────────────────┘
```

### Current prototype supports

- Patient registration
- Patient records
- Vitals recording
- Vitals storage
- Smart vitals status
- Basic health timeline

---

# 👩‍⚕️ Community Health Worker Layer

Community health workers can provide an important bridge for users who need assistance.

```mermaid
flowchart LR

P["🌾 Rural Patient"]
--> A["👩‍⚕️ ASHA / Community Worker"]

A --> S["🌐 SwasthyaSetu"]

S --> R["📋 Structured Information"]

R --> D["👨‍⚕️ Healthcare Professional"]

D --> G["💬 Guidance"]

G --> A

A --> P
```

Potential workflows include:

- Assisted registration
- Vitals recording
- Patient support
- Follow-up assistance
- Healthcare communication

---

# 📶 Offline-Resilient Vision

Connectivity can vary significantly across locations.

A future architecture can support local storage with synchronization when connectivity returns.

```mermaid
flowchart TD

A["📱 User Action"]
--> B{"Internet Available?"}

B -->|YES| C["☁️ Server"]

B -->|NO| D["📦 Local Storage"]

D --> E["⏳ Pending Sync"]

E --> F{"Connection Restored?"}

F -->|YES| C

F -->|NO| E

C --> G["🔄 Synchronize"]

G --> H["✅ Updated Record"]
```

---

# 🔐 Security & Privacy

Healthcare information is sensitive.

A production implementation would require appropriate security and privacy controls.

### Planned security considerations

| Layer | Approach |
|---|---|
| 🔐 Authentication | Secure user authentication |
| 👥 Authorization | Role-based access |
| 🛡️ Patient Records | Controlled access |
| 🔑 Credentials | Secure credential handling |
| 📜 Auditability | Activity logging |
| 🎙️ Voice Data | Responsible data handling |
| 🔒 Infrastructure | Secure deployment practices |

---

# 🏗️ System Architecture

```mermaid
flowchart TB

subgraph USERS["USER LAYER"]

P["👤 Patient"]
A["👩‍⚕️ ASHA Worker"]
D["👨‍⚕️ Healthcare Professional"]

end

subgraph INTERACTION["INTERACTION LAYER"]

UI["🌐 Web Interface"]
VOICE["🎙️ Voice Interface"]

end

subgraph INTELLIGENCE["INTELLIGENCE LAYER"]

STT["📝 Speech-to-Text"]
NLP["🧠 AI / NLP"]
TTS["🔊 Text-to-Speech"]

end

subgraph APPLICATION["APPLICATION LAYER"]

FLASK["⚙️ Flask Backend"]
AUTH["🔐 Authentication"]
LOGIC["🔗 Application Logic"]

end

subgraph DATA["DATA LAYER"]

DB["🗄️ SQLite"]
REC["📋 Patient Records"]
VIT["❤️ Vitals"]
TIME["⏱️ Health Timeline"]

end

P --> UI
P --> VOICE
A --> UI
D --> UI

VOICE --> STT
STT --> NLP
NLP --> FLASK

UI --> FLASK

FLASK --> AUTH
FLASK --> LOGIC

LOGIC --> DB
LOGIC --> REC
LOGIC --> VIT
LOGIC --> TIME

FLASK --> TTS
TTS --> VOICE
```

---

# 🧩 Core Modules

<table>
<tr>

<td width="33%" valign="top">

## 🎙️ Voice Layer

- Speech recognition
- Text-to-speech
- Language processing
- Voice interaction

</td>

<td width="33%" valign="top">

## 👤 Patient Layer

- Registration
- Profiles
- Health complaints
- Vitals
- Timeline

</td>

<td width="33%" valign="top">

## 👨‍⚕️ Healthcare Layer

- Doctor access
- ASHA workflows
- Follow-ups
- Healthcare guidance

</td>

</tr>

<tr>

<td valign="top">

## 🧠 Intelligence

- NLP
- Entity extraction
- Intent recognition
- Confidence handling

</td>

<td valign="top">

## 🗄️ Data

- Patient records
- Vitals
- Health timeline
- Interaction history

</td>

<td valign="top">

## 🔐 Security

- Authentication
- Authorization
- Access control
- Auditability

</td>

</tr>

</table>

---

# ✨ Key Features

| Feature | Purpose |
|---|---|
| 🎙️ Voice Interaction | Reduce dependence on typing |
| 👤 Patient Registration | Create structured profiles |
| 🩺 Health Complaints | Capture patient-reported concerns |
| ❤️ Vitals | Record basic health measurements |
| 📋 Health Timeline | Organize patient information |
| 👩‍⚕️ ASHA Support | Enable assisted workflows |
| 👨‍⚕️ Professional Connectivity | Facilitate information sharing |
| 🌐 Language Support | Improve accessibility |
| 📶 Offline Architecture | Handle connectivity constraints |
| 🧠 AI Assistance | Structure natural communication |
| 🔐 Security | Protect sensitive information |

---

# 🛠️ Technology Stack

<div align="center">

| Layer | Technology |
|---|---|
| 🎨 Frontend | HTML5 • CSS3 • JavaScript |
| ⚙️ Backend | Python • Flask |
| 🗄️ Database | SQLite |
| 🧠 Intelligence | AI / NLP |
| 🎙️ Voice | Speech-to-Text |
| 🔊 Response | Text-to-Speech |
| 🔐 Security | Authentication • RBAC |
| 📱 Future | PWA • Offline-first |

</div>

---

# 📂 Project Structure

```text
SwasthyaSetu/
│
├── app.py
├── database.py
├── database.db
├── requirements.txt
├── README.md
│
├── assets/
│   ├── swasthya-setu-logo.svg
│   └── swasthya-setu-hero.svg
│
├── templates/
│   ├── index.html
│   ├── register.html
│   ├── patients.html
│   ├── patient_details.html
│   └── vitals.html
│
├── static/
│   ├── css/
│   │   └── style.css
│   │
│   └── js/
│       └── script.js
│
└── screenshots/
    ├── dashboard.png
    ├── patient-registration.png
    ├── vitals.png
    └── health-timeline.png
```

---

# 🚀 Current Implementation

### Completed

- [x] Flask application setup
- [x] SQLite database
- [x] Patient registration
- [x] Patients list
- [x] Patient details
- [x] Vitals recording
- [x] Vitals database
- [x] Smart vitals status
- [x] Basic health timeline
- [x] Patient record management

### In Development

- [ ] Voice-based registration
- [ ] Voice health complaints
- [ ] Speech-to-text
- [ ] Text-to-speech
- [ ] Regional language support
- [ ] Doctor dashboard
- [ ] ASHA workflow
- [ ] Appointments
- [ ] Prescriptions
- [ ] Authentication
- [ ] Offline synchronization
- [ ] AI-assisted information extraction

---

# 🗺️ Development Roadmap

```mermaid
timeline

title SwasthyaSetu Roadmap

Foundation : Flask Backend
           : SQLite Database
           : Patient Records
           : Vitals
           : Health Timeline

Voice Layer : Voice Registration
            : Speech-to-Text
            : Voice Complaints
            : Text-to-Speech

Healthcare : Doctor Dashboard
           : ASHA Workflow
           : Appointments
           : Follow-ups

Intelligence : NLP
             : Entity Extraction
             : Intent Recognition
             : Confidence Detection

Scale : Offline Mode
      : PWA
      : Secure Cloud Deployment
```

---

# 📸 Interface

> Add screenshots of the **actual implemented application** here as the project evolves.

<div align="center">

### 🏠 Dashboard

<img src="screenshots/dashboard.png"
     width="88%"
     alt="SwasthyaSetu Dashboard">

<br><br>

### 👤 Patient Registration

<img src="screenshots/patient-registration.png"
     width="88%"
     alt="Patient Registration">

<br><br>

### ❤️ Vitals

<img src="screenshots/vitals.png"
     width="88%"
     alt="Vitals">

<br><br>

### 📋 Health Timeline

<img src="screenshots/health-timeline.png"
     width="88%"
     alt="Health Timeline">

</div>

---

# 💻 Getting Started

## 1. Clone the repository

```bash
git clone https://github.com/anshika-dev23/Swasthya-Setu.git
cd Swasthya-Setu
```

## 2. Create a virtual environment

### macOS / Linux

```bash
python3 -m venv venv
source venv/bin/activate
```

### Windows

```bash
python -m venv venv
venv\Scripts\activate
```

## 3. Install dependencies

```bash
pip install -r requirements.txt
```

## 4. Run the application

```bash
python app.py
```

Open:

```text
http://127.0.0.1:5000
```

---

# 🧪 Example Interaction

### 👤 Patient

> **"Mujhe teen din se bukhar hai aur raat mein bahut thand lagti hai."**

### 🎙️ Voice Layer

```text
Speech
 ↓
Speech-to-Text
```

### 🧠 Intelligence Layer

```text
Complaint → Fever
Duration → 3 Days
Additional → Chills at night
```

### 👨‍⚕️ Healthcare Professional

Reviews the available information and provides appropriate healthcare guidance.

### 🔊 Response Layer

The guidance can be transformed into an accessible voice interaction.

---

# 🌱 Future Vision

SwasthyaSetu can evolve into a broader rural healthcare communication ecosystem.

```mermaid
mindmap

root((🌾 SwasthyaSetu))

  🎙️ Voice
    Speech Recognition
    Text-to-Speech
    Regional Languages
    Accent Awareness

  👨‍⚕️ Healthcare
    Doctors
    ASHA Workers
    Appointments
    Follow-ups
    Prescriptions

  🧠 Intelligence
    NLP
    Entity Extraction
    Intent Recognition
    Confidence Detection

  📶 Accessibility
    Offline Mode
    PWA
    Low Bandwidth
    Simple Interface

  🔐 Trust
    Authentication
    Authorization
    Secure Records
    Audit Logs
```

---

# ⚠️ Responsible Use

SwasthyaSetu is a software prototype focused on healthcare communication and information organization.

It is **not intended to independently diagnose medical conditions or replace qualified healthcare professionals.**

A production implementation would require appropriate:

- Clinical validation
- Privacy safeguards
- Security controls
- Regulatory compliance
- Responsible AI evaluation
- Healthcare professional oversight

---

# 👥 Team

| Member | Contribution |
|---|---|
| **Anshika Srivastava** | Backend • Healthcare Platform • Voice-first Concept |
| Team Member | Add contribution |
| Team Member | Add contribution |
| Team Member | Add contribution |

---

<div align="center">

<img src="assets/swasthya-setu-logo.svg"
     width="120"
     alt="SwasthyaSetu Logo">

<br><br>

## 🌾 From Voice to Care.

**Listen. Understand. Connect. Care.**

<br>

<img src="https://img.shields.io/badge/Accessible-Healthcare-00C878?style=for-the-badge">
<img src="https://img.shields.io/badge/Voice-First-00D9FF?style=for-the-badge">
<img src="https://img.shields.io/badge/AI-Assisted-7C3AED?style=for-the-badge">

<br><br>

**SwasthyaSetu — Smart Voice-First Rural Healthcare Platform**

</div>
