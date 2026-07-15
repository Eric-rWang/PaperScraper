# Venous Oxygen Research Scan — 2026-07-15

**Search window:** Twenty-fourth scan in the series, run **two days** after 2026-07-13 (no scan on 07-14). Emphasis on work published or first-surfacing after 07-13, with the standard fallback to the best-available venous-specific work already catalogued. Sources searched today: PubMed/PMC, arXiv, bioRxiv/medRxiv, Optica (Biomed. Opt. Express, Optics Letters, Applied Optics), SPIE / *J. Biomed. Opt.*, *Photoacoustics* (ScienceDirect), IEEE Xplore, Nature / *Sci. Rep.* / *Commun. Med.*, Wiley (*Advanced Science*, *Adv. Healthcare Mater.*), IOPscience (*J. Phys. Photonics*), MDPI (*Biosensors*), Springer, De Gruyter, QIMS/AME, ClinicalTrials.gov, ResearchGate, Semantic Scholar, ADS.

**Verification caveat:** As in every prior scan, publisher **full-text** pages — including iopscience.iop.org, pmc.ncbi.nlm.nih.gov, arxiv.org, opg.optica.org and the Wiley/Nature domains — returned **HTTP 403** to direct `WebFetch` in this environment today (re-confirmed on IOPscience `ae637f` and PMC12047737). Every reference below was therefore cross-checked across **at least two independent search-index snippets**; per-item notes state what was confirmed and what could not be read directly on a publisher page.

---

## ⚠️ Read this first — day summary

**No new venous-specific *primary* paper today — but one substantive refinement to an already-catalogued item that materially upgrades its venous relevance.**

- **KEY REFINEMENT (Topics 1 & 2):** Deeper reading of **APM+ — Arterial Blood-Mediated Deep-Tissue Photoacoustic Oximetry** (Sastry et al., *Advanced Science* 2026, DOI `10.1002/advs.76366`) confirms that the paper does **not** stop at an arterial demonstration. It reports an **in-vivo, non-invasive estimate of the radial *vein* sO₂** — median **72.3 %** (IQR 8.9 %), squarely in the physiological venous 60–80 % band — in **8 healthy adult humans**, using the neighbouring radial *artery* as an in-situ fluence calibrator. No prior scan in this series captured that the venous measurement was actually performed; earlier files logged APM+ only as "arterial-demonstrated, transferable to venous." It is therefore promoted today from a transferable-technique entry to a **bona-fide non-invasive optical/PA venous-oximetry demonstration in humans** (Topic 2 §2.2), second only to the IJV-PA anchor.

Everything else returned by today's sweep is **previously surfaced** or out-of-scope: the jugular optical sensor (De Gruyter CDBME), the IJV DNN + Monte-Carlo work, Mespere VO100 jugular NIRS, the MRI iSvO₂ / SSL-oximetry references, the PACT venous-flow work, vis-OCT / hyperspectral retinal oximetry, and the deep-tissue thrombosis-PAT metrology paper (PMC12047737, already surfaced 06-11 / 06-22). Two IOPscience wearable-NIRS items appeared newest in the raw results — a low-cost multimodal StO₂ wearable (`10.1088/2515-7647/ae637f`) and a wearable-NIRS hardware review (`10.1088/2515-7647/ae6ae4`, published 2026-05-28) — but both are **tissue-level StO₂ / instrumentation**, not venous SvO₂, and are logged only as standing context. Consistent with the series' standing observation, **truly novel non-invasive venous-optical work is published at very low volume**; today produced no new primary, only a corrected/upgraded reading of an existing one.

---

## Topic 1 — Non-invasive monitoring of venous blood oxygen (SvO₂ / ScvO₂ / peripheral venous)

*No new items today.* The standing best-available set (all previously surfaced) with scores carried forward:

### 1.1 — Estimation of Venous Oxygen Saturation Through Non-Invasive Optical Sensing at the Jugular Veins *(previously surfaced — scan 06-10 §1.1; flagship optical-venous device paper)*
- **Authors:** Alqahtani et al.
- **Year / Venue:** 2024 · *Current Directions in Biomedical Engineering* 10(2) (De Gruyter; CDBME-2024-2072)
- **Link / DOI:** https://doi.org/10.1515/cdbme-2024-2072
- **Relevance:** **8/10** — true, non-invasive, optical, venous (but n=3, no invasive co-oximetry reference).
- **Novelty:** A pulse-oximeter-style optical sensor over the external jugular vein isolates the EJV waveform and returns SvO₂ estimates (~70–72 %) within the healthy 60–90 % band — still the closest thing to a wearable-form-factor optical SvO₂ device in the literature.
- **Integration insights:** The superficial/low-cost optical analogue of the deep IJV-PA anchor (§2.1); together they bracket the venous-optical problem from the shallow and deep ends. Its open problem — calibration against a blood-gas gold standard — is exactly what the APM+ artery-as-reference approach (§2.2) and MRI reference oximetry (§1.4) aim to close. *Metadata cross-confirmed via De Gruyter listing + ResearchGate; full text 403 (flagged).*

### 1.2 — Quantifying Changes in Oxygen Saturation of the Internal Jugular Vein In Vivo Using Deep Neural Networks and Subject-Specific 3-D Monte-Carlo Models *(previously surfaced — scan 06-10 §1.2)*
- **Year / Venue:** 2024 · *Optics Letters* 49(10):2669
- **Link / DOI:** https://opg.optica.org/ol/abstract.cfm?uri=ol-49-10-2669
- **Relevance:** **7/10** — IJV-specific, non-invasive, inverse-modeling for venous saturation *change*.
- **Novelty:** Multi-channel NIRS + DNNs trained on subject-specific 3-D Monte-Carlo forward models recover ΔSijvO₂ non-invasively, tying measured reflectance to a physically-modelled forward problem — sidestepping the labelled-data bottleneck via simulation.
- **Integration insights:** The inverse-modeling / fluence-correction leg of the program; the physics-simulation twin of the self-supervised-learning approach in §1.3. *Cross-confirmed via Optica listing + Semantic Scholar; full text 403 (flagged).*

### 1.3 — Leveraging Self-Supervised Learning for Non-Invasive Intra-Cardiac Magnetic Resonance Oximetry Assessment *(previously surfaced — scan 07-13 §1.1; MRI, not optical)*
- **Authors:** Jiayuan Chen, Thai-Hoang Pham, Ping Zhang, Juliet Varghese
- **Year / Venue:** 2026 (preprint posted 2026-07-01) · medRxiv
- **Link / DOI:** https://www.medrxiv.org/content/10.64898/2026.06.29.26356860v1.full — DOI `10.64898/2026.06.29.26356860`
- **Relevance:** **7/10** for non-invasive venous O₂; **3/10** for the optical thrust of Topic 2 (MRI, not optical).
- **Novelty:** Self-supervised pre-training (contrastive + masked image modeling) on >48,000 cardiac images, then fine-tuning for O₂-saturation regression **with uncertainty quantification** (MAE ≈ 3.70; claimed >15 % improvement over baselines). Recovers chamber-level (intra-cardiac) blood O₂ — true mixed-venous SvO₂ — non-invasively and reference-grade.
- **Integration insights:** The label-scarce SSL + uncertainty recipe is **directly portable** to the optical side, where labelled in-vivo SvO₂ ground truth is the binding constraint (cf. §1.2). Value as a cross-modality **validation target** and transferable ML methodology. *Metadata confirmed across two search snippets; abstract not readable (medRxiv 403).*

### 1.4 — Development and Validation of a Noninvasive Model of Mixed Venous Oxygen Saturation in Heart Failure (imaging-derived iSvO₂) *(previously surfaced — scan 07-07 §1.1)*
- **Authors:** McDiarmid et al.
- **Year / Venue:** 2025/2026 · *JACC: Advances*
- **Link / DOI:** https://doi.org/10.1016/j.jacadv.2025.102484 · PMC12869880 · PMID 41609283
- **Relevance:** **7/10** — true mixed-venous, non-invasive, clinically validated (MRI, not optical).
- **Novelty:** 628-patient validation of an imaging-derived mixed-venous SvO₂ from the RV/LV blood-pool T₂ ratio on cardiac MRI (R = 0.82 vs invasive SvO₂), anchored to right-heart catheterization and an independent predictor of mortality/HF-hospitalization.
- **Integration insights:** Sets the **absolute-accuracy and outcome-relevance benchmark** any optical SvO₂ method must match, in exactly the population (heart failure) where a cheap continuous optical surrogate would be most valuable. Its internal-reference (RV vs LV) logic recurs on the optical side as artery-vs-vein calibration (§2.2). *Cross-confirmed via JACC/ScienceDirect + PMC + PubMed; full text 403 (flagged).*

### 1.5 — A New Non-Invasive Method for the Assessment of Central Venous Oxygen Saturation (Mespere VO100 jugular NIRS) *(previously surfaced — scan 06-10 §1.3)*
- **Year / Venue:** 2023 · *J. Cardiothoracic and Vascular Anesthesia* (S1053-0770(23)00782-6)
- **Link / DOI:** https://www.sciencedirect.com/science/article/pii/S1053077023007826 · PMID 37827917
- **Relevance:** **7/10** — non-invasive NIRS surrogate for ScvO₂, clinical cohort.
- **Novelty:** Validates transcutaneous jugular NIRS (Mespere VO100) against invasive ScvO₂ in critically ill patients, reporting strong linear correlation with low bias/percentage error.
- **Integration insights:** The most clinically-mature non-invasive venous-NIRS device line — the practical baseline on bias and limits-of-agreement that any optical/PA method must beat. *Cross-confirmed via ScienceDirect + PubMed 37827917; full text 403 (flagged).*

**Topic-1 honesty note:** No new non-invasive venous-O₂ paper (optical or otherwise) appeared today. All five entries are previously surfaced.

---

## Topic 2 — Optical imaging techniques for non-invasive venous blood oxygen

*One entry materially upgraded (§2.2, APM+ radial-vein detail); no brand-new primary.*

### 2.1 — Noninvasive In Vivo Photoacoustic Measurement of Internal Jugular Venous Oxygenation in Humans *(previously surfaced — flagship, scan 06-10 §2.1)*
- **Authors:** Gao / Zhu et al. (Garcia-Uribe / WashU group)
- **Year / Venue:** 2023 · arXiv preprint (dual-wavelength PAT + US)
- **Link / DOI:** https://arxiv.org/abs/2303.10775
- **Relevance:** **10/10** — the single most on-target paper in the corpus: non-invasive, in-vivo, human, **internal-jugular venous** sO₂ (sijvO₂ = 72 ± 7 %, n=7) by photoacoustics co-registered with ultrasound.
- **Novelty:** Reference demonstration that optical/PA deep-vein venous oximetry is feasible in a named deep vein in humans, with arterial-admixture-free specificity.
- **Integration insights:** The optical-imaging anchor of the entire program; every fluence-correction, phantom-metrology and inverse-modeling advance is ultimately in service of making this class of measurement clinically robust. *Confirmed via arXiv listing + ADS; abstract page 403 (flagged).*

### 2.2 — ★ UPGRADED — Arterial Blood-Mediated Deep-Tissue Photoacoustic Oximetry (APM+): in-vivo human **radial-vein** sO₂ *(previously surfaced — scan 07-05 §2.5; today reclassified from transferable-technique to a genuine venous demonstration)*
- **Authors:** Sastry / Olick-Gibson et al.
- **Year / Venue:** 2026 · *Advanced Science* (Wiley)
- **Link / DOI:** https://advanced.onlinelibrary.wiley.com/doi/10.1002/advs.76366 — DOI `10.1002/advs.76366`
- **Relevance:** **8/10** (↑ from 6–7/10 in prior scans) — now credited as an **actual non-invasive optical/PA venous sO₂ measurement in humans**, not merely a transferable arterial method.
- **Novelty:** Uses a vessel of *known* high arterial sO₂ as an in-situ fluence calibrator to defeat spectral coloring, requiring only two wavelengths and no hardware change to a standard dual-wavelength PAT system. Median error **2.9 %** (vs **9.8 %** linear unmixing) in ex-vivo-tissue phantoms. **Critically — and newly captured this scan — APM+ was demonstrated in vivo estimating the sO₂ of the *radial vein* (using the radial artery for calibration) in 8 healthy adults, yielding median venous sO₂ = 72.3 % (IQR 8.9 %), within the typical 60–80 % venous range.**
- **Integration insights:** This is the second in-vivo human non-invasive optical venous-sO₂ result in the corpus after the IJV-PA anchor (§2.1), and it is the first to reach an *absolute* (not merely relative) deep-tissue venous number via an in-situ fluence reference. The artery-as-internal-reference calibration is the deep-tissue analogue of the MRI RV/LV T₂ ratio (§1.4) and the most concrete near-term route to quantitative deep-venous PA oximetry at other sites (IJV, femoral). *Radial-vein result (median 72.3 %, IQR 8.9 %, n=8) and phantom errors cross-confirmed across two independent search snippets of the Wiley article; full text 403 (flagged).*

### 2.3 — Adaptive Spectroscopic Visible-Light OCT for Clinical Retinal Oximetry *(previously surfaced — scan 06-11 §2.2)*
- **Year / Venue:** 2023 · *Communications Medicine* (Nature) — s43856-023-00288-8
- **Link / DOI:** https://www.nature.com/articles/s43856-023-00288-8
- **Relevance:** **7/10** — resolves **retinal-vein** sO₂ at single-vessel scale (venous ~48 % vs arterial ~92 % in normals); ~1 % bias vs blood-gas in phantoms (0–100 %), ~2.1 % RMSE vs pulse oximeter in human arteries.
- **Novelty:** ADS-vis-OCT adaptively removes per-vessel spectral contaminants, giving highly repeatable (≤2.5 %) per-vessel sO₂ across vessel types — the highest-accuracy per-vessel optical oximetry demonstrated.
- **Integration insights:** The retina is the one site where per-vessel optical venous saturation is routinely achievable; its adaptive spectral-contaminant-removal is exactly the class of correction a deep-vein PA/optical system needs to reach absolute SvO₂. *Cross-confirmed via Nature + PMC10126115 + OHSU pure listing; full text 403 (flagged).*

### 2.4 — Oxygenation Heterogeneity Facilitates Spatiotemporal Flow-Pattern Visualization Inside Human Blood Vessels Using PACT *(previously surfaced — scan 06-10 §2.x)*
- **Year / Venue:** 2024 · PMC11161372
- **Link / DOI:** https://pmc.ncbi.nlm.nih.gov/articles/PMC11161372/
- **Relevance:** **8/10** — recovers, in real time, the parabolic laminar-flow wavefront inside a deep human vein in vivo via multi-wavelength PA spectra.
- **Novelty:** First real-time in-vivo laminar-flow-profile recovery inside a deep vein; couples oxygenation contrast to flow dynamics.
- **Integration insights:** Extends venous PA from static sO₂ to **flow + oxygenation jointly** — the flow leg that, combined with saturation (§2.1/§2.2), yields true venous oxygen-flux. *Cross-confirmed via PMC listing; full text 403 (flagged).*

### 2.5 — Sulfate Phantoms to Mimic NIR Photoacoustic Response of Whole Blood at Selected Oxygen Saturations *(previously surfaced — scan 07-07 §2.2; metrology)*
- **Authors:** Davenet et al. (Sorbonne Université)
- **Year / Venue:** 2026 · *Applied Optics* 65(6):1974 (also arXiv 2512.01458, submitted 2025-12-01)
- **Link / DOI:** https://arxiv.org/abs/2512.01458 · https://opg.optica.org/ao/abstract.cfm?uri=ao-65-6-1974
- **Relevance:** **7/10** — metrology enabling venous-range PA oximetry (not itself a venous measurement).
- **Novelty:** Inorganic sulfate solutions reproduce both the optical absorption *and* the Grüneisen coefficient of whole blood at chosen sO₂ over 700–850 nm, injectable into tissue-mimicking phantoms.
- **Integration insights:** You cannot claim SvO₂ accuracy at depth under unknown fluence without a ground-truth phantom matching blood's *photoacoustic* response across the venous ≈40–75 % range that arterially-tuned phantoms handle poorly — a practical prerequisite for validating the §2.1/§2.2 systems. *Cross-confirmed via arXiv abstract + Optica listing; full text 403 (flagged).*

**Topic-2 honesty note:** No brand-new optical venous-O₂ paper appeared today. The only change is the **upgrade of APM+ (§2.2)** on confirming its in-vivo human radial-vein result; all other entries are previously surfaced with scores carried forward.

---

## Standing context leads (not ranked)

- **IOPscience *J. Phys. Photonics* — "Advances in fully integrated wearable near-infrared spectroscopy: hardware innovations and biomedical applications"** (review, published 2026-05-28; DOI `10.1088/2515-7647/ae6ae4`) — surveys CW/TD/FD wearable-NIRS hardware. **Tissue-oxygenation / instrumentation, not venous SvO₂**; logged as context for the wearable-optical-SvO₂ form-factor goal (cf. §1.1).
- **IOPscience *J. Phys. Photonics* — "Low-cost point-of-care wireless multimodal wearable to monitor vitals and tissue oxygen saturation"** (2026; DOI `10.1088/2515-7647/ae637f`) — wireless wearable measuring microvascular **StO₂** + vitals. Tissue-level, not venous; context only.
- **PMC12047737 — "Quantitative assessment of thrombosis-induced blood oxygenation change in deep tissues based on photoacoustic tomography: an ex vivo study"** (accepted Mar 2025) — inner-chromophore-signal correction for spectral coloring, accurate PA spectra to 30 mm depth; deep-vein (VTE) relevant metrology. **Already surfaced 06-11 / 06-22**; carried as a standing deep-tissue PA-oximetry technique lead.
- **arXiv 2512.15394 — "Deep Learning-Driven Quantitative Spectroscopic Photoacoustic Imaging for Segmentation and Oxygen Saturation Estimation" (Hybrid-Net, Dec 2025)** — joint vessel segmentation + sO₂ without explicit fluence estimation; general PA-oximetry method, not venous-specific. Standing technique lead.
- **ISDC — Integrated Spectral and Depth Compensation for PA sO₂/THb (*J. Biomed. Opt.* 31(2):026002, Feb 2026; DOI 10.1117/1.JBO.31.2.026002; PMC12869027)** — depth+spectral fluence correction; ovarian-lesion demonstration, transferable to deep-vein PA oximetry. Catalogued 07-09; standing lead.
- **ClinicalTrials.gov NCT06632197 — capnodynamic non-invasive mixed-venous SvO₂ in adults** — non-optical clinical-reference lead.

---

## Cross-topic synthesis

1. **Today's news is a correction, not a discovery — and it strengthens the map.** APM+ (§2.2) is no longer just an "arterial method that ought to transfer." It has already been run on a **vein**: an in-vivo, non-invasive, human **radial-vein** sO₂ of **72.3 %** using the radial artery as a fluence reference. That makes it the corpus's **second in-vivo human non-invasive optical venous-oximetry result** (after the IJV-PA anchor, §2.1) and the **first to deliver an absolute deep-tissue venous number** via an in-situ calibration reference — directly attacking the field's central obstacle.

2. **The central obstacle remains absolute quantification under unknown, wavelength- and depth-dependent fluence.** The methodological leads keep converging on it from complementary sides: internal-reference calibration (APM+ §2.2; non-optically, the RV/LV T₂ ratio §1.4), modelled spectral+depth compensation (ISDC lead), fluence-free deep learning (Hybrid-Net; §1.2 DNN + Monte-Carlo), and blood-mimicking phantoms across the venous range (§2.5). A clinically accurate deep-vein SvO₂ system will likely **stack** a phantom-validated forward model, a fluence/spectral correction, and an internal reference — and APM+ is now the clearest proof that the internal-reference leg works in a real human vein.

3. **The label problem (Topic 1) and the fluence problem (Topic 2) are the two walls, and MRI is emerging as the referee.** T2/intra-cardiac CMR oximetry (§1.3, §1.4) measures true mixed-venous SvO₂ non-invasively and reference-grade — a natural validation target for the jugular optical sensor (§1.1) and deep-vein PA/APM+ (§2.1–2.2), which chronically lack a non-invasive gold standard. The SSL + uncertainty recipe (§1.3) is portable to the label-starved optical side.

4. **The retina remains the proving ground.** Vis-OCT (§2.3, ~2 % accuracy/repeatability) already resolves per-vessel venous sO₂ routinely; it is where the spectral-unmixing and vessel-segmentation algorithms mature before a systemic deep-vein program adopts them. PACT venous-flow recovery (§2.4) adds the flow leg that, combined with saturation, would yield true venous oxygen-flux.

5. **Sparseness confirmed, not padded.** Across full sweeps of PubMed, arXiv, bioRxiv/medRxiv, Optica, SPIE, Wiley, Nature, MDPI and IOPscience, **no new venous-specific primary paper post-dated 07-13.** The only substantive change was a corrected/upgraded reading of an existing paper. Genuinely novel non-invasive **venous-optical** work continues to publish at very low volume; the §2.1 IJV-PA anchor, the now-upgraded §2.2 APM+ radial-vein result, and the §2.3 retinal vis-OCT result remain the anchors, and nothing newer displaces them.

**Open gaps (carried forward, still open):** (a) no continuous, calibrated, wearable optical SvO₂ device validated against blood-gas; (b) beyond APM+'s single-vessel radial-vein demonstration, no quantitative deep-venous PA sO₂ with an in-situ fluence reference across multiple deep sites and the full venous 40–75 % range; (c) no non-invasive optical/PA SvO₂ method benchmarked head-to-head against reference CMR oximetry — a study the maturity of §1.3/§1.4 now makes feasible.
