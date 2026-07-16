# Venous Oxygen Research Scan — 2026-07-16

**Search window:** Twenty-fifth scan in the series, run **one day** after 2026-07-15. Emphasis on work published or first-surfacing after 07-15, with the standard fallback to the best-available venous-specific work already catalogued. Sources searched today: PubMed/PMC, arXiv, bioRxiv/medRxiv, Optica (Biomed. Opt. Express, Optics Letters, Applied Optics), SPIE / *J. Biomed. Opt.*, *Photoacoustics* (ScienceDirect), IEEE Xplore, Nature / *Sci. Rep.* / *Commun. Med.*, Wiley (*Advanced Science*), IOPscience (*J. Phys. Photonics*), MDPI (*Biosensors*/*Sensors*), Springer (*BioMed. Eng. OnLine*), De Gruyter, ClinicalTrials.gov, ResearchGate, Semantic Scholar, ADS.

**Verification caveat:** As in every prior scan, publisher **full-text** pages — including arxiv.org, opg.optica.org, pmc.ncbi.nlm.nih.gov, sciencedirect.com, iopscience.iop.org and the Wiley/Nature domains — returned **HTTP 403** to direct `WebFetch` in this environment today (re-confirmed on arXiv 2303.10775). Every reference below was therefore cross-checked across **at least two independent search-index snippets**; per-item notes state what was confirmed and what could not be read directly on a publisher page.

---

## ⚠️ Read this first — day summary

**No new venous-specific paper today — optical or otherwise.** Today's full sweep returned nothing first-appearing since the 07-15 scan. Every item surfaced is **previously catalogued**: the IJV-PA anchor (arXiv 2303.10775), the jugular optical sensor (De Gruyter CDBME), the IJV DNN + Monte-Carlo work (*Optics Letters*), the APM+ radial-vein photoacoustic result (*Advanced Science*), the intra-cardiac SSL-MRI oximetry preprint (medRxiv), the imaging-derived iSvO₂ heart-failure model (*JACC: Advances*), the Mespere VO100 jugular NIRS device, retinal vis-OCT oximetry, PACT venous-flow visualization, and the ISDC / sulfate-phantom PA-metrology leads.

Two 2026 IOPscience wearable-NIRS items again appeared newest in the raw results — a low-cost multimodal **StO₂** wearable (`10.1088/2515-7647/ae637f`) and a wearable-NIRS hardware review (`10.1088/2515-7647/ae6ae4`, published 2026-05-28) — but both remain **tissue-level StO₂ / instrumentation**, not venous SvO₂, and are logged only as standing context. Consistent with the series' standing observation, **truly novel non-invasive venous-optical work is published at very low volume**; today produced no new primary. The lists below are therefore the best-available standing set, each item honestly flagged as previously surfaced with its relevance score carried forward.

---

## Topic 1 — Non-invasive monitoring of venous blood oxygen (SvO₂ / ScvO₂ / peripheral venous)

*No new items today.* Standing best-available set (all previously surfaced), scores carried forward:

### 1.1 — Estimation of Venous Oxygen Saturation Through Non-Invasive Optical Sensing at the Jugular Veins *(previously surfaced — scan 06-10 §1.1; flagship optical-venous device paper)*
- **Authors:** Alqahtani et al.
- **Year / Venue:** 2024 · *Current Directions in Biomedical Engineering* 10(2) (De Gruyter; CDBME-2024-2072)
- **Link / DOI:** https://doi.org/10.1515/cdbme-2024-2072
- **Relevance:** **8/10** — true, non-invasive, optical, venous (but n=3, no invasive co-oximetry reference).
- **Novelty:** A pulse-oximeter-style optical sensor over the external jugular vein isolates the EJV waveform and returns SvO₂ estimates (~70–72 %) within the healthy 60–90 % band — still the closest thing to a wearable-form-factor optical SvO₂ device in the literature.
- **Integration insights:** The superficial/low-cost optical analogue of the deep IJV-PA anchor (§2.1); together they bracket the venous-optical problem from the shallow and deep ends. Its open problem — calibration against a blood-gas gold standard — is exactly what the APM+ artery-as-reference approach (§2.2) and MRI reference oximetry (§1.3/§1.4) aim to close. *Metadata cross-confirmed via De Gruyter listing + ResearchGate; full text 403 (flagged).*

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

*No new items today.* Standing best-available set (all previously surfaced), scores carried forward:

### 2.1 — Noninvasive In Vivo Photoacoustic Measurement of Internal Jugular Venous Oxygenation in Humans *(previously surfaced — flagship, scan 06-10 §2.1)*
- **Authors:** Gao / Zhu et al. (Garcia-Uribe / WashU group)
- **Year / Venue:** 2023 · arXiv preprint (dual-wavelength PAT + US)
- **Link / DOI:** https://arxiv.org/abs/2303.10775
- **Relevance:** **10/10** — the single most on-target paper in the corpus: non-invasive, in-vivo, human, **internal-jugular venous** sO₂ (sijvO₂ = 72 ± 7 %, n=7) by photoacoustics co-registered with ultrasound at 5 fps.
- **Novelty:** Reference demonstration that optical/PA deep-vein venous oximetry is feasible in a named deep vein in humans, with arterial-admixture-free specificity.
- **Integration insights:** The optical-imaging anchor of the entire program; every fluence-correction, phantom-metrology and inverse-modeling advance is ultimately in service of making this class of measurement clinically robust. *Confirmed via arXiv listing + ADS; abstract page 403 (re-confirmed today, flagged).*

### 2.2 — Arterial Blood-Mediated Deep-Tissue Photoacoustic Oximetry (APM+): in-vivo human **radial-vein** sO₂ *(previously surfaced — scan 07-05 §2.5; upgraded to a genuine venous demonstration on 07-15 §2.2)*
- **Authors:** Sastry / Olick-Gibson et al.
- **Year / Venue:** 2026 · *Advanced Science* (Wiley)
- **Link / DOI:** https://advanced.onlinelibrary.wiley.com/doi/10.1002/advs.76366 — DOI `10.1002/advs.76366`
- **Relevance:** **8/10** — an **actual non-invasive optical/PA venous sO₂ measurement in humans**, not merely a transferable arterial method.
- **Novelty:** Uses a vessel of *known* high arterial sO₂ as an in-situ fluence calibrator to defeat spectral coloring, requiring only two wavelengths and no hardware change to a standard dual-wavelength PAT system. Median error **2.9 %** (vs **9.8 %** linear unmixing) in ex-vivo-tissue phantoms. Demonstrated in vivo estimating the sO₂ of the **radial vein** (using the radial artery for calibration) in 8 healthy adults, yielding median venous sO₂ = **72.3 %** (IQR 8.9 %), within the typical 60–80 % venous range.
- **Integration insights:** The second in-vivo human non-invasive optical venous-sO₂ result in the corpus after the IJV-PA anchor (§2.1), and the first to reach an *absolute* (not merely relative) deep-tissue venous number via an in-situ fluence reference. The artery-as-internal-reference calibration is the deep-tissue analogue of the MRI RV/LV T₂ ratio (§1.4) and the most concrete near-term route to quantitative deep-venous PA oximetry at other sites (IJV, femoral). *Cross-confirmed across two independent search snippets of the Wiley article; full text 403 (flagged).*

### 2.3 — Adaptive Spectroscopic Visible-Light OCT for Clinical Retinal Oximetry *(previously surfaced — scan 06-11 §2.2)*
- **Year / Venue:** 2023 · *Communications Medicine* (Nature) — s43856-023-00288-8
- **Link / DOI:** https://www.nature.com/articles/s43856-023-00288-8
- **Relevance:** **7/10** — resolves **retinal-vein** sO₂ at single-vessel scale (venous ~48 % vs arterial ~92 % in parafoveal vessels; ~72 % venous in larger vessels); ~1 % bias vs blood-gas in phantoms (0–100 %), ~2.1 % RMSE vs pulse oximeter in human arteries.
- **Novelty:** ADS-vis-OCT adaptively removes per-vessel spectral contaminants, giving highly repeatable (≤2.5 %) per-vessel sO₂ across vessel types — the highest-accuracy per-vessel optical oximetry demonstrated, validated across CRVO/DR/glaucoma/sickle-cell.
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

**Topic-2 honesty note:** No new optical venous-O₂ paper appeared today. The list is the best-available standing set; each item is previously surfaced with its score carried forward unchanged.

---

## Standing context leads (not ranked)

- **IOPscience *J. Phys. Photonics* — "Advances in fully integrated wearable near-infrared spectroscopy: hardware innovations and biomedical applications"** (review, published 2026-05-28; DOI `10.1088/2515-7647/ae6ae4`) — surveys CW/TD/FD wearable-NIRS hardware. **Tissue-oxygenation / instrumentation, not venous SvO₂**; logged as context for the wearable-optical-SvO₂ form-factor goal (cf. §1.1).
- **IOPscience *J. Phys. Photonics* — "Low-cost point-of-care wireless multimodal wearable to monitor vitals and tissue oxygen saturation"** (2026; DOI `10.1088/2515-7647/ae637f`) — wireless wearable measuring microvascular **StO₂** + vitals. Tissue-level, not venous; context only.
- **ISDC — Integrated Spectral and Depth Compensation for PA sO₂/THb (*J. Biomed. Opt.* 31(2):026002, Feb 2026; DOI 10.1117/1.JBO.31.2.026002; PMC12869027)** — Monte-Carlo-derived spectral + depth-wise fluence correction; validated on phantoms and 82 ovarian lesions, transferable to deep-vein PA oximetry. Catalogued 07-09; standing lead.
- **PMC12047737 — "Quantitative assessment of thrombosis-induced blood oxygenation change in deep tissues based on photoacoustic tomography: an ex vivo study"** (accepted Mar 2025) — inner-chromophore-signal correction for spectral coloring, accurate PA spectra to 30 mm depth; deep-vein (VTE) relevant metrology. Already surfaced 06-11 / 06-22; standing lead.
- **arXiv 2512.15394 — "Deep Learning-Driven Quantitative Spectroscopic Photoacoustic Imaging for Segmentation and Oxygen Saturation Estimation" (Hybrid-Net, Dec 2025)** — joint vessel segmentation + sO₂ without explicit fluence estimation; general PA-oximetry method, not venous-specific. Standing technique lead.
- **ClinicalTrials.gov NCT06632197 — capnodynamic non-invasive mixed-venous SvO₂ in adults** — non-optical clinical-reference lead (estimated completion Aug 2025).

---

## Cross-topic synthesis

1. **A genuinely quiet day — no new primary, and that is the honest headline.** A full sweep of PubMed, arXiv, bioRxiv/medRxiv, Optica, SPIE, Wiley, Nature, MDPI, Springer and IOPscience surfaced **no venous-specific paper post-dating 07-15**. Nothing displaces the standing anchors, and nothing was padded in to fill the list.

2. **The corpus's two in-vivo human non-invasive optical venous results remain the map.** The IJV-PA anchor (§2.1, sijvO₂ 72 ± 7 %) and the APM+ radial-vein result (§2.2, median 72.3 %) are still the only two demonstrations of an absolute non-invasive optical/PA venous sO₂ number in a named human vein. Their close agreement (~72 %) around the expected venous band is itself corroborating, given they use independent calibration strategies (co-registered US vs artery-as-fluence-reference).

3. **The central obstacle is unchanged: absolute quantification under unknown, wavelength- and depth-dependent fluence.** The standing methodological leads keep attacking it from complementary sides — internal-reference calibration (APM+ §2.2; non-optically the RV/LV T₂ ratio §1.4), modelled spectral+depth compensation (ISDC lead), fluence-free deep learning (Hybrid-Net; §1.2 DNN + Monte-Carlo), and blood-mimicking phantoms across the venous range (§2.5). A clinically accurate deep-vein SvO₂ system will likely **stack** a phantom-validated forward model, a fluence/spectral correction, and an internal reference.

4. **MRI continues to emerge as the non-invasive referee.** T2/intra-cardiac CMR oximetry (§1.3, §1.4) measures true mixed-venous SvO₂ non-invasively and reference-grade — a natural validation target for the jugular optical sensor (§1.1) and deep-vein PA/APM+ (§2.1–2.2), which chronically lack a non-invasive gold standard. The SSL + uncertainty recipe (§1.3) is portable to the label-starved optical side; the retina (§2.3) remains the proving ground where per-vessel spectral-unmixing algorithms mature.

5. **Sparseness confirmed, not padded.** Genuinely novel non-invasive **venous-optical** work continues to publish at very low volume; today produced none. The §2.1 IJV-PA anchor, the §2.2 APM+ radial-vein result, and the §2.3 retinal vis-OCT result remain the anchors.

**Open gaps (carried forward, still open):** (a) no continuous, calibrated, wearable optical SvO₂ device validated against blood-gas; (b) beyond APM+'s single-vessel radial-vein demonstration, no quantitative deep-venous PA sO₂ with an in-situ fluence reference across multiple deep sites and the full venous 40–75 % range; (c) no non-invasive optical/PA SvO₂ method benchmarked head-to-head against reference CMR oximetry — a study the maturity of §1.3/§1.4 now makes feasible.
