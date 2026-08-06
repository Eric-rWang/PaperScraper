# Venous Oxygen Research Scan — 2026-08-06

**Search window:** Thirty-second scan in the series, run **one day** after 2026-08-05. Emphasis on work published or first-surfacing after 08-05, with the standard fallback to the best-available venous-specific work already catalogued. Sources swept today: PubMed/PMC, arXiv (incl. physics.med-ph new-listing sweep), bioRxiv/medRxiv, Optica (Biomed. Opt. Express, Optics Letters, Applied Optics), SPIE / *J. Biomed. Opt.*, *Photoacoustics* (ScienceDirect), *Computers in Biology and Medicine*, Springer (Graefe's Archive), Wiley (*Advanced Science*, *J. Biophotonics*), De Gruyter, MDPI (*Biosensors/Sensors*), Frontiers (*Photonics*, *Oncology Reviews*), Nature / *Sci. Rep.* / *Commun. Med.*, IEEE Xplore, JMIR, ClinicalTrials.gov, USPTO, ResearchGate, Semantic Scholar.

**Verification caveat:** As in every prior scan, publisher **full-text** pages — including link.springer.com, pmc.ncbi.nlm.nih.gov, pubmed.ncbi.nlm.nih.gov, opg.optica.org, sciencedirect.com, frontiersin.org and the Nature/Wiley domains — returned **HTTP 403** to direct `WebFetch` in this environment today (the agent proxy itself reported healthy with no relay failures; the 403s are source-side anti-bot blocks). Every reference below was therefore cross-checked across **at least two independent search-index snippets** (Google Scholar–style result blocks + PubMed / PMC / Springer / Optica / ScienceDirect / Frontiers listings); per-item notes state what was confirmed and what could not be read directly on a publisher page.

---

## ⚠️ Read this first — day summary

**No new venous-specific *primary* measurement paper today — the eleventh consecutive scan cycle with none.** Consistent with the series' standing observation, truly novel non-invasive **venous**-optical measurement work publishes at very low volume, and today's one-day sweep produced **no new SvO₂/ScvO₂ demonstration**. The Topic-1 (true SvO₂) top-5 and the Topic-2 top-5 measurement anchors are unchanged and carried forward with scores held.

Today surfaced **two genuinely new-to-corpus items**, both under Topic 2, and both **tissue-level / tumor-microenvironment optoacoustic-methods work — not true intravascular venous sO₂**. They are logged honestly with low venous-relevance scores because the technique (multi-wavelength PA/optoacoustic sO₂ recovery) is directly transferable, not because either measures a vein:

- **★ NEW (Topic 2, tangential) — "Recent advances in photoacoustic–ultrasound dual-modality fusion imaging for functional visualization of the superficial tumor microenvironment," *Frontiers in Oncology Reviews*, 2026** (DOI 10.3389/or.2026.1881685). A 2026 review of PA/US fusion imaging for the tumor microenvironment, covering hemoglobin-sensitive PA estimation of total hemoglobin and blood **sO₂**, oxygenation heterogeneity and hypoxia mapping, co-registered with ultrasound for anatomical localization. Tissue/tumor-level oxygenation, **not venous SvO₂**; relevant only as a current-state scaffold for the PA-oximetry + US-coregistration approach the IJV-PA anchor (§2.2) embodies. *Title / venue / DOI / 2026 year cross-confirmed across the Frontiers listing + Google-Scholar-style snippet; full author list could not be read (publisher 403) and is flagged unverified.*

- **★ NEW (Topic 2, tangential) — "Advancing multispectral optoacoustic tomography (MSOT): Phasor analysis for real-time spectral unmixing," *Computers in Biology and Medicine*, 2025** (vol. 195, art. 110586; PMID 40554059; PII S0010482525009370). Di Giacinto F., Riente A., Mignini I., et al. A phasor-analysis method for **real-time spectral unmixing** in MSOT, demonstrated in the GI/inflammatory (Crohn's-lineage) tissue context. Improves the speed/robustness of separating HbO₂/Hb — hence sO₂ — from multi-wavelength optoacoustic data, but the readout is **tissue-level StO₂, not intravascular SvO₂**. Included as a transferable-methods item: real-time unmixing is exactly the bottleneck a bedside venous-PA device (§2.2/§2.3) must solve. *Title / authors / venue / volume+article / PMID / year cross-confirmed across PubMed + ScienceDirect index snippets; full text not read (publisher 403) — abstract/snippet-level.*

Everything else returned today is **previously surfaced** or out-of-scope: the jugular optical SvO₂ sensor (Alqahtani, De Gruyter CDBME-2024-2072), the IJV DNN + Monte-Carlo work (*Optics Letters* 49(10):2669), the peripheral-venous pulse-modulation proof-of-concept (*BioMed Eng OnLine* 2017), the UT-Austin arterial+venous optical **e-tattoo** (PMID 38083768 / patent US 20250025074), APM+ radial-vein PA oximetry (Sastry/Olick-Gibson et al., *Adv. Sci.* 2026, 10.1002/advs.76366), the IJV-PA anchor (arXiv:2303.10775), the retinal-oximetry review (Zhang et al., *Graefe's Archive* 2025, PMID 40254630), the hyperspectral retinal HSI system (PMC12997856), the ADS-vis-OCT retinal oximetry paper (*Commun. Med.* 2023), PACT intravascular oxygenation/flow (BOE 15(5):2741), the sulfate blood-phantom metrology paper (arXiv:2512.01458), Hybrid-Net / DL PA segmentation+sO₂ (arXiv:2512.15394), Mespere VO100 jugular NIRS, the McDiarmid MRI iSvO₂ model, the SSL intra-cardiac MR oximetry preprint, the classic ovine/large-vein optoacoustic SSS venous work (Esenaliev/Petrov lineage), and the Karlas MSOT arterial/venous-occlusion muscle pilot. **No new primary venous demonstration.**

Honest sparseness statement, per the standing brief: **fewer than 5 genuinely strong, genuinely venous, genuinely non-invasive-optical papers first-surfaced today for either topic** once arterial-only and tissue-level (StO₂) work is excluded. The lists below present the best available with honest relevance scores; several entries are explicitly flagged as tissue-/retinal-level, MRI-based, or metrology rather than true systemic SvO₂ optical measurement, and are retained only because the true-venous population is that thin.

---

## Topic 1 — Non-invasive monitoring of venous blood oxygen (SvO₂ / ScvO₂ / peripheral venous)

*No new items today.* The standing best-available set (all previously surfaced) with scores carried forward. This remains the sparse topic: **no primary non-invasive venous-O₂ measurement paper has first-surfaced since before 2026-07-15.**

### 1.1 — Estimation of Venous Oxygen Saturation Through Non-Invasive Optical Sensing at the Jugular Veins *(previously surfaced — scan 06-10 §1.1; flagship optical-venous device paper)*
- **Authors:** Alqahtani et al.
- **Year / Venue:** 2024 · *Current Directions in Biomedical Engineering* 10(2) (De Gruyter; CDBME-2024-2072)
- **Link / DOI:** https://doi.org/10.1515/cdbme-2024-2072
- **Relevance:** 9.0/10 — direct non-invasive optical SvO₂ at the external/internal jugular; the closest thing the corpus has to a pulse-oximeter-form venous device.
- **Novelty:** Proof-of-concept optical sensor that identifies the jugular venous waveform and estimates SvO₂ within the healthy 60–90% band (per-subject EJV estimates ≈71.1 / 72.2 / 70.4%) across a small subject set.
- **Integration insight:** The anchor for the "wearable venous pulse oximeter" thesis; every Topic-1 wearable/peripheral entry is a variation on isolating the venous component this device targets at the neck.

### 1.2 — Quantifying Changes in Oxygen Saturation of the Internal Jugular Vein In Vivo Using Deep Neural Networks and Subject-Specific 3-D Monte-Carlo Models *(previously surfaced — scan 06-10 §1.2)*
- **Authors:** (IJV DNN / Monte-Carlo group)
- **Year / Venue:** 2024 · *Optics Letters* 49(10):2669
- **Link / DOI:** https://opg.optica.org/ol/abstract.cfm?uri=ol-49-10-2669 (Optica abstract locator; raw DOI numeral unverified — see flag below)
- **Relevance:** 8.5/10 — model-based recovery of IJV sO₂ change from multi-channel NIRS reflectance.
- **Novelty:** Subject-specific 3-D Monte-Carlo forward models train a DNN to invert measured reflectance into IJV saturation change, addressing the partial-volume/overlying-tissue confound.
- **Integration insight:** Supplies the computational-inversion half of the jugular-NIRS approach; complements §1.1's hardware. The Monte-Carlo-to-DNN pattern recurs in the Topic-2 PA fluence-correction work.
- **Metadata flag:** DOI string could not be re-verified on the Optica page today (403); the stable Optica abstract locator (ol-49-10-2669) and title/authors/year are cross-confirmed via two search-index snippets. Treat the raw DOI numeral as **unverified**; cite via the Optica abstract URL.

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
- **Integration insight:** The wearable-form embodiment of the venous-oximetry goal; its arterial/venous separation problem is the same one §1.3 attacks by modulation and §1.1 sidesteps by anatomy (large jugular target). The standing JMIR hypoxia-accuracy caution bears directly on this device class.

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

*Two genuinely new-to-corpus entries today (§2.1a, §2.1b), both tissue-/tumor-level PA/optoacoustic methods rather than true venous — logged with honest low venous scores — plus the carried-forward measurement anchors §2.2–§2.6, scores held.*

### 2.1a — ★ NEW (tangential) — Recent Advances in Photoacoustic–Ultrasound Dual-Modality Fusion Imaging for Functional Visualization of the Superficial Tumor Microenvironment *(new to corpus; tissue/tumor-level PA sO₂, not venous)*
- **Authors:** (Frontiers review author group — full list unverified, publisher 403)
- **Year / Venue:** 2026 · *Frontiers in Oncology Reviews*
- **Link / DOI:** https://doi.org/10.3389/or.2026.1881685
- **Relevance:** 4.5/10 — a current-state review of PA/US fusion imaging that covers hemoglobin-sensitive PA estimation of total hemoglobin and **sO₂**, oxygenation heterogeneity and hypoxia, co-registered with ultrasound. **Tissue/tumor-level, not intravascular venous**; scored for transferable technique only.
- **Novelty:** Consolidates the 2024–2026 state of PA/US dual-modality functional imaging: multiparametric TME readouts (angiogenesis/perfusion, oxygenation heterogeneity/hypoxia, immune-related exploratory contrast) with US supplying anatomical localization and procedural guidance for the PA sO₂ map.
- **Integration insight:** The PA-oximetry-plus-ultrasound-coregistration architecture it reviews is exactly the modality pairing the IJV-PA anchor (§2.2) uses to place a venous sO₂ estimate on a named deep vein; the review's "oxygenation heterogeneity / hypoxia mapping" framing is the tumor-bed analogue of the intravascular heterogeneity the PACT work (§2.6) exploits inside veins.
- **Metadata flag:** Title / venue / DOI / 2026 year cross-confirmed (Frontiers listing + Scholar-style snippet); **author list and full text not read** (publisher 403) — abstract/snippet-level, authors flagged unverified.

### 2.1b — ★ NEW (tangential) — Advancing Multispectral Optoacoustic Tomography (MSOT): Phasor Analysis for Real-Time Spectral Unmixing *(new to corpus; tissue-level StO₂ methods, not venous)*
- **Authors:** Di Giacinto F., Riente A., Mignini I., Ainora M.E., Esposto G., Borriello R., Zocco M.A., Minordi L.M., Sala E., Scaldaferri F., Gasbarrini A., De Spirito M., Maulucci G.
- **Year / Venue:** 2025 · *Computers in Biology and Medicine* 195:110586
- **Link / DOI:** PMID 40554059 · https://www.sciencedirect.com/science/article/pii/S0010482525009370
- **Relevance:** 4.5/10 — a **real-time spectral-unmixing** method for MSOT (phasor analysis), demonstrated in a GI/inflammatory tissue context. Recovers HbO₂/Hb — hence sO₂ — faster/more robustly, but the readout is **tissue-level StO₂, not intravascular SvO₂**; scored for transferable technique only.
- **Novelty:** Adapts phasor analysis (a lifetime/spectral-imaging technique) to MSOT so oxygenation unmixing runs in real time without per-pixel iterative fitting — a speed/robustness advance over conventional linear or learned unmixing.
- **Integration insight:** Real-time unmixing is the throughput bottleneck any *bedside* venous-PA device (§2.2 IJV-PA, §2.3 APM+) must clear; a phasor front-end is a candidate accelerator for the multi-wavelength sO₂ inversion those venous methods depend on. Complements the fluence-decoloring line (§2.3) — decoloring fixes accuracy, phasor fixes speed.
- **Metadata flag:** Title / authors / venue / volume+article / PMID / year cross-confirmed (PubMed + ScienceDirect snippets); **full text not read** (publisher 403) — abstract/snippet-level.

### 2.2 — Noninvasive In Vivo Photoacoustic Measurement of Internal Jugular Venous Oxygenation in Humans *(previously surfaced — scan 06-10 §2.1; the Topic-2 anchor)*
- **Authors:** (IJV-PA human oximetry group)
- **Year / Venue:** 2023 · arXiv:2303.10775 / PA human-imaging lineage
- **Link / DOI:** https://arxiv.org/abs/2303.10775
- **Relevance:** 9.5/10 — the single most on-target Topic-2 paper: photoacoustic sO₂ of a named deep **vein** (internal jugular) in humans, non-invasively.
- **Novelty:** Demonstrates human IJV oxygenation from multi-wavelength PA, pushing PA oximetry from superficial microvessels to a clinically meaningful deep venous target.
- **Integration insight:** The proof that optical/PA venous oximetry can reach a central-venous surrogate; the bridge between Topic 1's clinical need and Topic 2's imaging physics. Both of today's new tangential items (§2.1a/§2.1b) describe the exact acquisition-and-unmixing machinery this anchor runs on.

### 2.3 — Arterial Blood-Mediated Deep-Tissue Photoacoustic Oximetry (APM+): in-vivo human radial-vein sO₂ *(previously surfaced — upgraded 07-15 §2.2)*
- **Authors:** Sastry, Olick-Gibson, et al.
- **Year / Venue:** 2026 · *Advanced Science* (Wiley)
- **Link / DOI:** https://doi.org/10.1002/advs.76366
- **Relevance:** 9.0/10 — in-vivo human **radial-vein** sO₂ via a deep-tissue PA method that explicitly tackles spectral coloring.
- **Novelty:** Uses arterial-blood-mediated calibration to correct wavelength-dependent fluence, recovering deep-tissue venous sO₂ where conventional linear unmixing fails (median error ≈2.9% vs ≈9.8% for linear unmixing in phantom/ex-vivo tests).
- **Integration insight:** The most recent (2026) primary PA venous-oximetry advance in the corpus; its fluence-correction strategy is the accuracy complement to today's §2.1b real-time-unmixing (speed) contribution.

### 2.4 — Adaptive Spectroscopic Visible-Light OCT for Clinical Retinal Oximetry (ADS-vis-OCT) *(previously surfaced — scan 06-11 §2.2)*
- **Authors:** (ADS-vis-OCT group)
- **Year / Venue:** 2023 · *Communications Medicine* 3:59
- **Link / DOI:** https://doi.org/10.1038/s43856-023-00288-8
- **Relevance:** 8.5/10 — per-vessel retinal **vein** sO₂ with reported repeatability SD ≈ 2.3% in veins.
- **Novelty:** Adaptively removes per-vessel spectral contaminants, yielding accurate, repeatable artery *and vein* sO₂ across varying vessel diameters in humans.
- **Integration insight:** The highest-precision per-vessel venous optical readout in the corpus; the concrete modality the retinal-oximetry review (standing lead) holds up as state-of-the-art for retinal venular oximetry.

### 2.5 — Development and Validation of a High-Resolution Hyperspectral Imaging System for the Retina *(previously surfaced — scan 07-31/08-03; per-vessel retinal artery/vein sO₂)*
- **Authors:** (UT Southwestern HSI retina group)
- **Year / Venue:** 2026 · PMC12997856 (accepted Feb 2026, published Mar 2026)
- **Link / DOI:** https://pmc.ncbi.nlm.nih.gov/articles/PMC12997856/
- **Relevance:** 8.0/10 — simultaneous per-vessel retinal vessel-diameter and oxygenation extraction; reports average arteriole sO₂ ≈98% vs venule sO₂ ≈58%, a clean per-vessel **venous** readout.
- **Novelty:** A validated high-resolution retinal HSI system extracting vessel diameter and oxygenation rate simultaneously from a single hyperspectral acquisition.
- **Integration insight:** The hyperspectral leg of the retinal venular-oximetry cluster (with §2.4 vis-OCT); the clear arteriole/venule sO₂ separation is the retinal proof that per-vessel venous saturation is recoverable when the vessel is directly imaged.

### 2.6 — Oxygenation Heterogeneity Facilitates Spatiotemporal Flow-Pattern Visualization Inside Human Blood Vessels Using PACT *(previously surfaced — scan 06-11 / 06-10)*
- **Authors:** (PACT intravascular flow/oxygenation group)
- **Year / Venue:** 2024 · *Biomedical Optics Express* 15(5):2741
- **Link / DOI:** https://doi.org/10.1364/BOE.518632 → https://opg.optica.org/boe/fulltext.cfm?uri=boe-15-5-2741
- **Relevance:** 8.0/10 — resolves sO₂ heterogeneity and laminar-flow structure *inside* human vessels (incl. veins) with PACT.
- **Novelty:** First-time recovery of the parabolic laminar-flow wavefront inside a deep vein in vivo by exploiting intravascular oxygenation heterogeneity across multi-wavelength PA spectra.
- **Integration insight:** Shows PACT can read *within-lumen* venous oxygen structure, not just a vessel-average — the deep-vessel counterpart to the retinal flow+oximetry fusion agenda, and the intravascular analogue of §2.1a's tumor-bed oxygenation-heterogeneity mapping.
- **Metadata flag:** DOI numeral could not be re-verified on the Optica page today (403); the stable Optica locator (boe-15-5-2741) + title/year cross-confirmed. Cite via the Optica URL; treat the raw DOI numeral as **unverified**.

---

## Standing context leads (not ranked in the top-5)

- **Retinal Oximetry: New Insights into Ocular and Systemic Diseases** — Zhang W., Tu X., Wang X., et al., *Graefe's Archive* 263:2101–2115, 2025 (DOI 10.1007/s00417-025-06831-8; PMID 40254630; PMC12414079). Review-level scaffold of per-vessel retinal artery+**vein** oximetry; ties §2.4/§2.5 together and enumerates the per-vessel decoloring confounds. Carried forward from 08-05.
- **AI-driven multimodal retinal imaging for early detection and risk stratification of vascular and neurodegenerative diseases** — *Graefe's Archive*, 2026 (DOI 10.1007/s00417-026-07273-6). Venous-oximetry relevance **unverified** (403). Watch-lead only.
- **Performance of Wearable Pulse Oximetry During Controlled Hypoxia Induction: Instrument Validation Study** — *JMIR Formative Research*, 2026 (formative.jmir.org/2026/1/e85253). **Arterial-only** wearable SpO₂ validation showing >FDA-threshold error in the hypoxemic range. Transferable caution for the wearable-venous device class (§1.3/§1.4), which operates at even lower saturations. Not a venous paper.
- **Deep Learning-Driven Quantitative Spectroscopic Photoacoustic Imaging for Segmentation and Oxygen Saturation Estimation** — arXiv:2512.15394. DL joint vessel-segmentation + sO₂; methods-transferable to venous PA, not venous-specific. Carried forward.
- **Quantitative oximetry with PACT: Principles, Progress, and Prospects** — *J. Innov. Opt. Health Sci.*, 2026 (DOI 10.1142/S1793545826300065). Review scaffold under the deep-vein PA anchors; authors unverified. Carried forward.
- **Classic ovine / large-vein optoacoustic SSS venous work** (Esenaliev/Petrov lineage; superior sagittal sinus, triple-wavelength optoacoustic large-vein oximetry). Foundational venous-optoacoustic prior art; predates the series window, retained as the historical root of deep-venous PA oximetry.
- **Karlas et al., MSOT of muscle perfusion/oxygenation under arterial and venous occlusion — human pilot** (*J. Biophotonics* 2020). Tissue-level (StO₂), not intravascular SvO₂, but the closest MSOT venous-challenge human data; retained as a tissue-level lead — and the direct clinical-application context for today's new §2.1b MSOT-unmixing method.

---

## Cross-topic synthesis

Today reinforces the series' central, honest finding: **non-invasive optical measurement of true venous blood oxygen is a low-volume field, and no new primary venous *measurement* appeared today** (eleventh consecutive dry cycle). The two topics remain coupled by one problem — **isolating the venous signal and correcting the confound that corrupts its saturation estimate** — solved by three complementary strategies:

1. **Anatomical targeting** of a large, named vein (jugular optical sensing §1.1, jugular NIRS §1.5, IJV-PA §2.2) — pick a vessel big enough that the venous signal dominates.
2. **Signal modulation / separation** to lift a small venous component out of a noisy mixed background (peripheral-venous modulation §1.3, e-tattoo spatial filtering §1.4, DNN inversion §1.2).
3. **Physics-based decoloring + fast unmixing** to correct wavelength-dependent fluence / spectral contaminants before, and while, unmixing (deep-tissue PA fluence correction §2.3, per-vessel spectral cleanup in vis-OCT §2.4, hyperspectral per-vessel extraction §2.5, intravascular PACT §2.6).

Both of today's new items land squarely on strategy 3 but on the *tissue* side of the venous line. The **Frontiers PA/US fusion review (§2.1a)** documents the acquisition architecture — hemoglobin-contrast PA sO₂ co-registered with ultrasound for localization — that is precisely what turns a raw PA oximetry map into a *named-vessel* venous reading (the move the IJV-PA anchor §2.2 makes). The **MSOT phasor-unmixing method (§2.1b)** attacks the other half of strategy 3: not accuracy (which APM+ §2.3 targets via decoloring) but **speed**, making multi-wavelength oxygenation unmixing real-time — a prerequisite for any continuous bedside venous-PA monitor. Neither measures a vein; both are logged with honest ~4.5/10 venous scores because the *machinery* transfers, not the target. Net: no bedside-ready systemic non-invasive SvO₂ optical device emerged today, and the honest population of strong, truly-venous, truly-optical papers remains **fewer than five per topic** once arterial-only and tissue-level work is excluded — the retinal venular cluster (§2.4/§2.5) and the deep-vein PA cluster (§2.2/§2.3/§2.6) continue to carry the field.

---

*Scan generated 2026-08-06 (UTC). Metadata cross-checked across ≥2 search-index snippets per item; publisher full-text pages returned HTTP 403 to direct fetch in this environment (source-side anti-bot; agent proxy healthy), so items flagged "full text not read" are abstract/snippet-verified. Flagged unverified fields are noted inline.*
