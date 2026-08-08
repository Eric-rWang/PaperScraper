# Venous Oxygen Research Scan — 2026-08-08

**Search window:** Thirty-second scan in the series, run **three days** after 2026-08-05 (no scans on 08-06 / 08-07). Emphasis on work published or first-surfacing after 08-05, with the standard fallback to the best-available venous-specific work already catalogued. Sources swept today: PubMed/PMC, arXiv (incl. physics.med-ph new-listing sweep), bioRxiv/medRxiv, Optica (Biomed. Opt. Express, Optics Letters, Applied Optics), SPIE / *J. Biomed. Opt.*, *Photoacoustics* (ScienceDirect), Springer (Graefe's Archive), Wiley (*Advanced Science*, *J. Biophotonics*), De Gruyter, Thieme (*J. Reconstr. Microsurg.* family), MDPI (*Biosensors/Sensors*), Frontiers (*Photonics*), Nature / *Sci. Rep.* / *Commun. Med.*, IEEE Xplore, JMIR, ClinicalTrials.gov, USPTO, ResearchGate, Semantic Scholar.

**Verification caveat:** As in every prior scan, publisher **full-text** pages — including link.springer.com, pmc.ncbi.nlm.nih.gov, pubmed.ncbi.nlm.nih.gov, opg.optica.org, sciencedirect.com, and the Nature/Wiley/Thieme domains — returned **HTTP 403 / egress-blocked** to direct `WebFetch` in this environment today (the agent proxy itself reported healthy; the blocks are source-side anti-bot / egress-policy restrictions). Every reference below was therefore cross-checked across **at least two independent search-index snippets** (Google Scholar–style result blocks + PubMed / PMC / Springer / Optica / De Gruyter / Thieme / USPTO listings); per-item notes state what was confirmed and what could not be read directly on a publisher page.

---

## ⚠️ Read this first — day summary

**No new venous-specific *primary* measurement paper today — the eleventh consecutive scan cycle with none.** Consistent with the series' standing observation, truly novel non-invasive **venous**-optical measurement work publishes at very low volume, and today's three-day sweep produced **no new SvO₂/ScvO₂ demonstration**. The Topic-1 (true SvO₂) top-5 and the Topic-2 measurement anchors are unchanged and carried forward with scores held.

Today surfaced **one genuinely new-to-corpus item**:

- **★ NEW entry (Topic 2) — "Next-Generation Flap Monitoring: Systematic Review and Meta-Analysis of Hyperspectral Imaging."** Atmodiwirjo P, Rininta C. Published **2026-01-30** via **Thieme** (*Journal of Reconstructive Microsurgery* family; open-access); **DOI 10.1055/a-2660-4344**; PMC12858309. A quantitative synthesis (nine studies, six focused on flap complications) of **hyperspectral imaging (HSI) tissue oximetry** for detecting compromised free flaps. Reports median sensitivity **93 %** (63–100 %) and specificity **96 %** (81–100 %) for compromised-flap detection, with four HSI parameters — **oxygen saturation (StO₂)**, tissue haemoglobin index (THI), tissue water index, and near-infrared perfusion index (NIR-PI) — differing significantly between viable and necrotic tissue, and HSI flagging perfusion deficits **up to 4.8 h before clinical signs**. This is a **tissue-level StO₂** review, **not** a true intravascular SvO₂ measurement — flagged accordingly — but it is genuinely venous-relevant, because the dominant failure mode it detects (flap congestion) is a **venous-outflow** problem, and skin/flap StO₂ is heavily venous-weighted (≈70–75 % of cutaneous blood volume is venous). It is the first HSI **flap-oximetry evidence-synthesis** to enter the corpus and quantifies HSI's real-world venous-congestion sensitivity. *Title / authors (Atmodiwirjo, Rininta) / venue (Thieme) / DOI / PMC ID / publication date and the four headline statistics all cross-confirmed across the PMC listing + a Thieme/search-index snippet; publisher full text and PMC could not be read directly (egress block) — abstract-/snippet-level content only, flagged as such.*

Everything else returned today is **previously surfaced** or out-of-scope, including: the jugular optical SvO₂ sensor (Alqahtani et al., De Gruyter CDBME-2024-2072), the IJV DNN + Monte-Carlo work (*Optics Letters* 49(10):2669), the 2017 peripheral-venous pulse-modulation proof-of-concept (*BioMed. Eng. OnLine* 16:60), the UT-Austin arterial+venous optical **e-tattoo** (PMID 38083768; IEEE 10340010; patent US 20250025074), APM+ radial-vein PA oximetry (Sastry/Olick-Gibson et al., *Adv. Sci.* 2026, 10.1002/advs.76366), the IJV-PA anchor, photoacoustic **vector tomography** for >5 mm-deep vein haemodynamics (*Nat. Biomed. Eng.* 2023, s41551-023-01148-5), the BOE PAT deep-tissue (30 mm) thrombosis/inner-chromophore-correction paper, the retinal-oximetry review ("Retinal oximetry: new insights…," *Graefe's Archive* 2025, 10.1007/s00417-025-06831-8 — first surfaced 08-05), the ADS-vis-OCT retinal oximetry paper (*Commun. Med.* 2023, s43856-023-00288-8), PACT intravascular oxygenation/flow (BOE 15(5):2741), the vis-OCT parafoveal-vessel baseline study (PMC9133487), Hybrid-Net spectroscopic-PA DL (arXiv:2512.15394), the sulfate blood-phantom PA metrology paper (arXiv:2512.01458), Mespere VO100 jugular NIRS, the cerebral-oximetry-as-SvO₂-surrogate NIRS work (Nature *Sci. Rep.* s41598-023-49078-1), the McDiarmid/MRI iSvO₂ line, and the SFDI tissue-oximetry family (SFDI-net). **No new primary venous demonstration.**

**Honest sparseness statement, per the standing brief:** **fewer than 5 genuinely strong, genuinely venous, genuinely non-invasive-optical papers first-surfaced today for either topic** once arterial-only and tissue-level (StO₂) work is excluded. The lists below present the best available with honest relevance scores; several entries are explicitly flagged as tissue-/retinal-level, MRI-based, or metrology rather than true systemic SvO₂ optical measurement, and are retained only because the true-venous population is that thin.

---

## Topic 1 — Non-invasive monitoring of venous blood oxygen (SvO₂ / ScvO₂ / peripheral venous)

*No new primary items today.* The standing best-available set (all previously surfaced) with scores carried forward. This remains the sparse topic: **no primary non-invasive venous-O₂ measurement paper has first-surfaced since before 2026-07-15.**

### 1.1 — Estimation of Venous Oxygen Saturation Through Non-Invasive Optical Sensing at the Jugular Veins *(previously surfaced — scan 06-10 §1.1; flagship optical-venous device paper)*
- **Authors:** Alqahtani et al.
- **Year / Venue:** 2024 · *Current Directions in Biomedical Engineering* 10(2) (De Gruyter; CDBME-2024-2072)
- **Link / DOI:** https://doi.org/10.1515/cdbme-2024-2072
- **Relevance:** 9.0/10 — direct non-invasive optical SvO₂ at the external/internal jugular; the closest thing the corpus has to a pulse-oximeter-form venous device.
- **Novelty:** Proof-of-concept optical sensor that identifies the jugular venous waveform and estimates SvO₂ within the healthy 60–90 % band across a small (n≈3) subject set.
- **Integration insight:** The anchor for the "wearable venous pulse oximeter" thesis; every Topic-1 wearable/peripheral entry is a variation on isolating the venous component this device targets at the neck. Still awaiting calibration/validation against blood-gas gold standard.

### 1.2 — Quantifying Changes in Oxygen Saturation of the Internal Jugular Vein In Vivo Using Deep Neural Networks and Subject-Specific 3-D Monte-Carlo Models *(previously surfaced — scan 06-10 §1.2)*
- **Authors:** (IJV DNN / Monte-Carlo group)
- **Year / Venue:** 2024 · *Optics Letters* 49(10):2669
- **Link / DOI:** https://opg.optica.org/ol/abstract.cfm?uri=ol-49-10-2669 (Optica abstract locator; raw DOI numeral unverified — see flag below)
- **Relevance:** 8.5/10 — model-based recovery of IJV sO₂ change from multi-channel NIRS reflectance.
- **Novelty:** Subject-specific 3-D Monte-Carlo forward models train a DNN to invert measured reflectance into IJV saturation change, addressing the partial-volume/overlying-tissue confound.
- **Integration insight:** Supplies the computational-inversion half of the jugular-NIRS approach; complements §1.1's hardware. The Monte-Carlo-to-DNN pattern recurs in the Topic-2 PA fluence-correction work.

> **Metadata flag:** §1.2 DOI string could not be re-verified on the Optica page today (egress block); the stable Optica abstract locator (ol-49-10-2669) and title/authors/year are cross-confirmed via two search-index snippets. Treat the raw DOI numeral as **unverified**; cite via the Optica abstract URL.

### 1.3 — Proof-of-Concept Non-Invasive Estimation of Peripheral Venous Oxygen Saturation (pulse-modulation venous oximetry) *(previously surfaced — scan 06-10/06-11; peripheral-venous proof-of-concept)*
- **Authors:** (peripheral-venous oximetry group; *BioMedical Engineering OnLine*)
- **Year / Venue:** 2017 · *BioMedical Engineering OnLine* 16:60
- **Link / DOI:** https://doi.org/10.1186/s12938-017-0351-x
- **Relevance:** 8.0/10 — a foundational demonstration that an induced/modulated venous signal yields a peripheral SvO₂ estimate optically.
- **Novelty:** Exploits the arterial/venous compliance difference to induce respiration-like modulation that makes venous blood pulsatile, lifting the venous component out of the low-SNR background so a PPG-style optical readout can estimate local venous saturation.
- **Integration insight:** The conceptual root of the "modulate the vein, then demodulate" family (muscle-stimulation PPG, e-tattoo spatial filtering). Landmark; recurs because nothing newer has displaced it as the peripheral-venous proof-of-concept.

### 1.4 — Towards Simultaneous Non-Invasive Arterial and Venous Oxygenation Monitoring with a Wearable Optical E-Tattoo *(previously surfaced — scan 07-01 §1.5-family)*
- **Authors:** Tan P., Lu N., et al. (UT Austin)
- **Year / Venue:** 2023/2024 · IEEE EMBC (10340010); PMID 38083768; related patent US 20250025074
- **Link / DOI:** https://pubmed.ncbi.nlm.nih.gov/38083768/ · patent: https://patents.justia.com/patent/20250025074
- **Relevance:** 8.0/10 — soft wrist e-tattoo measuring arterial and venous pulses simultaneously; directly targets the SvO₂ unmet need.
- **Novelty:** Characterises the arterial/venous **crosstalk** that defeats co-located SaO₂/SvO₂ extraction (simulation, in vitro, in vivo) and proposes **spatial filtering** to separate the two; explicitly motivates venous readout for sepsis/shock detection.
- **Integration insight:** The wearable-form-factor endpoint of the Topic-1 thesis; the crosstalk-suppression problem it frames is the central signal-processing obstacle every peripheral venous oximeter must solve.

### 1.5 — Non-invasive Tracking of Mixed Venous Oxygen Saturation via NIRS Cerebral Oximetry *(previously surfaced; retained as best-available surrogate)*
- **Authors:** (retrospective observational study group)
- **Year / Venue:** 2023 · *Scientific Reports* (s41598-023-49078-1)
- **Link / DOI:** https://www.nature.com/articles/s41598-023-49078-1
- **Relevance:** 6.5/10 — tracks trends in mixed SvO₂ via cerebral rScO₂, i.e. a **surrogate**, not a direct venous measurement.
- **Novelty:** Shows NIRS cerebral oximetry correlates with and can trend SvO₂ across an intraoperative cohort — useful for the "trend, not absolute" clinical framing.
- **Integration insight:** Marks the realistic near-term clinical bar (trend correlation) that a true non-invasive venous device must beat with absolute, catheter-comparable SvO₂.

> **Topic-1 honesty note:** Only §§1.1–1.4 are genuinely *venous-specific optical* work; §1.5 is a tissue/surrogate line included because the true-venous field is thin. No item below §1.4 should be read as a validated absolute-SvO₂ device.

---

## Topic 2 — Optical imaging techniques for non-invasively obtaining venous blood oxygen (PA/PACT, NIRS, DOI/DOT, hyperspectral, OCT, SFDI)

**One new entry today (§2.1, HSI flap-oximetry evidence synthesis, tissue-level).** Measurement anchors carried forward with scores held.

### 2.1 — ★ NEW · Next-Generation Flap Monitoring: Systematic Review and Meta-Analysis of Hyperspectral Imaging *(new to corpus 2026-08-08)*
- **Authors:** Atmodiwirjo P., Rininta C.
- **Year / Venue:** 2026 (published 2026-01-30) · Thieme (*Journal of Reconstructive Microsurgery* family; open access); PMC12858309
- **Link / DOI:** https://doi.org/10.1055/a-2660-4344
- **Relevance:** 6.5/10 — **tissue-level HSI StO₂**, not intravascular SvO₂; scored for strong *venous-congestion* relevance, not true venous oximetry.
- **Novelty:** First quantitative **meta-analysis** (9 studies; 6 on flap complications) of HSI tissue-oximetry for compromised-flap detection: median sensitivity **93 %**, specificity **96 %**; four HSI parameters (StO₂, THI, tissue-water index, NIR-PI) separate viable from necrotic tissue; perfusion deficits detected **up to 4.8 h before clinical signs**.
- **Integration insight:** Flap failure is predominantly a **venous-outflow (congestion)** event, and cutaneous StO₂ is venous-weighted, so this is the clearest evidence-synthesis to date that a **widefield optical oximeter reads out a clinically actionable venous-congestion signal** in humans — even though it reports mixed-tissue StO₂ rather than isolated SvO₂. It quantifies the sensitivity/lead-time bar a future *vessel-resolved* venous oximeter (e.g. HSI + PA, or the venous-occlusion-windowed SFDI protocol in the corpus) would need to match or beat. Bridges the Topic-2 hyperspectral and SFDI families toward a concrete venous clinical endpoint. *Flagged: tissue-level StO₂, publisher/PMC full text not directly readable today (egress block) — metadata + headline stats cross-confirmed via PMC listing + Thieme/index snippet.*

### 2.2 — Photoacoustic Vector Tomography for Deep Haemodynamic Imaging *(previously surfaced; deepest true-venous PA anchor)*
- **Authors:** (PAVT group)
- **Year / Venue:** 2023 · *Nature Biomedical Engineering* (s41551-023-01148-5); PMID 38036619
- **Link / DOI:** https://www.nature.com/articles/s41551-023-01148-5
- **Relevance:** 8.5/10 — quantifies haemodynamics in **veins >5 mm deep** in human hands/arms — genuine deep-venous optical access.
- **Novelty:** Vector (flow-resolved) photoacoustic tomography reaches deep veins that OR-PAM/superficial PA cannot, opening depth regimes relevant to true peripheral venous imaging.
- **Integration insight:** The depth-reach anchor for Topic 2; combined with spectral (sO₂) PA and fluence correction it is the most credible route to depth-resolved venous oximetry beyond the skin surface.

### 2.3 — Arterial Blood-Mediated Deep-Tissue Photoacoustic Oximetry (APM+, incl. radial-vein readout) *(previously surfaced — scan family)*
- **Authors:** Sastry, Olick-Gibson, et al.
- **Year / Venue:** 2026 · *Advanced Science* (Wiley); DOI 10.1002/advs.76366
- **Link / DOI:** https://advanced.onlinelibrary.wiley.com/doi/10.1002/advs.76366
- **Relevance:** 8.0/10 — deep-tissue PA oximetry with an explicit **radial-vein** demonstration; among the most recent true-vessel PA sO₂ work in the corpus.
- **Novelty:** Uses an arterial-blood-mediated correction (APM+) to counter spectral coloring and recover accurate deep-vessel sO₂, demonstrated on named peripheral vessels including a vein.
- **Integration insight:** Pairs with §2.2 (depth) and the fluence-correction/DL line to move PA toward calibrated absolute venous sO₂; one of the two or three papers that make "PA venous oximeter" more than aspirational.

### 2.4 — Adaptive Spectroscopic Visible-Light OCT for Clinical Retinal Oximetry (ADS-vis-OCT) *(previously surfaced; retinal-vein true-intravascular anchor)*
- **Authors:** (Northwestern vis-OCT group)
- **Year / Venue:** 2023 · *Communications Medicine* (s43856-023-00288-8); PMID 37095177; PMC10126115
- **Link / DOI:** https://www.nature.com/articles/s43856-023-00288-8
- **Relevance:** 8.0/10 — measures **retinal venular sO₂** intravascularly and non-invasively; retinal veins are one of the few sites where true venous sO₂ is read optically in humans.
- **Novelty:** Adaptive spectral-contaminant removal yields per-vessel sO₂ with RMSE ≈2.1 % vs pulse oximeter in arteries and repeatability ≈2.3 % in veins.
- **Integration insight:** The gold-standard-adjacent demonstration that vessel-resolved optical **venous** oximetry is achievable in vivo; sets the accuracy bar (~2–2.5 %) the PA and HSI lines are chasing. Complemented by the 2025 *Graefe's Archive* retinal-oximetry review (first surfaced 08-05) as the review-level scaffold.

### 2.5 — Deep Learning-Driven Quantitative Spectroscopic Photoacoustic Imaging for Segmentation and sO₂ Estimation (Hybrid-Net) *(previously surfaced — arXiv new-listing)*
- **Authors:** (Hybrid-Net group)
- **Year / Venue:** 2025 (posted 2025-12-17) · arXiv:2512.15394 [physics.med-ph] *(preprint — not peer-reviewed)*
- **Link / DOI:** https://arxiv.org/abs/2512.15394
- **Relevance:** 7.0/10 — vessel-agnostic sO₂ (applies to veins and arteries) with **fluence-free** estimation; technique directly transferable to venous targets.
- **Novelty:** A single network jointly **segments vessels** and estimates sO₂ **without** explicit optical-fluence modelling; reports segmentation ≥0.978 (sim)/0.998 (exp) and sO₂ MSE ≤0.048 (sim)/0.003 (exp).
- **Integration insight:** The fluence-free inversion is exactly what deep-venous PA (§§2.2–2.3) needs to escape spectral-coloring calibration; vessel segmentation could isolate the venous compartment automatically. Preprint status flagged — treat metrics as unreviewed.

> **Topic-2 honesty note:** Of the five, §§2.2–2.4 are genuine vessel-level optical work with a real venous component; §2.1 is **tissue-level StO₂** (venous-weighted, not intravascular) and §2.5 is an **unreviewed preprint**. No entry here is yet a validated, calibrated absolute-SvO₂ optical *device* — the field's central gap persists.

---

## Cross-topic synthesis

1. **The venous-optical field remains supply-limited, not attention-limited.** Eleven consecutive cycles with no new *primary* non-invasive venous-SvO₂ measurement paper is a signal about publication rate, not search coverage — today's three-day, ~20-source sweep again returned only re-surfaced anchors plus one adjacent evidence-synthesis. The honest read for a daily cadence is that meaningful movement should be expected on a **monthly-to-quarterly**, not daily, timescale.

2. **Today's one new item shifts the evidence from "can we?" toward "how well, and how early?"** The HSI flap meta-analysis (§2.1) does not measure SvO₂, but it quantifies — across nine studies — that a **widefield optical oximeter detects venous-congestion-driven tissue-O₂ deficits with 93 %/96 % sensitivity/specificity and ~4.8 h of lead time** over clinical exam. That converts the corpus's long-standing "venous congestion is the clinically dominant failure mode" assertion into a concrete performance bar, and it is a bar a *vessel-resolved* venous oximeter (retinal vis-OCT §2.4, deep PA §§2.2–2.3, or the venous-occlusion-windowed SFDI protocol) would have to justify itself against on lead-time and sensitivity, not just on measuring "true" SvO₂.

3. **The two topics keep converging on the same three-part recipe: depth + vessel isolation + fluence-free inversion.** Depth reach is anchored by PA vector tomography (§2.2) and deep-tissue APM+ (§2.3); vessel-isolated absolute accuracy is proven only in the retina by ADS-vis-OCT (§2.4) at ~2–2.5 %; and fluence-free DL inversion (§2.5) plus the jugular Monte-Carlo→DNN work (§1.2) supply the math to carry retinal-grade accuracy into deep, cluttered peripheral tissue. No single platform yet holds all three, which is precisely why the field is stuck at proof-of-concept for a wearable/deep venous device (§§1.1, 1.4).

4. **Clinical translation still runs through surrogates.** The realistic near-term bar (NIRS cerebral-oximetry SvO₂ *trending*, §1.5; HSI tissue-StO₂ congestion detection, §2.1) is trend/threshold utility, not absolute catheter-replacement. A device that delivers absolute, blood-gas-comparable SvO₂ non-invasively would leapfrog this entire surrogate tier — and remains unpublished as of today.

---

### Verification & provenance summary
- **New item (§2.1)** metadata (title, authors Atmodiwirjo & Rininta, Thieme venue, DOI 10.1055/a-2660-4344, PMC12858309, 2026-01-30 date, and the 93 %/96 %/4.8 h headline statistics) cross-confirmed across the PMC listing and a Thieme/search-index snippet; **publisher full text and PMC not directly readable today** (egress block) — content is abstract-/snippet-level, flagged in situ.
- **All Topic-1 and Topic-2 anchors** are previously surfaced and carried forward; DOIs/locators are the same ones verified in prior scans. The §1.2 Optica DOI numeral remains **unverified** (cite via abstract locator).
- **Environment note:** direct `WebFetch` to pmc.ncbi.nlm.nih.gov, link.springer.com, sciencedirect.com, opg.optica.org, nature.com, wiley, and Thieme returned **403 / egress-blocked** today, as in prior scans; verification relied on ≥2 independent index snippets per item.
