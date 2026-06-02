# Field Robotics and Perception Lab — Project Context

> Documento di contesto per la continuazione del lavoro con Claude.
> Ultimo aggiornamento: giugno 2026

---

## Obiettivo

Creare una presenza web e materiale di presentazione per il **Field Robotics and Perception Lab** (Istituto di Intelligenza Meccanica, Scuola Superiore Sant'Anna di Pisa) da condividere con potenziali partner EU per progetti Horizon Europe su droni autonomi indoor.

---

## Identità del lab

| Campo | Valore |
|-------|--------|
| Nome | Field Robotics and Perception Lab |
| Istituzione | Istituto di Intelligenza Meccanica · Scuola Superiore Sant'Anna · Pisa |
| Responsabile | Dott. Massimo Satler — massimo.satler@santannapisa.it |
| Team | Matteo Unetti, Giulia Bassani, Carlo Alberto Avizzano |
| Pagina BRIEF | https://biorob-hub.eu/infrastructures/wp6/terra-terrestrial-and-aerial-robotics-for-large-infrastructures-and-environment-monitoring/ |
| GitHub repo | https://github.com/ilNonn0/field-robotics-lab |
| GitHub Pages URL | https://ilNonn0.github.io/field-robotics-lab |

---

## Research pillars (ordine fisso)

### 01 — Autonomous Exploration & SLAM
**Summary:** SLAM algorithms and autonomous exploration strategies for unknown environments — indoor and outdoor, GPS-denied — with focus on target-oriented search for Search and Rescue (SaR) missions.

**Scientific highlights:** Active exploration + SLAM; Semantic SLAM; Lifelong SLAM; Deep SLAM; Multi-Agent Cooperative SLAM (C-SLAM). Challenges: temporal efficiency, map completeness, target localisation, onboard compute.

**Practical applications:** SaR in unknown 3D environments; indoor exploration; UAV/UGV/AUV in GPS-denied areas; AR tracking.

**Related publications:**
- Learning Heuristics for Efficient Environment Exploration Using GNN — ICAR 2023
- GNGraph: Self-Organizing Maps for Autonomous Aerial Vehicle Planning — RA-L 2022
- An Efficient Object-Oriented Exploration Algorithm for UAVs — ICUAS 2021
- An Efficient Framework for Autonomous UAV Missions in GNSS-Denied Environments — Drones 2023
- Towards Autonomous Firefighting UAVs — JIRS 2024
- Autonomous Exploration of Indoor Environments with a MAV — RED-UAS 2015
- A Lightweight SLAM Algorithm for Indoor Autonomous Navigation — ACRA 2014

**Media placeholder:** Autonomous indoor flight demo

---

### 02 — Heterogeneous Multi-Agent Cooperation
**Summary:** Coordination of autonomous agents with different structures and capabilities — combining aerial and ground robots for complex missions neither could accomplish alone.

**Scientific highlights:** MARL for decentralised decision-making; VLMs for visual reasoning in cooperative tasks; emergent compositional cooperation patterns.

**Practical applications:** Hierarchical task planning; multi-objective task allocation; joint aerial-ground SaR; GNSS-denied cooperative localisation (validated LDC 2023, 1st place).

**Related publications:**
- Heterogeneous Multi-robot Systems Cooperative Exploration of Unknown Environment — ERF 2025

**Media placeholders:** Multi-agent cooperative mission; LDC 2023 winning run

---

### 03 — Infrastructure Inspection
**Summary:** Autonomous UAVs for inspection of bridges, buildings, industrial plants, and confined spaces. Landmark activity: ENEL boiler inspection with custom MAV.

**Scientific highlights:** AI-enhanced drone methodology; deep learning for defect detection; FastLIVO2 (https://github.com/hku-mars/fast-livo2) deployed onboard for 3D reconstruction.

**Practical applications:** Bridges/dams/buildings in hazardous locations; industrial plant boilers; 3D structural reconstruction; digital twin generation.

**Related publications:**
- Confined Spaces Industrial Inspection with MAV and Laser Range Finder Localization — Int. J. Micro Air Vehicles 2018
- Towards an Autonomous Flying Robot for Inspections in Open and Constrained Spaces — SSD 2014

**Media placeholder:** Infrastructure inspection demo

---

### 04 — Environmental Monitoring
**Summary:** Aerial and ground robotic systems for large-scale periodic monitoring of natural and agricultural environments.

**Scientific highlights:** Remote sensing with multispectral/thermal/LiDAR UAVs; precision agriculture pipelines; photogrammetry-based mapping; adaptive flight in woodland/orchard settings with limited GPS.

**Practical applications:** Precision agriculture; contaminated area mapping; photogrammetric surveys; Agritech PNRR partnership.

**Related publications:**
- Towards Smart Farming and Sustainable Agriculture with Drones — Intelligent Environments 2015

**Media placeholder:** Environmental monitoring demo

---

## Infrastruttura fisica

### Motion Capture Arena — VICON
- 10 camere VICON Vero + Vicon Lock system
- 3 camere FLIR RGB
- Arena indoor: **4 × 6 × 3 metri**
- Accuratezza: **1 mm** · frequenza: **fino a 333 Hz**
- Ground truth 6-DoF per UAV e robot terrestri

### UAV Fleet
| Piattaforma | Dettagli |
|-------------|----------|
| 2× custom 7" quad | ROS 2, companion computer x86 |
| Drone X500 + Intel NUC | LiDAR Ouster OS0-32, FLIR Boson 640×512, OAK-D stereo |
| UAV edge inference | NVIDIA Jetson Orin NX onboard |

### Ground Platforms
| Piattaforma | Dettagli |
|-------------|----------|
| Clearpath Husky A200 | UGV all-terrain, ROS 2 |
| Unitree Go2 EDU Plus | Quadruped, Jetson Orin NX, 4D LiDAR Mid-360 |
| Kinova Gen3 7DoF | Braccio per **mobile manipulation su Husky** + gripper Robotiq 2F-85 |

### Sensing aggiuntivo
- Sevensense Core Research (Visual-Inertial, 5 camere global shutter + IMU)
- Ouster OS0-32 Rev7 LiDAR (128 ch, 5.24M pts/s, 90° FOV)
- Livox Mid-360 LiDAR (360°, SLAM per ground robots)
- Livox Avia LiDAR (long range, UAV/portable)

### Compute
- Workstation GPU (training & simulation)
- Multipli embedded x86 (edge deployment)
- NVIDIA Jetson Orin NX (onboard inference)

---

## Progetti

| Acronimo | Programma | Anni | G.A. | Ruolo lab |
|----------|-----------|------|------|-----------|
| DESIRE6G | Horizon Europe · SNS JU | 2023–2024 | 101096466 | Contributo al testbed UAV in infrastruttura 6G cloud-native |
| 6G-LEADER | Horizon Europe | in corso | 101192080 | Dataset collection + design piattaforma drone autonoma per test 6G |
| Leonardo Drone Contest | Nazionale (Leonardo S.p.A.) | 2021–2025 | — | Partecipante da edizione fondante; **vincitore ciclo 2023** |
| Agritech | PNRR · Partenariato Nazionale | in corso | — | SSSA partner; lab contribuisce con piattaforme aeree e terrestri |

**LDC dettaglio:** due cicli (2021–2023 e 2023–2025), 6→7 università italiane. Massimo presente dall'edizione fondante.

---

## News (ordine cronologico decrescente)

| Data | Notizia | Badge |
|------|---------|-------|
| 2026 | Paper accepted — *Autonomous UAVs as Rescue Agents* · Drones MDPI vol.10 | Paper |
| 2025 | Paper accepted — *Heterogeneous Multi-robot Systems* · ERF 2025 | Paper |
| 2025 | Paper accepted — *Augmented Reality in DESIRE6G* · IEEE CSCN 2025 | Paper |
| Sep 2024 | LDC 2024 — partecipazione · ciclo 2023–2025 | Event |
| 2024 | Paper accepted — *Towards Autonomous Firefighting UAVs* · JIRS Springer | Paper |
| **Sep 2023** | **🏆 LDC 2023 — 1° Classificato · Team Sant'Anna** | Award |
| Sep 2023 | LDC 2023 — partecipazione · ciclo 2023–2025 | Event |
| 2023 | Paper accepted — *Efficient Framework for Autonomous UAV Missions* · Drones MDPI | Paper |
| Sep 2022 | LDC 2022 — partecipazione · ciclo 2021–2023 | Event |
| **Jun 2022** | **🥉 ICUAS 2022 UAV Competition — 3° posto · Team SantDrone · Dubrovnik** | Award |
| Sep 2021 | LDC 2021 — partecipazione · edizione fondante | Event |
| **2021** | **🏅 Finalist — OpenCV Spatial AI Contest 2021** | Award |

---

## Pubblicazioni selezionate

| Anno | Titolo | Venue |
|------|--------|-------|
| 2026 | Autonomous UAVs as Rescue Agents: Blink Detection for Human-State-Aware Survivor Localization | Drones, MDPI · vol.10 n.6 · doi:10.3390/drones10060417 |
| 2026 | Artificial Intelligence and Digital Twins Applications in Industry 4.0 and 5.0 | IntechOpen |
| 2025 | Heterogeneous Multi-robot Systems Cooperative Exploration of Unknown Environment | European Robotics Forum · Springer |
| 2025 | Augmented Reality in the DESIRE6G Cloud-native Infrastructure with Multi-Agent System | IEEE CSCN 2025 |
| 2024 | Towards Autonomous Firefighting UAVs: Online Planners for Obstacle Avoidance and Payload Delivery | J. Intelligent & Robotic Systems · Springer |
| 2023 | An Efficient Framework for Autonomous UAV Missions in Partially-Unknown GNSS-Denied Environments | Drones, MDPI · vol.7 |
| 2023 | Learning Heuristics for Efficient Environment Exploration Using Graph Neural Networks | ICAR 2023 · IEEE |
| 2022 | GNGraph: Self-Organizing Maps for Autonomous Aerial Vehicle Planning | IEEE Robotics and Automation Letters |
| 2021 | An Efficient Object-Oriented Exploration Algorithm for UAVs | ICUAS 2021 · IEEE |
| 2018 | Confined Spaces Industrial Inspection with MAV and Laser Range Finder Localization | Int. J. Micro Air Vehicles · SAGE |
| 2015 | Autonomous Exploration of Indoor Environments with a MAV | RED-UAS 2015 · IEEE |
| 2015 | Towards Smart Farming and Sustainable Agriculture with Drones | Intelligent Environments 2015 · IEEE |
| 2014 | Towards an Autonomous Flying Robot for Inspections in Open and Constrained Spaces | SSD 2014 · IEEE |
| 2014 | A Lightweight SLAM Algorithm for Indoor Autonomous Navigation | ACRA 2014 |

---

## Deliverable prodotti

### 1. index.html — versione cinematografica
- Stile: Midnight Luxe (navy/champagne), GSAP ScrollTrigger, animazioni hero, shuffler, typewriter, stacking scroll
- Sezioni: Hero · Pillars accordion · Features (3 card interattive) · Infrastructure · Gallery+Lightbox · Video (4 placeholder) · News · Projects · Publications · People (nascosta) · Join Us · Footer
- Font: Playfair Display + Inter + JetBrains Mono (Google Fonts CDN)
- Immagine hero: Unsplash drone `photo-1473968512647-3e447244af8f`

### 2. classic.html — versione statica
- Stile: DM Serif Display + DM Sans, bianco/navy, nessuna animazione
- Stesse sezioni di index.html, stessa struttura accordion pillars
- Navbar sticky con backdrop-blur
- Zero dipendenze JS esterne

### 3. index_embedded.html — versione standalone
- Identica a index.html ma con tutte le 7 foto incorporate come base64
- Peso: ~17 MB — per preview/invio/uso offline

### 4. FRPL_pitch_deck.pptx
- 8 slide: Cover · Research Pillars · Infrastructure · UAV Fleet (foto) · EU Projects · LDC Winner · Publications · CTA
- Palette: Navy `1E2761` / Ice Blue `CADCFC` — font Cambria + Calibri
- Script sorgente: `deck.js` (Node.js, PptxGenJS 4.0.1)

### 5. File immagini (cartella img/)
| File | Contenuto |
|------|-----------|
| drone_fleet.jpg | Fleet overview 3 piattaforme |
| drone_custom_large.jpg | Custom MAV con VICON markers |
| drone_custom_compact.jpg | Custom quad compact |
| drone_custom_stereo.jpg | Custom quad con stereo+depth camera |
| ldc_award.jpg | LDC 2023 drone+UGV+trofeo |
| ldc_banner.jpg | LDC 2023 banner "7drone contest" |
| ldc_action.jpg | LDC in action UAV+UGV in arena |

---

## TODO

### Landing page (entrambe le versioni)
- [ ] **Video** — caricare 4 video su YouTube (unlisted) e sostituire i placeholder:
  ```html
  <div class="video-embed">
    <iframe src="https://www.youtube.com/embed/VIDEO_ID"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
      allowfullscreen></iframe>
  </div>
  ```
  Titoli: 1) Autonomous indoor flight 2) Multi-agent cooperative mission 3) LDC 2023 winning run 4) Infrastructure inspection

- [ ] **Sezione People** — aggiungere foto e bio del team (rimuovere `display:none` dal CSS `#people`):
  - Massimo Satler, Matteo Unetti, Giulia Bassani, Carlo Alberto Avizzano
  - Struttura: foto + nome + ruolo + link Scholar/LinkedIn

- [ ] **Foto TERRA/BRIEF** — aggiungere alla galleria (richiedono login su biorob-hub.eu):
  - Hero lab, Husky A200, Unitree Go2, X500, Kinova Gen3

- [ ] **Hosting** — pagina su GitHub Pages: https://ilNonn0.github.io/field-robotics-lab
  - Caricare img/ tramite drag & drop o git push
  - Rinominare lab_landing_page.html → index.html (già fatto)

- [ ] **Agritech** — aggiungere anni esatti del progetto

- [ ] **Scholar link** — già nel footer, verificare che sia corretto

### Pitch deck
- [ ] Slide team — foto e ruoli (Satler, Unetti, Bassani, Avizzano)
- [ ] Foto device BRIEF — Husky/Go2/X500 quando disponibili
- [ ] Timeline — valutare slide con storia del lab

---

## Ispirazione grafica

Sito di riferimento analizzato: **ARPL — Agile Robotics and Perception Lab** (https://arplaboratory.github.io)
- Struttura: Home (mission + news) · Publications · People · Join Us · Support
- Taglio: tecnico-accademico asciutto, orientato a ricercatori e potenziali collaboratori
- Elementi adottati: sezione News cronologica, People gerarchica, Join Us per studenti/ricercatori

---

## Note tecniche

- Landing page: Google Fonts CDN — richiede connessione internet
- Per uso offline: scaricare i font localmente
- Pitch deck: `node deck.js` per rigenerare (richiede PptxGenJS 4.0.1, sharp, react-icons)
- GitHub repo: `https://github.com/ilNonn0/field-robotics-lab`
- Per attivare GitHub Pages: Settings → Pages → Branch: main → / (root) → Save

---

## Scelte di design

| Aspetto | index.html | classic.html |
|---------|-----------|--------------|
| Palette | Navy `0D0D12` / Champagne `C9A84C` | Navy `1E2761` / White `ffffff` |
| Font titoli | Playfair Display serif | DM Serif Display |
| Font corpo | Inter | DM Sans |
| Font mono | JetBrains Mono | — |
| Animazioni | GSAP ScrollTrigger, hero stagger, SVG | Nessuna |
| Tono | Dark editorial cinematografico | Tecnico-raffinato pulito |
| Pillar | Accordion (1 aperto alla volta) | Accordion (1 aperto alla volta) |
| Badge News | Paper=verde, Award=ambra, Event=blu | Paper=verde, Award=ambra, Event=blu navy |
