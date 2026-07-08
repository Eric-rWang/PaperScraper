# Venous Oxygen Research Scan — 2026-07-08

**Scan scope:** Non-invasive venous blood oxygen monitoring (Topic 1) + optical imaging techniques for venous oxygen saturation (Topic 2).
**Prior scans in this repository:** 2026-06-10, 06-11, 06-14, 06-16, 06-17, 06-18, 06-19, 06-21, 06-22, 06-24, 06-25, 06-29, 06-30, 07-01, 07-03, 07-04, 07-05, 07-07. Every paper entered in those files — plus all items in their "previously surfaced," "honorable mentions," "reviewed and excluded" and "standing leads" sections — has already been catalogued and is not re-entered here except where the task's "top 5 per topic" mandate requires re-listing the best-available landmark work, in which case it is **explicitly flagged as previously surfaced**.
**Search window:** This is the **nineteenth scan** in the series, run **one day** after 2026-07-07. Emphasis on work published or first-surfacing after 07-07, with the standard fallback to the best-available venous-specific work already catalogued. Sources searched today: PubMed/PMC, arXiv, bioRxiv/medRxiv, Optica (Biomed. Opt. Express, Optics Letters, Applied Optics), SPIE / *J. Biomed. Opt.*, *Photoacoustics* (ScienceDirect), IEEE Xplore, Nature / *Sci. Rep.*, Wiley (*Advanced Science*), Elsevier (*CHEST*, *JACC: Advances*), IOPscience, Springer, De Gruyter, Frontiers, MDPI, ClinicalTrials.gov, ResearchGate, Semantic Scholar, ADS, Europe PMC, Science.gov.
**Verification caveat:** As in every prior scan, publisher **full-text** pages — including arxiv.org, opg.optica.org, pmc.ncbi.nlm.nih.gov, sciencedirect.com and the Wiley/Nature domains — returned **HTTP 403** to direct `WebFetch` in this environment today (re-confirmed on the arXiv abstract page for 2303.10775). Every reference below was therefore cross-checked across **at least two independent search-index sources**; per-item notes state what was confirmed and what could not be read directly on a publisher page.

---

## ⚠️ Read this first — day summary (NO new primary papers today)

This is a **one-day short-cycle scan** and, unlike the unusually productive 07-07 cycle (which added three new primary papers), **today's exhaustive multi-angle search surfaced no not-previously-catalogued primary papers** for either topic.

Repeated searches across every angle the series tracks — photoacoustic/optoacoustic oximetry (incl. arXiv 2512.15394 "Hybrid-Net" and photoacoustic vector tomography), NIRS/jugular venous oximetry, diffuse-optical/DOT/DCS cerebral SvO₂, hyperspectral retinal oximetry, visible-light OCT, SFDI, wearable optical sensors, capnodynamic mixed-venous methods, and the CMR-T₂ MRI reference — **re-surfaced only papers already catalogued** across the eighteen prior files. The two most recent primary candidates that appeared in today's results (arXiv **2512.15394**, Hybrid-Net spectroscopic-PA segmentation/sO₂; and **photoacoustic vector tomography**, PMC11136879) were both confirmed to be **already present in prior scans** and are not re-entered.

Accordingly, the ranked slots below are the **best-available already-catalogued corpus**, re-listed to satisfy the task's "top 5 per topic" mandate and **each flagged as previously surfaced** with honest relevance scores. No arterial-only SpO₂ padding was added to any ranked slot beyond the single explicitly-justified transferable-technique entry (§2.5). The standing scientific map is **unchanged** from 07-07.

---

## Topic 1 — Non-Invasive Monitoring of Venous Blood Oxygen (SvO₂ / ScvO₂ / Peripheral Venous Oxygenation)

### 1.1 — Estimation of Venous Oxygen Saturation Through Non-Invasive Optical Sensing at the Jugular Veins *(previously surfaced — scan 06-10 §1.1)*
- **Authors:** J. R. Hill, C. Campbell, J. G. Chase, J. L. Knopp (Pretty) — University of Canterbury
- **Year / Venue:** 2024 · *Current Directions in Biomedical Engineering* (De Gruyter) 10(4)
- **Link / DOI:** https://doi.org/10.1515/cdbme-2024-2072
- **Relevance:** **9 / 10** — the closest published **non-invasive, named-vein, optical** SvO₂ result. A pulse-oximeter-like optical sensor over the **external jugular vein** isolated the EJV waveform and returned SvO₂ in the healthy 60–90 % range (EJV-pulse 70.4–72.2 %; breathing-pulse 74.1–75.3 %) in 3 subjects. True venous (not tissue StO₂).
- **Novelty:** Demonstrates a simple transcutaneous optical probe over a superficial jugular vein can extract a venous pulsatile signal and yield a physiologically plausible SvO₂ — a direct step toward a "venous pulse oximeter."
- **Integration insights:** The superficial/cheap optical analogue of the deep IJV-PA result (Topic 2 §2.1); together they bracket the venous-optical problem from the superficial and deep ends. Small n and no invasive co-oximetry reference remain the gaps. **Verification:** title/authors/venue/DOI cross-confirmed via De Gruyter listing + ResearchGate (re-confirmed today); full text 403 (flagged).

### 1.2 — Development and Validation of a Noninvasive Model of Mixed Venous Oxygen Saturation in Heart Failure *(previously surfaced — scan 07-07 §1.1)*
- **Authors:** A. K. McDiarmid, B. S. Chambers, D. A. Broadbent, R. Patel, G. Matthews, O. Gonzalez-Fernandez, S. Plein, P. Garg, P. P. Swoboda
- **Year / Venue:** 2025/2026 · *JACC: Advances* (article 102484)
- **Link / DOI:** https://doi.org/10.1016/j.jacadv.2025.102484 · PMC12869880 · PMID 41609283
- **Relevance:** **8.5 / 10** — a genuinely non-invasive, **true mixed-venous SvO₂** estimate (imaging-derived iSvO₂) validated at unusually large scale (628 patients). Loses points only because the modality is **MRI, not optical** — so it informs, rather than instantiates, the optical program.
- **Novelty:** Models iSvO₂ from the **ratio of RV-to-LV blood-pool T₂ relaxation times** (deoxy-Hb shortens RV-pool T₂), calibrated against invasive right-heart catheterization in 30 patients, then validated in 628 newly-diagnosed HF patients where iSvO₂ was **prognostic** for all-cause mortality / HF hospitalization over ~3-year median follow-up.
- **Integration insights:** Establishes the **absolute-accuracy and outcome-relevance benchmark** any optical SvO₂ method must ultimately match — and does so in exactly the population (heart failure, where SvO₂ tracks cardiac output) where a cheap continuous optical surrogate would be most valuable. The internal-reference (RV vs LV) logic recurs across the optical methods below. **Verification:** title/authors/method/cohort cross-confirmed via JACC/ScienceDirect listing + PMC record + prior-scan cross-reference; full text 403 (flagged).

### 1.3 — Quantifying Changes in Oxygen Saturation of the Internal Jugular Vein In Vivo Using Deep Neural Networks and Subject-Specific 3-D Monte-Carlo Models *(previously surfaced — scan 06-10 §1.2)*
- **Authors:** Y. Sun et al.
- **Year / Venue:** 2024 · *Optics Letters* 49(10):2669
- **Link / DOI:** https://opg.optica.org/ol/abstract.cfm?uri=ol-49-10-2669
- **Relevance:** **8 / 10** — multi-channel NIRS + subject-specific Monte-Carlo + DNN to recover **internal-jugular** SijvO₂ changes non-invasively. Deep-vein, true venous target.
- **Novelty:** Couples subject-specific 3-D anatomy (Monte-Carlo photon transport) with a learned inverse model, directly addressing the partial-volume / overlying-tissue problem that defeats naïve transcutaneous NIRS over a deep vein.
- **Integration insights:** The modeling backbone (subject-specific MC + DNN inverse) is the template any deep-vein optical SvO₂ method — PA or NIRS — will need for clinical accuracy; the arterial-prior fluence-calibration idea (§2.5) slots naturally into it. **Verification:** confirmed via Optica listing + PubMed index (re-confirmed today).

### 1.4 — A New Non-Invasive Method for the Assessment of Central Venous Oxygen Saturation (Mespere VO100 jugular NIRS) *(previously surfaced — scan 06-10 §1.3)*
- **Authors:** Jeleff et al.
- **Year / Venue:** 2023 · *J. Cardiothorac. Vasc. Anesth.* (PMID 37827917)
- **Link / DOI:** https://www.sciencedirect.com/science/article/pii/S1053077023007826
- **Relevance:** **8 / 10** — a **79-patient** clinical cohort comparing transcutaneous jugular NIRS (Mespere VO100) against invasive ScvO₂. Among the largest human validations of a non-invasive venous-oximetry device.
- **Novelty:** Real clinical-scale device validation against the invasive standard — the cohort size the optical-venous field most lacks.
- **Integration insights:** Sets the empirical bias/limits-of-agreement bar optical/PA methods must beat for clinical adoption. **Verification:** confirmed via PubMed + ScienceDirect index (re-confirmed today).

### 1.5 — Non-Invasive Peripheral Venous Saturation via NIRS Venous-Occlusion in 226 Preterm Neonates *(previously surfaced — scan 06-24 §1.1)*
- **Authors:** Mileder et al.
- **Year / Venue:** 2022 · *Frontiers in Pediatrics* 10:834045 (also PMC8831784)
- **Link / DOI:** https://doi.org/10.3389/fped.2022.834045
- **Relevance:** **7 / 10** — largest venous-occlusion-NIRS cohort for **peripheral venous** saturation; true venous (occlusion-derived), not tissue StO₂.
- **Novelty:** Establishes feasibility and reference ranges for the venous-occlusion surrogate at population scale in a fragile cohort.
- **Integration insights:** Anchors the practical low-cost peripheral-venous surrogate branch against which optical vessel-resolved methods can be compared. **Verification:** confirmed via PubMed/PMC + Frontiers index (re-confirmed today).

> **Topic 1 sparseness note:** **No new Topic-1 primary paper this cycle.** §1.1–1.5 are the best-available already-catalogued corpus, re-listed to satisfy the "top 5" mandate and each flagged as previously surfaced. The most recent genuinely-new Topic-1 primary remains the 07-07 MRI iSvO₂ validation (§1.2 here).

---

## Topic 2 — Optical Imaging Techniques for Non-Invasively Obtaining Venous Blood Oxygen

### 2.1 — Noninvasive In Vivo Photoacoustic Measurement of Internal Jugular Venous Oxygenation in Humans *(previously surfaced — scan 06-10 §2.1)*
- **Authors:** Gao / Zhu et al. (arXiv 2303.10775)
- **Year / Venue:** 2023 · arXiv preprint (dual-wavelength PAT + US)
- **Link / DOI:** https://arxiv.org/abs/2303.10775
- **Relevance:** **9 / 10** — the flagship demonstration of **deep-vein, true venous** optical oximetry: dual-wavelength PAT/US imaged the **internal jugular vein** in 7 healthy volunteers and computed IJV sO₂ ≈ **72 ± 7 %**, matching literature.
- **Novelty:** First human non-invasive photoacoustic SvO₂ at a named deep vein — proof that optoacoustics can reach and quantify a clinically relevant deep venous target.
- **Integration insights:** The deep-vein anchor of the whole program; every fluence-correction (§2.5), phantom-metrology (§2.2) and inverse-modeling (§1.3) advance is ultimately in service of making this class of measurement clinically robust. **Verification:** confirmed via arXiv listing + ADS (re-confirmed today); abstract page 403 to direct fetch (flagged).

### 2.2 — Sulfate Phantoms to Mimic NIR Photoacoustic Response of Whole Blood at Selected Oxygen Saturations *(previously surfaced — scan 07-07 §2.2)*
- **Authors:** L. Davenet, A. Billon, J. Battaglia, S. L. Bridal, J. Gateau — Sorbonne Université (LIB)
- **Year / Venue:** 2026 · *Applied Optics* 65(6):1974 (also arXiv 2512.01458, submitted 2025-12-01)
- **Link / DOI:** https://arxiv.org/abs/2512.01458 · https://opg.optica.org/ao/abstract.cfm?uri=ao-65-6-1974
- **Relevance:** **7 / 10** — not a venous measurement itself, but **enabling metrology** for the multi-wavelength PA oximetry that any deep-vein PA-SvO₂ system depends on. Directly transferable, hence retained.
- **Novelty:** Provides a recipe for **injectable inorganic (sulfate) solutions** that reproduce **both** the optical absorption spectrum **and** the Grüneisen (thermoelastic) coefficient of whole blood at **chosen oxygenation levels** across **700–850 nm** — a stable, reproducible, non-clotting alternative to whole blood for validating PA oximeters.
- **Integration insights:** Venous PA oximetry's core difficulty is quantitative accuracy at depth under unknown fluence; you cannot claim SvO₂ accuracy without a ground-truth phantom that matches blood's *photoacoustic* (not just optical) response across the venous 40–75 % range that arterially-tuned phantoms handle poorly. A practical prerequisite for validating §2.1/§2.5 systems. **Verification:** title/authors/affiliation/wavelength range cross-confirmed via arXiv abstract + Optica *Applied Optics* listing; both full-text pages 403 (flagged).

### 2.3 — Development and Validation of a High-Resolution Hyperspectral Imaging System for the Retina *(previously surfaced — scan 07-07 §2.3)*
- **Authors:** M. H. Tran, M. Bryarly, K. Pruitt, A. Ali, I. Emordi, A. Jahadi, B. Fei — UT Southwestern (precursor: SPIE 13410, 2025; Proc. SPIE 12836, 2024)
- **Year / Venue:** 2026 journal paper (PMC12997856; accepted 2026-02-24)
- **Link / DOI:** https://pmc.ncbi.nlm.nih.gov/articles/PMC12997856/ *(journal name/DOI to confirm)* · precursor SPIE https://doi.org/10.1117/12.3047906
- **Relevance:** **7.5 / 10** — a **vessel-resolved optical** system that **directly reports retinal venule sO₂** (≈ **76 %**, vs arteriole ≈ 96 %), i.e. true venous saturation in a named vessel class, non-invasively. Retinal (not systemic) venous, hence not a full 10.
- **Novelty:** Dual-camera design fuses **hyperspectral** and **high-resolution RGB** channels so that **vessel diameter and per-vessel oxygenation are extracted simultaneously**; algorithms validated on a mouse retinal phantom then in anesthetized mice, now advanced to the human-system validation stage.
- **Integration insights:** Slots into the retinal-oximetry proving-ground branch alongside vis-OCT (§2.4). The retina is the one site where per-vessel optical venous saturation is routinely achievable, making it the natural testbed for the spectral-unmixing / vessel-segmentation algorithms a systemic deep-vein optical program (§2.1) must eventually generalize. Simultaneous diameter+sO₂ also connects to flow×saturation → venous oxygen-flux. **Verification:** title/date cross-confirmed via PMC record + UT Southwestern profile + SPIE precursor; venule sO₂ from SPIE precursor; PMC full text 403 (journal/DOI flagged unverified).

### 2.4 — Adaptive Spectroscopic Visible-Light OCT for Clinical Retinal Oximetry *(previously surfaced — scan 06-11 §2.2)*
- **Authors:** Beckmann, Miller et al. (Northwestern)
- **Year / Venue:** 2023 · *Communications Medicine* 3:39 (also PMC10126115)
- **Link / DOI:** https://www.nature.com/articles/s43856-023-00288-8
- **Relevance:** **8 / 10** — vessel-resolved retinal oximetry with **arterial and venous** sO₂; ADS-vis-OCT agrees with a blood-gas machine to ~**1 % bias** across 0–100 % ex vivo, with repeated-measurement SD ≈ 2.3 % in veins in vivo.
- **Novelty:** Adaptively removes per-vessel spectral contaminants, enabling accurate absolute sO₂ under the unique optical conditions of each vessel — a key robustness advance for clinical retinal oximetry.
- **Integration insights:** The high-accuracy optical benchmark for per-vessel venous saturation; its adaptive-spectral-correction philosophy parallels the fluence-correction (§2.5) and phantom-calibration (§2.2) strategies needed for systemic deep-vein optical SvO₂. **Verification:** confirmed via Nature + PMC index (re-confirmed today).

### 2.5 — Arterial Blood-Mediated Deep-Tissue Photoacoustic Oximetry (APM+) *(previously surfaced — scan 07-05 §2.5; arterial-demonstrated, transferable-technique clause)*
- **Authors:** Sastry et al.
- **Year / Venue:** 2026 · *Advanced Science* (DOI 10.1002/advs.76366)
- **Link / DOI:** https://advanced.onlinelibrary.wiley.com/doi/10.1002/advs.76366
- **Relevance:** **7 / 10** — arterial-demonstrated, but the **arterial-prior fluence-calibration** method maps directly onto the artery-and-vein-run-together anatomy (carotid/IJV, femoral) a deep-vein PA-SvO₂ system must exploit.
- **Novelty:** Uses a vessel of *known* high saturation (an artery) as an **in-situ fluence calibrator** to defeat spectral coloring, cutting median sO₂ error to **2.9 %** (vs 9.8 % for linear unmixing) with only **two wavelengths**.
- **Integration insights:** The most concrete recent recipe for absolute PA sO₂ at depth; its "reference-vessel-calibrates-a-neighbour" logic is exactly what a carotid-calibrated IJV venous measurement would use, and it echoes the RV/LV internal-reference idea in the §1.2 MRI paper. **Verification:** confirmed via Wiley listing + prior-scan cross-reference; Wiley full text 403 (flagged).

> **Topic 2 sparseness note:** **No new Topic-2 primary paper this cycle.** §2.1–2.4 are re-listed landmark/near-term corpus (each flagged previously surfaced); §2.5 is the single transferable-technique entry carried forward. The most recent genuinely-new Topic-2 primaries remain the 07-07 sulfate-phantom metrology (§2.2) and hyperspectral retinal venule sO₂ (§2.3).

---

## Standing context leads (not ranked)

- **arXiv 2512.15394 — "Deep Learning-Driven Quantitative Spectroscopic Photoacoustic Imaging for Segmentation and Oxygen Saturation Estimation" (Hybrid-Net, Dec 2025)** — joint vessel segmentation + sO₂ estimation trained on Monte-Carlo breast-tissue PA data at 700/850 nm. **Already catalogued in prior scans**; general PA-oximetry method, not venous-specific — carried as a standing technique lead.
- **Photoacoustic vector tomography for deep haemodynamic imaging (PMC11136879, 2024)** — images deep blood flow >5× the optical diffusion limit, incl. deep veins. **Already catalogued**; a *flow* (not saturation) method, carried as a standing lead relevant to venous oxygen-flux.
- **"Emerging Technology for Noninvasively Measuring Oxygen Saturations," *CHEST* 169(2):401–410 (Feb 2026; DOI 10.1016/j.chest.2025.09.025)** — landscape review of optics-/camera-/AI-based non-invasive SpO₂/StO₂; **arterial/tissue-oriented, not venous-specific**. Standing context review.
- **Capnodynamic non-invasive mixed-venous SvO₂ trial (ClinicalTrials.gov NCT06632197)** and **respiration-frequency-selected NIRS cerebral SvO₂ tracking (Sci. Rep. 2023, s41598-023-49078-1)** — non-optical / tissue-composite venous surrogates, already catalogued; carried as standing leads.
- **Wearable NIRS via the carotid** (PMC12384115, 2025) and **wearable-NIRS hardware review** (*J. Phys. Photonics* 2026, 10.1088/2515-7647/ae6ae4) — general wearable-NIRS instrumentation (arterial/tissue), standing technique leads.

---

## Cross-Topic Synthesis

Today is a **null-result short-cycle scan**: one day after the productive 07-07 cycle, exhaustive multi-angle searching surfaced **no not-previously-catalogued primary papers** for either topic. This is the expected baseline for this niche — genuinely novel non-invasive *venous* optical work publishes at very low volume, and most one- to two-day cycles add zero. The scientific map is therefore **unchanged from 07-07**, and the honest read is that the corpus is stable rather than growing this cycle.

The through-line of that stable map remains the **internal-reference principle**: absolute non-invasive venous saturation is reachable not through a standalone absorption read but through a compartment of *known* oxygenation calibrating the unknown venous one — the LV-vs-RV blood-pool T₂ ratio in the MRI reference (§1.2), an artery calibrating a neighbouring vessel's fluence in APM+ (§2.5), and per-vessel adaptive/hyperspectral spectral references in retinal oximetry (§2.3, §2.4). The **validation stack** the field now leans on is likewise unchanged: MRI-T₂ iSvO₂ as the outcome-anchored absolute benchmark (§1.2), blood-matched sulfate PA phantoms as bench-side ground truth across the venous 40–75 % range (§2.2), and the retina as the per-vessel optical proving ground (§2.3, §2.4).

**Honest volume note:** zero new primary papers today. The three ranked "front-line" entries (Hill superficial-jugular optical SvO₂, §1.1; Gao/Zhu deep IJV photoacoustic, §2.1; the 07-07 MRI/phantom/hyperspectral additions) continue to bracket the problem, but the core gap the series tracks — **non-invasive human deep-vein optical SvO₂ validated at clinical scale** — remains open and is not advanced by anything found today.
