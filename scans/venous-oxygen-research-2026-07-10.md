# Venous Oxygen Research Scan — 2026-07-10

**Search window:** This is the **twenty-first scan** in the series, run **one day** after 2026-07-09. Emphasis on work published or first-surfacing after 07-09, with the standard fallback to the best-available venous-specific work already catalogued. Sources searched today: PubMed/PMC, arXiv, bioRxiv/medRxiv, Optica (Biomed. Opt. Express, Optics Letters, Applied Optics), SPIE / *J. Biomed. Opt.*, *Photoacoustics* (ScienceDirect), IEEE Xplore, Nature / *Sci. Rep.*, Wiley (*Advanced Science*), Elsevier (*CHEST*, *JACC: Advances*), IOPscience, Springer, De Gruyter, Frontiers, MDPI, ClinicalTrials.gov, ResearchGate, Semantic Scholar, ADS, Europe PMC, Science.gov.

**Verification caveat:** As in every prior scan, publisher **full-text** pages — including arxiv.org, opg.optica.org, pmc.ncbi.nlm.nih.gov, sciencedirect.com and the Wiley/Nature domains — returned **HTTP 403** to direct `WebFetch` in this environment today (re-confirmed on PMC12024819). Every reference below was therefore cross-checked across **at least two independent search-index sources**; per-item notes state what was confirmed and what could not be read directly on a publisher page.

## ⚠️ Read this first — day summary (NO new primary papers today)

Repeated searches across every angle the series tracks — deep-vein/IJV photoacoustic oximetry (arXiv 2303.10775), NIRS/jugular venous oximetry (Mespere VO100; respiration-frequency-filtered cerebral SvO₂), diffuse-optical/DCS cerebral SvO₂/CMRO₂, hyperspectral retinal oximetry, visible-light OCT retinal oximetry, SFDI tissue oxygenation, wearable/PPG venous methods, capnodynamic mixed-venous methods, and the CMR-T₂ MRI reference — **re-surfaced only papers already catalogued** across the twenty prior files. The candidate items that appeared newest in today's results (arXiv **2512.15394** "Hybrid-Net" spectroscopic-PA; **ISDC** PA fluence compensation, *J. Biomed. Opt.* 31(2):026002; PMC12024819 "ML-based VO₂ estimation from wearable multiwavelength PPG") were each checked: the first two are **already catalogued**, and the third is an **oxygen-consumption (VO₂), not venous-saturation (SvO₂)** paper — not a venous slot (logged as a standing lead).

Accordingly, the ranked slots below are the **best-available already-catalogued corpus**, re-listed to satisfy the task's "top 5 per topic" mandate and **each flagged as previously surfaced** with honest relevance scores. No arterial-only SpO₂ padding was added to any ranked slot beyond the single explicitly-justified transferable-technique entry (§2.5). The standing scientific map is **unchanged** from 07-09.

## Topic 1 — Non-Invasive Monitoring of Venous Blood Oxygen (SvO₂ / ScvO₂ / Peripheral Venous Oxygenation)

### 1.1 — Estimation of Venous Oxygen Saturation Through Non-Invasive Optical Sensing at the Jugular Veins *(previously surfaced — scan 06-10 §1.1)*
- **Authors:** Alqahtani et al.
- **Year / Venue:** 2024 · *Current Directions in Biomedical Engineering* 10(2) (De Gruyter; CDBME-2024-2072)
- **Link / DOI:** https://doi.org/10.1515/cdbme-2024-2072
- **Relevance:** 8/10 (true, non-invasive, optical, venous — but n=3, no invasive co-oximetry reference)
- **Novelty:** A pulse-oximeter-like optical sensor placed over the external jugular vein correctly isolates the EJV waveform and estimates SvO₂ (71.1 %, 72.2 %, 70.4 %) within the healthy 60–90 % range.
- **Integration insights:** The superficial/cheap optical analogue of the deep IJV-PA result (Topic 2 §2.1); together they bracket the venous-optical problem from the superficial and deep ends. Small n and no invasive co-oximetry reference remain the gaps. **Verification:** title/authors/venue/DOI cross-confirmed via De Gruyter listing + ResearchGate (re-confirmed today); full text 403 (flagged).

### 1.2 — Development and Validation of a Noninvasive Model of Mixed Venous Oxygen Saturation in Heart Failure *(previously surfaced — scan 07-07 §1.1)*
- **Authors:** McDiarmid et al.
- **Year / Venue:** 2025/2026 · *JACC: Advances*
- **Link / DOI:** https://doi.org/10.1016/j.jacadv.2025.102484 · PMC12869880 · PMID 41609283
- **Relevance:** 7/10 (true mixed-venous, non-invasive — but MRI, not optical)
- **Novelty:** A 628-patient validation of an imaging-derived mixed-venous SvO₂ (iSvO₂) from the RV/LV blood-pool T₂ ratio on cardiac MRI, anchored to right-heart catheterization and shown to be prognostic for mortality/HF-hospitalization.
- **Integration insights:** Establishes the **absolute-accuracy and outcome-relevance benchmark** any optical SvO₂ method must ultimately match — in exactly the population (heart failure) where a cheap continuous optical surrogate would be most valuable. The internal-reference (RV vs LV) logic recurs across the optical methods below (artery vs vein in PA, cf. §2.5). **Verification:** title/authors/method/cohort cross-confirmed via JACC/ScienceDirect listing + PMC record; full text 403 (flagged).

### 1.3 — Quantifying Changes in Oxygen Saturation of the Internal Jugular Vein In Vivo Using Deep Neural Networks and Subject-Specific 3-D Monte-Carlo Models *(previously surfaced — scan 06-10 §1.2)*
- **Year / Venue:** 2024 · *Optics Letters* 49(10):2669
- **Link / DOI:** https://opg.optica.org/ol/abstract.cfm?uri=ol-49-10-2669
- **Relevance:** 7/10 (IJV-specific, non-invasive, inverse-modeling for venous saturation change)
- **Novelty:** DNNs trained on subject-specific 3-D Monte-Carlo models recover IJV saturation *changes* non-invasively, tying measured optical signal back to a physically-modelled forward problem.
- **Integration insights:** The inverse-modeling/fluence-correction leg of the program; complementary to the deep-vein PA anchor (§2.1) and the phantom-metrology work (§2.2). **Verification:** title/venue/citation cross-confirmed via Optica listing + Semantic Scholar; full text 403 (flagged).

### 1.4 — A New Non-Invasive Method for the Assessment of Central Venous Oxygen Saturation (Mespere VO100 jugular NIRS) *(previously surfaced — scan 06-10 §1.3)*
- **Year / Venue:** 2023 · *J. Cardiothoracic and Vascular Anesthesia* (S1053-0770(23)00782-6)
- **Link / DOI:** https://www.sciencedirect.com/science/article/pii/S1053077023007826 · PMID 37827917
- **Relevance:** 7/10 (non-invasive NIRS surrogate for ScvO₂, clinical cohort)
- **Novelty:** Validates transcutaneous jugular NIRS (Mespere VO100) against invasive ScvO₂ in critically ill patients as a continuous non-invasive central-venous surrogate.
- **Integration insights:** The most clinically-mature non-invasive venous-NIRS device line; the practical baseline any optical/PA method must beat on bias and limits-of-agreement. **Verification:** title/venue/PMID cross-confirmed via ScienceDirect + PubMed; full text 403 (flagged).

### 1.5 — Non-Invasive Peripheral Venous Saturation via NIRS Venous-Occlusion in 226 Preterm Neonates *(previously surfaced — scan 06-24 §1.1)*
- **Year / Venue:** 2022 · *Frontiers in Pediatrics* 10:834045
- **Link / DOI:** https://doi.org/10.3389/fped.2022.834045
- **Relevance:** 6/10 (peripheral venous SvO₂, non-invasive NIRS, large cohort — occlusion-based, not continuous)
- **Novelty:** NIRS venous-occlusion peripheral SvO₂ measured in a large (n=226) preterm-neonate cohort, demonstrating feasibility of the occlusion approach at scale in a fragile population.
- **Integration insights:** Anchors the peripheral (limb) venous-oximetry branch and the venous-occlusion signal-isolation strategy that PPG/optical methods (§1.1) reuse. **Verification:** title/venue/DOI cross-confirmed via Frontiers + PMC listing; full text 403 (flagged).

## Topic 2 — Optical Imaging Techniques for Non-Invasively Obtaining Venous Blood Oxygen

### 2.1 — Noninvasive In Vivo Photoacoustic Measurement of Internal Jugular Venous Oxygenation in Humans *(previously surfaced — scan 06-10 §2.1)*
- **Authors:** Gao / Zhu et al.
- **Year / Venue:** 2023 · arXiv preprint (dual-wavelength PAT + US)
- **Link / DOI:** https://arxiv.org/abs/2303.10775
- **Relevance:** 9/10 (true deep-vein SvO₂, non-invasive, optical, in humans)
- **Novelty:** Dual-wavelength photoacoustic tomography co-registered with ultrasound images the IJV in 7 healthy volunteers, yielding sijvO₂ = 72 ± 7 % — the reference demonstration that optical/PA deep-vein venous oximetry is feasible in humans.
- **Integration insights:** The deep-vein anchor of the whole program; every fluence-correction (§2.5, ISDC lead), phantom-metrology (§2.2) and inverse-modeling (§1.3) advance is ultimately in service of making this class of measurement clinically robust. **Verification:** confirmed via arXiv listing + ADS (re-confirmed today); abstract page 403 (flagged).

### 2.2 — Sulfate Phantoms to Mimic NIR Photoacoustic Response of Whole Blood at Selected Oxygen Saturations *(previously surfaced — scan 07-07 §2.2)*
- **Authors:** Davenet et al. (Sorbonne Université)
- **Year / Venue:** 2026 · *Applied Optics* 65(6):1974 (also arXiv 2512.01458, submitted 2025-12-01)
- **Link / DOI:** https://arxiv.org/abs/2512.01458 · https://opg.optica.org/ao/abstract.cfm?uri=ao-65-6-1974
- **Relevance:** 7/10 (metrology enabling venous-range PA oximetry; not itself a venous measurement)
- **Novelty:** Inorganic sulfate solutions that reproduce both the optical absorption *and* the Grüneisen coefficient of whole blood at chosen sO₂ over 700–850 nm, injectable into tissue-mimicking phantoms.
- **Integration insights:** You cannot claim SvO₂ accuracy at depth under unknown fluence without a ground-truth phantom matching blood's *photoacoustic* (not just optical) response across the venous ≈40–75 % range that arterially-tuned phantoms handle poorly — a practical prerequisite for validating §2.1/§2.5 systems. **Verification:** title/authors/affiliation/wavelength range cross-confirmed via arXiv abstract + Optica *Applied Optics* listing; both full-text pages 403 (flagged).

### 2.3 — Development and Validation of a High-Resolution Hyperspectral Imaging System for the Retina *(previously surfaced — scan 07-07 §2.3)*
- **Year / Venue:** 2026 (received Nov 2025, accepted Feb 2026, published Mar 2026)
- **Link / DOI:** https://pmc.ncbi.nlm.nih.gov/articles/PMC12997856/ *(journal name/DOI to confirm)* · precursor SPIE https://doi.org/10.1117/12.3047906
- **Relevance:** 6/10 (per-vessel retinal venous sO₂ testbed; not systemic venous)
- **Novelty:** A snapshot-hyperspectral + high-res RGB retinal system extracting vessel diameter and oxygenation simultaneously; reported arterial ≈90 % vs venous ≈70 % sO₂.
- **Integration insights:** The retina is the one site where per-vessel optical venous saturation is routinely achievable, making it the natural testbed for the spectral-unmixing / vessel-segmentation algorithms a systemic deep-vein optical program (§2.1) must eventually generalize; simultaneous diameter+sO₂ also connects to flow×saturation → venous oxygen-flux. **Verification:** title/date cross-confirmed via PMC record + UT Southwestern profile + SPIE precursor; venule sO₂ from SPIE precursor; PMC full text 403 (journal/DOI flagged unverified).

### 2.4 — Adaptive Spectroscopic Visible-Light OCT for Clinical Retinal Oximetry *(previously surfaced — scan 06-11 §2.2)*
- **Year / Venue:** 2023 · *Communications Medicine* (s43856-023-00288-8)
- **Link / DOI:** https://www.nature.com/articles/s43856-023-00288-8
- **Relevance:** 6/10 (per-vessel retinal venous sO₂; label-free, high accuracy — retinal-only)
- **Novelty:** ADS-vis-OCT adaptively removes per-vessel spectral contaminants; in ex-vivo blood phantoms it agrees with a blood-gas machine to within 1 % bias across 0–100 % sO₂.
- **Integration insights:** The highest-accuracy per-vessel optical oximetry demonstrated; its adaptive spectral-contaminant-removal is exactly the class of correction a deep-vein PA/optical system needs to reach absolute SvO₂. **Verification:** title/venue cross-confirmed via Nature + PMC (PMC10126115) + PubMed 37095177; full text 403 (flagged).

### 2.5 — Arterial Blood-Mediated Deep-Tissue Photoacoustic Oximetry (APM+) *(previously surfaced — scan 07-05 §2.5; arterial-demonstrated, transferable-technique clause)*
- **Authors:** Sastry et al.
- **Year / Venue:** 2026 · *Advanced Science* (DOI 10.1002/advs.76366)
- **Link / DOI:** https://advanced.onlinelibrary.wiley.com/doi/10.1002/advs.76366
- **Relevance:** 6/10 (arterial-demonstrated, but the internal-reference calibration is directly transferable to venous)
- **Novelty:** Uses a vessel of *known* saturation as an in-situ fluence calibrator to recover absolute deep-tissue sO₂ — attacking the same unknown-fluence problem that blocks absolute deep-vein PA-SvO₂.
- **Integration insights:** *Included under the transferable-technique clause:* the artery-as-internal-reference calibration is the deep-tissue analogue of §1.2's RV/LV T₂ ratio and a candidate front-end for making the IJV/femoral PA oximeter (§2.1) absolute rather than relative. **Verification:** title/authors/DOI cross-confirmed via Wiley listing + Semantic Scholar; full text 403 (flagged).

## Standing context leads (not ranked)

- **ISDC — Integrated Spectral and Depth Compensation for PA sO₂/THb (Wang et al., *J. Biomed. Opt.* 31(2):026002, Feb 2026; DOI 10.1117/1.JBO.31.2.026002; PMC12869027)** — depth+spectral fluence correction for quantitative PA sO₂; ovarian-lesion demonstration (82 lesions), transferable to deep-vein PA oximetry. **Catalogued 07-09**; carried as a standing technique lead.
- **arXiv 2512.15394 — "Deep Learning-Driven Quantitative Spectroscopic Photoacoustic Imaging for Segmentation and Oxygen Saturation Estimation" (Hybrid-Net, Dec 2025)** — joint vessel segmentation + sO₂ estimation trained on Monte-Carlo breast-tissue PA data at 700/850 nm; provides sO₂ without explicit fluence estimation. **Already catalogued**; general PA-oximetry method, not venous-specific — standing technique lead.
- **PMC12024819 — "Machine Learning-Based VO₂ Estimation Using a Wearable Multiwavelength Photoplethysmography Device"** — surfaced newest today, but targets **oxygen consumption (VO₂), not venous saturation (SvO₂)**; wearable-PPG angle only. Logged as a standing lead, **not** promoted into a venous slot. *(Full text 403; scope inferred from title/abstract listing.)*
- **"Emerging Technology for Noninvasively Measuring Oxygen Saturations," *CHEST* 169(2):401–410 (Feb 2026; DOI 10.1016/j.chest.2025.09.025)** — landscape review of optics-/camera-/AI-based non-invasive SpO₂/StO₂; **arterial/tissue-oriented, not venous-specific**. Standing context review.
- **ClinicalTrials.gov NCT06632197 — "Non-invasive Monitoring of Mixed Venous Oxygen Saturation Using the Capnodynamic Method in Adults"** — non-optical (capnodynamic) mixed-venous SvO₂; carried as the non-optical clinical-reference lead.

## Cross-Topic Synthesis

The picture is unchanged from the last several scans, and today adds no new primary venous paper — consistent with the series' running observation that genuinely novel *non-invasive venous-specific* work publishes at low volume. The field's structure remains:

1. **Two anchor demonstrations bracket the depth axis.** Superficial/cheap optical jugular sensing (Topic 1 §1.1, EJV PPG) and deep-vein photoacoustic IJV oximetry (Topic 2 §2.1, Gao/Zhu 72 ± 7 %) show non-invasive venous saturation is measurable at both the shallow and deep ends; neither yet delivers catheter-grade *absolute* SvO₂ in routine use.

2. **The central obstacle is absolute quantification under unknown, wavelength- and depth-dependent fluence.** Every methodological lead this cycle attacks that same problem from a different side: internal-reference calibration (APM+ §2.5; and, non-optically, the RV/LV T₂ ratio §1.2), modelled spectral+depth compensation (ISDC lead), fluence-free deep learning (Hybrid-Net lead; §1.3 DNN Monte-Carlo), and ground-truth blood-mimicking phantoms across the venous range (§2.2). These are complementary, not competing — a clinically accurate deep-vein SvO₂ system will likely stack a phantom-validated forward model, a fluence/spectral correction, and an internal reference.

3. **The retina remains the proving ground.** Vis-OCT (§2.4, ~1 % phantom bias) and hyperspectral retinal imaging (§2.3) already resolve per-vessel venous sO₂ routinely; they are where the spectral-unmixing and vessel-segmentation algorithms mature before a systemic deep-vein program can adopt them.

4. **Clinical benchmarks are getting stronger while optical primaries stall.** The 628-patient MRI iSvO₂ validation (§1.2) and the mature jugular-NIRS device line (§1.4) set the accuracy and outcome-relevance bar any optical method must clear. The gap the field most needs closed is still an *in-vivo optical/PA deep-vein study with paired invasive co-oximetry* across the full venous 40–75 % range — none appeared today.

*Honesty note:* no new venous-specific primary paper was found on 2026-07-10; all ranked entries are previously surfaced and flagged as such, with relevance scores reflecting the transferable-but-not-venous status of §2.5 and the tissue/retinal (vs true systemic SvO₂) status of §§2.3–2.4.
