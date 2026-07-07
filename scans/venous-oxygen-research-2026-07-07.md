# Venous Oxygen Research Scan — 2026-07-07

**Scan scope:** Non-invasive venous blood oxygen monitoring (Topic 1) + optical imaging techniques for venous oxygen saturation (Topic 2).
**Prior scans in this repository:** 2026-06-10, 06-11, 06-14, 06-16, 06-17, 06-18, 06-19, 06-21, 06-22, 06-24, 06-25, 06-29, 06-30, 07-01, 07-03, 07-04, 07-05. Every paper entered in those files — plus all items in their "previously surfaced," "honorable mentions," "reviewed and excluded" and "standing leads" sections — has already been catalogued and is not re-entered here except where the task's "top 5 per topic" mandate requires re-listing the best-available landmark work, in which case it is **explicitly flagged as previously surfaced**.
**Search window:** This is the **eighteenth scan** in the series, run **two days** after 2026-07-05. Emphasis on work published or first-surfacing after 07-05, with the standard fallback to the best-available venous-specific work already catalogued. Sources searched today: PubMed/PMC, arXiv, bioRxiv/medRxiv, Optica (Biomed. Opt. Express, Optics Letters, Applied Optics), SPIE / *J. Biomed. Opt.*, *Photoacoustics* (ScienceDirect), IEEE Xplore, Nature / *Sci. Rep.*, Wiley (*Advanced Science*), Elsevier (*CHEST*, *JACC: Advances*), IOPscience, Springer, De Gruyter, Frontiers, MDPI, ClinicalTrials.gov, ResearchGate, Semantic Scholar, ADS, Europe PMC, Science.gov.
**Verification caveat:** As in every prior scan, essentially all publisher **full-text** pages — including arxiv.org, opg.optica.org, pmc.ncbi.nlm.nih.gov, ebi.ac.uk/europepmc, jacc.org and sciencedirect.com — returned **HTTP 403** to direct `WebFetch` in this environment today (re-confirmed on the arXiv abstract page, the Optica *Applied Optics* page, the PMC hyperspectral page and the Europe PMC REST API). Every reference below was therefore cross-checked across **at least two independent search-index sources**; per-item notes state what was confirmed and what could not be read directly on a publisher page.

---

## ⚠️ Read this first — day summary (three genuinely new primary papers)

Unlike the several short-cycle scans that preceded it, **this scan surfaced three not-previously-catalogued primary papers** plus one new review, spanning both topics:

1. **★ NEW (Topic 1) — McDiarmid et al., "Development and Validation of a Noninvasive Model of Mixed Venous Oxygen Saturation in Heart Failure," *JACC: Advances* 2025/2026 (DOI 10.1016/j.jacadv.2025.102484; PMC12869880; PMID 41609283).** A **628-patient** validation of a **non-invasive imaging-derived mixed-venous SvO₂ (iSvO₂)** built from the **RV/LV blood-pool T₂ ratio** on cardiac MRI, anchored to invasive right-heart catheterization in a 30-patient discovery cohort and shown to be **prognostic** for mortality/HF-hospitalization. This is the concrete, large-N validation paper that the "CMR-T₂ absolute reference" the series has cited abstractly for weeks actually rests on. **Non-optical (MRI)**, but **true mixed-venous** and non-invasive → promoted into Topic 1's Top-5 (§1.1).
2. **★ NEW (Topic 2) — Davenet et al., "Sulfate phantoms to mimic NIR photoacoustic response of whole blood at selected oxygen saturations," *Applied Optics* 65(6):1974 (2026) (arXiv 2512.01458; Sorbonne Université).** A recipe for **inorganic (sulfate) solutions** that reproduce the **optical absorption *and* Grüneisen coefficient** of whole blood at chosen sO₂ over **700–850 nm**, injectable into tissue-mimicking phantoms to test the spectral/sensitivity performance of multi-wavelength PA oximeters. A **metrology/validation** contribution → Topic 2 Top-5 (§2.2).
3. **★ NEW (Topic 2) — Tran, … Fei et al., "Development and validation of a high-resolution hyperspectral imaging system for the retina," 2026 journal paper (PMC12997856; UT Southwestern; precursor SPIE 13410, 2025).** A dual-camera HSI retina system that **simultaneously extracts vessel diameter and per-vessel oxygenation**, reporting **venule sO₂ ≈ 76 %** vs arteriole ≈ 96 %. Directly measures **retinal venous** saturation → Topic 2 Top-5 (§2.3).

One further **not-previously-catalogued** item is a **review, not a venous primary paper**: **"Emerging Technology for Noninvasively Measuring Oxygen Saturations," *CHEST* 169(2):401–410 (Feb 2026; DOI 10.1016/j.chest.2025.09.025).** It surveys optics-/camera-/AI-based non-invasive SpO₂ and StO₂ but is **arterial/tissue-oriented**, not venous-specific; it is logged as a **standing context review** below, not promoted into a ranked slot.

Beyond these, repeated multi-angle searches (photoacoustic/optoacoustic, NIRS, diffuse-optical/DOT, hyperspectral, vis-OCT, SFDI, wearable/e-tattoo, retinal, jugular, capnodynamic, MRI-reference) **re-surfaced only papers already catalogued** across the seventeen prior files. No arterial-only SpO₂ padding was added to any ranked slot beyond the explicitly-justified transferable-technique entry (§2.5). The standing scientific map is **unchanged**, with two new tools (MRI-T₂ SvO₂ validation; PA-oximetry phantom metrology) and one new venous-resolving optical modality instance (hyperspectral retinal venule sO₂) added to the toolbox.

---

## Topic 1 — Non-Invasive Monitoring of Venous Blood Oxygen (SvO₂ / ScvO₂ / Peripheral Venous Oxygenation)

### 1.1 — ★ NEW — Development and Validation of a Noninvasive Model of Mixed Venous Oxygen Saturation in Heart Failure *(newly catalogued this cycle)*
- **Authors:** A. K. McDiarmid, B. S. Chambers, D. A. Broadbent, R. Patel, G. Matthews, O. Gonzalez-Fernandez, S. Plein, P. Garg, P. P. Swoboda
- **Year / Venue:** 2025/2026 · *JACC: Advances* (article 102484)
- **Link / DOI:** https://doi.org/10.1016/j.jacadv.2025.102484 · PMC12869880 · PMID 41609283
- **Relevance:** **8.5 / 10** — a genuinely non-invasive, **true mixed-venous SvO₂** estimate (imaging-derived iSvO₂) validated at unusually large scale. Loses points only because the modality is **MRI, not optical** — so it informs, rather than instantiates, the optical program.
- **Novelty:** Models iSvO₂ from the **ratio of RV-to-LV blood-pool T₂ relaxation times** (deoxy-Hb shortens RV-pool T₂), calibrated against invasive right-heart catheterization in 30 patients, then validated in **628** newly-diagnosed HF patients where iSvO₂ was **prognostic** for all-cause mortality / HF hospitalization over a ~3-year median follow-up. This is the concrete large-cohort paper behind the "CMR-T₂ absolute venous reference" the series has cited.
- **Integration insights:** Establishes the **absolute-accuracy and outcome-relevance benchmark** any optical SvO₂ method must ultimately match — and does so in exactly the population (heart failure, where SvO₂ tracks cardiac output) where a cheap continuous optical surrogate would be most valuable. The T₂-ratio idea also reinforces why an *internal* reference (RV vs LV here; artery vs vein in PA, cf. §2.5) is the recurring route to absolute venous saturation. **Verification:** title/authors/method/cohort cross-confirmed via JACC/ScienceDirect listing + PMC record + Medscape 2026 coverage; full text 403 to direct fetch (flagged).

### 1.2 — Estimation of Venous Oxygen Saturation Through Non-Invasive Optical Sensing at the Jugular Veins *(previously surfaced — scan 06-10 §1.1)*
- **Authors:** J. R. Hill, C. Campbell, J. G. Chase, J. L. Knopp (Pretty) — University of Canterbury
- **Year / Venue:** 2024 · *Current Directions in Biomedical Engineering* (De Gruyter) 10(4)
- **Link / DOI:** https://doi.org/10.1515/cdbme-2024-2072
- **Relevance:** **9 / 10** — the closest published **non-invasive, named-vein, optical** SvO₂ result. A pulse-oximeter-like optical sensor over the **external jugular vein** isolated the EJV waveform and returned SvO₂ in the healthy 60–90 % range (EJV-pulse 70.4–72.2 %; breathing-pulse 74.1–75.3 %) in 3 subjects. True venous (not tissue StO₂).
- **Novelty:** Demonstrates a simple transcutaneous optical probe over a superficial jugular vein can extract a venous pulsatile signal and yield a physiologically plausible SvO₂ — a direct step toward a "venous pulse oximeter."
- **Integration insights:** The superficial/cheap optical analogue of the deep IJV-PA result (Topic 2 §2.1); together they bracket the venous-optical problem from the superficial and deep ends. Small n and no invasive co-oximetry reference remain the gaps. **Verification:** title/authors/venue/DOI cross-confirmed via De Gruyter listing + ResearchGate (re-confirmed today); full text 403 (flagged).

### 1.3 — Quantifying Changes in Oxygen Saturation of the Internal Jugular Vein In Vivo Using Deep Neural Networks and Subject-Specific 3-D Monte-Carlo Models *(previously surfaced — scan 06-10 §1.2)*
- **Authors:** Y. Sun et al.
- **Year / Venue:** 2024 · *Optics Letters* 49(10):2669
- **Link / DOI:** https://opg.optica.org/ol/abstract.cfm?uri=ol-49-10-2669
- **Relevance:** **8 / 10** — multi-channel NIRS + subject-specific Monte-Carlo + DNN to recover **internal-jugular** SijvO₂ changes non-invasively. Deep-vein, true venous target.
- **Novelty:** Couples subject-specific 3-D anatomy (Monte-Carlo photon transport) with a learned inverse model, directly addressing the partial-volume / overlying-tissue problem that defeats naïve transcutaneous NIRS over a deep vein.
- **Integration insights:** The modeling backbone (subject-specific MC + DNN inverse) is the template any deep-vein optical SvO₂ method — PA or NIRS — will need for clinical accuracy; the APM+ fluence-calibration idea (§2.5) slots naturally into it. **Verification:** confirmed via Optica listing + PubMed index (re-confirmed today).

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

> **Topic 1 sparseness note:** One genuinely new primary paper (§1.1) this cycle — the first *new* Topic-1 primary since the 06-24 neonatal-occlusion entry. §1.2–1.5 are the best-available already-catalogued corpus, re-listed to satisfy the "top 5" mandate and flagged as previously surfaced.

---

## Topic 2 — Optical Imaging Techniques for Non-Invasively Obtaining Venous Blood Oxygen

### 2.1 — Noninvasive In Vivo Photoacoustic Measurement of Internal Jugular Venous Oxygenation in Humans *(previously surfaced — scan 06-10 §2.1)*
- **Authors:** Gao / Zhu et al. (arXiv 2303.10775)
- **Year / Venue:** 2023 · arXiv preprint (dual-wavelength PAT + US)
- **Link / DOI:** https://arxiv.org/abs/2303.10775
- **Relevance:** **9 / 10** — the flagship demonstration of **deep-vein, true venous** optical oximetry: dual-wavelength PAT/US imaged the **internal jugular vein** in 7 healthy volunteers and computed IJV sO₂ ≈ **72 ± 7 %**, matching literature.
- **Novelty:** First human non-invasive photoacoustic SvO₂ at a named deep vein — proof that optoacoustics can reach and quantify a clinically relevant deep venous target.
- **Integration insights:** The deep-vein anchor of the whole program; every fluence-correction (§2.5), phantom-metrology (§2.2) and inverse-modeling (§1.3) advance is ultimately in service of making this class of measurement clinically robust. **Verification:** confirmed via arXiv listing + ADS (re-confirmed today); PDF 403 to direct fetch (flagged).

### 2.2 — ★ NEW — Sulfate Phantoms to Mimic NIR Photoacoustic Response of Whole Blood at Selected Oxygen Saturations *(newly catalogued this cycle)*
- **Authors:** L. Davenet, A. Billon, J. Battaglia, S. L. Bridal, J. Gateau — Sorbonne Université (LIB)
- **Year / Venue:** 2026 · *Applied Optics* 65(6):1974 (also arXiv 2512.01458, submitted 2025-12-01)
- **Link / DOI:** https://doi.org/10.1364/AO.548xxx *(DOI to confirm)* · https://arxiv.org/abs/2512.01458 · https://opg.optica.org/ao/abstract.cfm?uri=ao-65-6-1974
- **Relevance:** **7 / 10** — not a venous measurement itself, but **enabling metrology** for the multi-wavelength PA oximetry that any deep-vein PA-SvO₂ system depends on. Directly transferable, hence included.
- **Novelty:** Provides a recipe for **injectable inorganic (sulfate) solutions** that reproduce **both** the optical absorption spectrum **and** the Grüneisen (thermoelastic) coefficient of whole blood at **chosen oxygenation levels** across **700–850 nm** — a stable, reproducible, non-clotting alternative to whole blood for validating the spectral/sensitivity performance of PA oximeters.
- **Integration insights:** Venous PA oximetry's core difficulty is quantitative accuracy at depth under unknown fluence; you cannot claim SvO₂ accuracy without a ground-truth phantom that matches blood's *photoacoustic* (not just optical) response. This gives the field a standardized calibration target spanning the exact venous saturation range (≈40–75 %) that arterially-tuned phantoms handle poorly — a practical prerequisite for validating §2.1/§2.5 systems. **Verification:** title/authors/affiliation/wavelength range cross-confirmed via arXiv abstract + Optica *Applied Optics* listing (AO 65(6):1974); both full-text pages 403 to direct fetch — exact page DOI string flagged as unverified pending a readable publisher page.

### 2.3 — ★ NEW — Development and Validation of a High-Resolution Hyperspectral Imaging System for the Retina *(newly catalogued this cycle)*
- **Authors:** M. H. Tran, M. Bryarly, K. Pruitt, A. Ali, I. Emordi, A. Jahadi, B. Fei — UT Southwestern (precursor: SPIE 13410, 2025; Proc. SPIE 12836, 2024)
- **Year / Venue:** 2026 journal paper (PMC12997856; received 2025-11-06, accepted 2026-02-24, issue Mar 2026)
- **Link / DOI:** https://pmc.ncbi.nlm.nih.gov/articles/PMC12997856/ *(journal name/DOI to confirm)* · precursor SPIE https://doi.org/10.1117/12.3047906
- **Relevance:** **7.5 / 10** — a **vessel-resolved optical** system that **directly reports retinal venule sO₂** (≈ **76 %**, vs arteriole ≈ 96 %), i.e. true venous saturation in a named vessel class, non-invasively. Retinal (not systemic) venous, hence not a full 10.
- **Novelty:** Dual-camera design fuses **hyperspectral** and **high-resolution RGB** channels so that **vessel diameter and per-vessel oxygenation are extracted simultaneously**; algorithms validated on a mouse retinal phantom then in anesthetized mice, now advanced to the human-system validation stage in the 2026 journal version.
- **Integration insights:** Slots into the retinal-oximetry proving-ground branch alongside vis-OCT (§2.4). The retina is the one site where per-vessel optical venous saturation is routinely achievable, making it the natural testbed for algorithms (spectral unmixing, vessel segmentation, oxygenation mapping) that a systemic deep-vein optical program (§2.1) must eventually generalize. The simultaneous diameter+sO₂ readout also connects to flow×saturation → venous oxygen-flux estimation. **Verification:** title/date cross-confirmed via PMC record + UT Southwestern Pure profile + SPIE precursor listings; venule sO₂ value taken from the SPIE precursor (dual-camera system); PMC full text 403 to direct fetch — journal name/DOI flagged as unverified pending a readable page.

### 2.4 — Adaptive Spectroscopic Visible-Light OCT for Clinical Retinal Oximetry *(previously surfaced — scan 06-11 §2.2)*
- **Authors:** Beckmann, Miller et al. (Northwestern)
- **Year / Venue:** 2023 · *Communications Medicine* 3:39 (also PMC10126115)
- **Link / DOI:** https://www.nature.com/articles/s43856-023-00288-8
- **Relevance:** **8 / 10** — vessel-resolved retinal oximetry with **arterial and venous** sO₂; ADS-vis-OCT agrees with a blood-gas machine to ~**1 % bias** across 0–100 % ex vivo.
- **Novelty:** Adaptively removes per-vessel spectral contaminants, enabling accurate absolute sO₂ under the unique optical conditions of each vessel — a key robustness advance for clinical retinal oximetry.
- **Integration insights:** The high-accuracy optical benchmark for per-vessel venous saturation; its adaptive-spectral-correction philosophy parallels the fluence-correction (§2.5) and phantom-calibration (§2.2) strategies needed for systemic deep-vein optical SvO₂. **Verification:** confirmed via Nature + PMC index (re-confirmed today).

### 2.5 — Arterial Blood-Mediated Deep-Tissue Photoacoustic Oximetry (APM+) *(previously surfaced — scan 07-05 §2.5; arterial-demonstrated, transferable-technique clause)*
- **Authors:** Sastry et al.
- **Year / Venue:** 2026 · *Advanced Science* (DOI 10.1002/advs.76366)
- **Link / DOI:** https://advanced.onlinelibrary.wiley.com/doi/10.1002/advs.76366
- **Relevance:** **7 / 10** — arterial-demonstrated, but the **arterial-prior fluence-calibration** method maps directly onto the artery-and-vein-run-together anatomy (carotid/IJV, femoral) a deep-vein PA-SvO₂ system must exploit.
- **Novelty:** Uses a vessel of *known* high saturation (an artery) as an **in-situ fluence calibrator** to defeat spectral coloring, cutting median sO₂ error to **2.9 %** (vs 9.8 % for linear unmixing) with only **two wavelengths**.
- **Integration insights:** The most concrete recent recipe for absolute PA sO₂ at depth; its "reference-vessel-calibrates-a-neighbour" logic is exactly what a carotid-calibrated IJV venous measurement would use, and it echoes the RV/LV internal-reference idea in the new §1.1 MRI paper. **Verification:** confirmed via Wiley listing + prior-scan cross-reference; Wiley full text 403 (flagged).

> **Topic 2 sparseness note:** Two genuinely new primary papers this cycle (§2.2 phantom metrology; §2.3 hyperspectral retinal venule sO₂), both included on true-venous-relevance or direct-transferability grounds. §2.1, §2.4 are re-listed landmark corpus (flagged previously surfaced); §2.5 is the transferable-technique entry carried from 07-05.

---

## Standing context leads (not ranked)

- **★ NEW review — "Emerging Technology for Noninvasively Measuring Oxygen Saturations," *CHEST* 169(2):401–410 (Feb 2026; DOI 10.1016/j.chest.2025.09.025).** Surveys optics-, white-light-, camera- and AI-based non-invasive SpO₂/StO₂ measurement. **Arterial/tissue-oriented, not venous-specific** — logged as a landscape review for the instrumentation context, not promoted into a ranked slot. *Verification: title/volume/pages/DOI cross-confirmed via CHEST + ScienceDirect + OVID listings; full text 403.*
- **Wearable NIRS via the carotid** (PMC12384115, 2025) and **wearable-NIRS hardware review** (*J. Phys. Photonics* 2026, 10.1088/2515-7647/ae6ae4) — general wearable-NIRS instrumentation (arterial/tissue), carried as standing technique leads from prior scans.

---

## Cross-Topic Synthesis

The recurring architecture of the whole field — visible again in **three** of today's entries — is the **internal reference**: use a compartment of known oxygenation to calibrate the unknown venous one. The new MRI paper (§1.1) does it with the **LV blood pool** (arterial) calibrating the **RV blood pool** (venous) via a T₂ ratio; APM+ (§2.5) does it with an **artery** calibrating a neighbouring vessel's fluence; retinal oximetry (§2.4, §2.3) does it implicitly per-vessel with adaptive/hyperspectral spectral references. This convergence is the strongest signal that **absolute non-invasive venous saturation is reachable only through relative, self-referencing measurement**, not standalone absorption reads.

Today also sharpened the **validation stack**. §1.1 supplies the **outcome-anchored absolute reference** (628-patient MRI-T₂ SvO₂, prognostic against RHC) that optical methods must ultimately match; §2.2 supplies the **bench-side ground truth** (blood-matched sulfate PA phantoms across the venous 40–75 % range) needed to certify PA oximeter accuracy before any in-vivo venous claim; and §2.3 extends the **vessel-resolved optical proving ground** (retinal venule sO₂ from hyperspectral imaging) alongside vis-OCT. The map is unchanged but better instrumented at both ends: MRI remains the absolute clinical benchmark, the retina remains the per-vessel optical testbed, and the **internal jugular vein remains the unfilled prize** for truly non-invasive human deep-vein optical SvO₂ at clinical scale.

**Honest volume note:** three new primary papers in one cycle is above this niche's baseline (most short-cycle scans add zero). Two are *enabling/reference* work (MRI validation, PA phantom metrology) rather than new venous optical instruments, and the one new optical venous instrument (§2.3) is **retinal**, not systemic — so the core gap the series tracks, **non-invasive human deep-vein optical SvO₂**, is not yet closed by anything found today.
