# Venous Oxygen Research Scan — 2026-07-03

**Scan scope:** Non-invasive venous blood oxygen monitoring (Topic 1) + optical imaging techniques for venous oxygen saturation (Topic 2).
**Prior scans in this repository:** 2026-06-10, 06-11, 06-14, 06-16, 06-17, 06-18, 06-19, 06-21, 06-22, 06-24, 06-25, 06-29, 06-30, 07-01. Every paper entered in those files — plus all items in their "previously surfaced", "honorable mentions", "reviewed and excluded" and "standing leads" sections — has already been catalogued and is not newly re-entered here except where the task's "top 5 per topic" mandate requires re-listing the best-available landmark work, in which case it is **explicitly flagged as previously surfaced**.
**Search window:** This is the **fifteenth scan** in the series, run **two days** after 2026-07-01. Emphasis on work published or first-surfacing after 07-01, with the standard fallback to the best-available venous-specific work already catalogued. Sources searched today: PubMed/PMC, arXiv, bioRxiv/medRxiv, Optica (Biomed. Opt. Express, Optics Letters), SPIE / *J. Biomed. Opt.*, *Photoacoustics* (ScienceDirect), IEEE Xplore, Nature / *Sci. Rep.* / *Light: Sci. Appl.*, Springer, De Gruyter, Wiley (*Advanced Science*), Frontiers, MDPI, ClinicalTrials.gov, ResearchGate, Semantic Scholar, Science.gov.
**Verification caveat:** As in every prior scan, essentially all publisher **full-text** pages, plus **arxiv.org**, **clinicaltrials.gov**, and De Gruyter/Springer/Wiley, returned **HTTP 403** to direct fetches in this environment today (re-confirmed on arXiv `2303.10775` and ClinicalTrials.gov `NCT06632197`). Every reference below was cross-checked across **at least two independent search-index sources**; per-item notes state what was confirmed and what could not be read directly on a publisher page.

---

## ⚠️ Read this first — honest sparseness report

This is the **fifteenth scan** of a genuinely low-volume niche. Consistent with every preceding short-cycle scan, **no brand-new (post-2026-07-01) venous-specific primary paper surfaced** for either topic today. Repeated multi-angle searches — across photoacoustic/optoacoustic, NIRS, diffuse-optical, hyperspectral, vis-OCT, SFDI, wearable/e-tattoo, retinal, jugular, capnodynamic and MRI-reference angles — re-surfaced **only papers already catalogued** across the fourteen prior files (the IJV-PA arXiv `2303.10775`, the De Gruyter jugular optical-sensing proof-of-concept, the flexible optoacoustic "stethoscope", qPACT reviews, the Dec-2025 deep-learning spectroscopic-PA preprint `2512.15394`, adaptive-spectroscopic vis-OCT, the hyperspectral retinal system, the CMR-T₂ iSvO₂ work, the capnodynamic Capno-SvO₂ family, the heart-failure SvO₂ model, and the *Graefe's* retinal-oximetry review).

The **only genuinely not-yet-catalogued artifact** found today is a **clinical-trial registration**, not a paper: **NCT06632197 (CAPNO-SVO2)**, a capnodynamic adult SvO₂ validation study, added below as a new **standing trial lead**.

Rather than pad with arterial-only SpO₂ work (which the mandate forbids), this scan does the honest thing: it presents each topic's **best-available Top-5 ranked corpus** with honest relevance scores, **each entry explicitly flagged as previously surfaced** and pointing to the file where it was first catalogued, so this file remains a usable standalone ranking without pretending anything new was published. New this cycle: one trial lead only.

**Bottom line for the day:** the standing scientific picture from 06-14 → 07-01 is **unchanged**. MRI (CMR-T₂ / susceptometry) remains the absolute-reference venous calibrator; the retina remains the proving ground for vessel-specific optical venous saturation (vis-OCT, hyperspectral, Oxymap); the internal-jugular vein remains the flagship deep-vein optical/optoacoustic target (IJV-PA, jugular NIRS/DNN); the venous-occlusion test and venous-pulsatility PPG remain the practical peripheral surrogates; the capnodynamic Capno-SvO₂ and the IDO₂ index remain the non-optical benchmarks the optical program must beat; and **truly non-invasive human deep-vein optical SvO₂ at clinical scale remains the unfilled prize.** No arterial-only padding was added.

---

## Topic 1 — Non-Invasive Monitoring of Venous Blood Oxygen (SvO₂ / ScvO₂ / Peripheral Venous Oxygenation)

> **Sparseness flag:** No brand-new post-07-01 venous-specific primary paper. The Top-5 below is the **best-available already-catalogued corpus**, re-listed to satisfy the "top 5 per topic" mandate and **flagged as previously surfaced**. One genuinely new item — a trial registration (NCT06632197) — is added as a standing lead.

### 1.1 — Estimation of Venous Oxygen Saturation Through Non-Invasive Optical Sensing at the Jugular Veins *(previously surfaced — scan 06-10 §1.1)*
- **Authors:** J. R. Hill, C. Campbell, J. G. Chase, J. L. Knopp (Pretty) — University of Canterbury
- **Year / Venue:** 2024 · *Current Directions in Biomedical Engineering* (De Gruyter) 10(4)
- **Link / DOI:** https://doi.org/10.1515/cdbme-2024-2072
- **Relevance:** **9 / 10** — the closest published **non-invasive, named-vein, optical** SvO₂ result. A pulse-oximeter-like optical sensor over the **external jugular vein** correctly identified the EJV waveform and returned SvO₂ in the healthy 60–90 % range (EJV-pulse estimates 70.4–72.2 %; breathing-pulse estimates 74.1–75.3 %) in 3 subjects. True venous (not tissue StO₂).
- **Novelty:** Demonstrates that a simple, low-cost optical probe placed transcutaneously over a superficial jugular vein can isolate a venous pulsatile signal and yield a physiologically plausible SvO₂ — a direct step toward a "venous pulse oximeter."
- **Integration insights:** This is the peripheral/superficial optical analogue of the deep IJV-PA result (Topic 2 §2.1); together they bracket the venous-optical problem from the superficial (cheap, low-depth) and deep (expensive, high-fidelity) ends. Small n and lack of invasive co-oximetry reference are the key gaps. **Verification:** title/authors/venue/DOI cross-confirmed via De Gruyter listing + ResearchGate; De Gruyter full text 403 to direct fetch (flagged).

### 1.2 — Quantifying Changes in Oxygen Saturation of the Internal Jugular Vein In Vivo Using Deep Neural Networks and Subject-Specific 3-D Monte-Carlo Models *(previously surfaced — scan 06-10 §1.2)*
- **Authors:** Y. Sun et al.
- **Year / Venue:** 2024 · *Optics Letters* 49(10):2669
- **Link / DOI:** https://opg.optica.org/ol/abstract.cfm?uri=ol-49-10-2669
- **Relevance:** **8 / 10** — multi-channel NIRS + subject-specific Monte-Carlo + DNN to recover **internal-jugular** SijvO₂ changes non-invasively. Deep-vein, true venous target.
- **Novelty:** Couples subject-specific 3-D anatomy (Monte-Carlo photon transport) with a learned inverse model, directly addressing the partial-volume / overlying-tissue problem that defeats naïve transcutaneous NIRS over a deep vein.
- **Integration insights:** The modeling backbone (subject-specific MC + DNN inverse) is the template any deep-vein optical SvO₂ method — PA or NIRS — will need to reach clinical accuracy. **Verification:** confirmed via Optica listing + PubMed index.

### 1.3 — A New Non-Invasive Method for the Assessment of Central Venous Oxygen Saturation (Mespere VO100 jugular NIRS) *(previously surfaced — scan 06-10 §1.3)*
- **Authors:** Jeleff et al.
- **Year / Venue:** 2023 · *J. Cardiothorac. Vasc. Anesth.* (PMID 37827917)
- **Link / DOI:** https://www.sciencedirect.com/science/article/pii/S1053077023007826
- **Relevance:** **8 / 10** — a **79-patient** clinical cohort comparing transcutaneous jugular NIRS (Mespere VO100) against invasive ScvO₂. Among the largest human validations of a non-invasive venous-oximetry device.
- **Novelty:** Real clinical-scale device validation against the invasive standard, the cohort size the optical-venous field most lacks.
- **Integration insights:** Sets the empirical accuracy bar (bias/limits-of-agreement) that optical/PA methods must beat to be clinically adopted. **Verification:** confirmed via PubMed + ScienceDirect index.

### 1.4 — Non-Invasive Peripheral Venous Saturation via NIRS Venous-Occlusion in 226 Preterm Neonates *(previously surfaced — scan 06-24 §1.1)*
- **Authors:** Mileder et al.
- **Year / Venue:** 2022 · *Frontiers in Pediatrics* 10:834045
- **Link / DOI:** https://doi.org/10.3389/fped.2022.834045
- **Relevance:** **7 / 10** — largest venous-occlusion-NIRS cohort for **peripheral venous** saturation; true venous (occlusion-derived), not tissue StO₂.
- **Novelty:** Establishes feasibility and reference ranges for the venous-occlusion surrogate at population scale in a fragile cohort.
- **Integration insights:** Anchors the practical, low-cost peripheral-venous surrogate branch (thenar/limb StO₂ → venous) against which optical vessel-resolved methods can be compared. **Verification:** confirmed via PubMed + Frontiers index.

### 1.5 — Towards Simultaneous Non-Invasive Arterial and Venous Oxygenation Monitoring with a Wearable Optical E-Tattoo *(previously surfaced — scan 06-17 §1.1; IP artifact catalogued 07-01 §1.1)*
- **Authors:** P. Tan, E. Wang, S. Tamma, S. Bhattacharya, N. Lu — UT Austin
- **Year / Venue:** 2023 conference paper (PMID 38083768); US Patent Application 20250025074 (2025)
- **Link / DOI:** https://pubmed.ncbi.nlm.nih.gov/38083768/ · patent https://patents.google.com/patent/US20250025074A1/en
- **Relevance:** **7 / 10** — a **wearable** patch deriving **both arterial and venous** SO₂ from co-located wrist vessels using venous **pulsatility** (not occlusion). Peripheral venous, not central SvO₂.
- **Novelty:** Arterio-venous signal-separation on a skin-conformal PPG array; the only wearable, simultaneous A+V optical venous thread in the repository.
- **Integration insights:** Represents the commercial-translation / wearable branch; complements the induced-fluctuation (Zhang 2016/17) and jugular-pulse (Hill 2024) approaches. **Verification:** paper via PubMed; patent via Google/Justia index (full text 403, flagged).

**★ NEW this cycle — standing trial lead (not a paper):**
- **NCT06632197 — "Non-invasive Monitoring of Mixed Venous Oxygen Saturation Using the Capnodynamic Method in Adults" (CAPNO-SVO2).** Sponsor: Fundación de Investigación Biomédica — Hospital Universitario de La Princesa (Madrid). Status: **not-yet-recruiting** (est. start Dec 2024, est. completion Aug 2025). Aims to validate capnodynamic Capno-SvO₂ against invasive PAC/Swan-Ganz co-oximetry in **adults** (prior capnodynamic validation was largely pediatric). Link: https://clinicaltrials.gov/study/NCT06632197. *Non-optical* benchmark the optical program must beat; added for completeness. **Verification:** title/sponsor/status/dates cross-confirmed via ClinicalTrials.gov listing + CenterWatch + Veeva index (ClinicalTrials.gov direct fetch 403, flagged).

**Previously surfaced — other standing venous-monitoring references (NOT re-entered):** Oh et al. 2023 cerebral-NIRS ScvO₂ surrogate (`10.1038/s41598-023-49078-1`, 06-10 §1.4); Zachia Alan et al. 2022 thenar StO₂→ScvO₂ (06-10 §1.5); McDiarmid et al. 2026 CMR-T₂ iSvO₂ (06-11 §1.1); heart-failure non-invasive SvO₂ model (PMID 41609283, 06-11); Skow et al. 2025 MRI-susceptometry venous oximetry (06-14 §1.1); Lahade et al. 2026 wearable FD-NIRS A-V transition (06-11 §1.2); hDOS 2025 Durduran-group venous-occlusion platform (06-17 §1.2); Zhang et al. 2016/2017 induced-venous-fluctuation peripheral SvO₂ (06-17 §1.3); Meng et al. 2026 NIRS cerebral-oxygen review (`10.3389/fnagi.2026.1809264`, 06-29 §1.1); capnodynamic Capno-SvO₂ family (ICMx 2025 `10.1186/s40635-025-00741-z`, *Sci. Rep.* 2024, *Anesth. Analg.* 2024) and the IDO₂ index (06-30 §1.1–1.2); peripheral-venous-vs-co-oximetry validation + artificial-venous-pulse PPG family (06-22).

**Standing trial leads (carried forward):** NCT01891188 (hepatic-vein NIRS); NCT06511999 (post-arrest jugular SjO₂, recruiting from Sep 2025); NCT05161884 (MRI-reference ScvO₂ validation); NCT04624009 / NCT04778150 (SjvO₂ NIRS in critically-ill / liver-transplant patients); NCT04885699 (capnodynamic SvO₂ validation); **NCT06632197 (capnodynamic adult SvO₂ — new this cycle).**

---

## Topic 2 — Optical Imaging Techniques for Non-Invasive Venous Blood Oxygen

> **Sparseness flag:** No brand-new post-07-01 optical-venous primary paper. The Top-5 below is the **best-available already-catalogued corpus**, re-listed to satisfy the "top 5 per topic" mandate and **flagged as previously surfaced**.

### 2.1 — Noninvasive In Vivo Photoacoustic Measurement of Internal Jugular Venous Oxygenation in Humans *(previously surfaced — flagship, catalogued from scan 06-10 onward)*
- **Authors:** (IJV-PA group) — dual-wavelength PAT + ultrasound
- **Year / Venue:** 2023 · arXiv 2303.10775
- **Link:** https://arxiv.org/abs/2303.10775
- **Relevance:** **10 / 10** — the **flagship deep-vein optical venous** result: dual-wavelength PAT+US imaged the **internal jugular vein** and estimated **SijvO₂ ≈ 72 ± 7 %** in **7 healthy volunteers**, with fast US co-registration enabling temporal tracking. True named-vein venous saturation at clinically meaningful depth.
- **Novelty:** First human, in-vivo, image-based, non-invasive SijvO₂ from a deep vein — the closest existing analogue to invasive jugular-bulb oximetry.
- **Integration insights:** The single most important proof that optical/optoacoustic imaging can reach a deep venous target non-invasively; every other Topic-2 entry is best read as either enabling it (qPACT fluence correction, DL unmixing, phantoms) or providing a vessel-resolved alternative (retinal vis-OCT/hyperspectral). Clinical-cohort validation remains the missing next step. **Verification:** SijvO₂ ≈ 72 ± 7 %, n = 7 cross-confirmed across multiple index sources and consistent across 14 prior scans; arXiv abs/PDF returned 403 to direct fetch today (flagged) — metadata not re-read on source this cycle.

### 2.2 — Adaptive Spectroscopic Visible-Light OCT for Clinical Retinal Oximetry *(previously surfaced — catalogued in prior scans)*
- **Authors:** (Northwestern / vis-OCT group)
- **Year / Venue:** 2023 · *Communications Medicine* (also PMC10126115; PMID 37095177)
- **Link / DOI:** https://www.ncbi.nlm.nih.gov/pmc/articles/PMC10126115/
- **Relevance:** **9 / 10** — vessel-resolved retinal **vein** sO₂ (venules ≈ 72 %) with adaptive spectral-contaminant removal, reporting ~1 % bias across 0–100 % in validation. The most accurate vessel-specific optical venous-saturation method in the corpus.
- **Novelty:** ADS spectral correction adapts per-vessel, overcoming the wavelength-dependent contaminants that limited earlier vis-OCT oximetry — enabling clinic-grade repeatability.
- **Integration insights:** The retina is the accessible "window vessel" where optical venous oximetry is already near-quantitative; its ~1 % bias is the accuracy target deep-vein PA/NIRS methods aspire to. **Verification:** confirmed via PMC + PubMed index.

### 2.3 — Flexible Optoacoustic "Blood Stethoscope" — Wearable Arterial + Venous sO₂ Patch *(previously surfaced — scan 06-30 §2.1)*
- **Year / Venue:** 2023 · *Nature Communications*
- **Link:** (Nat. Commun. 2023; catalogued 06-30 §2.1)
- **Relevance:** **8 / 10** — a skin-conformal optoacoustic patch reporting **both arterial and venous** sO₂ from underlying vessels; the wearable-hardware frontier for deep-vessel optoacoustic oximetry.
- **Novelty:** Miniaturized, flexible acoustic-detection front end — addressing the rigid-transducer / power bottleneck that blocks wearable PACT.
- **Integration insights:** The transducer-engineering complement to the IJV-PA science (§2.1); the wearable-acoustic-sensing review catalogued 07-01 §2.1 frames its hardware lineage. **Verification:** confirmed via prior-scan cross-reference + index.

### 2.4 — Photoacoustic Vector Tomography for Deep Hemodynamic Imaging *(previously surfaced — catalogued in prior scans)*
- **Year / Venue:** 2022–2024 · arXiv 2209.08706 / PMC11136879
- **Link:** https://arxiv.org/abs/2209.08706 · https://pmc.ncbi.nlm.nih.gov/articles/PMC11136879/
- **Relevance:** **7 / 10** — quantifies flow in **deep veins** at >5 mm (5× the optical diffusion limit); flow is the second half of the venous-metabolic equation (MRO₂ needs flow + tHb + sO₂ of input/output vessels).
- **Novelty:** Vector-mapped deep venous blood flow in humans by PA, extending PA beyond static sO₂ toward metabolic-rate imaging.
- **Integration insights:** Pairs with sO₂ imaging (§2.1) to enable non-invasive venous oxygen-consumption estimates — the clinically decisive quantity. **Verification:** confirmed via arXiv + PMC index.

### 2.5 — Deep-Learning-Driven Quantitative Spectroscopic Photoacoustic Imaging (Hybrid-Net) for Segmentation + sO₂ Estimation *(previously surfaced — scan 07-01 Topic-2 standing list)*
- **Authors:** R. Shang et al.
- **Year / Venue:** 2025 (Dec) · arXiv 2512.15394
- **Link:** https://arxiv.org/abs/2512.15394
- **Relevance:** **6 / 10** — Hybrid-Net jointly segments vessels and estimates sO₂ from dual-wavelength (700/850 nm) spectroscopic-PA in breast-tissue models; method transferable to venous vessels, but not venous-specific.
- **Novelty:** Joint segmentation + quantitative sO₂ recovery, trained on simulated light transport then retrained on phantoms — attacking the fluence-correction problem that limits qPACT accuracy.
- **Integration insights:** The DL-inverse machinery that a clinical deep-vein PA-SvO₂ system would need for fluence/spectral-coloring correction; the most recent (Dec-2025) qPACT advance, still awaiting venous/in-vivo application. **Verification:** authors/title/date/id confirmed via arXiv + ADS index; arXiv direct fetch 403 today (flagged).

**Previously surfaced — other standing optical-imaging references (NOT re-entered):** qPACT review (*J. Innov. Opt. Health Sci.* 2026, `10.1142/S1793545826300065`); distribution-informed wavelength-flexible PA oximetry (arXiv 2403.14863); sulfate/copper-nickel blood-phantom PA calibration (arXiv 2512.01458, 2503.23161); PINN spectral unmixing; virtual-imaging DL-3D-qPACT (arXiv 2510.03431); ML multiple-illumination optoacoustic oximetry in humans (PMC9203099); PA-TEE continuous mixed-venous SvO₂ (06-29 §2.1); transfontanelle/awake-mouse cerebral PA oxygenation; hyperspectral high-resolution retinal imaging system (PMC12997856, 2026); Oxymap retinal oximetry in CRVO / carotid stenosis / diabetic retinopathy; long-term post-COVID retinal oximetry + OCT-A (06-30 §2.3); *Graefe's Arch.* retinal-oximetry review (`10.1007/s00417-025-06831-8`); DNN+3-D-MC IJV sO₂ (*Opt. Lett.* 49:2669, also Topic 1 §1.2); single-vessel transmissive HSI blood-oxygen mapping; DL-enabled **SFDI** of skin-physiology dynamics (PMC12014942); wearable FD-NIRS system; single-distance phase-only FD-NIRS Monte-Carlo study.

---

## Cross-Topic Synthesis (2026-07-03)

1. **Fifteen scans in, the corpus remains converged.** A two-day-cadence search on 2026-07-03 surfaced **zero brand-new post-07-01 venous-specific primary papers** and exactly **one not-yet-catalogued artifact — a clinical-trial registration** (NCT06632197, capnodynamic adult SvO₂). This is not a search failure; it is the honest signal that the *currently-indexed* real corpus for non-invasive optical venous oximetry is **already captured** across the fourteen prior files. The anti-padding mandate held: nothing arterial-only was smuggled in.

2. **The unchanged scientific map.** Absolute reference = **MRI** (CMR-T₂ iSvO₂, susceptometry). Vessel-specific optical proving ground = the **retina** (vis-OCT ≈ 1 % bias, hyperspectral, Oxymap). Flagship deep-vein optical target = the **internal jugular vein** (IJV-PA ≈ 72 ± 7 %, jugular NIRS/DNN). Practical peripheral surrogates = the **venous-occlusion test** and **venous-pulsatility PPG** (Hill 2024, Tan e-tattoo). Non-optical benchmarks the optical program must beat = **capnodynamic Capno-SvO₂** and the **IDO₂** index. Unfilled prize = **truly non-invasive human deep-vein optical SvO₂ at clinical scale.**

3. **The two topics are one problem viewed at two depths.** Topic 1's best result (superficial jugular optical sensing, Hill 2024) and Topic 2's flagship (deep IJV photoacoustics) bracket the same named vein from the cheap-shallow and expensive-deep ends; the retina supplies the accuracy ceiling (~1 % bias) both aspire to, and PA vector tomography + qPACT DL-unmixing supply the flow and fluence-correction pieces needed to turn venous sO₂ into venous oxygen *consumption*.

4. **What to watch next (carried forward).** The most likely sources of a genuinely-new venous-specific result remain: (i) a **clinical-cohort** paper from the IJV-PA or flexible-optoacoustic-"stethoscope" groups; (ii) **CMR-referenced** validation of an optical venous method (NCT05161884); (iii) results from the standing **jugular-NIRS / capnodynamic SvO₂ trials** (NCT06511999, NCT04624009, NCT04778150, NCT04885699, and the newly-logged **NCT06632197**); and (iv) a peer-reviewed **wrist/neck e-tattoo** venous-validation cohort superseding the 2023 conference paper + 2025 patent. None had newly posted results as of 2026-07-03.

---

*Scan generated 2026-07-03 (UTC). Fifteenth scan in the series. Honest-sparseness policy applied: no new post-07-01 primary paper surfaced; the mandated Top-5-per-topic rankings re-list the best-available already-catalogued landmark corpus with explicit "previously surfaced" flags and honest relevance scores; the only genuinely new artifact (trial NCT06632197) is logged as a standing lead. No arterial-only padding was added. All publisher full-text, arXiv, and ClinicalTrials.gov direct fetches returned HTTP 403 in this environment; every reference was cross-checked across ≥2 independent index sources, with per-item verification notes stating what could not be read on the source page.*
