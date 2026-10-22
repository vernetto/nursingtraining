# Chapter 70. Scoring Systems and Clinical Decision Rules

## Learning objectives

After studying this chapter you should be able to:

1. Distinguish diagnostic rules, prognostic scores, risk-stratification tools, severity scores and early-warning scores, and state what each is designed (and not designed) to do.
2. Explain how a rule is derived, validated and implemented, and judge whether a rule applies to the patient in front of you (population, setting, prevalence, version).
3. Apply, step by step, the most widely used rules: Wells and PERC/YEARS (VTE), Centor/McIsaac/FeverPAIN (pharyngitis), CURB-65/CRB-65 (pneumonia), HEART (chest pain), CHA₂DS₂-VASc/CHA₂DS₂-VA and HAS-BLED (AF), Ottawa (ankle, foot, knee), Canadian CT head and C-spine rules, NEXUS, qSOFA/SIRS/NEWS2/SOFA (sepsis and deterioration), Glasgow-Blatchford (GI bleeding), Alvarado (appendicitis), Child-Pugh and MELD (liver), ABCD², sPESI, GCS and others.
4. Interpret a score as a probability estimate that updates, but does not replace, clinical judgement; know when to override.
5. Recognise common misuses: applying a rule outside its derivation population, using a score as a threshold for treatment without reasoning, ignoring the clinical gestalt, and calculation errors.
6. Use cut-offs correctly, including the meaning of "rule-out", "intermediate" and "high-risk" categories and the residual risk attached to each.
7. Communicate a scored risk to patients and colleagues, and document the use of a rule.

> **Note on versions and thresholds.** Rules are periodically revised (for example, the AF stroke-risk guidance moved from CHA₂DS₂-VASc to CHA₂DS₂-VA in 2024 in some guidelines). The thresholds below reflect widely used versions at the time of writing; always check the current local guideline and the validated version for your population.

---

## 1. Principles

### 1.1 Types of tools

| Type | Purpose | Examples |
|---|---|---|
| **Diagnostic probability rules** | Estimate the probability of a condition to guide testing | Wells (DVT, PE), Alvarado, Centor, Geneva |
| **Rule-out rules** | Identify patients so low-risk that testing can be omitted | PERC, Ottawa, Canadian CT head, NEXUS, HEART (low), YEARS |
| **Prognostic / risk-stratification scores** | Estimate outcome risk to guide level of care or therapy | CURB-65, PSI, sPESI, CHA₂DS₂-VASc, TIMI, GRACE, MELD, Child-Pugh, ABCD² |
| **Severity-of-illness scores** | Quantify organ dysfunction | SOFA, APACHE II, GCS, Glasgow-Blatchford |
| **Early-warning scores** | Detect deterioration from vital signs | NEWS2, MEWS, PEWS |
| **Screening questionnaires** | Detect disease or risk in groups | PHQ-9, GAD-7, AUDIT-C, 4AT, MoCA, STOP-BANG, FRAX, QRISK3 |
| **Functional status scales** | Describe baseline and trajectory | ECOG, Karnofsky, PPS, Barthel, Clinical Frailty Scale, modified Rankin |

### 1.2 How a rule is built

1. **Derivation** in a cohort: variables associated with the outcome are selected (logistic regression, recursion partitioning) and weighted.
2. **Internal validation** (bootstrapping) and **external validation** in other populations and settings.
3. **Impact analysis**: does using the rule change clinician behaviour and improve outcomes or reduce resource use (the real test)?
4. **Implementation** with decision support, and **re-calibration** when prevalence or practice changes.

### 1.3 Appraising a rule before using it

- **Population**: age, setting (emergency department vs primary care vs inpatient), presenting complaint, exclusion criteria. A rule derived in the emergency department may overestimate risk in primary care and vice versa.
- **Outcome**: what exactly is predicted (30-day mortality, MACE, fracture requiring treatment, clinically important injury)?
- **Performance**: sensitivity and negative predictive value for rule-out tools (target usually > 95–99%); calibration and discrimination (AUC) for prognostic scores; **how many patients are classified as low risk** (yield).
- **Residual risk**: even a "low-risk" category has a nonzero event rate; compare it with your tolerance and the cost of a miss.
- **Version and local calibration**; **inter-rater variability** of subjective items ("alternative diagnosis less likely", "history suggestive").
- **Is it validated for this subgroup** (pregnancy, children, elderly, cancer, immunocompromised, repeat visits)? Many rules exclude them.

### 1.4 Using scores well

1. Calculate the score from the **data actually available**, not assumptions; missing data should be handled explicitly (assume normal only if justified).
2. Treat the result as one input: **pre-test probability → rule → test → decision** (chapter 69).
3. **Clinical override** is legitimate and should be documented ("HEART 3 but pain typical and prior stents; admitted").
4. Do not **treat the score** (e.g., CURB-65 = 1 does not mean home if she is socially isolated, vomiting or hypoxic).
5. **Reassess**: scores are time-point snapshots; patients change.
6. **Document** the score, the components and the action.
7. **Explain risks to patients** as natural frequencies ("about 2 in 100 people with this score have a heart attack within 6 weeks").

---

## 2. Venous thromboembolism

### 2.1 Wells score for DVT

| Item | Points |
|---|---|
| Active cancer (treatment within 6 months or palliative) | +1 |
| Paralysis, paresis or recent plaster immobilisation of the leg | +1 |
| Recently bedridden ≥ 3 days or major surgery within 12 weeks | +1 |
| Localised tenderness along the deep venous system | +1 |
| Entire leg swollen | +1 |
| Calf swelling > 3 cm compared with the asymptomatic leg (10 cm below tibial tuberosity) | +1 |
| Pitting oedema confined to the symptomatic leg | +1 |
| Collateral superficial (non-varicose) veins | +1 |
| Previous documented DVT | +1 |
| Alternative diagnosis at least as likely as DVT | −2 |

**Two-tier**: ≥ 2 = "DVT likely" (about 25–30% prevalence) → proximal compression ultrasound (± D-dimer if ultrasound delayed, start anticoagulation if delay > 4 h); ≤ 1 = "DVT unlikely" (~5%) → D-dimer; negative D-dimer excludes. **Three-tier**: ≤ 0 low (~5%), 1–2 moderate (~17%), ≥ 3 high (~53%).

### 2.2 Wells score for PE

| Item | Points |
|---|---|
| Clinical signs and symptoms of DVT | 3.0 |
| PE is the most likely diagnosis (or equally likely) | 3.0 |
| Heart rate > 100/min | 1.5 |
| Immobilisation ≥ 3 days or surgery in the previous 4 weeks | 1.5 |
| Previous PE or DVT | 1.5 |
| Haemoptysis | 1.0 |
| Malignancy (treatment within 6 months or palliative) | 1.0 |

**Two-tier**: > 4 = "PE likely" → CTPA directly (anticoagulate while waiting if delay and no contraindication); ≤ 4 = "PE unlikely" → D-dimer (age-adjusted cut-off: age × 10 µg/L FEU above 50 years) → negative excludes PE. **Three-tier**: < 2 low (~1–3%), 2–6 moderate (~16–20%), > 6 high (~40–50%).

### 2.3 PERC (Pulmonary Embolism Rule-out Criteria)

Applies **only** when clinical gestalt estimates a **low pre-test probability (< 15%)**. If **all eight** criteria are met, the probability of PE is < 2% and no D-dimer or imaging is needed:

1. Age < 50 years
2. Heart rate < 100/min
3. SaO₂ ≥ 95% (room air)
4. No haemoptysis
5. No exogenous oestrogen use
6. No prior DVT/PE
7. No unilateral leg swelling
8. No surgery or trauma requiring hospitalisation within 4 weeks

Do **not** apply PERC in intermediate/high-probability patients or where gestalt is uncertain (pregnancy is excluded in most studies).

### 2.4 YEARS algorithm

Three items: clinical signs of DVT; haemoptysis; PE the most likely diagnosis. **No items**: PE excluded if D-dimer < 1000 ng/mL. **≥ 1 item**: PE excluded if D-dimer < 500 ng/mL; otherwise CTPA. This reduces CTPA use by about 14% compared with the standard Wells pathway; also validated in pregnancy (with leg compression ultrasound first).

### 2.5 sPESI (simplified Pulmonary Embolism Severity Index)

One point each: age > 80; history of cancer; chronic cardiopulmonary disease; heart rate ≥ 110/min; systolic BP < 100 mmHg; SaO₂ < 90%. **0 = low risk** (30-day mortality ~1%) → consider outpatient treatment if no other reason for admission; ≥ 1 = not low risk. Combine with RV imaging and troponin (ESC intermediate-high risk categories).

---

## 3. Respiratory and infection

### 3.1 CURB-65 and CRB-65

One point each: **C**onfusion (new disorientation or AMTS ≤ 8), **U**rea > 7 mmol/L (BUN > 19 mg/dL), **R**espiratory rate ≥ 30/min, **B**lood pressure (systolic < 90 or diastolic ≤ 60 mmHg), age ≥ **65**.

| Score | 30-day mortality | Suggested site of care |
|---|---|---|
| 0–1 | ~1–3% | Home treatment (if no other concerns) |
| 2 | ~9% | Hospital (short stay or supervised outpatient) |
| 3–5 | 15–40% | Hospital; consider ICU for 4–5 or if other severity markers |

**CRB-65** omits urea (primary care). Always add judgement: hypoxaemia (SpO₂ < 92%), multilobar infiltrates, comorbidities, inability to take oral therapy, social factors. The **Pneumonia Severity Index (PSI/PORT)** is more sensitive for comorbidity but more complex; **ATS/IDSA minor/major criteria** guide ICU admission (major: mechanical ventilation, septic shock requiring vasopressors).

### 3.2 Centor, McIsaac and FeverPAIN (sore throat)

- **Centor**: tonsillar exudate +1; tender/swollen anterior cervical nodes +1; fever (history or > 38 °C) +1; **absence** of cough +1.
- **McIsaac (modified Centor)**: adds age 3–14 y +1; 15–44 y 0; ≥ 45 y −1.
- Interpretation (McIsaac): ≤ 0–1 → GAS probability ~1–10%: no test, no antibiotic; 2–3 → ~15–35%: rapid antigen test or culture (adults: treat if positive); ≥ 4 → ~50%: test (or treat empirically in some guidelines).
- **FeverPAIN**: Fever in last 24 h; Purulence (tonsillar pus); Attend rapidly (within 3 days); severely Inflamed tonsils; No cough or coryza. 0–1: ~13–18% streptococcus → no antibiotics; 2–3: ~34–40% → delayed prescription; 4–5: ~62–65% → immediate antibiotics if severe or delayed.
- Red flags override: peritonsillar abscess (trismus, uvula deviation), epiglottitis, Lemierre syndrome, immunosuppression.

### 3.3 Asthma, COPD and other respiratory

- **Acute asthma severity** (BTS): moderate PEF 50–75%; acute severe PEF 33–50%, RR ≥ 25, HR ≥ 110, inability to complete sentences; life-threatening PEF < 33%, SpO₂ < 92%, silent chest, cyanosis, exhaustion, confusion.
- **DECAF** (COPD exacerbation mortality): Dyspnoea (eMRCD 5a/5b), Eosinopenia, Consolidation, Acidaemia, atrial Fibrillation.
- **STOP-BANG** (obstructive sleep apnoea): Snoring, Tired, Observed apnoea, Pressure (hypertension), BMI > 35, Age > 50, Neck > 40 cm, male Gender; ≥ 3 intermediate, ≥ 5 high risk.

---

## 4. Cardiovascular

### 4.1 HEART score (undifferentiated chest pain)

| Component | 0 | 1 | 2 |
|---|---|---|---|
| **H**istory | Slightly suspicious | Moderately suspicious | Highly suspicious |
| **E**CG | Normal | Non-specific repolarisation changes, LBBB, LVH, paced | Significant ST deviation |
| **A**ge | < 45 | 45–64 | ≥ 65 |
| **R**isk factors* | None | 1–2 | ≥ 3, or known atherosclerotic disease |
| **T**roponin | ≤ normal | 1–3 × normal | > 3 × normal |

*Hypertension, hypercholesterolaemia, diabetes, obesity (BMI > 30), smoking (current or ≤ 3 months), positive family history.

**0–3**: low risk, 30-day MACE ~1–2% → early discharge/outpatient follow-up, particularly with serial hs-troponin; **4–6**: moderate risk, ~12–17% → observation, further testing (CT coronary angiography, stress imaging); **7–10**: high, ~50–65% → admit, early invasive strategy. The score assumes serial troponin and ECG; a "low" HEART with a convincing story of ischaemia and ECG evolution should be treated on its merits.

Other chest pain/ACS tools: **TIMI** (UA/NSTEMI: age ≥ 65, ≥ 3 risk factors, known CAD ≥ 50%, aspirin use, ≥ 2 anginal episodes in 24 h, ST changes, positive marker), **GRACE** (in-hospital and 6-month mortality; used to time angiography), **ESC 0/1-h hs-troponin algorithm**.

### 4.2 CHA₂DS₂-VASc / CHA₂DS₂-VA (stroke risk in AF)

| Item | Points |
|---|---|
| **C**ongestive heart failure / LV dysfunction | 1 |
| **H**ypertension | 1 |
| **A**ge ≥ 75 | 2 |
| **D**iabetes mellitus | 1 |
| **S**troke/TIA/thromboembolism | 2 |
| **V**ascular disease (prior MI, PAD, aortic plaque) | 1 |
| **A**ge 65–74 | 1 |
| **S**ex category: female | 1 (omitted in CHA₂DS₂-VA, 2024 ESC) |

Guideline summary (ESC 2020): anticoagulate if score ≥ 2 in men or ≥ 3 in women; consider at 1 in men or 2 in women. ESC 2024 uses CHA₂DS₂-VA: ≥ 2 recommended, 1 considered, 0 no therapy. Annual stroke risk rises from ~0.2% (score 0) to ~2% (score 2) to ≥ 10% (score ≥ 7) untreated. Applies to non-valvular AF; moderate–severe mitral stenosis and mechanical valves require warfarin regardless. Flutter is managed similarly.

### 4.3 HAS-BLED (bleeding risk on anticoagulation)

**H**ypertension (uncontrolled, SBP > 160) 1; **A**bnormal renal (dialysis, transplant, creatinine > 200 µmol/L) 1 and/or liver function (cirrhosis, bilirubin > 2 × ULN with AST/ALT > 3 × ULN) 1; **S**troke 1; **B**leeding history or predisposition (anaemia) 1; **L**abile INR (TTR < 60%) 1; **E**lderly > 65 1; **D**rugs (antiplatelets, NSAIDs) 1 and/or alcohol (≥ 8 drinks/week) 1. Score ≥ 3 = high risk → **do not withhold anticoagulation** on the basis of the score alone; instead correct modifiable factors (BP, NSAIDs, alcohol, INR control) and review more often.

### 4.4 Other cardiovascular tools

- **Pre-test probability of coronary disease** (ESC/NICE): age, sex, symptom typicality (Diamond–Forrester).
- **ASCVD risk calculators**: SCORE2/SCORE2-OP (Europe), QRISK3 (UK), Pooled Cohort Equations (US); use for primary prevention decisions (chapter 40).
- **Heart failure**: NYHA class, ACC/AHA stage; MAGGIC; H₂FPEF score for HFpEF.
- **Syncope**: Canadian Syncope Risk Score, San Francisco Syncope Rule, EGSYS (chapter 36 and 41). High-risk: abnormal ECG, structural heart disease, syncope during exertion/supine, absent prodrome, family history of sudden death.
- **Aortic dissection**: ADD-RS (Aortic Dissection Detection Risk Score): high-risk conditions (Marfan, family history, known aortic disease, recent aortic manipulation), high-risk pain features (abrupt, severe, ripping), high-risk examination (pulse deficit, SBP differential > 20 mmHg, focal neurological deficit with pain, new aortic regurgitation murmur, hypotension/shock): 0 low (with D-dimer < 500: exclusion), ≥ 1 moderate, ≥ 2 high → CT angiography.

---

## 5. Sepsis, deterioration and critical illness

### 5.1 SIRS and qSOFA

- **SIRS** (≥ 2 of 4): temperature > 38 or < 36 °C; heart rate > 90/min; respiratory rate > 20/min (or PaCO₂ < 32 mmHg); WBC > 12 or < 4 × 10⁹/L (or > 10% bands). Sensitive but non-specific (about 90% of hospitalised patients meet it at some point).
- **qSOFA** (bedside prompt, ≥ 2 of 3): respiratory rate ≥ 22/min; altered mentation (GCS < 15); systolic BP ≤ 100 mmHg. Specific but insensitive; not a screening tool for sepsis (the Surviving Sepsis Campaign discourages using qSOFA alone).
- **Sepsis-3 definition**: life-threatening organ dysfunction due to dysregulated host response to infection = acute SOFA increase ≥ 2.

### 5.2 SOFA (Sequential Organ Failure Assessment)

Scores 0–4 for six systems: respiration (PaO₂/FiO₂), coagulation (platelets), liver (bilirubin), cardiovascular (MAP/vasopressors), CNS (GCS), renal (creatinine/urine output). Baseline SOFA 0 in healthy patients; ≥ 2 rise indicates ~10% hospital mortality; SOFA in ICU is used for severity and trend (a rising score over 48 h predicts mortality). **APACHE II/IV** and **SAPS** provide admission-based mortality predictions for ICU benchmarking.

### 5.3 NEWS2 (National Early Warning Score 2)

Parameters: respiratory rate, SpO₂ (Scale 1; Scale 2 for hypercapnic respiratory failure with target 88–92%), air or oxygen, systolic BP, pulse, consciousness (ACVPU), temperature. Each scores 0–3.

| Aggregate | Clinical risk | Response |
|---|---|---|
| 0–4 | Low | Ward-based monitoring (minimum 4–6-hourly) |
| **3 in any single parameter** | Low–medium | Urgent ward-based review |
| 5–6 | Medium | Urgent review by a competent clinician; consider critical care outreach |
| ≥ 7 | High | Emergency assessment; transfer to higher level of care |

NEWS2 detects deterioration and sepsis risk but does not replace clinical concern; "worried" nurses and relatives are strong predictors. Paediatric: PEWS; obstetric: MEOWS.

### 5.4 Glasgow Coma Scale (GCS)

Eye opening (1–4), verbal response (1–5), motor response (1–6): total 3–15. Report components (e.g., E3 V4 M5 = 12). Severe ≤ 8 (airway at risk), moderate 9–12, mild 13–15. Pitfalls: intubated patients (V "T"), eye swelling, sedation, aphasia, spinal injury; use **FOUR score** or AVPU as complements. In children use the paediatric GCS.

### 5.5 Other severity tools

**MASCC** and **CISNE** (febrile neutropenia, chapter 62); **Ranson/Glasgow/BISAP** (acute pancreatitis; BISAP: BUN > 8.9 mmol/L [25 mg/dL], impaired mental status, SIRS, age > 60, pleural effusion; ≥ 3 high mortality); **Revised Trauma Score**, **Injury Severity Score**; **Burns: Rule of Nines, Parkland formula** (4 mL × kg × %TBSA over 24 h, half in the first 8 h); **APGAR** (newborns).

---

## 6. Trauma and musculoskeletal decision rules

### 6.1 Ottawa ankle and foot rules

Order ankle radiographs if there is **pain in the malleolar zone** and: bone tenderness at the posterior edge or tip of the lateral malleolus (distal 6 cm), or of the medial malleolus, **or** inability to bear weight (4 steps) both immediately and in the ED. Order **foot** radiographs if pain in the midfoot zone and: bone tenderness at the base of the fifth metatarsal, or at the navicular, **or** inability to bear weight. Sensitivity ~98–100% for fractures; reduces radiographs by ~30–40%. Not validated in children < 5 (Low Risk Ankle Rule in children), intoxicated or distracted patients, or multiple injuries.

### 6.2 Ottawa knee rule

Radiograph if **any**: age ≥ 55; isolated tenderness of the patella; tenderness of the fibular head; inability to flex to 90°; inability to bear weight (4 steps) both immediately and in the ED. Sensitivity ~98–100%.

### 6.3 Canadian CT head rule (CCHR)

For patients with minor head injury (GCS 13–15) and loss of consciousness, amnesia or disorientation. CT if **high risk** (neurosurgical intervention): GCS < 15 at 2 hours, suspected open or depressed skull fracture, any sign of basilar skull fracture, vomiting ≥ 2 episodes, age ≥ 65. **Medium risk** (brain injury on CT): amnesia before impact ≥ 30 minutes, dangerous mechanism (pedestrian struck, ejected, fall > 1 m or 5 stairs). Excluded: anticoagulated patients, age < 16, seizure, unstable (NICE and other guidelines have separate recommendations: anticoagulant users usually require CT). **PECARN** for children: age < 2 years vs ≥ 2 years criteria (GCS < 15, altered mental status, palpable skull fracture, LOC, severe mechanism, severe headache/vomiting).

### 6.4 Cervical spine: NEXUS and Canadian C-spine rule

- **NEXUS** (all must be absent to clear without imaging): midline cervical tenderness; focal neurological deficit; altered level of alertness; intoxication; painful distracting injury.
- **Canadian C-spine rule (CCR)** for alert, stable trauma patients: (1) any **high-risk factor** (age ≥ 65, dangerous mechanism, paraesthesias in extremities) → radiography; (2) any **low-risk factor** allowing safe assessment of range of motion (simple rear-end collision, sitting in ED, ambulatory at any time, delayed onset of neck pain, absence of midline tenderness); (3) can the patient actively rotate the neck 45° left and right? If yes → no imaging. CCR is more sensitive than NEXUS (99–100%).

### 6.5 Other

**Pittsburgh knee rules**, **Ottawa SAH rule** (headache: age ≥ 40, neck pain/stiffness, witnessed LOC, onset during exertion, thunderclap onset, limited neck flexion on examination; any one → investigate), **San Francisco Syncope Rule**, **Canadian TIA Score**, **Hip fracture risk**, **FRAX/QFracture** (fracture risk).

---

## 7. Abdomen, GI and liver

### 7.1 Alvarado score (appendicitis)

| Item | Points |
|---|---|
| Migration of pain to the right iliac fossa | 1 |
| Anorexia | 1 |
| Nausea/vomiting | 1 |
| Tenderness in the right iliac fossa | 2 |
| Rebound tenderness | 1 |
| Elevated temperature (≥ 37.3 °C) | 1 |
| Leukocytosis (> 10 × 10⁹/L) | 2 |
| Neutrophil left shift | 1 |

Total 10. **1–4**: appendicitis unlikely (consider discharge with safety net); **5–6**: possible → observation/imaging (ultrasound in children/pregnancy; CT otherwise); **7–8**: probable → surgical review; **9–10**: very probable → surgery. Performance is lower in women, children and the elderly; alternatives: AIR score, Paediatric Appendicitis Score, RIPASA, Adult Appendicitis Score.

### 7.2 Glasgow-Blatchford score (upper GI bleeding)

Components: blood urea (6.5–7.9: 2; 8–9.9: 3; 10–24.9: 4; ≥ 25 mmol/L: 6), haemoglobin (men 120–129: 1; 100–119: 3; < 100: 6 g/L; women 100–119: 1; < 100: 6), systolic BP (100–109: 1; 90–99: 2; < 90: 3), pulse ≥ 100 (1), melaena (1), syncope (2), hepatic disease (2), cardiac failure (2). **Score 0 (or ≤ 1 in some guidelines)** identifies patients suitable for outpatient management (no need for urgent endoscopy); higher scores predict need for transfusion, intervention or death. The pre-endoscopy **Rockall** is less discriminating for need for intervention; the full Rockall includes endoscopic findings.

### 7.3 Liver: Child-Pugh and MELD

- **Child-Pugh**: bilirubin (< 34 µmol/L 1; 34–50 2; > 50 3), albumin (> 35 g/L 1; 28–35 2; < 28 3), INR (< 1.7 1; 1.7–2.3 2; > 2.3 3), ascites (none 1; mild/diuretic-responsive 2; moderate–severe/refractory 3), encephalopathy (none 1; grade 1–2 2; grade 3–4 3). Class A 5–6 (1-year survival ~100%), B 7–9 (~80%), C 10–15 (~45%).
- **MELD / MELD-Na / MELD 3.0**: based on bilirubin, INR, creatinine, ± sodium (± albumin, sex); ranks transplant candidates; MELD-Na ≥ 15 supports transplant evaluation.
- **Maddrey discriminant function** (alcoholic hepatitis): 4.6 × (PT − control PT) + bilirubin (mg/dL); ≥ 32 → consider prednisolone (Lille score at day 7 guides continuation). **ABIC**, **Glasgow alcoholic hepatitis score**.
- **FIB-4** (age × AST)/(platelets × √ALT): < 1.3 low risk of advanced fibrosis (< 2.0 if age > 65); > 2.67 high risk; elastography for intermediate values (chapter 64).
- **West Haven grading** of hepatic encephalopathy (grade 1: mild confusion, sleep reversal; 4: coma).

### 7.4 Other

**Ranson/BISAP/Glasgow-Imrie** (pancreatitis), **Truelove and Witts** (severe ulcerative colitis: ≥ 6 bloody stools/day plus HR > 90, T > 37.8 °C, Hb < 105 g/L, ESR > 30), **Harvey–Bradshaw/CDAI** (Crohn), **Rome IV criteria** (functional GI disorders), **Bristol stool chart**, **Mannheim peritonitis index**, **Boey score** (perforated ulcer).

---

## 8. Neurology, psychiatry and geriatrics

- **NIHSS** (stroke severity 0–42: 0 no deficit, 1–4 minor, 5–15 moderate, 16–20 moderate to severe, 21–42 severe). **FAST/BE-FAST/ROSIER/ face-arm-speech tests** for recognition. **ABCD²** (TIA): Age ≥ 60 (1), BP ≥ 140/90 (1), Clinical features (unilateral weakness 2, speech disturbance without weakness 1), Duration (≥ 60 min 2; 10–59 min 1), Diabetes (1): 0–3 low (2-day stroke risk ~1%), 4–5 moderate (~4%), 6–7 high (~8%). Because ABCD² misses carotid disease and AF, guidelines favour urgent specialist assessment of all suspected TIA irrespective of score.
- **modified Rankin Scale** (0–6) for disability, **Barthel Index**, **Clinical Frailty Scale** (1–9; ≥ 5 frail).
- **Cognitive**: MMSE (< 24/30 suggests impairment), **MoCA** (< 26/30), **Mini-Cog**, **AMTS**, **4AT** (delirium: alertness, AMT4, attention [months backward], acute change; score ≥ 4 delirium likely), **CAM** (acute onset/fluctuating course + inattention + disorganised thinking or altered consciousness).
- **Depression and anxiety**: **PHQ-2/PHQ-9** (≥ 10 moderate depression; item 9 suicidality requires immediate enquiry), **GDS-15**, **EPDS** (postnatal), **GAD-7** (≥ 10 clinically significant). **C-SSRS** and **SAD PERSONS** (the latter poorly predictive; avoid reliance) for suicide risk: no rule predicts suicide; structured assessment is the standard (chapter 56).
- **Substance use**: **AUDIT** (≥ 8 hazardous; ≥ 20 dependence likely), **AUDIT-C** (≥ 5 men, ≥ 4 women), **CAGE**, **CIWA-Ar** (alcohol withdrawal severity; ≥ 15 severe), **COWS** (opioid withdrawal), **DAST-10**.
- **Falls and pressure injury**: **Morse Fall Scale**, **STRATIFY**, **Braden Scale** (≤ 18 at risk).
- **Pain scales**: NRS, VAS, Wong–Baker FACES, PAINAD/Abbey (non-verbal).
- **Performance status**: **ECOG** 0–5, **Karnofsky** 100–0, **Palliative Performance Scale** (chapter 63).

---

## 9. Women's health, paediatrics and other

- **Apgar** (0–10 at 1 and 5 minutes: appearance, pulse, grimace, activity, respiration). **Bishop score** (cervical favourability for induction). **Ballard** (gestational age).
- **PECARN** rules (head, abdominal trauma in children), **Rochester/Boston criteria and the Step-by-Step approach** (febrile infants), **PAS** (appendicitis), **Westley croup score**, **Pediatric Respiratory Assessment Measure**, **Yale observation scale**; **paediatric early warning scores**; **Centor in children** (McIsaac age adjustments); **Kawasaki criteria**; **Tanner staging**.
- **Pregnancy**: **Bishop**, **pre-eclampsia risk factors** (NICE/ACOG), **MEOWS**, **Edinburgh Postnatal Depression Scale**.
- **Cancer**: **TNM staging**, **Gleason/ISUP grade**, **Nottingham prognostic index**, **Wells in cancer**, **Khorana score** (VTE risk with chemotherapy), **PHQ for oncology**.
- **Nutrition and frailty**: **MUST** (malnutrition universal screening tool), **NRS-2002**, **SARC-F**, **BMI, waist circumference**.
- **Renal**: **KDIGO AKI staging** (stage 1: creatinine ≥ 26.5 µmol/L rise within 48 h or 1.5–1.9 × baseline; stage 2: 2.0–2.9 ×; stage 3: ≥ 3.0 × or ≥ 354 µmol/L or RRT), **CKD staging** (GFR and albuminuria categories), **Cockcroft–Gault** CrCl for drug dosing: [(140 − age) × weight (kg) × 1.23 (men) or 1.04 (women)] / creatinine (µmol/L).

---

## 10. Misuse, limitations and equity

1. **Applying outside the derivation population**: PERC in pregnancy; CCHR in anticoagulated; CURB-65 in immunosuppressed; HEART in non-ED settings; Wells in inpatients (limited validation).
2. **Treating a threshold as a bright line**: a patient with CURB-65 = 1 can still need admission; Alvarado 4 can have appendicitis.
3. **"Garbage in, garbage out"**: inaccurate vital signs, undocumented history; unverified "alternative diagnosis" judgement in Wells.
4. **Over-reliance on subjective items**: e.g., "PE the most likely diagnosis" varies between clinicians.
5. **Calibration drift**: prevalence and practice change (troponin generation, COVID-19, new treatments); scores derived years ago may mis-predict.
6. **Bias and equity**: eGFR race coefficients (now removed), pulse-oximetry bias in darker skin affecting NEWS2/SOFA, under-representation of women, older adults and ethnic minorities in derivation cohorts, language/cognitive barriers in questionnaires (MMSE, PHQ-9). Use validated translations and interpret with context.
7. **Automation and alert fatigue**: electronic prompts can improve adherence but over-alerting reduces trust; clinicians remain accountable.
8. **Defensive documentation**: documenting a "low score" to justify discharge without real reasoning.
9. **Missing the rare but serious** with low-risk scores (e.g., low Wells with a clinically obvious sub-massive PE, low HEART with typical unstable angina).
10. **Over-testing despite a low-risk score**: clinicians sometimes do the test anyway ("just to be safe"), defeating the purpose.

---

## Worked cases

### Case 1: Pleuritic pain, calf tenderness and the right pathway

**Presentation.** Mr A., 52, returned from a 10-hour flight 5 days ago, now has pleuritic chest pain, calf tenderness and swelling (3.5 cm difference), HR 104, SpO₂ 95%. No haemoptysis, no cancer. He thinks it is "a pulled muscle".

**Reasoning.** Wells PE: clinical signs of DVT (3) + HR > 100 (1.5) = 4.5; PE as likely as alternatives (add 3 if judged most likely: total 7.5). Either way > 4 → "PE likely", three-tier "moderate–high". D-dimer is not useful for exclusion; PERC not applicable (HR ≥ 100, leg swelling).

**Action.** Start therapeutic anticoagulation (DOAC or LMWH) immediately if no contraindication and imaging cannot be done within 1–4 hours; CTPA to confirm PE and assess RV strain, plus compression ultrasound of the leg (a confirmed proximal DVT may by itself justify treatment); sPESI: age ≤ 80, no cancer, no chronic cardiopulmonary disease, HR 104 (< 110), SBP and SaO₂ ≥ 90% preserved → 0 = low risk (if no other concerns) → consider outpatient management with follow-up; troponin/echo if concern.

**Lessons.** Choose the pathway from the clinical probability, not from the symptom alone. When probability is high, skip D-dimer, treat early.

### Case 2: Pneumonia in an 82-year-old woman living alone

**Presentation.** Mrs B., 82, 3 days of cough and fever. Confusion absent, urea 6.8 mmol/L, RR 24, BP 118/70, SpO₂ 91%, lives alone, vomited this morning.

**Reasoning.** CURB-65: Age ≥ 65 only → score 1 (low). But hypoxaemia (91%), vomiting (cannot reliably take oral antibiotics), age 82, frailty and living alone are not captured by CURB-65. Guidelines state that severity scores support but do not replace judgement.

**Action.** Admit (or hospital-at-home), CXR, IV antibiotics initially, oxygen, hydration, review at 48 h; early mobilisation; discharge planning with social care; advance care planning discussion.

**Lessons.** Score ≠ disposition. Always integrate hypoxia, intake, comorbidity, support and frailty.

### Case 3: HEART 3, but

**Presentation.** Mr C., 44, smoker, one-hour exertional chest tightness resolved at rest, relieved with 2 minutes of rest, normal ECG, hs-troponin 4 ng/L at 0 and 1 h (normal), BP 135/85, father had MI at 50.

**Reasoning.** HEART: History highly suspicious (2), ECG normal (0), Age < 45 (0), Risk factors (smoking + family history = 2 factors → 1), Troponin normal (0) = 3 (low). Serial negative hs-troponin supports early discharge (MACE ~1–2%); however, the history is typical angina.

**Action.** Not "non-cardiac pain": arrange rapid-access chest pain clinic or CT coronary angiography/stress test within days, start aspirin/statin per assessment, safety-net (rest pain, prolonged pain, syncope), modify risk factors (smoking cessation). Document: "HEART 3, discharged with expedited outpatient testing given typical history."

**Lessons.** A low HEART score means low short-term MACE, not "no coronary disease"; plan the elective work-up.

### Case 4: AF anticoagulation and bleeding risk

**Presentation.** Mrs D., 71, hypertension, type 2 diabetes, new AF, no stroke, taking ibuprofen daily for knee OA, drinks 2 glasses of wine nightly, creatinine 95 µmol/L, SBP 150.

**Reasoning.** CHA₂DS₂-VASc: hypertension 1 + diabetes 1 + age 65–74 1 + female 1 = 4 (CHA₂DS₂-VA = 3). Anticoagulation recommended. HAS-BLED: uncontrolled hypertension (SBP > 160? no, 150 → 0), drugs (NSAID 1), alcohol (< 8 drinks/week → 0), age > 65 (1) = 2 (not high, but modifiable factors exist).

**Action.** Start a DOAC (e.g., apixaban 5 mg bd; dose reduction only if ≥ 2 of age ≥ 80, weight ≤ 60 kg, creatinine ≥ 133 µmol/L); stop ibuprofen (use paracetamol/topical), optimise BP, counsel on alcohol; consider PPI if GI risk; follow-up at 1 month; do not withhold on the basis of HAS-BLED.

**Lessons.** Use bleeding scores to modify risk factors, not to deny anticoagulation.

### Case 5: Sepsis and the false reassurance of qSOFA

**Presentation.** Ms E., 68, on chemotherapy, fever 38.9 °C, RR 20, HR 118, SBP 112, GCS 15, lactate 3.4. qSOFA = 0.

**Reasoning.** qSOFA is insensitive; SIRS positive (T, HR); lactate 3.4 mmol/L raises concern; chemotherapy → neutropenia risk. NEWS2: temp 38.9 (1), HR 118 (2), RR 20 (0), SBP 112 (0), SpO₂ 97% (0), alert (0) = 3 (low) but concern persists.

**Action.** Treat as sepsis until proven otherwise: blood cultures, FBC (ANC 0.3), broad-spectrum antibiotics within 1 hour, 30 mL/kg fluid if lactate ≥ 4 or hypotension (here 20 mL/kg bolus and reassess), repeat lactate, escalate; MASCC for neutropenia (chapter 62).

**Lessons.** No single score identifies sepsis; use clinical judgement, lactate and risk factors.

### Case 6: Knee injury and the Ottawa rule

**Presentation.** Mr F., 30, twisting football injury, knee swelling, can walk four steps, flex to 100°, no tenderness at the fibular head or patella, age < 55.

**Reasoning.** Ottawa knee rule negative (none of the five criteria): probability of fracture < 1%; radiography unnecessary. Ligament/meniscal injury is likely.

**Action.** RICE-type measures, physiotherapy, hinged knee brace if needed; review for ligamentous examination at 5–7 days (Lachman, McMurray), MRI if locked knee or persistent instability; return advice for inability to weight-bear.

**Lessons.** Rules avoid unnecessary imaging; they do not address ligament injury.

### Case 7: Appendicitis in a young woman: the score and the CT

**Presentation.** Ms G., 24, periumbilical pain migrating to the right iliac fossa 18 hours, anorexia, T 37.6 °C, WBC 13.5, RIF tenderness, no rebound; LMP 4 weeks ago, urine hCG negative.

**Reasoning.** Alvarado: migration 1 + anorexia 1 + RIF tenderness 2 + temp 1 + leukocytosis 2 = 7 (probable). In women of reproductive age, gynaecological conditions (ovarian torsion, ruptured cyst, PID, ectopic) mimic appendicitis; scores have lower specificity.

**Action.** Surgical review; ultrasound first (limited sensitivity) or CT/MRI per local practice; if confirmed, laparoscopic appendicectomy; if equivocal and score high, diagnostic laparoscopy; antibiotics-first strategy is an option in uncomplicated cases after shared decision.

**Lessons.** A score of 7 justifies imaging/surgical review; imaging reduces negative appendicectomy rates, especially in women.

---

## Common pitfalls

1. **Using a rule on the wrong patient** (outside the derivation population or setting).
2. **Misunderstanding the target**: confusing rule-out and prognostic tools; treating a diagnostic probability as a mortality estimate.
3. **Calculation errors** or incomplete data; using out-of-date versions.
4. **Ignoring the gestalt**: overriding a convincing clinical picture because of a low score.
5. **Equating "low risk" with "no risk"**; failing to safety-net.
6. **Using scores to withhold effective treatment** (HAS-BLED and anticoagulation).
7. **Applying PERC without a low gestalt probability.**
8. **Using qSOFA as a sepsis screening test.**
9. **Not repeating** the score as the patient evolves (NEWS2 trends, SOFA).
10. **Ignoring bias in inputs** (pulse oximetry, eGFR, language).
11. **Not documenting** the score, the reasoning and the plan.
12. **Over-complicating:** using many scores when a simple clinical question would suffice.

---

## Key points

- Clinical rules estimate probability or risk; they support, not replace, clinical judgement.
- Know the intended population, outcome and performance of each rule; check the current version.
- Core rules to master: Wells/PERC/YEARS, CURB-65, HEART, CHA₂DS₂-VASc/HAS-BLED, Ottawa/CCHR/NEXUS/CCR, qSOFA/SIRS/NEWS2/SOFA, Glasgow-Blatchford, Alvarado, Child-Pugh/MELD, ABCD², GCS.
- Rule-out tools need high sensitivity; use them only when pre-test probability is low enough.
- A "low-risk" score still carries residual risk: safety-net, arrange follow-up, and respect red flags.
- Bleeding scores identify modifiable risk; they do not contraindicate anticoagulation by themselves.
- Document the components, the score and your reasoning, including overrides.
- Be alert to bias, miscalibration and misuse.

---

## Self-assessment

**Questions**

1. Distinguish a rule-out rule from a prognostic score, with one example of each.
2. Calculate the Wells score for PE for a patient with HR 110, recent surgery 2 weeks ago, and no other features, with PE judged as likely as other diagnoses.
3. State the eight PERC criteria and the condition for using PERC.
4. A woman aged 76 with hypertension and diabetes and no other risk factors has AF. Calculate the CHA₂DS₂-VASc score and recommendation.
5. What is the CURB-65 score for a 68-year-old with RR 32, BP 100/62, urea 9, and normal mentation, and what does it suggest?
6. When is an ankle radiograph needed according to the Ottawa rule?
7. What does a HEART score of 3 mean, and what caveats apply?
8. Why is qSOFA unsuitable as a screening test for sepsis?
9. What is the role of HAS-BLED?
10. What are three reasons a validated rule may fail in your patient?

**Answers**

1. A rule-out rule identifies patients with such a low risk that testing/imaging can be omitted (e.g., Ottawa ankle rules, PERC); a prognostic score estimates the likelihood of an outcome to guide level of care or therapy (e.g., CURB-65, CHA₂DS₂-VASc).
2. HR > 100 (1.5) + surgery within 4 weeks (1.5) + PE equally likely (3) = 6.0 → "PE likely" (> 4) in the two-tier model, moderate in the three-tier model.
3. Age < 50; HR < 100; SaO₂ ≥ 95%; no haemoptysis; no oestrogen use; no prior DVT/PE; no unilateral leg swelling; no recent surgery/trauma needing hospitalisation within 4 weeks. Use only when gestalt pre-test probability is low (< 15%).
4. Age ≥ 75 (2) + hypertension (1) + diabetes (1) + female sex (1) = 5 (CHA₂DS₂-VA = 4): oral anticoagulation recommended.
5. Confusion 0, urea > 7 (1), RR ≥ 30 (1), BP: SBP 100 and DBP 62 (neither <90 nor ≤60) → 0, age ≥ 65 (1) = 3: severe pneumonia, hospital admission (consider high-dependency care).
6. If there is pain in the malleolar zone and bone tenderness at the posterior edge/tip of the lateral or medial malleolus, or inability to bear weight for four steps immediately and in the ED.
7. Low risk (about 1–2% 30-day MACE); safe for early discharge with serial negative hs-troponin and normal ECG, but caveats: a typical history may justify further evaluation, and outpatient testing and safety-net are needed.
8. It has low sensitivity: many septic patients have qSOFA < 2; it is a prognostic prompt, not a screening or diagnostic tool.
9. It identifies modifiable bleeding risk factors in patients on anticoagulation (BP, NSAIDs, alcohol, labile INR) for correction and closer follow-up; a high score should not by itself withhold anticoagulation.
10. Different population/setting from the derivation cohort; changed prevalence or practice (poor calibration); inaccurate or biased inputs (subjective items, measurement bias); outdated version; atypical presentation or special groups (pregnancy, children, immunosuppression).
