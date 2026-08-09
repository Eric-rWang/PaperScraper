# Venous Oxygen Research Scan — 2026-08-09

**Search window:** Thirty-second scan in the series, run **four days** after 2026-08-05 (no scans on 08-06/07/08). Emphasis on work published or first-surfacing after 08-05, with the standard fallback to the best-available venous-specific work already catalogued. Sources swept today: PubMed/PMC, arXiv (incl. physics.med-ph new-listing sweep), bioRxiv/medRxiv, Optica (Biomed. Opt. Express, Optics Letters, Applied Optics), SPIE / *J. Biomed. Opt.*, *Photoacoustics* (ScienceDirect), Springer (Graefe's Archive, *Biomed. Mater. Devices*), Wiley (*Advanced Science*, *J. Biophotonics*), De Gruyter, MDPI (*Sensors/Biosensors*), Frontiers (*Photonics*), Nature / *Sci. Rep.* / *Commun. Med.*, IEEE Xplore, JMIR, ClinicalTrials.gov, ResearchGate, Semantic Scholar.

**Verification caveat:** Publisher **full-text** pages — link.springer.com, pmc.ncbi.nlm.nih.gov, pubmed.ncbi.nlm.nih.gov, opg.optica.org, sciencedirect.com, nature.com, wiley.com — again returned **HTTP 403** to direct `WebFetch`, and **arxiv.org is egress-blocked** in this environment today (the agent proxy itself reported healthy; the blocks are source-/policy-side, not relay failures). Every reference below was therefore cross-checked across **at least two independent search-index snippets** (Google Scholar–style result blocks + PubMed / PMC / Springer / Optica / De Gruyter listings); per-item notes state what was confirmed and what could not be read directly on a publisher page.

---

## ⚠️ Read this first — day summary

**No new venous-specific *primary* measurement paper today — the eleventh consecutive scan cycle with none.** Consistent with the series' standing observation, truly novel non-invasive **venous**-optical measurement work publishes at very low volume, and today's four-day sweep produced **no new SvO₂/ScvO₂ demonstration**. The Topic-1 (true SvO₂) top-5 and Topic-2 top-5 measurement anchors are unchanged and carried forward with scores held.

Every candidate returned by today's searches is **previously surfaced**:

- **APM+ deep-tissue PA venous oximetry** (Sastry, Olick-Gibson et al., *Advanced Science* 2026, DOI 10.1002/advs.76366) — corpus §2.3, still the most recent primary PA venous advance; no new version.
- **Wearable arterial+venous e-tattoo** (Tan/Lu, UT Austin, PMID 38083768; patent US 20250025074) — corpus §1.4.
- **Optical Inversion and Spectral Unmixing of Spectroscopic PA Images with Physics-Informed Neural Networks** (arXiv:2602.16357) — surfaced 06-11; a PA decoloring/unmixing method, not venous-specific; unchanged.
- **Wearable NIRS carotid/neck-vessel hemodynamics preliminary study** (PMC12384115) — previously logged; **arterial (carotid)**, transferable-only.
- The retinal-oximetry review (Zhang et al., *Graefe's Archive* 2025, §2.1), IJV-PA human anchor (arXiv:2303.10775, §2.2), ADS-vis-OCT (§2.4), intravascular PACT (BOE 15(5):2741, §2.5), Alqahtani jugular optical sensor (§1.1), IJV DNN/Monte-Carlo (§1.2), peripheral-venous modulation (§1.3), Mespere VO100 jugular NIRS (§1.5), the JMIR wearable-hypoxia caution, the JIOHS PACT-oximetry review, and the Esenaliev/Petrov SSS optoacoustic lineage — all **carried forward, no change**.

**No new primary venous demonstration surfaced.** Per the standing brief: **fewer than 5 genuinely strong, genuinely venous, genuinely non-invasive-optical papers first-surfaced today for either topic** once arterial-only and tissue-level (StO₂) work is excluded. The lists below present the best available with honest relevance scores; entries flagged tissue-/retinal-level, MRI-based, or commercial-device are retained only because the true-venous population is that thin.

---

## Topic 1 — Non-invasive monitoring of venous blood oxygen (SvO₂ / ScvO₂ / peripheral venous)

*No new primary items today.* Standing best-available set (all previously surfaced), scores carried forward. This remains the sparse topic: **no primary non-invasive venous-O₂ measurement paper has first-surfaced since before 2026-07-15.**

### 1.1 — Estimation of Venous Oxygen Saturation Through Non-Invasive Optical Sensing at the Jugular Veins *(previously surfaced — scan 06-10 §1.1; flagship optical-venous device paper)*
- **Authors:** Alqahtani et al.
- **Year / Venue:** 2024 · *Current Directions in Biomedical Engineering* 10(2) (De Gruyter; CDBME-2024-2072)
- **Link / DOI:** https://doi.org/10.1515/cdbme-2024-2072
- **Relevance:** 9.0/10 — direct non-invasive optical SvO₂ at the external/internal jugular; the closest thing the corpus has to a pulse-oximeter-form venous device.
- **Novelty:** Proof-of-concept optical sensor that identifies the jugular venous waveform and estimates SvO₂ within the healthy 60–90% band (71.1 / 72.2 / 70.4% across a three-subject set).
- **Integration insight:** The anchor for the "wearable venous pulse oximeter" thesis; every Topic-1 wearable/peripheral entry is a variation on isolating the venous component this device targets at the neck.

### 1.2 — Quantifying Changes in Oxygen Saturation of the Internal Jugular Vein In Vivo Using Deep Neural Networks and Subject-Specific 3-D Monte-Carlo Models *(previously surfaced — scan 06-10 §1.2)*
- **Authors:** (IJV DNN / Monte-Carlo group)
- **Year / Venue:** 2024 · *Optics Letters* 49(10):2669
- **Link / DOI:** https://opg.optica.org/ol/abstract.cfm?uri=ol-49-10-2669 (Optica abstract locator; raw DOI numeral unverified — see flag below)
- **Relevance:** 8.5/10 — model-based recovery of IJV sO₂ change from multi-channel NIRS reflectance.
- **Novelty:** Subject-specific 3-D Monte-Carlo forward models train a DNN to invert measured reflectance into IJV saturation change, addressing the partial-volume/overlying-tissue confound.
- **Integration insight:** Supplies the computational-inversion half of the jugular-NIRS approach; complements §1.1's hardware. The Monte-Carlo-to-DNN pattern recurs in the Topic-2 PA fluence-correction work.
- **Metadata flag:** DOI string not re-verifiable on the Optica page today (403); the stable Optica locator (ol-49-10-2669) and title/authors/year are cross-confirmed via two search-index snippets. Treat the raw DOI numeral as **unverified**; cite via the Optica abstract URL.

### 1.3 — Proof-of-Concept Non-Invasive Estimation of Peripheral Venous Oxygen Saturation (pulse-modulation venous oximetry) *(previously surfaced — scan 06-10/06-11)*
- **Authors:** (peripheral-venous oximetry group; BioMedical Engineering OnLine)
- **Year / Venue:** 2017 · *BioMedical Engineering OnLine* 16:60
- **Link / DOI:** https://doi.org/10.1186/s12938-017-0351-x
- **Relevance:** 8.0/10 — foundational demonstration that an induced/modulated venous signal yields a peripheral SvO₂ estimate optically.
- **Novelty:** Uses external stimulation to induce cyclical venous fluctuation, lifting the venous component out of the low-SNR background so a PPG-style optical readout can estimate local venous saturation.
- **Integration insight:** Conceptual root of the "modulate the vein, then demodulate" family (muscle-stimulation PPG, e-tattoo spatial filtering). Landmark; recurs because nothing newer has displaced it as the peripheral-venous proof-of-concept.

### 1.4 — Towards Simultaneous Non-Invasive Arterial and Venous Oxygenation Monitoring with a Wearable Optical E-Tattoo *(previously surfaced — scan 07-01 §1.5-family)*
- **Authors:** Tan P., Lu N., et al. (UT Austin)
- **Year / Venue:** 2023/2024 · IEEE (EMBC-lineage); related patent US 20250025074
- **Link / DOI:** https://pubmed.ncbi.nlm.nih.gov/38083768/ · patent: https://patents.justia.com/patent/20250025074
- **Relevance:** 8.0/10 — explicitly names non-invasive **venous** oxygenation as the unmet need and targets it with a wrist-worn optical patch.
- **Novelty:** Ultra-thin self-adherent optical e-tattoo measures arterial + venous pulses from multiple wrist sites; proposes spatial filtering to separate arterial/venous crosstalk.
- **Integration insight:** The wearable-form embodiment of the venous-oximetry goal; its arterial/venous separation problem is the same one §1.3 attacks by modulation and §1.1 sidesteps by anatomy. The standing JMIR hypoxia-accuracy caution bears directly on this device class.

### 1.5 — A New Non-Invasive Method for the Assessment of Central Venous Oxygen Saturation (Mespere VO100 jugular NIRS) *(previously surfaced — scan 06-14; commercial NIRS device)*
- **Authors:** (VO100 clinical validation group)
- **Year / Venue:** 2023/2024 · *J. Cardiothorac. Vasc. Anesth.* (S1053-0770 lineage) / ScienceDirect
- **Link / DOI:** https://www.sciencedirect.com/science/article/pii/S1053077023007826
- **Relevance:** 7.5/10 — the one commercially available non-invasive jugular-NIRS ScvO₂ estimator; clinically evaluated in critically ill patients.
- **Novelty:** Continuous non-invasive ScvO₂ estimate from an external jugular NIRS sensor, positioned as an alternative when catheter-based sampling is difficult.
- **Integration insight:** The clinical-translation benchmark for Topic 1 — the accuracy/bias any research-grade optical venous device (§1.1–1.4) must beat to matter at the bedside.

**Topic 1 honest note:** every entry above is previously surfaced; nos. 1.3 and 1.5 predate 2023. The absence of *new* primary venous measurement work today is itself the finding, not a gap in searching.

---

## Topic 2 — Optical imaging techniques for non-invasively obtaining venous blood oxygen (PA/PACT, NIRS, DOI/DOT, hyperspectral, vis-OCT, SFDI)

*No new items today.* Carried-forward measurement anchors with scores held.

### 2.1 — Retinal Oximetry: New Insights into Ocular and Systemic Diseases *(previously surfaced — scan 08-05 §2.1; review of per-vessel retinal artery+vein sO₂)*
- **Authors:** Zhang W., Tu X., Wang X., et al.
- **Year / Venue:** 2025 · *Graefe's Archive for Clinical and Experimental Ophthalmology* 263:2101–2115
- **Link / DOI:** https://doi.org/10.1007/s00417-025-06831-8 · PMID 40254630 · PMC12414079
- **Relevance:** 7.5/10 — retinal veins are among the very few human sites where a true **intravascular venous sO₂** is read optically and non-invasively; the corpus's dedicated review of that measurement. (Not systemic SvO₂; retinal venular, per-vessel.)
- **Novelty:** Consolidates retinal oximetry across spectrophotometric-fundus, hyperspectral, and vis-OCT modalities; frames retinal artery *and vein* saturation as biomarkers of ocular + systemic microcirculation; enumerates vessel-diameter, pigmentation, and media-transparency error sources; flags wide-field, non-mydriatic, blood-flow-fusion, and AI directions as the accuracy frontier.
- **Integration insight:** Ties the Topic-2 retinal cluster (HSI; ADS-vis-OCT §2.4) into one framework and names, at review level, the exact per-vessel confounds a venular oximeter must correct — the retinal analogue of the fluence/spectral-coloring problem the deep-vein PA anchors face.
- **Metadata flag:** Bibliographic fields cross-confirmed (Springer + PubMed + PMC); **full text not read** (403) — summary is abstract/snippet-level.

### 2.2 — Noninvasive In Vivo Photoacoustic Measurement of Internal Jugular Venous Oxygenation in Humans *(previously surfaced — scan 06-10 §2.1; the Topic-2 anchor)*
- **Authors:** (IJV-PA human oximetry group; Garcia-Uribe / Wang lineage)
- **Year / Venue:** 2023 · arXiv:2303.10775 / PA human-imaging lineage
- **Link / DOI:** https://arxiv.org/abs/2303.10775
- **Relevance:** 9.5/10 — the single most on-target Topic-2 paper: photoacoustic sO₂ of a named deep **vein** (internal jugular) in humans, non-invasively (sijvO₂ ≈ 72 ± 7%).
- **Novelty:** Demonstrates human IJV oxygenation from multi-wavelength PA, pushing PA oximetry from superficial microvessels to a clinically meaningful deep venous target.
- **Integration insight:** The proof that optical/PA venous oximetry can reach a central-venous surrogate; the bridge between Topic 1's clinical need and Topic 2's imaging physics.

### 2.3 — Arterial Blood-Mediated Deep-Tissue Photoacoustic Oximetry (APM+): in-vivo human radial-vein sO₂ *(previously surfaced — upgraded 07-15 §2.2)*
- **Authors:** Sastry, Olick-Gibson, et al.
- **Year / Venue:** 2026 · *Advanced Science* (Wiley)
- **Link / DOI:** https://doi.org/10.1002/advs.76366
- **Relevance:** 9.0/10 — in-vivo human **radial-vein** sO₂ via a deep-tissue PA method that explicitly tackles spectral coloring.
- **Novelty:** The arterial prior method (APM+) leverages high arterial sO₂ to locally calibrate optical fluence and correct wavelength-dependent spectral coloring, recovering deep-tissue venous sO₂ where conventional linear unmixing fails.
- **Integration insight:** The most recent (2026) primary PA venous-oximetry advance in the corpus; its fluence-correction strategy is the deep-vein counterpart to the retinal per-vessel corrections §2.1 catalogues, and to the PINN spectral-unmixing lead (arXiv:2602.16357).

### 2.4 — Adaptive Spectroscopic Visible-Light OCT for Clinical Retinal Oximetry (ADS-vis-OCT) *(previously surfaced — scan 06-11 §2.2)*
- **Authors:** (ADS-vis-OCT group)
- **Year / Venue:** 2023 · *Communications Medicine* 3:59
- **Link / DOI:** https://doi.org/10.1038/s43856-023-00288-8
- **Relevance:** 8.5/10 — per-vessel retinal **vein** sO₂ with reported repeatability SD ≈ 2.3% in veins; ~1% bias vs blood-gas across 0–100%.
- **Novelty:** Adaptively removes per-vessel spectral contaminants, yielding accurate, repeatable artery *and vein* sO₂ across varying vessel diameters in humans.
- **Integration insight:** The highest-precision per-vessel venous optical readout in the corpus; the concrete modality the §2.1 review holds up as state-of-the-art for retinal venular oximetry.

### 2.5 — Oxygenation Heterogeneity Facilitates Spatiotemporal Flow-Pattern Visualization Inside Human Blood Vessels Using PACT *(previously surfaced — scan 06-11 / 06-10)*
- **Authors:** (PACT intravascular flow/oxygenation group)
- **Year / Venue:** 2024 · *Biomedical Optics Express* 15(5):2741
- **Link / DOI:** https://doi.org/10.1364/BOE.518632 → https://opg.optica.org/boe/fulltext.cfm?uri=boe-15-5-2741
- **Relevance:** 8.0/10 — resolves sO₂ heterogeneity and laminar-flow structure *inside* human vessels (incl. veins) with PACT.
- **Novelty:** First-time recovery of the parabolic laminar-flow wavefront inside a deep vein in vivo by exploiting intravascular oxygenation heterogeneity across multi-wavelength PA spectra.
- **Integration insight:** Shows PACT can read *within-lumen* venous oxygen structure, not just a vessel-average — the imaging counterpart to §2.1's "fuse oximetry with blood-flow measurement" thesis.
- **Metadata flag:** DOI numeral not re-verifiable on the Optica page today (403); the stable Optica locator (boe-15-5-2741) + title/year cross-confirmed. Cite via the Optica URL; treat the raw DOI numeral as **unverified**.

---

## Standing context leads (not ranked in the top-5)

- **Optical Inversion and Spectral Unmixing of Spectroscopic PA Images with Physics-Informed Neural Networks** — arXiv:2602.16357 (surfaced 06-11). PA decoloring/spectral-unmixing method; not venous-specific, but directly relevant to the fluence-correction problem the deep-vein PA anchors (§2.2/§2.3) face. Carried forward; **arxiv.org egress-blocked today**, so re-verified only via search-index snippet.
- **Wearable NIRS for neck-vessel (carotid) hemodynamics — preliminary study** (PMC12384115). **Arterial (carotid)**, not venous; retained as a transferable wearable-NIRS lead for the neck-vessel form factor (§1.1/§1.5 family). Not a venous paper.
- **Performance of Wearable Pulse Oximetry During Controlled Hypoxia Induction** — *JMIR Formative Research*, 2026 (formative.jmir.org/2026/1/e85253). **Arterial-only** wearable SpO₂ validation (Apple Watch S7, Masimo MightySat Rx) showing >FDA-threshold error in the hypoxemic range. Transferable caution for the wearable-venous device class (§1.3/§1.4), which operates at even lower saturations.
- **Quantitative Oximetry with PACT: Principles, Progress, and Prospects** — *J. Innov. Opt. Health Sci.*, 2026 (DOI 10.1142/S1793545826300065). Review-level scaffold under the deep-vein PA anchors; authors unverified. Carried forward.
- **Classic ovine / large-vein optoacoustic SSS venous work** (Esenaliev/Petrov lineage; superior sagittal sinus, triple-wavelength optoacoustic large-vein oximetry). Foundational venous-optoacoustic prior art; historical root of deep-venous PA oximetry.
- **Karlas et al., MSOT of muscle perfusion/oxygenation under arterial and venous occlusion — human pilot** (*J. Biophotonics* 2020). Tissue-level (StO₂), not intravascular SvO₂, but the closest MSOT venous-challenge human data; retained as a tissue-level lead.

---

## Cross-topic synthesis

Today reinforces the series' central, honest finding: **non-invasive optical measurement of true venous blood oxygen is a low-volume field, and no new primary venous *measurement* appeared today** (eleventh consecutive dry cycle). The two topics remain coupled by one problem — **isolating the venous signal and correcting the confound that corrupts its saturation estimate** — addressed by three complementary strategies the corpus continues to organize around:

1. **Anatomical targeting** of a large, named vein (jugular optical sensing §1.1, jugular NIRS §1.5, IJV-PA §2.2) — pick a vessel big enough that the venous signal dominates.
2. **Signal modulation / separation** to lift a small venous component out of a noisy mixed background (peripheral-venous modulation §1.3, e-tattoo spatial filtering §1.4, DNN inversion §1.2).
3. **Physics-based decoloring** to correct wavelength-dependent fluence / spectral contaminants before unmixing (deep-tissue PA fluence correction §2.3, per-vessel spectral cleanup in vis-OCT §2.4, intravascular PACT §2.5, PINN spectral unmixing lead).

No entry moved between these strategies today and no new instance of any of them surfaced. The most mature, highest-precision proving ground for the strategy-3 corrections remains **retinal venular oximetry** (§2.1/§2.4), where a directly imaged intravascular venous target makes per-vessel decoloring tractable; the hardest open problem remains the **systemic deep vein**, where §2.2/§2.3 are pushing PA fluence correction toward a clinically meaningful central-venous surrogate. The counterweight is unchanged: even *arterial* wearable oximetry (the JMIR lead) fails in the low-saturation range where venous measurement lives, so the accuracy bar for any wearable venous device (§1.3/§1.4) is, if anything, higher than the arterial state of the art. Net: **no bedside-ready systemic non-invasive SvO₂ optical device emerged today**, and the honest population of strong, truly-venous, truly-optical papers remains **fewer than five per topic** once arterial-only and tissue-level work is excluded.

---

*Scan generated 2026-08-09 (UTC). Metadata cross-checked across ≥2 search-index snippets per item; arxiv.org was egress-blocked and publisher full-text pages returned HTTP 403 to direct fetch in this environment (source-/policy-side; agent proxy healthy), so items flagged "full text not read" are abstract/snippet-verified and flagged unverified fields are noted inline.*
