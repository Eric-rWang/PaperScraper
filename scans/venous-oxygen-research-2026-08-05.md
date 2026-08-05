# Venous Oxygen Research Scan — 2026-08-05

**Search window:** Thirty-first scan in the series, run **two days** after 2026-08-03 (no scan on 08-04). Emphasis on work published or first-surfacing after 08-03, with the standard fallback to the best-available venous-specific work already catalogued. Sources swept today: PubMed/PMC, arXiv (incl. physics.med-ph new-listing sweep), bioRxiv/medRxiv, Optica (Biomed. Opt. Express, Optics Letters, Applied Optics), SPIE / *J. Biomed. Opt.*, *Photoacoustics* (ScienceDirect), Springer (Graefe's Archive), Wiley (*Advanced Science*, *J. Biophotonics*), De Gruyter, MDPI (*Biosensors/Sensors*), Frontiers (*Photonics*), Nature / *Sci. Rep.* / *Commun. Med.*, IEEE Xplore, JMIR, ClinicalTrials.gov, USPTO, ResearchGate, Semantic Scholar.

**Verification caveat:** As in every prior scan, publisher **full-text** pages — including link.springer.com, pmc.ncbi.nlm.nih.gov, pubmed.ncbi.nlm.nih.gov, opg.optica.org, formative.jmir.org, sciencedirect.com and the Nature/Wiley domains — returned **HTTP 403** to direct `WebFetch` in this environment today (the agent proxy itself reported healthy with no relay failures; the 403s are source-side anti-bot blocks). Every reference below was therefore cross-checked across **at least two independent search-index snippets** (Google Scholar–style result blocks + PubMed / PMC / Springer / Optica / De Gruyter / USPTO listings); per-item notes state what was confirmed and what could not be read directly on a publisher page.

---

## ⚠️ Read this first — day summary

**No new venous-specific *primary* measurement paper today — the tenth consecutive scan cycle with none.** Consistent with the series' standing observation, truly novel non-invasive **venous**-optical measurement work publishes at very low volume, and today's two-day sweep produced **no new SvO₂/ScvO₂ demonstration**. The Topic-1 (true SvO₂) top-5 and the Topic-2 top-5 measurement anchors are unchanged and carried forward with scores held.

Today surfaced **one genuinely new-to-corpus item**, plus two tangential standing leads:

- **★ NEW entry (Topic 2) — "Retinal oximetry: new insights into ocular and systemic diseases," *Graefe's Archive for Clinical and Experimental Ophthalmology*, 2025.** Zhang W, Tu X, Wang X, et al.; vol. 263, pp. 2101–2115; DOI 10.1007/s00417-025-06831-8; PMID 40254630; PMC12414079. A dedicated review of retinal oximetry that treats **retinal venular sO₂ as a first-class quantity** (retinal veins are one of the very few sites where a truly *intravascular venous* oxygen saturation is read optically and non-invasively in humans), surveys the spectrophotometric-fundus, hyperspectral, and vis-OCT modalities, and catalogues the vessel-diameter / pigmentation / media-transparency error sources that any per-vessel venous oximeter must contend with. Not a new *device*, but the first review-level scaffold of retinal **venous** oximetry to enter the corpus. *Title / authors (Zhang, Tu, Wang et al.) / venue / volume+pages / DOI / PMID / PMC ID all cross-confirmed across Springer + PubMed + PMC + springermedicine.com index snippets; full text could not be read directly (publisher 403) — abstract-level content only, flagged as such.*

- **★ NEW lead (Topic 2, tangential) — "AI-driven multimodal retinal imaging for early detection and risk stratification of vascular and neurodegenerative diseases," *Graefe's Archive*, 2026** (DOI 10.1007/s00417-026-07273-6). A 2026 review of AI + multimodal retinal imaging for vascular risk stratification. Whether it treats per-vessel *venous* oximetry specifically could **not be verified** (publisher 403; no abstract snippet obtained). Logged as a watch-lead only, **relevance to venous sO₂ unconfirmed**.

- **★ NEW lead (Topic 1, transferable-relevance) — "Performance of Wearable Pulse Oximetry During Controlled Hypoxia Induction: Instrument Validation Study," *JMIR Formative Research*, 2026** (formative.jmir.org/2026/1/e85253). An **arterial-only** SpO₂ validation of consumer wearables (Apple Watch Series 7, Masimo MightySat Rx) under controlled hypoxia, reporting errors exceeding FDA thresholds in the hypoxemic range. Included **only** as a transferable methodological caution: the wearable-optical venous ambition (e-tattoo §1.5, peripheral-venous §1.5-family) inherits and *amplifies* exactly this hypoxic-range accuracy problem, since venous saturations sit lower than arterial. Not a venous paper → standing lead, honest low venous score.

Everything else returned today is **previously surfaced** or out-of-scope: the IJV jugular optical sensor (Alqahtani, De Gruyter CDBME-2024-2072), the IJV DNN + Monte-Carlo work (*Optics Letters* 49(10):2669), the peripheral-venous pulse-modulation proof-of-concept, the UT-Austin arterial+venous optical **e-tattoo** (PMID 38083768 / patent US 20250025074), APM+ radial-vein PA oximetry (Sastry/Olick-Gibson et al., *Adv. Sci.* 2026, 10.1002/advs.76366), the IJV-PA anchor (Noninvasive In Vivo PA of internal jugular venous oxygenation), the hyperspectral retinal HSI system, the ADS-vis-OCT retinal oximetry paper (*Commun. Med.* 2023), PACT intravascular oxygenation/flow (BOE 15(5):2741), the sulfate blood-phantom metrology paper (arXiv:2512.01458), Hybrid-Net (arXiv:2512.15394), Mespere VO100 jugular NIRS, the McDiarmid MRI iSvO₂ model, the SSL intra-cardiac MR oximetry preprint, the classic ovine/large-vein optoacoustic SSS venous work (Esenaliev/Petrov lineage), and the Karlas MSOT arterial/venous-occlusion muscle pilot. **No new primary venous demonstration.**

Honest sparseness statement, per the standing brief: **fewer than 5 genuinely strong, genuinely venous, genuinely non-invasive-optical papers first-surfaced today for either topic** once arterial-only and tissue-level (StO₂) work is excluded. The lists below present the best available with honest relevance scores; several entries are explicitly flagged as tissue-/retinal-level, MRI-based, or metrology rather than true systemic SvO₂ optical measurement, and are retained only because the true-venous population is that thin.

---

## Topic 1 — Non-invasive monitoring of venous blood oxygen (SvO₂ / ScvO₂ / peripheral venous)

*No new primary items today.* The standing best-available set (all previously surfaced) with scores carried forward. This remains the sparse topic: **no primary non-invasive venous-O₂ measurement paper has first-surfaced since before 2026-07-15.**

### 1.1 — Estimation of Venous Oxygen Saturation Through Non-Invasive Optical Sensing at the Jugular Veins *(previously surfaced — scan 06-10 §1.1; flagship optical-venous device paper)*
- **Authors:** Alqahtani et al.
- **Year / Venue:** 2024 · *Current Directions in Biomedical Engineering* 10(2) (De Gruyter; CDBME-2024-2072)
- **Link / DOI:** https://doi.org/10.1515/cdbme-2024-2072
- **Relevance:** 9.0/10 — direct non-invasive optical SvO₂ at the external/internal jugular; the closest thing the corpus has to a pulse-oximeter-form venous device.
- **Novelty:** Proof-of-concept optical sensor that identifies the jugular venous waveform and estimates SvO₂ within the healthy 60–90% band across a small subject set.
- **Integration insight:** The anchor for the "wearable venous pulse oximeter" thesis; every Topic-1 wearable/peripheral entry is a variation on isolating the venous component this device targets at the neck.

### 1.2 — Quantifying Changes in Oxygen Saturation of the Internal Jugular Vein In Vivo Using Deep Neural Networks and Subject-Specific 3-D Monte-Carlo Models *(previously surfaced — scan 06-10 §1.2)*
- **Authors:** (IJV DNN / Monte-Carlo group)
- **Year / Venue:** 2024 · *Optics Letters* 49(10):2669
- **Link / DOI:** https://opg.optica.org/ol/abstract.cfm?uri=ol-49-10-2669 (Optica abstract locator; raw DOI numeral unverified — see metadata flag below)
- **Relevance:** 8.5/10 — model-based recovery of IJV sO₂ change from multi-channel NIRS reflectance.
- **Novelty:** Subject-specific 3-D Monte-Carlo forward models train a DNN to invert measured reflectance into IJV saturation change, addressing the partial-volume/overlying-tissue confound.
- **Integration insight:** Supplies the computational-inversion half of the jugular-NIRS approach; complements §1.1's hardware. The Monte-Carlo-to-DNN pattern recurs in the Topic-2 PA fluence-correction work.

> **Metadata flag:** §1.2 DOI string could not be re-verified on the Optica page today (403); the stable Optica abstract locator (ol-49-10-2669) and title/authors/year are cross-confirmed via two search-index snippets. Treat the raw DOI numeral as **unverified**; cite via the Optica abstract URL.

### 1.3 — Non-Invasive Estimation of Peripheral Venous Oxygen Saturation (pulse-modulation venous oximetry) *(previously surfaced — scan 06-10/06-11; peripheral-venous proof-of-concept)*
- **Authors:** (peripheral-venous oximetry group; BioMedical Engineering OnLine)
- **Year / Venue:** 2017 · *BioMedical Engineering OnLine* 16:60
- **Link / DOI:** https://doi.org/10.1186/s12938-017-0351-x
- **Relevance:** 8.0/10 — a foundational demonstration that an induced/modulated venous signal yields a peripheral SvO₂ estimate optically.
- **Novelty:** Uses external stimulation to induce cyclical venous fluctuation, lifting the venous component out of the low-SNR background so a PPG-style optical readout can estimate local venous saturation.
- **Integration insight:** The conceptual root of the "modulate the vein, then demodulate" family (muscle-stimulation PPG, e-tattoo spatial filtering). Landmark; recurs because nothing newer has displaced it as the peripheral-venous proof-of-concept.

### 1.4 — Towards Simultaneous Non-Invasive Arterial and Venous Oxygenation Monitoring with a Wearable Optical E-Tattoo *(previously surfaced — scan 07-01 §1.5-family)*
- **Authors:** Tan P., Lu N., et al. (UT Austin)
- **Year / Venue:** 2023/2024 · IEEE (EMBC-lineage); related patent US 20250025074
- **Link / DOI:** https://pubmed.ncbi.nlm.nih.gov/38083768/ · patent: https://patents.justia.com/patent/20250025074
- **Relevance:** 8.0/10 — explicitly names non-invasive **venous** oxygenation as the unmet need and targets it with a wrist-worn optical patch.
- **Novelty:** Ultra-thin self-adherent optical e-tattoo measures arterial + venous pulses from multiple wrist sites; proposes spatial filtering to separate arterial/venous crosstalk.
- **Integration insight:** The wearable-form embodiment of the venous-oximetry goal; its arterial/venous separation problem is the same one §1.3 attacks by modulation and §1.1 sidesteps by anatomy (large jugular target). Today's JMIR hypoxia-accuracy caution (standing lead) bears directly on this device class.

### 1.5 — A New Non-Invasive Method for the Assessment of Central Venous Oxygen Saturation (Mespere VO100 jugular NIRS) *(previously surfaced — scan 06-14; commercial NIRS device)*
- **Authors:** (VO100 clinical validation group)
- **Year / Venue:** 2023/2024 · *J. Cardiothorac. Vasc. Anesth.* (S1053-0770 lineage) / ScienceDirect
- **Link / DOI:** https://www.sciencedirect.com/science/article/pii/S1053077023007826
- **Relevance:** 7.5/10 — the one commercially available non-invasive jugular-NIRS ScvO₂ estimator; clinically evaluated in critically ill patients.
- **Novelty:** Continuous non-invasive ScvO₂ estimate from an external jugular NIRS sensor (Mespere VO100), positioned as an alternative when catheter-based sampling is difficult.
- **Integration insight:** The clinical-translation benchmark for Topic 1 — the accuracy/bias any research-grade optical venous device (§1.1–1.4) must beat to matter at the bedside.

**Topic 1 honest note:** every entry above is previously surfaced; nos. 1.3 and 1.5 predate 2023. The absence of *new* primary venous measurement work today is itself the finding, not a gap in searching.

---

## Topic 2 — Optical imaging techniques for non-invasively obtaining venous blood oxygen (PA/PACT, NIRS, DOI/DOT, hyperspectral, vis-OCT, SFDI)

*One genuinely new entry today (§2.1), plus the carried-forward measurement anchors.*

### 2.1 — ★ NEW — Retinal Oximetry: New Insights into Ocular and Systemic Diseases *(new to corpus; review of per-vessel retinal artery+vein sO₂)*
- **Authors:** Zhang W., Tu X., Wang X., et al.
- **Year / Venue:** 2025 · *Graefe's Archive for Clinical and Experimental Ophthalmology* 263:2101–2115
- **Link / DOI:** https://doi.org/10.1007/s00417-025-06831-8 · PMID 40254630 · PMC12414079
- **Relevance:** 7.5/10 — retinal veins are among the very few human sites where a true **intravascular venous sO₂** is read optically and non-invasively; this is the first dedicated review of that measurement to enter the corpus. (Not systemic SvO₂; retinal venular, per-vessel.)
- **Novelty:** Consolidates the state of retinal oximetry across spectrophotometric-fundus, hyperspectral, and vis-OCT modalities; frames retinal artery *and vein* saturation as biomarkers of ocular + systemic microcirculation (diabetic retinopathy, glaucoma, cardiovascular, renal); explicitly enumerates the vessel-diameter, retinal-pigmentation, and optical-media-transparency error sources, and flags wide-field, non-mydriatic, blood-flow-fusion, and AI directions as the accuracy frontier.
- **Integration insight:** Ties the Topic-2 retinal cluster (hyperspectral HSI system; ADS-vis-OCT §2.4) into one framework and names, at review level, the exact per-vessel confounds a venular oximeter must correct — the retinal analogue of the fluence/spectral-coloring problem the deep-vein PA anchors face. Its "integrate oximetry with blood-flow measurement + AI" thesis is the retinal mirror of the PACT flow-pattern work (§2.5).
- **Metadata flag:** All bibliographic fields cross-confirmed (Springer + PubMed + PMC + springermedicine index); **full text not read** (publisher 403) — summary is abstract/snippet-level.

### 2.2 — Noninvasive In Vivo Photoacoustic Measurement of Internal Jugular Venous Oxygenation in Humans *(previously surfaced — scan 06-10 §2.1; the Topic-2 anchor)*
- **Authors:** (IJV-PA human oximetry group)
- **Year / Venue:** 2023 · arXiv:2303.10775 / PA human-imaging lineage
- **Link / DOI:** https://arxiv.org/abs/2303.10775
- **Relevance:** 9.5/10 — the single most on-target Topic-2 paper: photoacoustic sO₂ of a named deep **vein** (internal jugular) in humans, non-invasively.
- **Novelty:** Demonstrates human IJV oxygenation from multi-wavelength PA, pushing PA oximetry from superficial microvessels to a clinically meaningful deep venous target.
- **Integration insight:** The proof that optical/PA venous oximetry can reach a central-venous surrogate; the bridge between Topic 1's clinical need and Topic 2's imaging physics.

### 2.3 — Arterial Blood-Mediated Deep-Tissue Photoacoustic Oximetry (APM+): in-vivo human radial-vein sO₂ *(previously surfaced — upgraded 07-15 §2.2)*
- **Authors:** Sastry, Olick-Gibson, et al.
- **Year / Venue:** 2026 · *Advanced Science* (Wiley)
- **Link / DOI:** https://doi.org/10.1002/advs.76366
- **Relevance:** 9.0/10 — in-vivo human **radial-vein** sO₂ via a deep-tissue PA method that explicitly tackles spectral coloring.
- **Novelty:** Uses arterial-blood-mediated calibration to correct wavelength-dependent fluence, recovering deep-tissue venous sO₂ where conventional linear unmixing fails.
- **Integration insight:** The most recent (2026) primary PA venous-oximetry advance in the corpus; its fluence-correction strategy is the technique the new §2.1 review would classify under "learning/statistical decoloring," and the deep-vein counterpart to the retinal per-vessel corrections §2.1 catalogues.

### 2.4 — Adaptive Spectroscopic Visible-Light OCT for Clinical Retinal Oximetry (ADS-vis-OCT) *(previously surfaced — scan 06-11 §2.2)*
- **Authors:** (ADS-vis-OCT group)
- **Year / Venue:** 2023 · *Communications Medicine* 3:59
- **Link / DOI:** https://doi.org/10.1038/s43856-023-00288-8
- **Relevance:** 8.5/10 — per-vessel retinal **vein** sO₂ with reported repeatability SD ≈ 2.3% in veins.
- **Novelty:** Adaptively removes per-vessel spectral contaminants, yielding accurate, repeatable artery *and vein* sO₂ across varying vessel diameters in humans.
- **Integration insight:** The highest-precision per-vessel venous optical readout in the corpus; the concrete modality the new §2.1 review holds up as state-of-the-art for retinal venular oximetry.

### 2.5 — Oxygenation Heterogeneity Facilitates Spatiotemporal Flow-Pattern Visualization Inside Human Blood Vessels Using PACT *(previously surfaced — scan 06-11 / 06-10)*
- **Authors:** (PACT intravascular flow/oxygenation group)
- **Year / Venue:** 2024 · *Biomedical Optics Express* 15(5):2741
- **Link / DOI:** https://doi.org/10.1364/BOE.518632 → https://opg.optica.org/boe/fulltext.cfm?uri=boe-15-5-2741
- **Relevance:** 8.0/10 — resolves sO₂ heterogeneity and laminar-flow structure *inside* human vessels (incl. veins) with PACT.
- **Novelty:** First-time recovery of the parabolic laminar-flow wavefront inside a deep vein in vivo by exploiting intravascular oxygenation heterogeneity across multi-wavelength PA spectra.
- **Integration insight:** Shows PACT can read *within-lumen* venous oxygen structure, not just a vessel-average — the imaging counterpart to §2.1's "fuse oximetry with blood-flow measurement" thesis, and the deep-vessel analogue to retinal flow+oximetry fusion.
- **Metadata flag:** §2.5 DOI numeral could not be re-verified on the Optica page today (403); the stable Optica locator (boe-15-5-2741) + title/year cross-confirmed. Cite via the Optica URL; treat the raw DOI numeral as **unverified**.

---

## Standing context leads (not ranked in the top-5)

- **★ NEW — "AI-driven multimodal retinal imaging for early detection and risk stratification of vascular and neurodegenerative diseases," *Graefe's Archive*, 2026** (DOI 10.1007/s00417-026-07273-6). 2026 review of AI + multimodal retinal imaging for vascular risk. **Venous-oximetry relevance unverified** (403; no abstract snippet). Watch-lead only.
- **★ NEW — "Performance of Wearable Pulse Oximetry During Controlled Hypoxia Induction: Instrument Validation Study," *JMIR Formative Research*, 2026** (formative.jmir.org/2026/1/e85253). **Arterial-only** wearable SpO₂ validation (Apple Watch S7, Masimo MightySat Rx) showing >FDA-threshold error in the hypoxemic range. Transferable caution for the wearable-venous device class (§1.4/§1.3), which operates at even lower saturations. Not a venous paper.
- **Quantitative oximetry with PACT: Principles, Progress, and Prospects** — *J. Innov. Opt. Health Sci.*, 2026 (DOI 10.1142/S1793545826300065). Review-level scaffold under the deep-vein PA anchors (§2.2/§2.3); authors unverified (prior scan). Carried forward.
- **Classic ovine / large-vein optoacoustic SSS venous work** (Esenaliev/Petrov lineage; superior sagittal sinus, triple-wavelength optoacoustic large-vein oximetry). Foundational venous-optoacoustic prior art; predates the series window, retained as the historical root of deep-venous PA oximetry.
- **Frontiers in Photonics editorial, "Diffusive optics for medical imaging," 2026** (DOI 10.3389/fphot.2026.1842429). Context marker for the DOT/SFDI/DCS branch of Topic 2; not venous-specific.
- **Karlas et al., MSOT of muscle perfusion/oxygenation under arterial and venous occlusion — human pilot** (*J. Biophotonics* 2020). Tissue-level (StO₂), not intravascular SvO₂, but the closest MSOT venous-challenge human data; retained as a tissue-level lead.

---

## Cross-topic synthesis

Today reinforces the series' central, honest finding: **non-invasive optical measurement of true venous blood oxygen is a low-volume field, and no new primary venous *measurement* appeared today** (tenth consecutive dry cycle). The two topics remain coupled by one problem — **isolating the venous signal and correcting the confound that corrupts its saturation estimate** — solved by three complementary strategies that the day's one new item helps organize:

1. **Anatomical targeting** of a large, named vein (jugular optical sensing §1.1, jugular NIRS §1.5, IJV-PA §2.2) — pick a vessel big enough that the venous signal dominates.
2. **Signal modulation / separation** to lift a small venous component out of a noisy mixed background (peripheral-venous modulation §1.3, e-tattoo spatial filtering §1.4, DNN inversion §1.2).
3. **Physics-based decoloring** to correct wavelength-dependent fluence / spectral contaminants before unmixing (deep-tissue PA fluence correction §2.3, per-vessel spectral cleanup in vis-OCT §2.4, intravascular PACT §2.5).

The genuinely new item today — the **Zhang et al. retinal-oximetry review (§2.1)** — sits at the intersection of strategies 1 and 3 for the *retinal* venous bed: retinal veins give an anatomically clean, directly imaged intravascular venous target, and the review's core message is that per-vessel accuracy is now gated by **decoloring-type corrections** (vessel diameter, pigmentation, media) plus **fusion with blood-flow measurement and AI** — precisely the agenda the deep-vein PA (§2.3) and intravascular PACT (§2.5) anchors are pursuing in the systemic vasculature. Retinal venular oximetry is thus the most mature, highest-precision proving ground for the corrections that the harder deep-venous problem still needs; the day's tangential JMIR lead is the counterweight, a reminder that even *arterial* wearable oximetry fails in the low-saturation range where venous measurement lives. Net: no bedside-ready systemic non-invasive SvO₂ optical device emerged today, and the honest population of strong, truly-venous, truly-optical papers remains **fewer than five per topic** once arterial-only and tissue-level work is excluded.

---

*Scan generated 2026-08-05 (UTC). Metadata cross-checked across ≥2 search-index snippets per item; publisher full-text pages returned HTTP 403 to direct fetch in this environment (source-side anti-bot; agent proxy healthy), so items flagged "full text not read" are abstract/snippet-verified. Flagged unverified fields are noted inline.*
