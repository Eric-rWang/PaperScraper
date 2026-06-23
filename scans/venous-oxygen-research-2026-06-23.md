# Venous Oxygen Research Scan — 2026-06-23

*Scheduled daily scan. Scope: (1) non-invasive monitoring of venous blood oxygen (SvO₂ / ScvO₂ / peripheral venous oxygenation); (2) optical imaging techniques for non-invasively obtaining venous blood oxygen (PA/PACT, NIRS, DOT, HSI, OCT/vis-OCT, SFDI). Ranked by relevance to **non-invasive venous** (not arterial) blood oxygen.*

---

## ⚠️ Read this first — honest sparseness report

- **Topic 1 (systemic non-invasive venous monitoring): one previously-uncatalogued primary paper added this cycle.** A **2022 Frontiers in Pediatrics study (Mileder et al.) reporting non-invasively measured peripheral muscle venous oxygen saturation (pSvO₂) via NIRS + venous-occlusion in preterm neonates** had not appeared in any prior scan. It is venous-specific (true pSvO₂, not just tissue StO₂) and is catalogued below with an honest relevance score. Everything else returned today was already in the repository (jugular NIRS / Hill 2024, Sun 2024, Mespere VO100 / Jeleff 2023, Oh 2023, the venous-occlusion test / Zachia Alan 2022, the MRI references, the 2016/2017 Zhang venous-modulation methods, the artificial-venous-pulse PPG family, the e-tattoo, hDOS). One **new venous-specific trial lead** (NCT04778150, liver-transplant SjvO₂ NIRS) surfaced and is recorded alongside the standing trial set.
- **Topic 2 (optical imaging): empty for new entries.** No genuinely new (post-2026-06-22) photoacoustic, NIRS-imaging, DOT, SFDI, HSI, or vis-OCT primary study surfaced. The strongest recent items (Hybrid-Net / arXiv:2512.15394, the qPACT virtual-imaging framework / PMC12858365, the venous-range sulfate phantoms / arXiv:2512.01458, the SP-SFDI retinal venous biomarker, the high-resolution HSI retina system, the IJV-PA proof-of-concept arXiv:2303.10775, the carotid-stenosis retinal-oximetry study, the *J. Innovative Optical Health Sciences* qPACT review) are all already in the repository. The only fresh-dated Topic-2 hit, **"Integrated spectral and depth compensation … in photoacoustic tomography for ovarian lesion diagnosis" (Feb 2026, PMC12869027)**, is tumor-angiogenesis sO₂/HbT estimation — not venous-specific — and is logged as context only, not entered.

---

## Topic 1 — Non-Invasive Monitoring of Venous Blood Oxygen (SvO₂ / ScvO₂ / Peripheral Venous Oxygenation)

### Paper 1.1 — NEW THIS CYCLE (previously uncatalogued)

**Title:** Non-invasively Measured Venous Oxygen Saturation as Early Marker of Impaired Oxygen Delivery in Preterm Neonates
**Authors:** Mileder, Buchmayer, Baik-Schneditz, Schwaberger, Höller, Andersen, Stark, Pichler, Urlesberger *(author list assembled from search synthesis; see verification note)*
**Year:** 2022
**Venue:** *Frontiers in Pediatrics*, 10:834045
**Link / DOI:** https://doi.org/10.3389/fped.2022.834045 — PMC8831784
**Relevance:** 7.5 / 10
**Novelty:** A clinical demonstration that **peripheral muscle venous oxygen saturation (pSvO₂)** and peripheral fractional oxygen extraction (pFOE) can be derived **non-invasively with NIRS using a venous-occlusion maneuver** in preterm neonates within the first 72 h of life. Key finding: infants with early neonatal inflammation/infection showed **significantly lower pSvO₂ within the first 24 h** *despite normal arterial SpO₂* — i.e., the venous metric detected impaired oxygen delivery/extraction that pulse oximetry missed. This is genuinely venous (not a generic StO₂ surrogate): the venous-occlusion method isolates the venous compartment.
**Integration insights:** Strengthens the central thesis of this program — that the venous saturation carries clinically actionable information orthogonal to arterial SpO₂ — and does so in a real patient population with a deployable optical method. It is the same **venous-occlusion + NIRS lineage** as Zachia Alan 2022 (thenar StO₂→ScvO₂) and the hDOS platform (2026-06-17 §1.2), reinforcing venous occlusion as the most clinically validated *non-imaging* optical route to peripheral SvO₂. Caveat for the broader goal: it is peripheral *muscle* venous saturation, not a named central vessel (SVC/IJV) and not blood-gas-calibrated against simultaneous co-oximetry — so it informs *trend/extraction* monitoring rather than absolute central SvO₂.
**Verification note:** Title, year, journal (Front. Pediatr. 10:834045) and DOI/PMCID are cross-confirmed across PMC and Frontiers listings. The **full author list could not be confirmed by direct page fetch** (Frontiers and Europe PMC returned HTTP 403); the authorship above is from search-engine synthesis and should be treated as **tentative pending direct verification**.

### Previously surfaced — re-confirmed, not re-entered

- **Hill, Campbell, Chase & Pretty 2024**, optical SvO₂ sensing at the external jugular vein — *Curr. Dir. Biomed. Eng.* 10(4):295–298 (DOI 10.1515/cdbme-2024-2072). Prior scan **2026-06-10 §1.1**. (Re-surfaced today under the longer title *"Estimation of Venous Oxygen Saturation Through Non-Invasive Optical Sensing at the Jugular Veins"* — same paper.)
- **Sun et al. 2024**, IJV SijvO₂ via NIRS + subject-specific Monte Carlo + DNN — *Optics Letters* 49(10):2669–2672. Prior scan **2026-06-10 §1.2**.
- **Jeleff et al. 2023**, Mespere VO100 jugular NIRS vs invasive ScvO₂, 79 ICU patients — *J. Cardiothorac. Vasc. Anesth.* (PMID 37827917). Prior scan **2026-06-10 §1.3**.
- **Oh et al. 2023**, cerebral-NIRS surrogate tracking of mixed SvO₂ — *Sci. Rep.* (DOI 10.1038/s41598-023-49078-1; PMC10709586). Prior scan **2026-06-10 §1.4**.
- **Zachia Alan et al. 2022**, thenar StO₂ → ScvO₂ during the venous-occlusion test — *Critical Care Science* (DOI 10.5935/0103-507X.20220023-en). Prior scan **2026-06-10 §1.5**.
- **McDiarmid et al. 2026**, cardiac-MRI T₂ iSvO₂, 628-patient HF cohort — *JACC: Advances* 5(1):102484. Prior scan **2026-06-11 §1.1**.
- **Skow et al. 2025**, MRI susceptometry-based venous oximetry during exercise — *Am. J. Physiol. Heart Circ. Physiol.* 328(6) (DOI 10.1152/ajpheart.00134.2025). Prior scan **2026-06-14 §1.1**.
- **Lahade et al. 2026**, wearable FD-NIRS (ASIC), forearm-occlusion arterio-venous transition — *Biomed. Opt. Express* 17(2):555–571 (DOI 10.1364/BOE.585068). Prior scan **2026-06-11 §1.2**.
- **Tan et al. 2023**, wearable arterial+venous optical e-tattoo (EMBC 2023, PMID 38083768). Prior scan **2026-06-17 §1.1**.
- **"hDOS" 2025** (Durduran group), automated hybrid diffuse-optical platform built around the venous-occlusion test — *J. Biomed. Opt.* 2025 / medRxiv 2025.06.03.25328859. Prior scan **2026-06-17 §1.2**.
- **Zhang et al. 2016**, light-absorption SvO₂ via induced venous fluctuation (RMSE 5.31, r 0.72 vs invasive) — *BioMed. Eng. OnLine* 15 (DOI 10.1186/s12938-016-0208-8; PMC4952148). Prior scan **2026-06-17 §1.3**.
- **Zhang et al. 2017**, proof-of-concept non-invasive peripheral SvO₂ — *BioMed. Eng. OnLine* 16 (DOI 10.1186/s12938-017-0351-x; PMC5437414). Prior scan 2026-06-17 honorable mention.
- **Peripheral-venous-saturation-vs-co-oximetry validation** (PMC5655584, *J. Clin. Monit. Comput.*, PMID 27873173) and the **artificial-venous-pulse PPG** family. Same Zhang/peripheral-PPG lineage already catalogued — not re-entered.

### Clinical-trial leads (no results papers)

- **NCT04778150 (newly recorded this cycle)** — *"Non-Invasive Measurement of SjvO₂ Using Near Infrared Spectroscopy in Patients Undergoing Liver Transplantation Surgery."* A **venous-specific** jugular-venous-saturation NIRS validation effort in liver-transplant surgery — distinct from the previously-catalogued hepatic-vein trial NCT01891188. Surfaced via ClinicalTrials.gov; direct page fetch returned HTTP 403, so status/dates are **unverified**; recorded as a lead, not an entry. Consistent with the Mespere VO100 / jugular-NIRS thread.
- **NCT01891188** — *"Using NIRS to Noninvasively Evaluate Hepatic Venous Saturation"* (hepatic regional StO₂ vs SvHO₂; Phoenix Children's). Record updated Jan 2026; no results paper.
- **NCT06511999** — *"Continuous Jugular Venous Oxygen Saturation (SjO₂) Measurement After Cardiac Arrest"* (U. Pittsburgh; recruiting; est. completion Dec 2027). No results yet.
- **NCT05161884** — *"Validation of a Non-invasive Assessment of ScvO₂ by Using MRI"* (MRI-reference validation). No results paper.
- **NCT04624009** — *"Non-Invasive Measurement of SjvO₂ Using Near Infrared Spectroscopy in Critically Ill Patients."* No results publication located.

---

## Topic 2 — Optical Imaging Techniques for Non-Invasive Venous Blood Oxygen

**No new entries this cycle.** No genuinely new (post-2026-06-22) primary imaging study tied to *venous* sO₂ surfaced. The standing top-5 imaging set remains the strongest available and is carried forward unchanged:

1. **Distribution-informed, wavelength-flexible data-driven PA oximetry** (arXiv:2403.14863) and the **Hybrid-Net spectroscopic-PA segmentation + sO₂ estimator** (arXiv:2512.15394) — learning-based qPAI sO₂ that, at venous-range saturations, is the most credible imaging route to vessel-resolved venous sO₂. Prior scans (06-17/06-22).
2. **qPACT virtual-imaging framework for 3D learning-based reconstruction** (PMC12858365) — validation scaffolding for deep-learning qPACT sO₂; relevant to whether any imaging method can hit blood-gas accuracy. Prior scan.
3. **IJV photoacoustic oximetry proof-of-concept** (arXiv:2303.10775) — still the only direct **human named-vein** photoacoustic sO₂ result. Prior scans.
4. **Sulfate phantoms mimicking NIR-PA response of whole blood at selected sO₂** (arXiv:2512.01458) — venous-range PA calibration standards. Prior scan 2026-06-21.
5. **vis-OCT / SP-SFDI / HSI retinal venous oximetry** — single-vessel retinal **venous** saturation (arterial ≈95%, venous ≈72%) and the carotid-stenosis clinical retinal-oximetry study (2026-06-19). Vessel-level, not systemic SvO₂; comorbidity-confounded. Prior scans.

**Context-only (not entered):** *"Integrated spectral and depth compensation approach for optimizing oxygen saturation and total hemoglobin estimation in photoacoustic tomography for ovarian lesion diagnosis"* (PMC12869027, *Feb 2026*). A 2026-dated qPAT sO₂/HbT advance, but its target is ovarian-lesion tumor angiogenesis — **not venous-specific**; logged for technique-transfer awareness (spectral + depth fluence compensation is exactly the correction that deep-vein venous PA oximetry needs).

---

## Cross-Topic Synthesis

### What this scan establishes
- **Topic 1 gained one real, previously-missed data point.** The Mileder et al. preterm-neonate NIRS pSvO₂ paper (2022) is venous-specific, clinical, and shows the venous metric flagging impaired oxygen delivery that SpO₂ missed — a clean clinical argument for the whole program. It joins the **venous-occlusion + NIRS** cluster (Zachia Alan; hDOS) that is now the best-validated *non-imaging* optical route to peripheral SvO₂.
- **A second venous-specific NIRS trial (NCT04778150, liver transplant) is now tracked**, bringing the venous-trial set to five registered efforts — still none with a results publication. Topic 1's forward motion remains dominated by trials, not papers.
- **Topic 2 produced nothing new for venous sO₂.** The Feb-2026 ovarian qPAT paper confirms the field's momentum is in tumor/arterial-vascular sO₂, with venous-vessel imaging still concentrated in the retina and in murine/phantom PA.

### Persisting gaps (carried forward, unchanged and still open)
- **No new in-vivo human venous-PA sO₂ result.** The 2023 IJV-PA proof-of-concept remains the only direct human named-vein photoacoustic oximetry result; clinical-scale validation still does not exist.
- **The MRI validation-scale gap still dominates.** Two MRI venous-SvO₂ methods (T₂ iSvO₂; susceptometry) are blood-gas-validated at cohort scale; no optical method approaches that bar. An MRI-reference ScvO₂ validation trial is registered.
- **Vessel-specific venous separation remains proven mainly in the retina (and thin/murine tissue).** Extension to an accessible systemic vein in thick human tissue is still unshown.
- **Comorbidity / confounding remains an explicitly documented obstacle** (carotid-stenosis retinal-oximetry study, 2026-06-19): venous/A–V endpoints did not track disease severity cleanly because of individual comorbidities — a standing warning for any optical venous-oximetry biomarker.

### Bottom line
A modestly productive day for Topic 1: one genuine, previously-uncatalogued venous-specific clinical paper (Mileder 2022, preterm pSvO₂ by NIRS venous occlusion) plus one new venous NIRS trial. Topic 2 added nothing venous-specific. The structural picture is unchanged — venous-occlusion NIRS is the clinically validated non-imaging route, photoacoustics is the most promising *imaging* route but still pre-clinical for deep human veins, and MRI remains the only cohort-scale validated non-invasive venous oximetry.

---

*Verification caveats: Frontiers, Europe PMC, PMC, and ClinicalTrials.gov pages returned HTTP 403 to automated fetching today; metadata for Paper 1.1 (esp. the full author list) and NCT04778150 status/dates are flagged as not directly page-verified. All DOIs/PMCIDs and titles were cross-checked across at least two search-indexed listings.*
