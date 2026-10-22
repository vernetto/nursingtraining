# Chapter 71. Flowcharts and Diagnostic Algorithms

## Learning objectives

After studying this chapter you should be able to:

1. Explain what a diagnostic algorithm is, what it does well (consistency, speed, safety) and where it fails (atypical cases, comorbidity, rigid application).
2. Read and construct a flowchart: entry criteria, decision nodes, actions, exit points, safety nets and review points.
3. Apply a "safety-first" structure to any symptom: (1) recognise the unstable patient and treat, (2) exclude the dangerous diagnoses, (3) narrow to the likely diagnosis, (4) plan follow-up.
4. Use core algorithms for common presentations: chest pain, acute dyspnoea, syncope, acute headache, acute abdominal pain, acute confusion, shock/hypotension, fever, GI bleeding, jaundice, anaemia, hyponatraemia, acute kidney injury, haematuria, haemoptysis, palpitations, weight loss, and back pain.
5. Recognise how an algorithm's branches combine pre-test probability, red flags, scores (chapter 70) and tests (chapter 69).
6. Adapt algorithms to the patient (age, pregnancy, immunosuppression, frailty, local resources) and document deviations.
7. Appraise algorithms critically (evidence base, version, local adaptation) and use them for teaching, audit and communication.

> **Note.** The flowcharts in this chapter are teaching schematics based on widely used approaches (ESC, AHA/ACC, NICE, BTS, SSC, KDIGO and similar). They are simplified: local protocols, current guidelines and specialist advice take precedence. They are written as text so they can be reproduced in notes and adapted.

---

## 1. Principles

### 1.1 What an algorithm is

An algorithm is an explicit sequence of questions and actions that leads from a starting presentation to a decision. Good algorithms embody three things: **epidemiology** (what is common and dangerous), **evidence** (which tests and treatments work), and **logistics** (what can be done now, here).

| Strengths | Weaknesses |
|---|---|
| Reduce variation and omission errors | Assume a single-problem patient |
| Make reasoning visible and teachable | Can be applied mechanically ("cookbook medicine") |
| Support junior clinicians and non-specialists | Out-of-date if not maintained |
| Enable audit and quality improvement | Rarely cover atypical presentations, multimorbidity, pregnancy, frailty |
| Provide a common language between teams | Derived in a population different from yours |

### 1.2 The universal skeleton

Almost every acute algorithm follows the same seven steps:

```
1. Immediate safety: ABCDE, monitoring, IV access, glucose, resuscitation if unstable
        |
2. Focused history + exam + red flags
        |
3. First-line tests (ECG, bedside glucose, gas, lactate, troponin, imaging as indicated)
        |
4. Is a time-critical diagnosis present or still possible?
      YES --> treat/escalate (do not wait for full work-up)
      NO  --> continue
        |
5. Narrow the differential (risk scores, further tests)
        |
6. Disposition: admit / observe / discharge, with a specific plan
        |
7. Safety net + follow-up + responsible clinician for pending results
```

### 1.3 How to read a flowchart

- **Rectangles** (actions); **diamonds** (yes/no questions); **ovals** (start/end). In text form: indented lines, "→" arrows, and "IF… THEN…" statements.
- Follow **the first red-flag exit**: if a dangerous condition is present, leave the pathway and treat.
- **Each decision needs data**: if the data are not available, the branch is not reached; choose the safest default.
- **Loops**: re-evaluate after treatment or time (response to therapy is diagnostic).

### 1.4 Building your own algorithm (for teaching or local protocol)

1. Define the **entry point** (symptom or sign) and the population (adults, ED, primary care).
2. List the **dangerous diagnoses** and their time-critical treatments.
3. Define **red flags** and the **tests** that identify each dangerous diagnosis; state their performance.
4. Use **validated rules** where they exist.
5. Add **disposition criteria** and **safety nets**.
6. Pilot, audit, update; document sources and version/date.

---

## 2. Chest pain (adult, acute, undifferentiated)

```
START: Chest pain (current or recent)
|
|-- Unstable? (shock, SBP <90, syncope, hypoxia, severe dyspnoea, ongoing pain with arrhythmia)
|     YES -> Resus: monitor, O2 if SpO2 <90%, IV access, 12-lead ECG, bedside echo/FAST, call senior
|
|-- 12-lead ECG within 10 min:
|     ST elevation / equivalent (posterior, de Winter, LBBB+Sgarbossa, hyperacute T) -> STEMI pathway: aspirin, P2Y12, anticoagulant, primary PCI (<120 min) or lysis
|     Other dangerous: VT/AV block/Brugada -> arrhythmia pathway
|
|-- Think of the "deadly six": ACS, PE, aortic dissection, tension pneumothorax, oesophageal rupture, cardiac tamponade
|     Aortic: tearing pain, pulse/BP differential, neuro deficit, wide mediastinum -> ADD-RS -> CT angiography
|     PE: Wells/PERC/YEARS -> D-dimer or CTPA
|     Pneumothorax: absent breath sounds, ultrasound/CXR -> decompress if tension
|     Tamponade: Beck's triad, effusion on echo -> pericardiocentesis
|     Oesophageal rupture: vomiting, subcutaneous emphysema -> CT contrast swallow
|
|-- hs-troponin 0 h and 1 h (or 0/2 h or 0/3 h) + ECG:
|     Rule-out (very low, no delta, >3 h from onset if single) -> low-risk: HEART <=3 -> discharge + outpatient testing
|     Rule-in (high or rising) -> NSTEMI: antiplatelets, anticoagulation, GRACE, early invasive strategy
|     Observe zone -> repeat at 3 h, imaging (CT coronary angiography), echo
|
|-- Troponin elevated but no ACS: consider myocarditis, pericarditis (PR depression, diffuse ST elevation), PE, HF, Takotsubo, sepsis, CKD, arrhythmia
|
|-- Non-cardiac causes: musculoskeletal, GI (reflux, ulcer, pancreatitis, biliary), pleuritic (pneumonia), herpes zoster, anxiety
|
END: disposition + safety net + follow-up (chest pain clinic if indicated)
```

**Key decision**: do not discharge on a single early normal ECG and troponin; use serial high-sensitivity troponin and the symptom-onset time.

---

## 3. Acute dyspnoea

```
START: Acute breathlessness
|
|-- ABCDE: SpO2, RR, HR, BP, work of breathing, silent chest, stridor, cyanosis, GCS
|     Life threat (stridor, silent chest, exhaustion, SpO2 <90% on O2, shock, altered consciousness) -> airway/oxygen/NIV/ICU, treat cause
|
|-- Rapid bedside tests: ECG, glucose, chest X-ray (or lung ultrasound), ABG/VBG, FBC, U&E, troponin, BNP, D-dimer (if low risk)
|
|-- Pattern recognition:
|     Wheeze + known asthma/COPD -> bronchodilators, steroids, ± antibiotics/NIV; CXR for pneumothorax/pneumonia
|     Orthopnoea, oedema, crackles, raised JVP, cardiomegaly/B-lines -> acute heart failure: diuretics, NIV, nitrates; look for ischaemia/arrhythmia
|     Fever, cough, consolidation -> pneumonia: CURB-65, antibiotics
|     Pleuritic pain, DVT, risk factors, clear CXR -> PE: Wells/YEARS; CTPA
|     Unilateral absent breath sounds/hyperresonance -> pneumothorax: decompress/drain
|     Stridor -> airway obstruction/anaphylaxis/epiglottitis: adrenaline IM, senior airway help
|     Metabolic acidosis (Kussmaul): DKA, sepsis, renal failure, toxins -> treat cause
|     Anaemia, thyrotoxicosis, anxiety, pregnancy-related cardiomyopathy etc. -> consider
|
|-- Persistent diagnosis unclear -> CT chest, echocardiography, bronchoscopy, specialist
```

---

## 4. Syncope and transient loss of consciousness (TLOC)

```
START: Transient loss of consciousness
|
|-- Was it syncope (rapid onset, short, spontaneous recovery) vs seizure vs other (hypoglycaemia, concussion, psychogenic)?
|
|-- Initial evaluation: history (prodrome, posture, exertion, triggers, witnesses), examination (orthostatic BP at 1 and 3 min, murmurs), 12-lead ECG, glucose
|
|-- High-risk features (admit/urgent cardiology):
|     Exertional or supine syncope; no prodrome; palpitations before syncope; family history of sudden death <50;
|     abnormal ECG (AV block II/III, bifascicular block, QTc >480-500, Brugada, pre-excitation, Q waves, LBBB, sinus brady <40, VT);
|     structural heart disease (HF, AS, HCM, prior MI), severe anaemia, GI bleed, hypotension, age >65 with comorbidity
|
|-- Low-risk: typical vasovagal (triggers: standing, heat, pain, fear), situational (cough, micturition), orthostatic (drugs, volume depletion)
|     -> reassurance, fluids/salt, counter-manoeuvres, review drugs; outpatient follow-up
|
|-- Intermediate: observation, telemetry, echocardiography, ambulatory ECG (Holter, loop recorder), tilt test
|
|-- Seizure features (tongue biting lateral, prolonged post-ictal confusion, jerks >30 s, aura) -> neurology/EEG/MRI
|
|-- Driving and safety advice per local law; documentation
```

---

## 5. Acute headache

```
START: Headache
|
|-- Red flags ("SNOOP"): Systemic (fever, cancer, HIV, pregnancy), Neurological signs, Onset sudden (thunderclap) or after 50 years, Other (trauma, positional, Valsalva), Previous headache pattern changed
|
|-- Thunderclap (peak <1 min) -> non-contrast CT head <6 h from onset (sensitivity ~100% with modern scanner and expert read);
|     if CT negative and >6 h -> LP with xanthochromia/CT angiography; consider cerebral venous thrombosis, dissection, RCVS, pituitary apoplexy
|
|-- Fever + neck stiffness/photophobia/rash/altered consciousness -> meningitis: immediate antibiotics (+ dexamethasone), CT if indicated, LP
|
|-- Age >50, jaw claudication, scalp tenderness, visual symptoms, ESR/CRP high -> giant cell arteritis: prednisolone 40-60 mg immediately, temporal artery biopsy/ultrasound within days
|
|-- Papilloedema, morning headache, vomiting -> raised ICP: MRI/CT; consider IIH (obese young woman): LP with opening pressure, visual field testing
|
|-- Post-trauma, anticoagulants -> CT head per rule
|
|-- Red eye + halos + vomiting -> acute angle-closure glaucoma: urgent ophthalmology
|
|-- Carbon monoxide: multiple household members, winter -> COHb
|
|-- No red flags: primary headache -> migraine (ICHD-3: 4-72 h, unilateral, pulsating, moderate-severe, nausea or photo/phonophobia), tension-type, cluster (trigeminal autonomic features) -> treat and plan prevention; avoid medication overuse
```

---

## 6. Acute abdominal pain

```
START: Acute abdominal pain
|
|-- Unstable? Shock, peritonism, rigid abdomen, tachycardia -> resuscitate, analgesia, IV antibiotics if sepsis, surgical review
|
|-- Think by location and dangerous causes:
|     Epigastric: ACS, pancreatitis, perforated ulcer, aortic aneurysm/dissection, oesophageal
|     RUQ: biliary colic, cholecystitis, cholangitis (Charcot: fever, jaundice, pain), hepatitis, pneumonia
|     RLQ: appendicitis, ectopic, ovarian torsion, mesenteric adenitis, Crohn, psoas abscess, hernia
|     LLQ: diverticulitis, ectopic, torsion
|     Flank: renal colic, pyelonephritis, AAA
|     Diffuse: bowel obstruction, mesenteric ischaemia (pain out of proportion), DKA, gastroenteritis
|
|-- Women of childbearing age: pregnancy test first
|
|-- Tests: FBC, CRP, U&E, LFT, lipase, glucose/ketones, lactate, urinalysis, ECG, erect CXR (if perforation suspected), ultrasound (biliary, pelvic, renal, aorta), CT abdomen/pelvis with contrast for undifferentiated severe pain
|
|-- Decisions: surgical emergency (peritonitis, obstruction with strangulation, ischaemia, perforation, ruptured AAA/ectopic) -> theatre; medical (DKA, pancreatitis, gastroenteritis); discharge with safety net if benign with improving pain
|
|-- Elderly/immunosuppressed: low threshold for CT; atypical presentations; consider mesenteric ischaemia, malignancy
```

---

## 7. Acute confusion (delirium)

```
START: Acute change in cognition/attention (4AT >= 4, CAM positive)
|
|-- Immediate: ABCDE, glucose, oxygenation, temperature, pain, urinary retention, constipation
|
|-- "I WATCH DEATH": Infection, Withdrawal, Acute metabolic, Trauma, CNS pathology, Hypoxia, Deficiencies, Endocrine, Acute vascular, Toxins/drugs, Heavy metals
|
|-- Investigations: FBC, U&E, Ca, glucose, LFT, TFTs (selected), B12, CRP, urinalysis (only with symptoms/signs), ECG, CXR, blood cultures if septic, drug review (anticholinergics, benzodiazepines, opioids, steroids), ABG, ammonia (rarely), CT head if focal signs/trauma/anticoagulants/no cause, LP if meningitis/encephalitis suspected, EEG if non-convulsive status
|
|-- Wernicke: alcohol/malnutrition + confusion, ataxia, ophthalmoplegia -> IV thiamine before glucose
|
|-- Management: treat cause; non-drug measures (orientation, glasses, hearing aids, sleep, mobilise, family); antipsychotic (haloperidol 0.5 mg) only for distress/danger; avoid benzodiazepines except withdrawal
|
|-- Differentials: dementia (insidious), depression (pseudodementia), psychosis, stroke (aphasia), non-convulsive status
|
|-- Follow-up: delirium predicts dementia; cognitive assessment after recovery (chapter 61)
```

---

## 8. Hypotension and shock

```
START: SBP <90 or MAP <65 or signs of hypoperfusion (lactate >2, mottling, oliguria, altered consciousness)
|
|-- Treat while diagnosing: airway, oxygen, 2 large IVs, monitor, ECG, glucose, bedside ultrasound (RUSH), lactate, cultures
|
|-- Identify the type by "pump, tank, pipes":
|     HYPOVOLAEMIC (haemorrhage, dehydration): cold, empty veins, small IVC -> blood/fluids, control bleeding (trauma: massive transfusion, TXA, surgery)
|     CARDIOGENIC (MI, arrhythmia, valve, myocarditis): raised JVP, pulmonary oedema, poor LV -> ECG/echo, revascularise, inotropes, treat arrhythmia, mechanical support
|     OBSTRUCTIVE (PE, tamponade, tension pneumothorax): dilated RV, effusion, absent sliding -> thrombolysis, pericardiocentesis, decompression
|     DISTRIBUTIVE (sepsis, anaphylaxis, neurogenic, adrenal crisis): warm, bounding pulse -> sepsis bundle (antibiotics <1 h, 30 mL/kg crystalloid, noradrenaline MAP >=65), anaphylaxis (IM adrenaline 0.5 mg), steroids (hydrocortisone 100 mg IV) for adrenal crisis/refractory shock
|
|-- Reassess every 15 min: MAP, lactate clearance, capillary refill, urine output; escalate to ICU
|
|-- Look for hidden: GI bleed, ruptured ectopic/AAA, occult retroperitoneal bleed, drug toxicity (beta-blocker, CCB overdose), adrenal insufficiency, hypothyroid/myxoedema
```

---

## 9. Fever: from the ED to fever of unknown origin (FUO)

```
START: Fever (>= 38.0 C)
|
|-- Sepsis screen (SIRS/NEWS2/qSOFA, lactate); immunocompromised? neutropenic? asplenic? returning traveller? pregnant? post-operative? line/device?
|
|-- Source search: head (sinuses, ears, meninges), throat, chest, abdomen, skin/soft tissue, urine, joints, lines, perineum/spine, genitalia; rash and eyes
|
|-- Tests: cultures (blood x2, urine, sputum, wound), FBC with differential, CRP/PCT, U&E, LFT, lactate, CXR, urinalysis, viral PCR, malaria film if travel
|
|-- Emergency syndromes (empirical treatment now): bacterial meningitis, sepsis/septic shock, necrotising fasciitis, neutropenic sepsis (<60 min), malaria (falciparum), endocarditis, toxic shock, severe CAP, cholangitis, spinal epidural abscess
|
|-- Persistent fever >3 weeks with no diagnosis after 3 days inpatient/3 outpatient visits = FUO (classic)
|     Causes in thirds: infection (TB, endocarditis, abscess, osteomyelitis, EBV/CMV, HIV), inflammatory (GCA, Still, vasculitis, SLE, sarcoid, IBD), neoplasm (lymphoma, renal, liver), other (drug fever, thromboembolism, factitious, periodic fever syndromes)
|     Approach: repeat history/exam (travel, animals, drugs, family, occupation), repeat cultures, imaging (CT chest/abdomen/pelvis, PET/CT), echocardiography, biopsies (temporal artery, liver, marrow, lymph node), review drugs; consider diagnostic therapeutic trials only with a plan
```

---

## 10. Gastrointestinal bleeding

```
START: Haematemesis/melaena/haematochezia
|
|-- Resuscitation: IV access x2, bloods (FBC, U&E, coagulation, group & crossmatch, lactate), restrictive transfusion (Hb <70 g/L; <80 if CVD), correct coagulopathy (PCC/vit K for warfarin; reversal agent for DOAC if life-threatening)
|
|-- Risk: Glasgow-Blatchford score; 0 -> outpatient; others -> inpatient endoscopy within 24 h (urgent <12 h if unstable)
|
|-- UPPER: IV PPI (pre-endoscopic optional), endoscopy (injection/clips/thermal), H. pylori testing; variceal suspicion (cirrhosis): terlipressin/octreotide, antibiotic prophylaxis (ceftriaxone), endoscopic band ligation, TIPS if refractory
|
|-- LOWER: haemodynamically unstable -> exclude upper source (NG/endoscopy) and CT angiography; stable -> colonoscopy after prep within 24 h; causes: diverticular, angiodysplasia, colitis, haemorrhoids, cancer
|
|-- If persistent bleeding and unlocalised: CT angiography -> interventional radiology embolisation or surgery
|
|-- Antithrombotics: hold, resume early when safe; aspirin for secondary prevention should usually continue/resume within 1-3 days
```

---

## 11. Jaundice

```
START: Raised bilirubin / clinical jaundice
|
|-- Fractionate bilirubin: unconjugated vs conjugated
|     UNCONJUGATED predominant (LFT otherwise normal): Gilbert (fasting, illness), haemolysis (retics, LDH, haptoglobin, DAT, film), Crigler-Najjar (rare)
|     CONJUGATED: hepatocellular vs cholestatic
|
|-- Pattern: ALT/AST >> ALP -> hepatocellular: viral hepatitis (A,B,C,E, EBV, CMV), drugs (paracetamol, others), alcohol, autoimmune, ischaemic, Wilson, haemochromatosis;
|     ALP/GGT >> ALT -> cholestatic: ultrasound/MRCP: dilated ducts -> obstruction (stones, tumour: ERCP/surgery; cholangitis: antibiotics + urgent drainage);
|     no dilatation -> intrahepatic: PBC (AMA), PSC, drugs, infiltrative, sepsis
|
|-- Red flags: fever + RUQ pain + jaundice (Charcot) -> cholangitis; confusion/coagulopathy -> acute liver failure (INR >=1.5 + encephalopathy): NAC, ICU, transplant centre; pregnancy third trimester (HELLP, AFLP, obstetric cholestasis)
|
|-- Tests: viral serology, autoimmune screen, immunoglobulins, ferritin, caeruloplasmin, AAT, paracetamol level, ultrasound, CT/MRCP; EUS/ERCP; liver biopsy when needed
```

---

## 12. Anaemia

```
START: Low Hb
|
|-- Stability: acute bleeding/haemodynamic compromise -> resuscitate/transfuse, find source
|
|-- MCV + reticulocytes + film + ferritin/CRP:
|     Microcytic: ferritin low -> iron deficiency -> find the blood loss (GI endoscopy/colonoscopy in men and postmenopausal women; coeliac serology; menstrual history; diet);
|                 ferritin normal/high + low TSAT -> chronic disease; thalassaemia trait (Hb electrophoresis, normal ferritin, high RBC count)
|     Normocytic: retics high -> haemolysis (LDH, bilirubin, haptoglobin, DAT, film) or blood loss; retics low -> CKD, chronic disease, marrow failure, endocrine, early iron deficiency
|     Macrocytic: B12/folate, alcohol, liver disease, hypothyroidism, drugs, MDS
|
|-- Red flags: pancytopenia, blasts, schistocytes with thrombocytopenia (TMA - emergency), leucoerythroblastic film
|
|-- Treat cause; transfuse only if symptomatic/Hb <70 g/L (<80 with cardiac disease); IV iron when oral not tolerated/ineffective or ongoing loss
```

---

## 13. Hyponatraemia

```
START: Na <135
|
|-- Check serum osmolality, glucose, lipids/protein (exclude pseudo/hypertonic)
|
|-- Hypotonic (osm <275): volume status + urine Na/osmolality:
|     Hypovolaemic: urine Na <30 -> extrarenal loss (GI, burns, third spacing) ; urine Na >30 -> renal loss (thiazide, diuretics, adrenal insufficiency, salt wasting)
|     Euvolaemic: urine osm >100 and Na >30 -> SIADH (check TSH, cortisol; causes lung, CNS, drugs, malignancy, pain) ; urine osm <100 -> primary polydipsia, low solute (beer, tea and toast)
|     Hypervolaemic: heart failure, cirrhosis, nephrotic, CKD -> treat underlying; fluid/sodium restriction, loop diuretic
|
|-- Severe symptoms (seizure, coma, vomiting with confusion): 150 mL 3% saline over 20 min (repeat x2), target rise 4-6 mmol/L in first 6 h; limit <=8-10 mmol/L/24 h
|-- Chronic, mild-moderate: treat cause; fluid restriction (SIADH), salt tablets/urea, stop offending drugs
|-- Overcorrection risk: hypokalaemia, alcoholism, malnutrition, liver disease -> monitor Na q2-4 h; if overshoot -> DDAVP + hypotonic fluid
```

---

## 14. Acute kidney injury

```
START: Creatinine rise >=26.5 umol/L in 48 h, or >=1.5 x baseline, or UO <0.5 mL/kg/h for 6 h
|
|-- Immediate: stop nephrotoxins (NSAIDs, ACEi/ARB, aminoglycosides, contrast, SGLT2i when unwell), review doses, check K, acidosis, fluid status, bladder scan
|
|-- Hyperkalaemia with ECG changes -> calcium gluconate IV, insulin + dextrose, salbutamol; pulmonary oedema/acidosis/uraemic pericarditis/refractory -> dialysis
|
|-- PRE-RENAL (volume depletion, hypotension, HF, cirrhosis): fluids/vasopressors as indicated; FeNa <1%, FeUrea <35%
|-- INTRINSIC: ATN (sepsis, toxins, contrast; muddy brown casts, FeNa >2%), AIN (drugs, eosinophiluria, rash), glomerulonephritis (haematuria, RBC casts, proteinuria, hypertension: nephritic -> urgent nephrology, biopsy), vasculitis, rhabdomyolysis (CK), TMA, myeloma (free light chains)
|-- POST-RENAL: ultrasound for hydronephrosis, catheter for retention, nephrostomy/stent for upper tract obstruction
|
|-- Tests: urine dip/microscopy, ACR/PCR, renal ultrasound, CK, complement, ANCA/ANA/anti-GBM, immunoglobulins/free light chains, hepatitis B/C/HIV
|-- Follow-up: eGFR/ACR at 3 months (AKI-to-CKD), medication review, sick-day rules
```

---

## 15. Haematuria

```
START: Visible (macroscopic) or non-visible haematuria (>=3 RBC/hpf microscopy)
|
|-- Symptomatic UTI? treat; repeat urinalysis in 6 weeks; persistent -> investigate
|-- Glomerular signs (dysmorphic RBCs, red cell casts, proteinuria, hypertension, raised creatinine) -> nephrology
|-- Risk of urothelial cancer (age >=40-45, smoking, occupational exposure, visible haematuria, previous radiation): cystoscopy + imaging (CT urogram or ultrasound + alternative per local protocol)
|-- Visible haematuria painless -> urgent urology referral (2-week wait in UK)
|-- Loin pain + haematuria -> stone: low-dose CT KUB; infection + obstruction -> urgent decompression
|-- Anticoagulation does not explain haematuria; investigate anyway
|-- Exclude non-urological (menstrual blood, myoglobinuria, beeturia, drugs: rifampicin)
```

---

## 16. Haemoptysis

```
START: Coughing blood
|
|-- Massive (>100-600 mL/24 h or any airway compromise): ABC, position bleeding lung down, protect airway (selective intubation), CT angiography, bronchoscopy, bronchial artery embolisation
|-- Non-massive: CXR, FBC, coagulation, U&E, urinalysis (vasculitis), sputum (AFB, culture)
|     Causes: bronchitis, pneumonia, bronchiectasis, TB, lung cancer (smokers >40), PE, vasculitis/Goodpasture, mitral stenosis, aspergilloma, cocaine
|-- CT chest (contrast) if CXR abnormal or high-risk (smoker, age >40, >30 pack-years) even if CXR normal
|-- Bronchoscopy when CT suggests endobronchial lesion or cause unclear
|-- Stop anticoagulants if possible; tranexamic acid (inhaled or oral); treat infection; refer urgently for suspected cancer
```

---

## 17. Palpitations and arrhythmia

```
START: Palpitations / fast or irregular pulse
|
|-- Unstable (SBP <90, chest pain, HF, reduced consciousness) -> synchronised DC cardioversion (VT/SVT/AF); pulseless -> ALS
|
|-- 12-lead ECG:
|     Narrow regular -> vagal manoeuvres -> adenosine 6/12 mg -> if recurs, EP referral; if flutter 2:1 suspect -> rate control/cardioversion
|     Narrow irregular -> AF (pre-excitation? avoid AV blockers) -> rate/rhythm control, CHA2DS2-VASc, cause (thyroid, alcohol, sepsis, PE)
|     Wide regular -> VT until proven otherwise -> amiodarone/cardioversion; avoid verapamil
|     Wide irregular -> AF with BBB or pre-excited AF (WPW) -> procainamide/cardioversion; avoid AV nodal blockers
|     Polymorphic with long QT -> torsades -> magnesium 2 g IV, correct K, pacing
|
|-- Intermittent palpitations with normal ECG: Holter (24-72 h), patch (7-14 d), event recorder, loop recorder; TSH, FBC, electrolytes, echo; lifestyle (caffeine, alcohol, stimulants, anxiety)
```

---

## 18. Unintentional weight loss

```
START: >5% body weight in 6-12 months, unintentional
|
|-- Confirm (measured weights); quantify appetite/intake; screen drugs, alcohol, depression, dentition, dysphagia, social/economic factors
|-- Examination: cachexia, lymph nodes, abdomen, rectal/breast/thyroid/skin as indicated
|-- Baseline tests: FBC, CRP/ESR, U&E, LFT, calcium, glucose/HbA1c, TSH, ferritin, coeliac serology, HIV, urinalysis, CXR, FIT (if bowel symptoms), faecal calprotectin as relevant
|-- If normal and still unexplained: CT chest/abdomen/pelvis, endoscopy, further based on age/symptoms; review in 4-6 weeks
|-- Common causes: malignancy, depression, dementia, hyperthyroidism, diabetes (uncontrolled), COPD/HF cachexia, malabsorption, TB, HIV, chronic infection, medications
|-- 2-week-wait/urgent cancer referral pathways for red-flag combinations
```

---

## 19. Acute low back pain

```
START: Back pain
|
|-- Red flags: age <20 or >55 new onset, trauma, cancer history, fever/immunosuppression/IV drug use, weight loss, night/rest pain, progressive neuro deficit,
|     saddle anaesthesia, bladder/bowel dysfunction (cauda equina), severe/inflammatory pain (>3 months, <40 y, morning stiffness)
|-- Cauda equina / cord compression -> emergency MRI + neurosurgery
|-- Suspected infection (discitis/epidural abscess): MRI with contrast, ESR/CRP, cultures
|-- Suspected malignancy: MRI, myeloma screen, PSA (men), imaging
|-- Fracture (osteoporosis, steroids, trauma) -> X-ray/CT
|-- Abdominal causes: AAA, pancreatitis, renal colic -> examine, ultrasound
|-- No red flags: non-specific back pain -> stay active, analgesia (NSAID short course), physiotherapy, avoid imaging; review at 2-4 weeks; psychosocial yellow flags (STarT Back)
|-- Radiculopathy: usually improves in 6-12 weeks; MRI if persistent beyond 6 weeks and surgery considered or progressive deficit
```

---

## 20. How to use algorithms safely

1. **Check the entry criteria** (population, setting).
2. **Complete the immediate safety step** first.
3. **Use the algorithm as the backbone, add the patient's reality**: comorbidity, drugs, preferences, resources.
4. **Treat dangerous conditions on suspicion** (sepsis, meningitis, GCA, ACS) without waiting for algorithm completion.
5. **Document the pathway used**, the findings at each node, and reasons for deviation.
6. **Safety-net** (chapter 73) at every exit.
7. **Audit**: outcomes, missed diagnoses, inappropriate discharges, over-testing.
8. **Update**: guideline versions change (troponin pathways, D-dimer thresholds, AF scores).
9. **Teach the logic, not just the arrows**: understand why each branch exists, so that you can reason when the patient does not fit.

---

## Worked cases

### Case 1: An algorithm that almost failed

**Presentation.** Mr A., 66, 2 hours of epigastric discomfort and nausea. ECG normal, hs-troponin 0 h below the rule-out threshold. The ED pathway classifies him as rule-out, and he is discharged with "dyspepsia". He returns 4 hours later with pain, ST elevation in V1–V4 and troponin of 900 ng/L.

**Reasoning.** The pathway's single-troponin rule-out applies only when symptom onset is **> 3 hours** before sampling (assay dependent); he presented at 2 hours (too early), and the 1-hour sample was skipped. Anchoring on a benign presentation compounded the miss.

**Action (for the system).** Enforce the time-from-onset checkbox and serial sampling; add decision-support prompts; train for atypical presentations (diabetes, women, older adults). Personal: apply the pathway literally; if in doubt, repeat the ECG and troponin.

**Lessons.** An algorithm's entry criteria and timing conditions matter as much as its branches.

### Case 2: A patient who fits two algorithms

**Presentation.** Mrs B., 74, acute dyspnoea and leg swelling; CXR with pulmonary congestion; BNP 1200; D-dimer 1600. Diuretics improve the breathlessness but SpO₂ remains 92%.

**Reasoning.** Heart failure explains the congestion, but elevated D-dimer is non-specific in HF, age and inflammation. If improvement is incomplete and risk factors for PE exist (recent immobility, asymmetric leg swelling), PE remains possible. The dyspnoea algorithm requires reassessing after treatment ("response to therapy is diagnostic").

**Action.** Calculate Wells (asymmetric swelling +3), leg compression ultrasound reveals DVT → start anticoagulation; echo for RV strain and LV function; treat HF aetiology (ischaemia, AF); no need for CTPA if DVT confirmed and treatment is the same.

**Lessons.** Patients can have two diagnoses; algorithms address one presenting problem at a time; re-enter the algorithm when the response is incomplete.

### Case 3: Thunderclap headache with a normal CT at 9 hours

**Presentation.** Ms C., 41, sudden worst headache, 9 hours ago; CT head normal; neck stiffness mild.

**Reasoning.** The "< 6 hours" rule for CT sensitivity does not apply; sensitivity declines with time. Pathway: LP at ≥ 12 hours from onset for xanthochromia (spectrophotometry), or CT angiography to look for aneurysm; consider other causes (RCVS, cerebral venous thrombosis, dissection).

**Action.** CT angiography and LP at 12 hours (xanthochromia and RBC count tubes 1 and 4); neurosurgical contact if positive.

**Lessons.** Algorithms with time windows demand accurate timing in the history.

### Case 4: Hyponatraemia algorithm applied to a runner

**Presentation.** Marathon runner, 38, collapse near the finish, seizure, Na 123 mmol/L, drank large volumes of water.

**Reasoning.** Exercise-associated hyponatraemic encephalopathy (overdrinking with non-osmotic ADH release). Severe symptoms mandate immediate hypertonic saline without waiting for further tests; no fluid restriction delay.

**Action.** 100–150 mL 3% saline bolus IV (repeat up to twice at 10-minute intervals) until symptoms improve; monitor Na; cause is water excess; recovery usually rapid with low risk of overcorrection.

**Lessons.** The severe-symptom branch overrides the diagnostic algorithm.

### Case 5: Fever of unknown origin that was not infectious

**Presentation.** Mr D., 70, 5 weeks of fever (to 39 °C), night sweats, weight loss, headache, CRP 120, ESR 98. Cultures negative, CT chest/abdomen/pelvis normal, echocardiogram normal.

**Reasoning.** FUO in older adults: giant cell arteritis and PMR are leading non-infectious causes; temporal artery signs may be absent. Algorithm step: biopsies and imaging for vasculitis.

**Action.** Temporal artery ultrasound/biopsy; PET/CT shows large-vessel vasculitis (aortitis); start prednisolone 40–60 mg daily with bone and gastric protection; refer to rheumatology.

**Lessons.** In FUO, consider the three thirds; repeat history; PET/CT can reveal large-vessel vasculitis and occult sources.

### Case 6: Following the AKI pathway and finding glomerulonephritis

**Presentation.** Ms E., 32, creatinine 310 µmol/L (baseline 70) after a sore throat 2 weeks ago, blood pressure 160/100, tea-coloured urine, ankle oedema. Urine dipstick: blood +++, protein ++; microscopy: red cell casts; ultrasound: normal-sized kidneys, no hydronephrosis.

**Reasoning.** Intrinsic renal AKI with nephritic syndrome: post-infectious glomerulonephritis, IgA nephropathy, or crescentic GN (ANCA, anti-GBM, lupus). The algorithm's glomerulonephritis branch mandates urgent nephrology involvement and serology.

**Action.** ANA, dsDNA, C3/C4, ANCA, anti-GBM, ASOT/anti-DNase B, hepatitis B/C, HIV, immunoglobulins; blood pressure control, fluid balance; renal biopsy (urgent if rapidly progressive); methylprednisolone ± cyclophosphamide/rituximab if crescentic disease or vasculitis; plasma exchange for anti-GBM or severe ANCA with pulmonary haemorrhage.

**Lessons.** A normal ultrasound and no obstruction/volume depletion point to intrinsic disease; haematuria with casts points to glomerular disease. Time matters.

---

## Common pitfalls

1. **Using the wrong algorithm** (wrong population or setting) or an outdated one.
2. **Skipping the safety step**: starting the work-up before stabilising.
3. **Algorithm tunnel vision**: failing to consider a second diagnosis or atypical presentation.
4. **Ignoring entry conditions** (time since onset, age, pregnancy, anticoagulation).
5. **Using an algorithm to avoid thinking**; not recognising when the patient "does not fit."
6. **Not documenting** the pathway or deviations.
7. **Incomplete data** leading to default "low-risk" branch.
8. **No safety net** at the exit; no responsible clinician for pending tests.
9. **Not reassessing** after treatment.
10. **Over-reliance on a single test in the algorithm** (D-dimer, troponin, CT).
11. **Failing to adapt for frailty, language, social context**.
12. **Not auditing or updating** local protocols.

---

## Key points

- Algorithms make reasoning explicit and reduce error, but only if applied to the right patient and completed at each node.
- Always start with immediate safety, then exclude the dangerous diagnoses before refining.
- Time-critical conditions (STEMI, sepsis, meningitis, GCA, tension pneumothorax, ruptured AAA/ectopic) are treated on suspicion.
- Learn the common algorithms for chest pain, dyspnoea, syncope, headache, abdominal pain, confusion, shock, fever, GI bleeding, jaundice, anaemia, hyponatraemia, AKI, haematuria and haemoptysis.
- Re-enter the pathway when the response to treatment is incomplete or new findings emerge.
- Document, safety-net, follow-up, audit and update.

---

## Self-assessment

**Questions**

1. List the seven steps of the universal acute-care skeleton.
2. In a chest pain algorithm, name the six "deadly" diagnoses and one test or finding for each.
3. What is the role of time since symptom onset in single-troponin rule-out?
4. Describe the first-line approach to a hypotensive patient using "pump, tank, pipes".
5. In syncope, which features define high risk requiring admission?
6. What is the correct treatment of symptomatic severe hyponatraemia?
7. How do you approach haematuria in a 58-year-old smoker with visible painless haematuria?
8. In AKI, what findings point to a glomerular cause, and what are the urgent actions?
9. What conditions are treated before diagnostic confirmation in suspected fever with neck stiffness and rash?
10. Why must an algorithm be adapted to the individual patient?

**Answers**

1. Immediate safety/resuscitation; focused history, examination and red flags; first-line tests; ask whether a time-critical diagnosis is present or possible and treat; narrow the differential with scores/tests; disposition; safety net and follow-up.
2. ACS (ECG, serial troponin); PE (Wells/D-dimer/CTPA); aortic dissection (ADD-RS, CT angiography); tension pneumothorax (clinical, ultrasound, decompress); oesophageal rupture (history of vomiting, subcutaneous emphysema, CT with contrast); tamponade (Beck's triad, echo).
3. Single very-low troponin rules out MI only if symptom onset was long enough before sampling (typically ≥ 3 hours for many assays); earlier samples require serial testing (0/1 h or 0/3 h).
4. Pump: ECG/echo for LV function, tamponade, RV strain; Tank: IVC, lungs, abdomen/FAST, bleeding or fluid loss; Pipes: aorta (AAA/dissection) and veins (DVT); then target treatment (blood, fluids, vasopressors, pericardiocentesis, thrombolysis, antibiotics, etc.).
5. Exertional/supine syncope, no prodrome, palpitations, family history of sudden death, abnormal ECG (AV block, bifascicular block, long QT, Brugada, pre-excitation), structural heart disease/HF, severe anaemia or bleeding, hypotension, older age with comorbidity.
6. 150 mL of 3% saline over 20 minutes (repeat up to twice) to raise Na by 4–6 mmol/L, limit correction to ≤ 8–10 mmol/L in 24 hours, monitor Na every 2–4 hours; treat the cause.
7. Urgent urology referral for cystoscopy and upper tract imaging (CT urogram or alternative), exclude infection/stone and glomerular causes; check coagulation/anticoagulants but investigate regardless.
8. Dysmorphic RBCs, red cell casts, proteinuria, hypertension, oedema, rapidly rising creatinine; urgent nephrology, serology (ANCA, anti-GBM, ANA, complement), renal biopsy, treatment of hypertension/fluid, immunosuppression/plasma exchange as indicated.
9. Suspected bacterial meningitis/meningococcaemia: immediate IV antibiotics (ceftriaxone ± vancomycin, add ampicillin if risk for Listeria) and dexamethasone, resuscitation, cultures; LP/imaging should not delay treatment.
10. Algorithms are derived from populations and typical presentations; individual comorbidity, pregnancy, frailty, drugs, preferences and resources alter risk and options; the clinician must reason, deviate when justified, and document.
