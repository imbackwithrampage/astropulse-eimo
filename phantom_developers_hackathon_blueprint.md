# AstroPulse EIMO: Complete Hackathon Blueprint, Clinical Triage Matrix & Submission Package

**Challenge:** [Create Health Monitoring Software for Astronauts on Space Missions](https://www.spaceappschallenge.org/2026/challenges/health-monitoring-software/) ([2026 NASA Space Apps Challenges Directory](https://www.spaceappschallenge.org/2026/challenges/))  
**Authoring Agency Partner:** Brazilian Space Agency ([2026 Challenge Overview Video by Acting President Rodrigo Leonardi](https://www.youtube.com/watch?v=RERG3gEmdC8))  
**Team Name:** Phantom Developers (Team Owner: Sunil Sachindar S A)  
**Event Track:** 2026 Universal Event ([Local Event Confirmation Email](https://mail.google.com/mail/?authuser=sunilsachindarsa1205@gmail.com#all/thread-f:1881445368032031549))

## 1. Executive Project Summary & Pitch Script (Ready for Submission Page)

### Project Title
**AstroPulse EIMO: Autonomous Crew Health Monitoring, Anatomical Diagnostic HUD & Earth-Independent Triage Platform**

### High-Impact Short Description (150-Character Pitch)
An offline-first astronaut health HUD & EIMO triage engine mapping multi-modal vitals and ultrasound to NASA HRP's 5 spaceflight hazards.

### Executive Summary (Copy-Paste Ready for Space Apps Project Page)
Long-duration lunar outposts under NASA's Artemis campaign and future Mars transit missions expose astronauts to [NASA's 5 Hazards of Human Spaceflight](https://www.nasa.gov/hrp/hazards/)—space radiation, isolation and confinement, distance from Earth (averaging 140 million miles to Mars with up to 20-minute one-way radio latency per the [SciTechDaily NASA HRP Overview](https://scitechdaily.com/5-hazards-astronauts-face-in-human-spaceflight/)), altered gravity fields, and hostile/closed environments. Because astronauts are not physicians and cannot rely on real-time ground telemetry during deep-space emergencies or communication blackouts, **AstroPulse EIMO** implements [Earth Independent Medical Operations (EIMO)](https://pmc.ncbi.nlm.nih.gov/articles/PMC10810302/) in a single unified interface:

1. **Interactive Clickable Anatomical Body Map:** Displays 6 physiological systems (`Head/Ocular/CNS`, `Cardiovascular`, `Renal/Metabolic`, `Musculoskeletal`, `Immune/Hematologic`, and `Behavioral/Circadian`) with color-coded status badges (`Nominal`, `Caution`, `Critical`), spaceflight risk mechanisms, and non-physician examination guides.
2. **Multi-Modal Health Indicator & Ultrasound Logger:** Captures blood pressure (`mmHg`), heart rate (`bpm`), fasting blood glucose (`mg/dL`), core temperature (`°C`), daily sleep duration (`hrs`), [ARCHeR Behavioral Readiness](https://hrpdatachallenge.org/) mood scores (`1–10`), [NASA SHOP Hydration](https://www.frontiersin.org/journals/physiology/articles/10.3389/fphys.2026.1950155/full) (`L/day`), and point-of-care ultrasound/camera captures with step-by-step microgravity probe placement instructions.
3. **Environment-Aware Risk & Emergency Triage Engine:** Adapts thresholds across **Space Station (LEO)**, **Spacecraft (Mars Transit)**, **Surface Rover (EVA)**, and **Planetary Base (0.16g Moon / 0.38g Mars)**, walking crew through autonomous emergency stabilization (including the [2026 Challenge Overview Video's](https://www.youtube.com/watch?v=RERG3gEmdC8) halfway-to-Mars chest pain collapse scenario) while generating Store-and-Forward telemetry packets for Ground Flight Surgeons.
4. **Dynamic Longitudinal Trends & Gamified Countermeasure Routine:** Plots multi-SOL biomarker trajectories and gamifies daily preventive countermeasures (ARED resistive exercise against 1–1.5%/month bone mineral loss, SHOP nutrition/hydration, and circadian lighting) with XP rewards and mission streaks.

## 2. Clinical Triage Matrix Mapped to NASA's 5 Hazards of Human Spaceflight

Every rule in **AstroPulse EIMO** is grounded in [NASA's Human Research Program (HRP)](https://www.nasa.gov/hrp/), [Risks of Human Spaceflight](https://www.nasa.gov/hrp/risks/), [Artemis II Spaceflight Standard Measures](https://www.nasa.gov/reference/artemis-ii-standard-measures/), and [NASA's Integrated Medical Model (IMM)](https://www.nasa.gov/general/nasas-integrated-medical-model-imm/):

| NASA HRP Spaceflight Hazard | Primary Physiological & Clinical Risks | Tracked Health Indicators & Modalities | Nominal Range | Caution Threshold (Async Flight Surgeon Consult) | Critical Threshold (Immediate Autonomous Crew Action) | Guided Non-Physician Countermeasure & Triage Protocol |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **1. Space Radiation** ([NASA HRP Hazards](https://www.nasa.gov/hrp/hazards/)) | Acute Radiation Sickness (ARS), latent viral reactivation, endothelial dysfunction ([NIH PMC Deep Space CVD Study](https://pmc.ncbi.nlm.nih.gov/articles/PMC13291221/)) | Core Temp (`°C`), Resting HR (`bpm`), Dry Saliva Immune Booklet ([HRP Data Challenge](https://hrpdatachallenge.org/)) | `36.3–37.3 °C`; normal salivary cortisol/IgA | `37.4–37.9 °C` or mild prodromal fatigue | `>= 38.0 °C` or post-Solar Particle Event nausea | Shelter inside high-mass water-wall storm zone; administer oral ondansetron (`4 mg`) + electrolyte hydration; log point-of-care leukocyte & saliva assay. |
| **2. Isolation & Confinement** ([Starlust HRP Review](https://starlust.org/gallery/nasa-identifies-five-space-dangers-that-can-make-life-in-space-brutal-for-astronauts-mqkq3ksa/)) | Circadian desynchronization, sleep fragmentation, cognitive decline, mood disorders ([Spaceflight Standard Measures](https://pmc.ncbi.nlm.nih.gov/articles/PMC12612093/)) | Actigraphy Sleep Duration (`hrs/24h`), ARCHeR Mood Score (`1–10`) | `7.0–8.5 hrs/day`; Mood `7–10` | `5.2–6.5 hrs/day`; Mood `5–6` | `< 5.2 hrs/day` for 2+ SOLs or Mood `<= 4` | Enforce 8-hour protected sleep recovery block; activate `480 nm` blue-enriched morning LEDs; schedule private behavioral decompression & audio/video family sync. |
| **3. Distance from Earth** ([NASA IMM Overview](https://www.nasa.gov/general/nasas-integrated-medical-model-imm/)) | Up to 20-min one-way Mars comms delay; zero medical evacuation; acute cardiac event ([Challenge Video](https://www.youtube.com/watch?v=RERG3gEmdC8)) | Brachial BP (`mmHg`), 3-Lead Wearable ECG (`bpm`), Parasternal Cardiac Echo | `95–129 / 60–84 mmHg`; `52–85 bpm` | `130–139 / 85–89 mmHg` or `92–114 bpm` | `>= 140/90` or `< 90/58 mmHg`; HR `>= 115` or `< 45 bpm`; chest pain | Secure patient in 0g medical restraint; attach AED/ECG pads & administer `100% O2` (`4 L/min`) + chewed Aspirin (`324 mg`); capture 6s parasternal echo loop; transmit Priority-1 Store-and-Forward packet. |
| **4. Gravity Fields** (`0g` Transit, `0.16g` Moon, `0.38g` Mars) ([NASA Fundamentals of Health](https://www.nasa.gov/reference/fundamentals-of-human-health/)) | `1–1.5%/month` bone mineral density loss, renal stones (#2 IMM condition), cephalad fluid shift / SANS ocular changes | Ocular Ultrasound (`ONSD mm`), Fasting Glucose (`mg/dL`), Hydration (`L/day`), Urine Dipstick | `ONSD < 5.5 mm`; Glucose `72–105 mg/dL`; Water `2.1–2.5 L/day` | `ONSD 5.5–5.8 mm`; Glucose `106–139 mg/dL`; Water `1.5–2.0 L/day` | `ONSD > 5.8 mm` + visual blur; Glucose `>= 140` or `< 65 mg/dL`; flank colic + hematuria | **SANS:** LBNP session + Space Anticipation Glasses + cabin CO2 audit. **Renal Stone:** Oral ketorolac + tamsulosin (`0.4 mg`), renal ultrasound for hydronephrosis, bolus hydration `>= 2.8 L/day`. |
| **5. Hostile / Closed Environments** ([SHOP Nutrition Framework](https://www.frontiersin.org/journals/physiology/articles/10.3389/fphys.2026.1950155/full)) | Inadequate nutrition, elevated cabin CO2 headaches, microbial cross-contamination, EVA decompression sickness | Daily Caloric Macro Split, Fiber (`g/day`), Cabin CO2 (`mmHg`) | Protein `1.3–1.6 g/kg/d`, Carbs `50–55%`, Fat `25–35%`, Fiber `>= 40 g/d` | Mild caloric deficit or CO2 `3.0–4.0 mmHg` | Acute barotrauma, smoke inhalation, or CO2 `> 4.0 mmHg` | Adjust LiOH/amine CO2 scrubbers, verify HEPA microbial filters, and enforce SHOP macronutrient & hydration countermeasure streaks. |

## 3. Production TypeScript Data Schema (For React Native / Expo / Electron Extension)

If you extend the single-file Canvas web application into a multi-platform **React Native (Expo) + Electron** repository during the hackathon weekend, drop this TypeScript schema directly into `src/types/telemetry.ts`:

```typescript
export type MissionEnvironmentId = 'station' | 'transit' | 'rover' | 'base';

export type SpaceflightHazard =
  | 'SPACE_RADIATION'
  | 'ISOLATION_AND_CONFINEMENT'
  | 'DISTANCE_FROM_EARTH'
  | 'GRAVITY_FIELDS'
  | 'HOSTILE_CLOSED_ENVIRONMENT';

export type AnatomicalZoneId =
  | 'neuro'
  | 'cardio'
  | 'renal'
  | 'musculo'
  | 'immune'
  | 'behavioral';

export type TriageStatus = 'nominal' | 'caution' | 'critical';

export interface CrewVitalsRecord {
  sol: string;                  // e.g. "SOL-08"
  timestampIso: string;
  environment: MissionEnvironmentId;
  bpSystolicMmHg: number;       // Nominal: 95-129 mmHg
  bpDiastolicMmHg: number;      // Nominal: 60-84 mmHg
  heartRateBpm: number;         // Nominal: 52-85 bpm
  bloodGlucoseMgDl: number;     // Nominal: 72-105 mg/dL
  coreTempCelsius: number;      // Nominal: 36.3-37.3 C
  sleepDurationHours: number;   // ARCHeR Nominal: 7.0-8.5 hrs
  moodReadinessScore: number;   // ARCHeR Scale: 1-10
  hydrationLiters: number;      // NASA SHOP Minimum: 2.1-2.5 L/day
  diagnosticImaging?: {
    modality: 'ocular_onsd' | 'renal_stone' | 'cardiac_echo' | 'saliva_assay';
    quantitativeFinding: string;
    imageDataUri?: string;
  };
}

export interface EimoTelemetryPacket {
  packetId: string;
  crewMemberId: string;
  missionEnvironment: MissionEnvironmentId;
  oneWayLightTimeSeconds: number;
  crewHealthIndexPercent: number; // NASA IMM CHI (0-100%)
  escalationPriority: 'ROUTINE_STORE_FORWARD' | 'ASYNC_FLIGHT_SURGEON' | 'PRIORITY_1_EMERGENCY';
  latestVitals: CrewVitalsRecord;
  activeHazardFlags: SpaceflightHazard[];
}
```

## 4. 36-Hour Hackathon Execution Roadmap & Team Checklist (`Phantom Developers`)

Per NASA Space Apps' October 28, 2026 email (*"[Challenge Statements are Live! 📝](https://mail.google.com/mail/?authuser=sunilsachindarsa1205@gmail.com#all/thread-f:1880313721308824458)"*) and your November 10, 2026 event update (*"[Local Event Confirmed: Universal Event](https://mail.google.com/mail/?authuser=sunilsachindarsa1205@gmail.com#all/thread-f:1881445368032031549)"*):

- **Pre-Kickoff Check (Today — Friday, November 13, 2026):**
  - **Confirm Universal Event Team Size (2–6 Members):** Because **Phantom Developers** is registered under the **2026 Universal Event**, global judging rules require **at least 2 and at most 6 team members**, all registered for the **Universal Event**. Approve or coordinate with your pending requester (`lr10` from *"[Someone has requested to join your team Phantom Developers](https://mail.google.com/mail/?authuser=sunilsachindarsa1205@gmail.com#all/thread-f:1881100004162295021)"*) or add a teammate on the [Find a Team portal](https://www.spaceappschallenge.org/2026/find-a-team/).
  - **Check Official Resources Tab:** Review the newly unlocked datasets under the [Health Monitoring Software Challenge Page](https://www.spaceappschallenge.org/2026/challenges/health-monitoring-software/) and [Space Apps Connect Discussion #1772](https://github.com/nasa/spaceapps/discussions/1772).
- **Day 1 Morning (Saturday, November 14, 2026, 09:00–14:00 IST):**
  - Initialize the repository after 9:00 AM IST, deploy the **AstroPulse EIMO** interactive web app (`astro_pulse_health_monitor.html`), and verify all 4 environment profiles and 6 clickable SVG anatomical zones.
- **Day 1 Afternoon & Evening (Saturday, November 14, 2026, 14:00–22:00 IST):**
  - Wire the 5 emergency clinical scenarios (Acute Chest Pain on Mars Transit, Renal Stone Colic, SANS Ocular Shift, Solar Particle Event Radiation, and ARCHeR Circadian Fatigue) and test dynamic Chart.js trajectories.
- **Day 2 Morning & Afternoon (Sunday, November 15, 2026, 09:00–18:00 IST):**
  - Record a 30-second to 2-minute demonstration video showing: (1) clicking the astronaut SVG body map, (2) triggering the "Halfway-to-Mars Acute Chest Pain" emergency triage protocol, (3) logging a new SOL vitals entry with ultrasound guidance, and (4) checking off gamified countermeasure tasks.
- **Day 2 Final Submission Window (Sunday, November 15, 2026, 18:00–23:59 IST):**
  - Paste the Executive Summary and explicit NASA resource citations ([NASA Human Research Program](https://www.nasa.gov/hrp/), [5 Hazards of Human Spaceflight](https://www.nasa.gov/hrp/hazards/), [Artemis II Spaceflight Standard Measures](https://www.nasa.gov/reference/artemis-ii-standard-measures/), and [NASA Integrated Medical Model (IMM)](https://www.nasa.gov/general/nasas-integrated-medical-model-imm/)) into your Space Apps project submission page before 11:59 PM IST.
