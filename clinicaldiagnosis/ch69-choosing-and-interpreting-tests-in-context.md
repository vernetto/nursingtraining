# Chapter 69. Choosing and Interpreting Tests in Context

## Learning objectives

After studying this chapter you should be able to:

1. State the purpose of a diagnostic test (change probability, change management) and ask "What will I do differently with the result?" before ordering.
2. Estimate pre-test probability from prevalence, presentation, risk factors and clinical prediction rules, and update it with likelihood ratios (Bayes' theorem, Fagan nomogram).
3. Explain the test threshold and treatment threshold, and use them to decide whether to test, treat or do nothing.
4. Choose between sensitive tests (rule-out) and specific tests (rule-in), single tests and sequential strategies, and between imaging modalities.
5. Interpret continuous results (ROC curves, cut-offs), borderline values, regression to the mean and the effects of repeat testing.
6. Recognise biases in test evaluation (spectrum, verification, incorporation) and in clinical use (anchoring, confirmation, availability, premature closure).
7. Manage incidental findings ("incidentalomas"), overdiagnosis, false positives and the cascade effect, including screening versus case finding.
8. Apply cost, harm (radiation, invasive risk), patient preference and shared decision-making to test choices; know the principles of "Choosing Wisely" and low-value care.
9. Communicate probabilistic results and uncertainty to patients and colleagues.

> **Note.** The numerical examples are teaching illustrations. Real sensitivities, specificities and prevalences depend on population, setting and test generation.

---

## 1. Why test? The purpose of diagnostic testing

A test is justified only if its result can change **what you do** or **what the patient understands and decides**. Reasons to test:

| Purpose | Example |
|---|---|
| **Diagnosis** (confirm/exclude) | Troponin for suspected MI; CT pulmonary angiography for PE |
| **Severity and staging** | Creatinine in AKI; CT staging in cancer |
| **Prognosis** | BNP in heart failure; PSA kinetics |
| **Monitoring** | HbA1c, INR, viral load, tumour markers |
| **Screening** (asymptomatic) | Mammography, colorectal FIT, cervical HPV testing |
| **Safety / pre-procedure** | Pregnancy test before CT; coagulation before surgery in bleeding history |
| **Reassurance** (use with caution) | Normal imaging for headache in a worried patient; may increase anxiety if results are borderline |
| **Medicolegal / documentation** | Rarely a valid reason: defensive testing inflates harm and cost |

Before each request ask: (1) What am I trying to find out? (2) How likely is it (pre-test probability)? (3) How accurate is the test for this patient? (4) Will the result change management? (5) What are the harms and costs? (6) What does the patient want?

---

## 2. Probability and Bayesian reasoning

### 2.1 Pre-test probability

The pre-test probability (PTP) is your estimate of disease before the test. Sources:

1. **Base rate (prevalence) in the setting**: PE in an unselected emergency patient with dyspnoea ≈ 5–10%; in a patient with unilateral leg swelling and recent surgery, much higher.
2. **Clinical features** (symptoms, signs, risk factors) via gestalt and **clinical prediction rules**: Wells (DVT, PE), PERC, Geneva, HEART, CURB-65, Centor, Ottawa rules (chapter 70).
3. **Local epidemiology**: season (influenza, RSV), outbreaks, endemic infections, travel.
4. **Response to previous tests/treatment** (sequential testing).

Clinicians often over- or under-estimate PTP. Anchoring on a vivid diagnosis (e.g., rare conditions) inflates it; neglecting base rates ("zebra retreat" vs "horses") deflates it. Prediction rules calibrate intuition.

### 2.2 Updating with likelihood ratios

**Odds form of Bayes' theorem**: post-test odds = pre-test odds × likelihood ratio (LR).

- Odds = p/(1 − p); probability = odds/(1 + odds).
- LR+ = sensitivity / (1 − specificity); LR− = (1 − sensitivity) / specificity.
- Rules of thumb for the change in probability (McGee): LR 2 ≈ +15%, 5 ≈ +30%, 10 ≈ +45%; LR 0.5 ≈ −15%, 0.2 ≈ −30%, 0.1 ≈ −45% (valid for mid-range probabilities).

| LR+ | Effect | LR− | Effect |
|---|---|---|---|
| > 10 | Large, often conclusive | < 0.1 | Large, often conclusive |
| 5–10 | Moderate | 0.1–0.2 | Moderate |
| 2–5 | Small | 0.2–0.5 | Small |
| 1–2 | Minimal | 0.5–1 | Minimal |

**Worked calculation.** Test with sensitivity 90%, specificity 80%: LR+ = 0.9/0.2 = 4.5; LR− = 0.1/0.8 = 0.125.
- Pre-test 10% (odds 0.111): positive → odds 0.5 → **33%**; negative → odds 0.0139 → **1.4%**.
- Pre-test 50% (odds 1): positive → odds 4.5 → **82%**; negative → odds 0.125 → **11%**.
- Pre-test 90% (odds 9): positive → odds 40.5 → **98%**; negative → odds 1.125 → **53%** (a negative result barely helps).

**Principle:** a test result is most informative when the pre-test probability is intermediate; at the extremes, it rarely changes the decision. **A test should not be ordered if no plausible result would cross a decision threshold.**

### 2.3 Predictive values and prevalence

PPV and NPV depend on prevalence. For a test with sensitivity 95% and specificity 95%: prevalence 1% → PPV 16%, NPV 99.95%; prevalence 20% → PPV 83%, NPV 98.7%; prevalence 50% → PPV 95%, NPV 95%. Screening programmes must therefore weigh the false positives generated in low-prevalence populations.

### 2.4 Sequential and parallel testing

- **Series (confirmatory) testing**: require both tests positive. Raises specificity, lowers sensitivity (e.g., HIV screening immunoassay then confirmatory assay).
- **Parallel testing**: either positive. Raises sensitivity, lowers specificity (e.g., ECG + troponin for MI exclusion).
- **Reflex testing and algorithms** reduce unnecessary tests (e.g., TSH then free T4 if abnormal; Hb and ferritin).
- Tests are rarely independent: repeating a test with the same error mechanism (e.g., interference) does not add information; use a different method.

---

## 3. Thresholds: when to test, treat, or wait

### 3.1 The Pauker–Kassirer thresholds

Consider two thresholds on the probability of disease:

- **Test threshold (T_test)**: below this, the probability is so low that testing does not help (risk of false positives exceeds benefit): do nothing.
- **Treatment threshold (T_treat)**: above this, probability is high enough that treatment benefits outweigh harms: treat without further testing.
- Between the two: test, then act on the result.

The treatment threshold is determined by **benefit/harm ratio of treatment**: treatments with high benefit and low risk (antibiotics for meningitis, aspirin in suspected MI) have a low threshold; risky treatments (thrombolysis, chemotherapy, surgery) have a high threshold. The test threshold depends on the test's harm and accuracy.

**Example**: Suspected PE. Anticoagulation harm is moderate; CTPA harms are small but non-zero (radiation, contrast, incidental findings, overdiagnosis of subsegmental PE). Wells-based approach: low probability + PERC negative → no test; low/intermediate + D-dimer → test; high probability → imaging (or empirical anticoagulation if imaging delayed).

### 3.2 Applying thresholds

1. Estimate probability.
2. Ask how large the net benefit of treating a true case is vs the harm of treating a non-case.
3. Ask how accurate and how harmful the test is.
4. Decide: observe, test (which one), or treat.

Examples:
- **Sepsis**: the treatment threshold is low (benefit of early antibiotics large; harm modest): do not wait for tests.
- **Appendicitis in a young man with classical signs**: probability high → surgical review; imaging optional in young men with classic presentation, but valuable in women of reproductive age and atypical cases.
- **Low-risk chest pain with normal serial troponins** and low HEART score: stop testing (below test threshold).
- **Back pain without red flags**: no imaging (probability of serious pathology < 1%; imaging finds incidental degenerative changes and leads to overtreatment).

---

## 4. Choosing the right test

### 4.1 Sensitive tests rule out; specific tests rule in

- **SnNout**: a highly **sens**itive test, when **n**egative, rules **out** (e.g., D-dimer in low probability; hs-troponin at 0/1 hour; urine dipstick nitrite and LE in a young woman with UTI symptoms).
- **SpPin**: a highly **spec**ific test, when **p**ositive, rules **in** (e.g., rhomboid lung point for pneumothorax; positive urinary Legionella antigen; positive culture of a sterile site).
- Tests are good at one direction; look at LR+ and LR−, not sensitivity/specificity alone.

### 4.2 Questions to ask about a test

1. **Is the test valid and reliable** in this population (spectrum, setting, device)?
2. **What is the reference standard**, and was it applied to all (verification bias)?
3. **Does the test change the post-test probability enough to cross a threshold?**
4. **What is the turn-around time**, availability and cost?
5. **What are the harms** (invasive, radiation, contrast, false positives leading to cascades)?
6. **Is there a better alternative** (ultrasound vs CT, MRI vs CT, observation, trial of therapy)?
7. **Is the patient willing** to undergo it and to act on the result?

### 4.3 Imaging selection principles

| Question | Best first test (typical) | Reason |
|---|---|---|
| Pneumothorax, effusion, pulmonary oedema (bedside) | Chest radiograph or lung ultrasound | Quick, adequate |
| Pulmonary embolism | Clinical probability → D-dimer → CTPA (V/Q if renal failure/contrast allergy/young women) | Balance harms |
| Acute appendicitis (child, pregnant) | Ultrasound → MRI | Avoid radiation |
| Appendicitis (adult) | CT abdomen/pelvis | Higher accuracy |
| Renal colic | Low-dose non-contrast CT; ultrasound in pregnancy/children | Detect stones |
| Subarachnoid haemorrhage (≤ 6 h from onset) | Non-contrast CT head (high sensitivity within 6 h with modern scanners and expert reading) | Possible LP if later |
| Stroke | Non-contrast CT (exclude haemorrhage) → CT angiography ± perfusion/MRI | Time-critical |
| Back pain with cord compression signs | MRI whole spine | Visualises cord |
| Knee/ankle trauma | Clinical decision rules (Ottawa) → X-ray | Avoids 60–80% of films |
| Head injury | Canadian CT head rule, NICE criteria | Targeted CT |
| Suspected aortic dissection | CT angiography (or TOE if unstable/renal failure) | Speed and accuracy |
| Soft-tissue/joint pathology | Ultrasound/MRI | Better soft-tissue contrast |
| Staging cancer | CT ± PET/CT, MRI as indicated | Specific protocols |
| Neurological (dementia, epilepsy) | MRI | Sensitivity |

### 4.4 Laboratory tests: focused rather than panels

- **Targeted sets**: troponin + ECG for chest pain; creatinine + K for suspected AKI; TSH for fatigue; FBC + ferritin for anaemia; HbA1c for diabetes.
- **Avoid "routine" panels** without indication (preoperative tests in low-risk surgery, admission "screens", "tick-box" requests).
- **Order in sequence** when the result changes the next step (e.g., TSH first, FT4 only if abnormal).
- **Timing**: draw troponin at presentation and at defined intervals; cultures before antibiotics; drug levels at trough; cortisol at 9 a.m.; avoid tests that reflect transient illness (thyroid function in acute illness, iron studies during inflammation).

### 4.5 Treat the patient, not the test

A "trial of therapy" can be a diagnostic strategy (e.g., PPI for reflux, bronchodilator reversibility, steroid for suspected PMR, iron for iron deficiency), and sometimes the **best test is time** (watchful waiting with safety-netting, chapter 73).

---

## 5. Interpreting results

### 5.1 Reference intervals, cut-offs and continuous variables

- Continuous tests have no natural threshold: a **cut-off** trades sensitivity for specificity. Lowering the cut-off increases sensitivity (fewer false negatives) and decreases specificity.
- **ROC curve**: plots sensitivity vs 1 − specificity; **AUC** summarises discrimination (0.5 = chance, 0.7–0.8 acceptable, 0.8–0.9 good, > 0.9 excellent). The optimal cut-off depends on the clinical consequences of false positives vs false negatives (e.g., screening favours high sensitivity; confirming before major surgery favours high specificity).
- **Multilevel LRs** use result strata (e.g., ferritin < 15: LR+ 51 for iron deficiency; 15–45: 8.8; 46–100: 2.5; > 100: 0.1) and are more informative than a dichotomy.
- **Age/sex/ethnicity-adjusted** thresholds (D-dimer age-adjusted, hs-troponin sex-specific, eGFR race-free equations, haemoglobin).

### 5.2 Variation, regression to the mean and repeat testing

- **Biological and analytic variation**: repeat results differ even in stable patients. For many analytes (creatinine, ALT) the reference change value (RCV) is ~15–40%: smaller changes may be noise.
- **Regression to the mean**: an extreme first measurement (e.g., blood pressure, cholesterol, ALT) tends to be closer to average at retest. Confirm before labelling (hypertension: repeat measurements, ambulatory or home BP).
- **Repeating tests**: useful when the first result was unexpected or borderline and the condition could change; not helpful if repeated hoping for a different answer ("test shopping"). In serial testing (troponin), look at **change**, not just the single value.

### 5.3 Borderline and "grey-zone" results

For results near the threshold, rely on pre-test probability, clinical course and other tests. Options: repeat, use an orthogonal test, observe with defined review, or treat on clinical grounds. Document reasoning.

### 5.4 Interpreting multiple results

Probability estimates for multiple findings cannot be simply multiplied when they are correlated (e.g., fever, CRP, tachycardia in sepsis). Be sceptical of "collecting positives." Beware of the **multiple comparisons problem**: the more tests, the more chance of an incidental abnormality (chapter 64: 64% chance with 20 tests).

### 5.5 Negative and positive "in context"

- **Negative result** + high clinical suspicion = consider a false negative (technique, timing, spectrum, sampling error); consider further testing or treatment.
- **Positive result** + low clinical suspicion = consider a false positive (cross-reaction, contamination, colonisation, incidentaloma); confirm before acting.
- **Discordance** between tests and clinical picture: first check pre-analytical errors (patient identity, sample timing), then reconsider the diagnosis.

---

## 6. Biases and cognitive pitfalls in testing

### 6.1 Study-level biases (affect published accuracy)

| Bias | Description | Effect |
|---|---|---|
| **Spectrum bias** | Test evaluated in extremes (sick vs healthy), not in the real mix | Overestimates accuracy |
| **Verification (work-up) bias** | Only test-positive patients receive the reference standard | Inflates sensitivity, deflates specificity |
| **Incorporation bias** | The test is part of the reference standard | Inflates accuracy |
| **Publication bias, selective reporting** | Positive studies get published | Overestimates utility |
| **Lead-time and length bias, overdiagnosis** (screening) | Earlier detection appears to prolong survival without benefit; slow-growing cancers over-represented | Overestimates screening benefit |

### 6.2 Clinician-level cognitive biases

- **Anchoring**: sticking to the first impression.
- **Confirmation bias**: seeking and valuing data that support the favoured diagnosis.
- **Availability**: recent or memorable cases inflate perceived probability.
- **Premature closure**: stopping once a diagnosis fits.
- **Framing / diagnostic momentum**: a label (from previous notes or triage) carries forward.
- **Overconfidence**; **posterior probability error** (assuming the next patient will have the same diagnosis as the last); **base-rate neglect**; **representativeness**; **search satisficing**; **order effects**.
- **Test-driven medicine** or **"treating the number"**: performing or acting on tests without reasoning.
- **Defensive medicine**: tests ordered to protect the clinician.

**Countermeasures**: state PTP explicitly; list a differential and what would change it; ask "what else could this be?"; use cognitive forcing strategies (e.g., "worst-case first"), checklists, second opinions and diagnostic time-outs; reflect on misses.

---

## 7. Incidental findings, overdiagnosis and cascades

### 7.1 Incidentalomas

Findings unrelated to the clinical question: adrenal nodules (up to 5% of CT scans), thyroid nodules (up to 50% on ultrasound in adults), pulmonary nodules (up to 30% of CT chest), renal cysts, pituitary lesions, liver haemangiomas, brain white-matter hyperintensities, disc bulges, degenerative spine changes, carotid plaques, coronary calcium, "unspecific" ECG changes, mildly abnormal labs.

**Approach**: (1) Is it clinically significant? Use evidence-based algorithms (Fleischner for lung nodules; ACR white papers for adrenal, renal, thyroid, liver, pancreas incidentals). (2) Estimate malignancy risk and decide on surveillance versus ignoring. (3) Discuss with the patient (anxiety, insurance, cost). (4) Document the plan and follow-up responsibility. (5) Avoid cascades.

### 7.2 Overdiagnosis and overtreatment

Overdiagnosis is detection of "disease" that would never have caused symptoms or death (e.g., a proportion of screen-detected breast and prostate cancers, thyroid papillary microcarcinoma, subsegmental PE, mild hypertension in the very old, low-grade DCIS). It harms through anxiety, overtreatment complications and cost. Newer, more sensitive tests (CT, high-sensitivity assays) increase it. Screening programmes should demonstrate net mortality or quality-of-life benefit in randomised trials.

### 7.3 The cascade effect

An incidental or false-positive result triggers further tests, procedures and complications (the "Ulysses syndrome"). Example: a mildly raised ALT leads to ultrasound, which shows a liver cyst, then CT, then MRI, then biopsy with a bleeding complication. Break the cascade by asking at each step whether the next test will change management, discussing with the patient, and being comfortable with watchful waiting.

### 7.4 Screening vs case-finding vs diagnostic testing

- **Screening**: asymptomatic population; requires a condition that is important, has a detectable pre-clinical phase, an accepted treatment that improves outcomes when started earlier, an acceptable test, adequate resources (Wilson–Jungner criteria). Harms (false positives, overdiagnosis, incidental findings, radiation) are borne by many for the benefit of few. Use shared decision-making with absolute numbers (e.g., per 1000 screened).
- **Case-finding**: targeted at those at higher risk (e.g., HbA1c in obesity, HIV testing in indicator conditions, AF pulse palpation in > 65).
- **Diagnostic testing**: symptomatic patients, higher PTP.
- Do not apply screening tests to symptomatic patients as if the screening characteristics hold (e.g., a negative FIT in someone with rectal bleeding should not stop investigation per guidelines: use diagnostic pathways).

---

## 8. Harms, value and patient-centred testing

### 8.1 Harms of testing

| Type | Examples |
|---|---|
| **Physical** | Radiation (CT abdomen ≈ 8–10 mSv ≈ 3–4 years of background; cumulative cancer risk small but non-zero, higher in children), contrast nephropathy/anaphylaxis, invasive complications (biopsy bleeding, pneumothorax with lung biopsy, perforation at colonoscopy), sedation risk |
| **Psychological** | Anxiety from false positives and incidental results, labelling, medicalisation |
| **Financial and logistical** | Out-of-pocket costs, time off work, insurance consequences |
| **Systemic** | Resource waste, delays for others |
| **Downstream** | Further tests, overtreatment, adverse drug effects |

### 8.2 Value-based and "Choosing Wisely" principles

Evidence-based lists from professional societies discourage low-value tests: imaging for nonspecific low back pain in the first 6 weeks, CT for uncomplicated headache, routine preoperative testing before low-risk surgery, repeated daily labs in stable inpatients, vitamin D or thyroid-function screening without indication, blood cultures when not indicated, D-dimer in high-probability patients, urine culture in asymptomatic older adults, PSA screening without discussion, cardiac stress testing for asymptomatic patients, ANA as a screening test, and "just-in-case" tests. Ask the "five questions": Do I really need it? What are the risks? Are there simpler, safer options? What happens if I do nothing? What will it cost?

### 8.3 Shared decision-making about tests

1. Explain **why** the test is considered and what it can and cannot tell.
2. Offer options, including **no test** or watchful waiting.
3. Present **probabilities** in natural frequencies (e.g., "Out of 100 people like you, 5 will have this condition; the test will find 4 of them and will give a false alarm in 10 of the 95 others").
4. Explore **values** (anxiety tolerance, willingness to treat, preference for certainty).
5. Agree on **what happens after each possible result** (including what a negative or equivocal result means).
6. Document consent and plan; set follow-up.

### 8.4 Communicating results and uncertainty

Use plain language, absolute risks, ranges and visuals; avoid "all clear" for tests that do not exclude disease (say "this makes X much less likely, but not impossible; contact us if..."); tell patients **who will inform them** and **when**; ensure **someone is accountable** for pending results. Avoid false dichotomies ("normal"/"abnormal"); explain borderline results and the plan.

---

## 9. A practical framework for a test decision

1. **Define the clinical question and the decision** it informs.
2. **Estimate PTP** (rule, prevalence, gestalt). Write it down as a number or range.
3. **Locate it relative to thresholds**: below test threshold (no test), between (test), above treatment threshold (treat).
4. **Pick the test** with the best LR for the question and acceptable harm/cost/availability; consider safety (pregnancy, renal function, allergy).
5. **Predict the post-test probability** for each plausible result and ensure at least one result would change the plan.
6. **Interpret in context**: technical quality, timing, interferences, concordance.
7. **Act** (treat, further test, observe) and **document**, including the safety net and who follows up.
8. **Review**: did the result and outcome fit? What would you do differently?

---

## Worked cases

### Case 1: Chest pain in a young woman

**Presentation.** Ms A., 28, no cardiovascular risk factors, sharp left-sided chest pain worse on deep inspiration for 6 hours, on the combined oral contraceptive pill, HR 92, SpO₂ 98%, normal examination. She asks for "a scan to rule out clots".

**Reasoning.** Wells PE score: no DVT signs, no tachycardia > 100, no recent surgery, no haemoptysis, PE not the leading diagnosis → "PE unlikely" (0). PERC criteria: age < 50, HR < 100, SpO₂ ≥ 95%, no haemoptysis, no oestrogen use (fails: she takes the COCP), no previous VTE, no recent surgery, no leg swelling. PERC cannot be applied because of oestrogen. D-dimer is appropriate (PTP ~4%, below intermediate). A negative result has NPV > 99%.

**Action.** D-dimer (age-adjusted threshold not needed at 28; standard cut-off 500 µg/L). Result 280 µg/L → PE excluded; diagnosis musculoskeletal/pleuritic pain; explanation, analgesia, review if symptoms change. Had D-dimer been positive (e.g., 900), CTPA would be next (PTP now intermediate), accepting radiation to breast tissue and weighing alternatives.

**Lessons.** For low PTP, a sensitive rule-out test avoids CT in most; imaging only when the post-test probability crosses the threshold. Shared decision-making addressed her request.

### Case 2: Low back pain and the MRI

**Presentation.** Mr B., 45, 10 days of low back pain after lifting, no leg symptoms, no red flags (no trauma, cancer history, weight loss, fever, neurological deficit, bladder/bowel changes, age < 50). He requests an MRI "to see what's wrong".

**Reasoning.** PTP of serious pathology < 1%. MRI findings of disc bulge/degeneration are frequent in asymptomatic adults (disc bulges 50% at age 40, degenerative changes 60–80% at age 60), rarely explain pain, and lead to unnecessary surgery and anxiety. Below the test threshold.

**Action.** Explain natural history (most improve in 4–6 weeks), stay active, analgesia, simple physiotherapy, safety net for red flags (saddle numbness, urinary retention, progressive weakness, fever), review at 2–4 weeks; offer MRI if no improvement at 6 weeks and surgery would be considered or red flags develop.

**Lessons.** Resist low-value imaging; explain why; provide a plan and safety net.

### Case 3: The incidental adrenal nodule

**Presentation.** Mrs C., 62, CT abdomen after fall shows a 2.4 cm right adrenal nodule, homogeneous, 5 HU unenhanced (lipid-rich adenoma pattern), no symptoms; BP 128/78.

**Reasoning.** Incidental adrenal masses occur in ~3–5% of adults. A homogeneous mass < 4 cm with unenhanced attenuation ≤ 10 HU is almost certainly a benign adenoma; imaging follow-up is unnecessary. Hormonal evaluation is needed for functionality: 1 mg dexamethasone suppression test (autonomous cortisol secretion), plasma metanephrines (if unenhanced HU > 10 or not typical), aldosterone/renin ratio if hypertension or hypokalaemia.

**Action.** Dexamethasone suppression test: cortisol 42 nmol/L (suppressed); metanephrines normal; no hypertension → no further work-up, reassure, no routine imaging follow-up. If HU > 20 or heterogeneity → further imaging (washout CT or MRI) or surgical review.

**Lessons.** Use incidental-finding algorithms; most incidentalomas are benign, and over-testing is harmful.

### Case 4: Troponin raised: two patients, two meanings

**Presentation.** (a) Mr D., 60, smoker, 90 minutes of central pressure radiating to the jaw, ECG normal; hs-cTnT 8 ng/L at 0 h, 35 ng/L at 1 h. (b) Mr E., 82, CKD 4, admitted with pneumonia, no chest pain, hs-cTnT 42 ng/L at 0 h and 44 ng/L at 3 h.

**Reasoning.** (a) PTP of ACS is high (typical symptoms, risk factors), troponin shows a significant delta (+27 ng/L): rule-in NSTEMI (post-test probability > 90%). (b) PTP of acute MI is low (no ischaemic symptoms); chronic stable elevation without delta in CKD/critical illness reflects myocardial injury, not MI. The same absolute number has different meaning.

**Action.** (a) Treat as NSTEMI-ACS: antiplatelets, anticoagulation, early angiography based on risk. (b) No ACS treatment; treat pneumonia; consider echo later; document baseline troponin.

**Lessons.** Pre-test probability and delta determine meaning. Tests do not diagnose by themselves.

### Case 5: The negative test in the sick child

**Presentation.** A 3-year-old with fever 39.8 °C for 5 days, conjunctival injection, red cracked lips, cervical lymphadenopathy, swollen hands; CRP 110, platelets normal, rapid strep test negative, COVID/influenza negative.

**Reasoning.** Features are strongly suggestive of Kawasaki disease (PTP high); there is no confirmatory test. Negative infection tests do not alter the probability much. The treatment threshold is low because untreated Kawasaki disease causes coronary aneurysms; IVIG is relatively safe.

**Action.** Do not wait for echocardiography or for a platelet rise (appears in week 2). Admit, echocardiogram, IVIG 2 g/kg and aspirin within 10 days of onset; monitor; seek paediatric cardiology.

**Lessons.** When a disease has no gold-standard test, rely on clinical criteria, set the treatment threshold by harm of missing it, and avoid false reassurance from irrelevant negatives.

### Case 6: The screening conversation

**Presentation.** Mr F., 58, healthy, asks his doctor whether he should have a PSA test "because my friend had prostate cancer".

**Reasoning.** PSA screening reduces prostate cancer mortality modestly (about 1 death prevented per 1000 men screened over 13 years in ERSPC), with overdiagnosis (about 2–5 men per death prevented), false positives, biopsy complications, and treatment effects (incontinence, erectile dysfunction). MRI-first pathways reduce unnecessary biopsies. The decision is preference-sensitive.

**Action.** Shared decision-making using natural frequencies and decision aids; explore values; if he chooses testing, PSA with MRI-triage pathway for raised results; if not, document. His friend's diagnosis does not change his own prior probability much.

**Lessons.** Screening is a trade-off of benefits and harms; absolute numbers and patient values decide.

### Case 7: Cognitive error: anchoring on a normal ECG

**Presentation.** Mrs G., 54, epigastric discomfort and sweating, normal ECG and troponin at 0 h; labelled "gastritis" at triage; discharged on a PPI. Returns the next day with chest pain; troponin now 2400 ng/L.

**Reasoning.** An early normal ECG and single troponin cannot exclude MI (sensitivity limits, early presentation, atypical symptoms in women and diabetics). Anchoring, premature closure and triage cueing led to the miss. PTP of ACS was not explicitly estimated; no serial testing was done.

**Action (system and personal).** Use pathways with serial troponin and repeat ECG; calculate HEART score; avoid premature labels ("gastritis" is a diagnosis of exclusion); explicit worst-case thinking; reflect in the morbidity review; communicate openly with the patient.

**Lessons.** The test result is only as good as the reasoning around it; build in diagnostic time-outs and safety nets.

---

## Common pitfalls

1. **Ordering without a question** or a plan for the result.
2. **Ignoring pre-test probability** (testing everyone, or not testing high-risk patients).
3. **Treating sensitivity/specificity as predictive values.**
4. **Using a sensitive test to rule in or a specific test to rule out.**
5. **Over-reliance on a single result**; failing to consider timing and pre-analytical issues.
6. **Repeating tests until normal** ("test shopping") or retesting unnecessarily.
7. **Testing in the wrong population** (D-dimer in high-risk PE; screening tests in symptomatic patients).
8. **Chasing incidental findings** without a framework.
9. **Defensive medicine**; inadequate documentation of the decision not to test.
10. **Failing to follow up** results or pending tests.
11. **Cognitive biases**: anchoring, premature closure, confirmation, availability.
12. **Ignoring patient values** and not discussing options, harms and uncertainty.
13. **Equating normal tests with no disease** and abnormal tests with disease.
14. **Using imaging that adds radiation without benefit** (CT in children, repeated CT).

---

## Key points

- Test only if the result can change management or decisions; ask what you will do with each plausible result.
- Estimate the pre-test probability explicitly; update it using likelihood ratios; tests are most informative at intermediate probabilities.
- Use test and treatment thresholds: harmless, effective treatments are started on lower probabilities; risky treatments require more certainty.
- Sensitive tests rule out (SnNout); specific tests rule in (SpPin); sequential testing balances sensitivity and specificity.
- Interpret results in context: timing, spectrum, interference, concordance with the clinical picture; trends and deltas beat single values.
- Recognise biases (study-level and cognitive); use clinical rules, checklists and diagnostic time-outs.
- Manage incidental findings with algorithms; avoid overdiagnosis and cascades.
- Share decisions with patients using natural frequencies; communicate uncertainty and follow-up.

---

## Self-assessment

**Questions**

1. Define pre-test probability and give three sources for estimating it.
2. A test has sensitivity 80% and specificity 90%. Calculate LR+ and LR−. With a pre-test probability of 20%, what is the post-test probability after a positive result?
3. Explain the test threshold and treatment threshold.
4. Why is a D-dimer not useful in a patient with a high pre-test probability of PE?
5. What is spectrum bias and how does it affect a published test's performance?
6. List five cognitive biases relevant to diagnostic testing and one mitigating strategy for each.
7. How should a 1.2 cm incidental thyroid nodule found on carotid ultrasound be approached?
8. Give three examples of low-value tests and the reasons.
9. How would you explain a screening test's benefits and harms to a patient?
10. A patient has a mildly abnormal result on a test that was ordered "just to be sure". What should you do?

**Answers**

1. The probability of disease before the test; sources: prevalence/base rate in the setting, clinical features and risk factors (including prediction rules such as Wells, HEART), local epidemiology, clinical gestalt, response to prior tests/treatment.
2. LR+ = 0.8/0.1 = 8; LR− = 0.2/0.9 = 0.22. Pre-test odds = 0.2/0.8 = 0.25; post-test odds = 0.25 × 8 = 2.0; probability = 2/3 = 67%.
3. Test threshold: probability below which testing is not worthwhile (observe); treatment threshold: above which one should treat without further testing; between them, test. They depend on test accuracy/harm and treatment benefit/harm.
4. The negative predictive value falls at high pre-test probability: a negative D-dimer does not rule out PE (post-test probability remains too high), so imaging is needed regardless.
5. Evaluating a test in a population that is not representative (very sick vs healthy controls) overstates accuracy; in practice the spectrum of disease and mimics lowers performance.
6. Examples: anchoring (generate a differential and ask what else), confirmation bias (seek disconfirming evidence), availability (check base rates), premature closure (diagnostic time-out; "what else could it be?"), framing/diagnostic momentum (re-take the history, re-evaluate labels), overconfidence (seek second opinion/feedback).
7. Assess risk (history, ultrasound features: suspicious criteria such as microcalcifications, irregular margins, taller-than-wide shape); apply TI-RADS/ATA size thresholds; FNA only if features and size meet criteria; check TSH; otherwise reassure/observe; avoid unnecessary biopsy and surgery.
8. Imaging for non-specific low back pain < 6 weeks (self-limiting, incidental findings); routine preoperative tests in low-risk surgery (no change in management); daily labs in stable inpatients (cascade, blood loss); urine culture in asymptomatic older adults (treatment harms); ANA screening without suggestive features (low PPV).
9. Use natural frequencies and absolute numbers (benefits: deaths prevented per 1000; harms: false positives, overdiagnosis, complications), discuss uncertainty, explore the patient's values, and respect their choice, including declining.
10. Reassess the pre-test probability and the clinical relevance; consider biological variation, errors or interferences; avoid reflex cascades; decide whether to repeat, observe or act; communicate honestly and document the plan.
