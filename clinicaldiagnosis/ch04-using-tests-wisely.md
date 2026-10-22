## Chapter 4. Using Tests Wisely

### Learning objectives

After studying this chapter you should be able to:

1. Define sensitivity, specificity, predictive values and likelihood ratios, and calculate them from a 2×2 table.
2. Explain why predictive values depend on prevalence while sensitivity and specificity do not (in principle).
3. Apply the threshold model: when to test, when to treat without testing, and when to do neither.
4. Recognise common traps in test interpretation: spectrum bias, verification bias, the multiple-testing problem, and incidental findings.
5. Decide when *not* to test, and explain this to a patient.

---

### 4.1 What a test is for

A diagnostic test is a question you ask the patient's body. Like any question, it is worth asking only if **the answer could change what you do**. Before ordering, ask yourself:

1. *What am I trying to find out?* (confirm, exclude, stage, monitor?)
2. *How likely is the disease before the test?* (pre-test probability)
3. *What will I do if it is positive? If negative?*
4. *Could the test harm the patient?* (radiation, contrast reactions, invasive risk, false positives, anxiety, cost, cascades of further testing)

If the plan is identical whatever the result, the test does not belong.

Tests serve several different purposes, and the ideal test differs for each:

| Purpose | Question | Desirable property |
|---|---|---|
| Screening | Does this apparently healthy person have early disease? | High sensitivity, safe, cheap, treatable disease |
| Exclusion (rule-out) | Can I safely send this person home? | High sensitivity / very low LR− |
| Confirmation (rule-in) | Do I now have enough certainty to start treatment? | High specificity / very high LR+ |
| Staging / severity | How bad is it? | Reproducible measurement |
| Monitoring | Is it responding? | Sensitive to change |
| Prognosis | What is likely to happen? | Validated predictive value |

---

### 4.2 The 2×2 table

Every basic accuracy measure comes from comparing the test result with a **reference standard** (the best available way of establishing the truth):

| | Disease present | Disease absent |
|---|---|---|
| **Test positive** | True positive (TP) | False positive (FP) |
| **Test negative** | False negative (FN) | True negative (TN) |

From this table:

- **Sensitivity** = TP / (TP + FN): the proportion of diseased people who test positive.
- **Specificity** = TN / (TN + FP): the proportion of healthy people who test negative.
- **Positive predictive value (PPV)** = TP / (TP + FP): of those with a positive test, the proportion who have the disease.
- **Negative predictive value (NPV)** = TN / (TN + FN): of those with a negative test, the proportion who are free of disease.
- **LR+** = sensitivity / (1 − specificity).
- **LR−** = (1 − sensitivity) / specificity.

#### Interpretation

- **Sensitivity** answers: "If the patient has the disease, will the test catch it?" A highly sensitive test has few false negatives, so a *negative result is reassuring* (**SnNout**: a Sensitive test, when Negative, rules Out).
- **Specificity** answers: "If the patient is healthy, will the test say so?" A highly specific test has few false positives, so a *positive result is convincing* (**SpPin**: a Specific test, when Positive, rules In).
- **Predictive values** answer the question the clinician actually asks ("Given this result, what is the chance this patient has the disease?"), but they depend on prevalence.

The mnemonics (SnNout, SpPin) are helpful but not perfect; likelihood ratios are better because they quantify the shift in probability.

---

### 4.3 Prevalence and predictive values (a second look)

As shown in Chapter 1, the same test behaves differently as prevalence changes. Here is a more realistic example.

**HIV screening with a fourth-generation laboratory test**, with illustrative performance of sensitivity 99.5% and specificity 99.5%.

Apply to 100,000 people with a prevalence of 0.1% (100 infected, 99,900 uninfected):

- True positives = 100 × 0.995 ≈ 99.5
- False positives = 99,900 × 0.005 ≈ 499.5
- PPV = 99.5 / (99.5 + 499.5) ≈ **16.6%**

Despite an excellent test, **about five of every six positive screens are false positives** in this low-prevalence population. That is why a single reactive result is never reported as a diagnosis: it triggers a confirmatory algorithm using different assays.

Apply the same test where the prevalence is 10% (10,000 infected, 90,000 uninfected):

- True positives = 9,950
- False positives = 450
- PPV = 9,950 / 10,400 ≈ **95.7%**

*Take-home:* an unexpected positive result in a low-risk setting should be treated as "probably a false positive until confirmed"; the same result in a high-risk setting is "probably real."

(Sensitivity and specificity are usually described as properties of the test, but they can vary across populations; see spectrum bias, 4.6.)

---

### 4.4 Likelihood ratios in practice

Likelihood ratios are the most practical measure because they can be applied to any pre-test probability. Recall:

> **Post-test odds = pre-test odds × LR**

For many tests the results are not merely "positive" or "negative" but graded (e.g. D-dimer level, white cell count, troponin concentration). **Multilevel likelihood ratios** give a separate LR to each band of the result, which preserves information that dichotomising throws away.

**A pocket approximation.** For pre-test probabilities between roughly 10% and 90%, you can estimate the change in probability from the LR:

| LR | Approximate change in probability |
|---|---|
| 2 | +15% |
| 5 | +30% |
| 10 | +45% |
| 0.5 | −15% |
| 0.2 | −30% |
| 0.1 | −45% |

This is a crude rule (the exact change depends on the starting point), but it prevents the commonest misreadings.

**Worked example 1: a strong rule-out.** A patient has a pre-test probability of 20% for a given diagnosis. A test with LR− = 0.1 is negative.

- Pre-test odds = 0.20 / 0.80 = 0.25
- Post-test odds = 0.25 × 0.1 = 0.025
- Post-test probability = 0.025 / 1.025 ≈ **2.4%**

**Worked example 2: a weak rule-out.** Same patient, a test with LR− = 0.7.

- Post-test odds = 0.25 × 0.7 = 0.175
- Post-test probability = 0.175 / 1.175 ≈ **14.9%**

The weak negative has barely helped; it should not be allowed to end the work-up.

**Worked example 3: a strong rule-in.** Pre-test probability 30%, LR+ = 15.

- Pre-test odds = 0.30 / 0.70 = 0.429
- Post-test odds = 0.429 × 15 = 6.43
- Post-test probability = 6.43 / 7.43 ≈ **86.5%**

---

### 4.5 The threshold model: when to test, when to treat

Imagine a probability line from 0% to 100% that the patient has the disease.

- Below the **test threshold** the chance is so low that neither testing nor treatment is justified: **do nothing** (reassure, watch).
- Between the **test threshold** and the **treatment threshold**, **testing** is useful, because the result can move the patient across a threshold.
- Above the **treatment threshold**, the chance is high enough that you should **treat without further testing**.

Where the thresholds sit depends on:

- **Harm of the treatment** (higher harm raises the treatment threshold: you need more certainty).
- **Harm of missing the disease** (higher harm lowers both thresholds).
- **Risk and cost of the test** (high risk raises the test threshold).
- **Availability** of the test and of treatment.

**Example A: pulmonary embolism.** Missing PE has a high mortality, and anticoagulation is effective but carries a bleeding risk. For a patient with a *low* pre-test probability, a sensitive D-dimer is a safe rule-out. For a patient with a *high* pre-test probability, a negative D-dimer is not reliable enough, so you proceed to imaging, or even start anticoagulation while arranging it if imaging will be delayed.

**Example B: sore throat in an adult.** The harm of missing streptococcal pharyngitis is small and complications are rare in most settings. Clinicians using a score (Centor / McIsaac, Chapter 70) with a low score neither test nor treat; with a middle score they test; with a high score some treat directly.

**Example C: bacterial meningitis.** The danger of delayed treatment is high, and the harm of a short course of antibiotics is low. The treatment threshold is *very low*: if suspicion is real, treat first and test in parallel.

The threshold model also explains why testing is wasteful at both ends: the very-low-probability patient (test results will mostly be false positives) and the very-high-probability patient (a negative result will not change the plan).

---

### 4.6 Sources of error in test interpretation

#### Spectrum bias

A test's apparent sensitivity and specificity depend on the patients studied. A test evaluated in **severely ill** patients (easy cases) and **healthy** controls overestimates its performance. In real practice, with **mild or early disease** and **look-alikes**, performance is poorer.

*Example.* A rapid test evaluated in patients with obvious, advanced disease may miss many early cases in the clinic.

#### Verification (work-up) bias

Only patients with positive screening results go on to receive the reference test, so the rest are never "verified". This distorts the estimated sensitivity.

#### Incorporation bias

The test under evaluation is itself part of the criteria used to define disease. This inflates apparent accuracy.

#### Test performance varies across settings

Even for the same assay, performance depends on operator skill (ultrasound, ECG reading), timing (troponin soon after symptom onset is less sensitive), and sample quality.

#### The multiple-testing problem

Reference ranges are typically set to include 95% of healthy people; so **5% of healthy people will fall outside the range for any single test**. If you order many independent tests, the chance of at least one "abnormal" result in a healthy person climbs quickly:

- 1 test: 5%
- 5 tests: 1 − 0.95⁵ ≈ 23%
- 10 tests: 1 − 0.95¹⁰ ≈ 40%
- 20 tests: 1 − 0.95²⁰ ≈ **64%**

A healthy patient who has a 20-test panel is more likely than not to be told that something is "abnormal." Each abnormal result then triggers a need for explanation, repeat testing, referral and anxiety: a **cascade**.

#### Incidental findings ("incidentalomas")

Imaging often finds unexpected abnormalities: adrenal nodules, thyroid nodules, pulmonary nodules, renal cysts. The majority are benign. Their discovery can start a chain of follow-up that carries its own risks. The best defence is *not to image without a clear question*, and to have an agreed approach (guidelines) to the finding when it occurs.

#### Anchoring on a single abnormal result

An isolated mildly abnormal result (a slightly raised ALT, a borderline sodium) in an asymptomatic person is more often noise or normal variation than disease. Repeat testing, trend over time, and clinical context all matter.

---

### 4.7 When not to test

Not testing is a clinical decision, and sometimes the best one. Situations in which testing usually adds more harm than benefit:

1. **Low pre-test probability** and low consequence if missed (e.g. routine blood tests in a well person with a minor, self-limiting illness).
2. **The result will not change management.** (Imaging in acute non-specific low back pain without red flags: the majority resolve within weeks, and findings such as disc bulges are common in asymptomatic people.)
3. **A false positive is likely and the follow-up is invasive.**
4. **The patient's goals make the information irrelevant** (e.g. in advanced illness where the result will not alter a plan focused on comfort).
5. **The test has not been validated** for the question being asked.
6. **"Just in case" or defensive testing**, when no specific diagnostic question can be stated.
7. **Repeat testing without a reason.** Daily bloods in a stable patient is not monitoring; it is habit.

How to explain this to a patient:

> "Your symptoms and examination point strongly to a muscle strain. A scan is unlikely to show anything that would change our treatment, and scans often show age-related changes that look worrying but are not the cause of the pain. So I'd suggest we start with the plan I've described and review you in two weeks. If you notice any of these warning signs, come back straight away."

The explanation is as important as the decision. Patients who understand the reasoning are more likely to accept it, and the safety-net reassures them.

---

### 4.8 Practical guidance for common situations

- **Order tests to answer a specific question**, and write the question in the request. ("Anaemia? Looking for MCV and ferritin.") Better questions produce better interpretation.
- **Know your tests.** Understand the time course (when does the test turn positive?), the sample requirements, and the typical false-positive and false-negative causes.
- **Use clinical prediction rules** with validated cut-offs, when available, to decide whom to test (Chapter 70).
- **Be cautious with panels** and "check-up" bundles.
- **Look at the patient, then the numbers.** A normal lactate does not make a shocked patient well. A mildly abnormal result in a well patient may not matter.
- **Trend, don't just snapshot.** A haemoglobin that has dropped by 30 g/L over two days matters more than one that is stable at an abnormal value.
- **Follow up every result.** An unviewed result is a latent error.
- **Beware the unit.** Always check the units and reference range of the specific laboratory.

---

### 4.9 Worked cases

#### Case 1: D-dimer and a low-risk patient

A 32-year-old woman presents with pleuritic chest pain for one day after a minor viral illness. She is not on any oestrogen, has no history of venous thromboembolism, no leg symptoms, a heart rate of 80 and oxygen saturation of 99%. A clinical prediction score for PE places her in the *low-probability* group (prevalence of PE in this group is roughly 1–5%).

*Reasoning.* A D-dimer (high sensitivity, low specificity) is the right test: a negative result gives a post-test probability well below 1%, which is acceptable to stop the work-up. Skipping straight to CT pulmonary angiography would expose her to radiation and contrast, with a probability that a positive finding would be false or clinically trivial.

*If the D-dimer is positive,* it simply moves her into the group requiring imaging; it does not diagnose PE. Positive D-dimers have many causes (infection, inflammation, pregnancy, cancer, recent surgery, age).

*Age-adjusted note.* In patients over 50, D-dimer specificity falls; a commonly used adjustment is a cut-off of age × 10 µg/L (fibrinogen-equivalent units) rather than the standard 500 µg/L.

#### Case 2: When the test should not be believed

A 60-year-old man has had intermittent central chest pressure on exertion for 3 weeks, relieved by rest, with a pre-test probability for obstructive coronary disease of perhaps 50–60%. An exercise ECG is performed and is *negative*.

*Reasoning.* The test has limited sensitivity (a modest LR−, in the region of 0.5 in many populations). A pre-test probability of 55% (odds 1.22) × LR− 0.5 = odds 0.61, a post-test probability of about **38%**. This is still far too high to dismiss. A negative exercise test should not reassure the clinician; the patient requires further evaluation (stress imaging, CT coronary angiography or invasive angiography) according to local pathways.

*Lesson.* With a high pre-test probability, a weakly discriminating "negative" result leaves the diagnosis very much alive.

#### Case 3: Low back pain and the MRI

A 38-year-old man has had 5 days of lumbar pain after lifting a heavy box. The pain radiates to the buttock but not below the knee. He has no weakness, numbness, saddle anaesthesia, bladder or bowel change, fever, weight loss or history of cancer. He requests an MRI.

*Reasoning.* There are no red flags. The likelihood of serious spinal pathology is very low. Most acute low back pain improves substantially in 2–6 weeks. MRI frequently shows disc bulges or degeneration in asymptomatic adults, so the scan is likely to reveal an abnormality that will be incidentally blamed, potentially prompting unnecessary interventions.

*Plan.* Explain the reasoning, give analgesia and advice to stay active, specify the red flags that would prompt immediate return, and review at 2 weeks. If symptoms persist or red flags emerge, imaging becomes appropriate.

#### Case 4: The unexpected abnormal result

A 45-year-old woman attends for an insurance medical. A panel of 24 tests is run. Her serum ALT is 1.2 times the upper limit of normal; every other value is within range. She has no symptoms, drinks little alcohol, and takes no regular drugs.

*Reasoning.* With 24 tests, the chance of one mild abnormality in a healthy person is high (1 − 0.95²⁴ ≈ 71%). A mild isolated rise of ALT has many benign explanations (recent exercise, mild fatty liver, a recent painkiller, normal variation).

*Plan.* Review the history for drugs and risk factors, and repeat the test in a few weeks. If it remains elevated, follow a structured evaluation for liver disease (viral hepatitis serology, metabolic risk factors, ultrasound); if it is normal, document it and move on.

*Lesson.* Resist the reflex to investigate every mild laboratory deviation immediately; trend it and consider the context.

#### Case 5: Troponin timing

A 59-year-old man has an episode of severe chest pain lasting 30 minutes, which settled one hour before he reaches the emergency department. A high-sensitivity troponin drawn on arrival (about 1.5 hours after symptom onset) is below the assay's lowest decision threshold.

*Reasoning.* Because troponin rises over hours after myocardial injury, a single very early sample can be falsely reassuring. Modern high-sensitivity assays have excellent NPV in validated rapid protocols (which use a second sample 1–3 hours later, depending on the protocol), but the interpretation requires the pathway to be followed and the clinical pre-test probability to be taken into account.

*Plan.* Follow your institution's validated rule-out protocol (serial troponin plus ECG plus risk assessment). A high-risk story (e.g. typical pain, known coronary disease) calls for caution and not only a single low value.

*Lesson.* Know the time course and the validated pathway for each test, and avoid stopping on a single sample when timing matters.

---

### 4.10 Common pitfalls

- **Ordering first, thinking later.** The result becomes a problem rather than an answer.
- **Treating "normal" as "excluded".** A negative result with a poor LR− does not exclude disease.
- **Treating "abnormal" as "diagnosed".** A positive result with a low PPV does not confirm disease.
- **Ignoring pre-test probability.**
- **Ignoring the test's performance characteristics.** Not all "negative" results are equal.
- **Dichotomising continuous results** and losing information.
- **Failing to act on a result,** or failing to find it.
- **Screening without a plan** for positives.
- **Not discussing the possibility of incidental findings** with patients before imaging.

---

### 4.11 Key points

- Order a test only when the result could change what you do.
- Sensitivity and specificity describe the test; predictive values describe the *patient in context* and depend on prevalence.
- Likelihood ratios let you apply any test to any pre-test probability: **post-test odds = pre-test odds × LR**.
- Use the threshold model: don't test below the test threshold or above the treatment threshold.
- Beware spectrum bias, multiple testing, incidental findings, and test timing.
- Not testing is a legitimate decision, and explaining it well is part of good care.

---

### 4.12 Self-assessment

1. A test has sensitivity 95% and specificity 80%. Calculate LR+ and LR−.
   *Answer: LR+ = 0.95 / 0.20 = 4.75; LR− = 0.05 / 0.80 = 0.0625.*

2. In 1,000 people, prevalence is 2%, sensitivity 90%, specificity 95%. How many true and false positives are there, and what is the PPV?
   *Answer: 20 diseased → 18 TP; 980 healthy → 49 FP; PPV = 18 / 67 ≈ 27%.*

3. Why is a 20-test panel in a healthy person likely to return at least one abnormal result?
   *Answer: With 95% reference ranges, each test has about a 5% chance of falling outside the range in a healthy person; with 20 independent tests, the chance of at least one is about 64%.*

4. A test with LR− = 0.5 is negative in a patient with pre-test probability 60%. What is the post-test probability?
   *Answer: Pre-test odds 1.5; post-test odds 0.75; probability ≈ 43%. Still too high to exclude disease.*

5. Give three situations where you would not order a test.
   *Answer (any three): very low pre-test probability; result won't change management; high likelihood of false positives leading to invasive follow-up; patient goals make it irrelevant; no validated role for the test; routine repeated testing without indication.*
