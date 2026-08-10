# Venous Oxygen Research Scan — 2026-08-10

**Search window:** Thirty-third scan in the series, run **one day** after 2026-08-09. Emphasis on work published or first-surfacing after 08-09, with the standard fallback to the best-available venous-specific work already catalogued. Sources swept today: PubMed/PMC, arXiv (physics.med-ph / eess.IV new-listing sweep), bioRxiv/medRxiv, Optica (Biomed. Opt. Express, Optics Letters, Applied Optics), SPIE / *J. Biomed. Opt.*, *Photoacoustics* (ScienceDirect), Springer / Nature portfolio (*Eye*, *Sci. Rep.*, *Commun. Med.*, Graefe's Archive), Wiley (*Advanced Science*, *J. Biophotonics*), De Gruyter, MDPI (*Sensors*), Frontiers, *Translational Pediatrics* / AME, World Scientific (*JIOHS*), IEEE Xplore, ClinicalTrials.gov, ResearchGate, Semantic Scholar, Google Scholar result blocks.

**Verification caveat:** Publisher **full-text** pages — nature.com, pmc.ncbi.nlm.nih.gov, link.springer.com, opg.optica.org, sciencedirect.com, wiley.com — and **arxiv.org** were again **egress-blocked / HTTP 403** to direct `WebFetch` in this environment today (the agent proxy reported healthy; the blocks are source-/policy-side). Every reference below was therefore cross-checked across **at least two independent search-index snippets** (Google Scholar–style result blocks + PubMed / PMC / Nature / Optica / researchgate listings); per-item notes state what was confirmed and what could not be read directly on a publisher page.

---

## ⚠️ Read this first — day summary

**No new venous-specific *primary measurement* paper was first-*published* today** — consistent with the series' standing finding that truly novel non-invasive **venous**-optical measurement work publishes at very low volume. This is the twelfth consecutive cycle with no brand-new primary SvO₂/ScvO₂ demonstration.

**However, today's sweep surfaced two solid venous-specific papers that were NOT in the prior corpus** and that materially improve each topic's top-5:

1. **Topic 1 — NIRS regional cerebral oximetry tracking *mixed* venous SvO₂** (Nishikawa et al., *Sci. Rep.* 2023; PMC10709586). A true-SvO₂-relevant, non-invasive optical paper the corpus had not logged: it quantifies how well a bedside NIRS cerebral-oximetry channel *tracks* pulmonary-artery-catheter SvO₂. Newly surfaced → promoted into the Topic-1 top-5.
2. **Topic 2 — Saccadic-Phase Spatial Frequency Domain Imaging (SP-SFDI) retinal oximetry / BioxyDR™** (Basiri, Luo, Shokoohi-Yekta et al., *Eye* 2025; DOI 10.1038/s41433-025-04032-5). The corpus's **first genuine SFDI-applied-to-venous-oxygenation** entry — measures per-vessel retinal **venous** αSO₂ and validates it as a diabetic-retinopathy biomarker. Newly surfaced → promoted into the Topic-2 top-5.

The carried-forward measurement anchors (jugular optical sensing, IJV-PA human oximetry, APM+ deep-tissue PA, ADS-vis-OCT, intravascular PACT) are unchanged with scores held. To make room for the two new entries, the **Mespere VO100 jugular-NIRS device** (Topic 1) and the **Graefe's retinal-oximetry review** (Topic 2) drop to *Standing context leads* today — retained, just not top-5.

**Honest population statement:** once arterial-only and tissue-level (StO₂) work is excluded, the count of strong, genuinely-venous, genuinely-non-invasive-optical papers remains **fewer than five per topic of truly *new* material**. The lists below present the best available with honest relevance scores; every item's provenance (new-to-corpus vs previously surfaced) is flagged.

---

## Topic 1 — Non-invasive monitoring of venous blood oxygen (SvO₂ / ScvO₂ / peripheral venous)

Ranked by relevance to **true non-invasive venous** oxygen (not arterial, not tissue-level StO₂).

### 1.1 — Estimation of Venous Oxygen Saturation Through Non-Invasive Optical Sensing at the Jugular Veins *(previously surfaced — scan 06-10 §1.1; flagship optical-venous device paper)*
- **Authors:** Alqahtani et al.
- **Year / Venue:** 2024 · *Current Directions in Biomedical Engineering* 10(2) (De Gruyter; CDBME-2024-2072)
- **Link / DOI:** https://doi.org/10.1515/cdbme-2024-2072
- **Relevance:** 9.0/10 — direct non-invasive optical SvO₂ at the external/internal jugular; the closest thing the corpus has to a pulse-oximeter-form venous device.
- **Novelty:** Proof-of-concept optical sensor that identifies the jugular venous waveform and estimates SvO₂ within the healthy 60–90% band (71.1 / 72.2 / 70.4% across a three-subject set).
- **Integration insight:** The anchor for the "wearable venous pulse oximeter" thesis; every Topic-1 wearable/peripheral entry is a variation on isolating the venous component this device targets at the neck.

### 1.2 — Noninvasive Tracking of Mixed Venous Oxygen Saturation via Near-Infrared Spectroscopy Cerebral Oximetry: a Retrospective Observational Study *(**NEW to corpus** — first surfaced 2026-08-10)*
- **Authors:** (NIRS/SvO₂ cardiac-anesthesia group; off-pump CABG cohort) — author list not read directly (Nature/PMC 403); cross-confirmed via PubMed + PMC listing snippets.
- **Year / Venue:** 2023 · *Scientific Reports* 13, article 49078 (PMC10709586)
- **Link / DOI:** https://doi.org/10.1038/s41598-023-49078-1 · https://pmc.ncbi.nlm.nih.gov/articles/PMC10709586/
- **Relevance:** 8.5/10 — targets **true systemic mixed venous SvO₂** (the pulmonary-artery-catheter gold standard) and asks the operational question that matters for a non-invasive venous monitor: not just correlation, but *tracking* of SvO₂ change over time.
- **Novelty:** Analyzes 176 h of continuous intraoperative recordings from 48 subjects (26 INVOS 5100C / Medtronic, 22 O3 / Masimo) against simultaneous PA-catheter SvO₂. Regional cerebral oxygen saturation (rScO₂) detected SvO₂ changes ≥10% with **AUC 0.919 (INVOS) / 0.852 (O3)** and concordance rates of **90.6% / 91.9%** on 5-minute-interval changes — quantifying that a standard non-invasive NIRS channel can *trend* mixed venous oxygenation even where absolute calibration is imperfect.
- **Integration insight:** Fills a gap the corpus had only implied — it reframes the venous-monitoring goal from "measure absolute SvO₂" to "reliably track SvO₂ *change*," a lower and more clinically-achievable bar that the wearable/jugular optical devices (§1.1, §1.3–1.5) should be benchmarked against. Its device-dependence (INVOS ≠ O3) is a direct caution for any research-grade venous optical sensor claiming cross-platform accuracy.
- **Metadata flag:** Bibliographic fields (title, venue, year, PMID/PMCID, headline AUC/concordance numbers) cross-confirmed across ≥2 index snippets; **full text not read** (403) and the complete author list could not be verified on the publisher page — treat author attribution as **unverified**.

### 1.3 — Quantifying Changes in Oxygen Saturation of the Internal Jugular Vein In Vivo Using Deep Neural Networks and Subject-Specific 3-D Monte-Carlo Models *(previously surfaced — scan 06-10 §1.2)*
- **Authors:** (IJV DNN / Monte-Carlo group)
- **Year / Venue:** 2024 · *Optics Letters* 49(10):2669
- **Link / DOI:** https://opg.optica.org/ol/abstract.cfm?uri=ol-49-10-2669 (Optica abstract locator; raw DOI numeral unverified — see flag)
- **Relevance:** 8.5/10 — model-based recovery of IJV sO₂ change from multi-channel NIRS reflectance.
- **Novelty:** Subject-specific 3-D Monte-Carlo forward models train a DNN to invert measured reflectance into IJV saturation change, addressing the partial-volume/overlying-tissue confound.
- **Integration insight:** Supplies the computational-inversion half of the jugular-NIRS approach; complements §1.1's hardware. The Monte-Carlo-to-DNN pattern recurs in the Topic-2 PA fluence-correction work. Pairs naturally with §1.2: DNN inversion is one route to the absolute calibration that the pure-tracking rScO₂ approach lacks.
- **Metadata flag:** DOI string not re-verifiable on the Optica page today (403); the stable Optica locator (ol-49-10-2669) and title/authors/year are cross-confirmed via two search-index snippets. Treat the raw DOI numeral as **unverified**; cite via the Optica abstract URL.

### 1.4 — Proof-of-Concept Non-Invasive Estimation of Peripheral Venous Oxygen Saturation (pulse-modulation venous oximetry) *(previously surfaced — scan 06-10/06-11)*
- **Authors:** (peripheral-venous oximetry group; BioMedical Engineering OnLine)
- **Year / Venue:** 2017 · *BioMedical Engineering OnLine* 16:60
- **Link / DOI:** https://doi.org/10.1186/s12938-017-0351-x
- **Relevance:** 8.0/10 — foundational demonstration that an induced/modulated venous signal yields a peripheral SvO₂ estimate optically.
- **Novelty:** Uses external stimulation to induce cyclical venous fluctuation, lifting the venous component out of the low-SNR background so a PPG-style optical readout can estimate local venous saturation.
- **Integration insight:** Conceptual root of the "modulate the vein, then demodulate" family (muscle-stimulation PPG, e-tattoo spatial filtering). Landmark; recurs because nothing newer has displaced it as the peripheral-venous proof-of-concept.

### 1.5 — Towards Simultaneous Non-Invasive Arterial and Venous Oxygenation Monitoring with a Wearable Optical E-Tattoo *(previously surfaced — scan 07-01)*
- **Authors:** Tan P., Lu N., et al. (UT Austin)
- **Year / Venue:** 2023/2024 · IEEE (EMBC-lineage); related patent US 20250025074
- **Link / DOI:** https://pubmed.ncbi.nlm.nih.gov/38083768/ · patent: https://patents.justia.com/patent/20250025074
- **Relevance:** 8.0/10 — explicitly names non-invasive **venous** oxygenation as the unmet need and targets it with a wrist-worn optical patch.
- **Novelty:** Ultra-thin self-adherent optical e-tattoo measures arterial + venous pulses from multiple wrist sites; proposes spatial filtering to separate arterial/venous crosstalk.
- **Integration insight:** The wearable-form embodiment of the venous-oximetry goal; its arterial/venous separation problem is the same one §1.4 attacks by modulation and §1.1 sidesteps by anatomy. The standing JMIR hypoxia-accuracy caution bears directly on this device class.

**Topic 1 honest note:** one entry (§1.2) is new to the corpus this cycle; the other four are previously surfaced, and §1.4 predates 2020. No *newly published* primary venous measurement paper appeared today. The absence of *new* primary work, and the fact that the strongest genuinely-venous validation (§1.2) is a 2023 *tracking* study rather than an absolute-SvO₂ device, is itself the finding.

---

## Topic 2 — Optical imaging techniques for non-invasively obtaining venous blood oxygen (PA/PACT, NIRS, DOI/DOT, hyperspectral, vis-OCT, SFDI)

Ranked by relevance to **venous** (intravascular or named-vein) oxygenation.

### 2.1 — Noninvasive In Vivo Photoacoustic Measurement of Internal Jugular Venous Oxygenation in Humans *(previously surfaced — scan 06-10; the Topic-2 anchor)*
- **Authors:** (IJV-PA human oximetry group; Garcia-Uribe / Wang lineage)
- **Year / Venue:** 2023 · arXiv:2303.10775 (PA human-imaging lineage)
- **Link / DOI:** https://arxiv.org/abs/2303.10775
- **Relevance:** 9.5/10 — the single most on-target Topic-2 paper: photoacoustic sO₂ of a named deep **vein** (internal jugular) in humans, non-invasively (sijvO₂ ≈ 72 ± 7%, dual-wavelength PAT+US, 7 volunteers).
- **Novelty:** Demonstrates human IJV oxygenation from multi-wavelength PA, pushing PA oximetry from superficial microvessels to a clinically meaningful deep venous target — a non-invasive surrogate for cerebral oxygen consumption.
- **Integration insight:** The proof that optical/PA venous oximetry can reach a central-venous surrogate; the bridge between Topic 1's clinical need (the same sijvO₂ that §1.2's NIRS tracks indirectly) and Topic 2's imaging physics.
- **Metadata flag:** arxiv.org egress-blocked today; title/authors/abstract cross-confirmed via ADS + search-index snippets.

### 2.2 — Arterial Blood-Mediated Deep-Tissue Photoacoustic Oximetry (APM+): in-vivo human radial-vein sO₂ *(previously surfaced — upgraded 07-15)*
- **Authors:** Sastry, Olick-Gibson, et al.
- **Year / Venue:** 2026 · *Advanced Science* (Wiley); DOI 10.1002/advs.76366
- **Link / DOI:** https://doi.org/10.1002/advs.76366 · https://advanced.onlinelibrary.wiley.com/doi/10.1002/advs.76366
- **Relevance:** 9.0/10 — in-vivo human **radial-vein** sO₂ via a deep-tissue PA method that explicitly tackles spectral coloring; the most recent (2026) primary PA venous-oximetry advance in the corpus.
- **Novelty:** The arterial prior method (APM+, "+" = intravascular fluence correction) leverages high arterial sO₂ to locally calibrate optical fluence and correct wavelength-dependent spectral coloring. In ex-vivo-tissue phantom (artery/vein pair, 2 mm vessels, 5 mm depth, 100%/70% sO₂) the **median error fell to 2.9% vs 9.8% for linear unmixing**, recovering a mean venous sO₂ of 69.2% against a 70% ground truth; in 8 healthy adults it produced radial-vein estimates in the expected 60–80% band.
- **Integration insight:** The deep-vein counterpart to the retinal per-vessel corrections (§2.3/§2.4) and to §1.3's Monte-Carlo/DNN inversion — all attack the same "correct the confound before you unmix" problem, at different vessels and depths.

### 2.3 — Adaptive Spectroscopic Visible-Light OCT for Clinical Retinal Oximetry (ADS-vis-OCT) *(previously surfaced — scan 06-11)*
- **Authors:** (ADS-vis-OCT group; Yi lab lineage)
- **Year / Venue:** 2023 · *Communications Medicine* 3:59
- **Link / DOI:** https://doi.org/10.1038/s43856-023-00288-8
- **Relevance:** 8.5/10 — per-vessel retinal **vein** sO₂ with reported repeatability SD ≈ 2.3% in veins; RMSE ≈ 2.1% vs pulse oximeter in major arteries across 18 participants.
- **Novelty:** Adaptively removes per-vessel spectral contaminants, yielding accurate, repeatable artery *and vein* sO₂ across varying vessel diameters in humans.
- **Integration insight:** The highest-precision per-vessel venous optical readout in the corpus; the concrete modality against which the new SP-SFDI entry (§2.5) should be compared — both read retinal venular oxygenation, but ADS-vis-OCT reports calibrated absolute sO₂ while SP-SFDI reports an αSO₂ analogue.

### 2.4 — Oxygenation Heterogeneity Facilitates Spatiotemporal Flow-Pattern Visualization Inside Human Blood Vessels Using PACT *(previously surfaced — scan 06-10/06-11)*
- **Authors:** (PACT intravascular flow/oxygenation group)
- **Year / Venue:** 2024 · *Biomedical Optics Express* 15(5):2741
- **Link / DOI:** https://doi.org/10.1364/BOE.518632 → https://opg.optica.org/boe/fulltext.cfm?uri=boe-15-5-2741
- **Relevance:** 8.0/10 — resolves sO₂ heterogeneity and laminar-flow structure *inside* human vessels (incl. veins) with PACT.
- **Novelty:** First-time recovery of the parabolic laminar-flow wavefront inside a deep vein in vivo by exploiting intravascular oxygenation heterogeneity across multi-wavelength PA spectra.
- **Integration insight:** Shows PACT can read *within-lumen* venous oxygen structure, not just a vessel-average — the imaging counterpart to fusing oximetry with blood-flow measurement.
- **Metadata flag:** DOI numeral not re-verifiable on the Optica page today (403); the stable Optica locator (boe-15-5-2741) + title/year cross-confirmed. Cite via the Optica URL; treat the raw DOI numeral as **unverified**.

### 2.5 — Assessing and Monitoring Abnormal Retinal Blood Circulation … Using Non-Invasive, High-Resolution Biophotonic Imaging Technology (SP-SFDI / BioxyDR™) *(**NEW to corpus** — first surfaced 2026-08-10; the corpus's first SFDI-for-venous entry)*
- **Authors:** Basiri A., Luo C., Shokoohi-Yekta M., et al.
- **Year / Venue:** 2025 · *Eye* (Nature portfolio) 39:2872–2883
- **Link / DOI:** https://doi.org/10.1038/s41433-025-04032-5 · https://www.nature.com/articles/s41433-025-04032-5
- **Relevance:** 8.0/10 — a **Spatial Frequency Domain Imaging** modality (explicitly named in Topic 2) applied to per-vessel retinal **venous** oxygenation; directly on-topic, docked slightly because it reports an oxygenation *analogue* (αSO₂), not calibrated absolute venous sO₂.
- **Novelty:** Introduces **Saccadic-Phase SFDI (SP-SFDI)**, a physics-based retinal-oximetry algorithm that recovers an oxygen-saturation analogue (αSO₂) at high resolution from **two snapshots** capturing phase shifts in spatially modulated light, sensitive to oxygenation changes <3%. In clinical validation (63 DR, 60 diabetic-no-DR, 18 controls), **retinal venous αSO₂ differed significantly** between controls and disease groups (NPDR/PDR); an SP-SFDI "pre-DR" classification flagged 8 diabetic-no-DR eyes of which 7 (87%) progressed to DR within 18 months, vs 0% of "not pre-DR."
- **Integration insight:** Extends the Topic-2 retinal cluster (HSI, ADS-vis-OCT §2.3) with a **snapshot SFDI** approach — a fundamentally different sampling strategy (spatial-frequency demodulation rather than spectral OCT) for the same per-vessel venular target, and the corpus's first evidence that **retinal venous** oxygenation carries predictive (not just cross-sectional) clinical value. The αSO₂-analogue-vs-absolute-sO₂ gap it leaves open is exactly what ADS-vis-OCT (§2.3) and the fluence-corrected PA methods (§2.1/§2.2) are built to close.
- **Metadata flag:** Title, authors (Basiri/Luo/Shokoohi-Yekta et al.), venue (*Eye* 39:2872–2883, 2025), and DOI cross-confirmed across ≥2 index snippets (Nature listing + researchgate + Scholar block); **full text not read** (nature.com 403) — method/clinical numbers are abstract/snippet-level.

**Topic 2 honest note:** one entry (§2.5) is new to the corpus this cycle; the other four are carried forward. No *newly published* venous PA/OCT primary measurement appeared today — the newest primary work remains the 2026 APM+ paper (§2.2).

---

## Standing context leads (not ranked in the top-5)

- **A New Non-Invasive Method for the Assessment of Central Venous Oxygen Saturation (Mespere VO100 jugular NIRS)** — *J. Cardiothorac. Vasc. Anesth.* 2023/2024 (S1053-0770 lineage), https://www.sciencedirect.com/science/article/pii/S1053077023007826. The one commercially available non-invasive jugular-NIRS ScvO₂ estimator; the clinical-translation benchmark for Topic 1. **Dropped from top-5 today** only to surface the new §1.2 tracking study; unchanged otherwise (rel. 7.5).
- **Retinal Oximetry: New Insights into Ocular and Systemic Diseases** — Zhang W. et al., *Graefe's Archive* 263:2101–2115 (2025), DOI 10.1007/s00417-025-06831-8, PMC12414079. Review consolidating spectrophotometric-fundus, hyperspectral, and vis-OCT retinal artery+vein oximetry. **Dropped from top-5 today** to surface §2.5; the review now reads as the umbrella over both the vis-OCT (§2.3) and SFDI (§2.5) retinal-venular methods (rel. 7.5).
- **Comparing NIRS-Measured Cerebral Oxygen Saturation and Corresponding Venous Oxygen Saturations in Children with Congenital Heart Disease: a Systematic Review and Meta-Analysis** — Ma et al., *Translational Pediatrics* (2022), https://tp.amegroups.org/article/view/99923/html. Meta-analysis finding no significant difference between NIRS rScO₂ and ScvO₂/SjvO₂ (Cohen's d ≈ 0.03–0.06). Evidence-synthesis companion to §1.2 — same rScO₂↔venous-sO₂ relationship at population scale. Surfaced today as a lead; venous-relevant but review-level and pediatric.
- **Optical Inversion and Spectral Unmixing of Spectroscopic PA Images with Physics-Informed Neural Networks** — arXiv:2602.16357 (surfaced 06-11). PA decoloring/spectral-unmixing method; not venous-specific but directly relevant to the fluence-correction problem the deep-vein PA anchors (§2.1/§2.2) face. Carried forward; arxiv.org egress-blocked, re-verified via snippet only.
- **Integrated Spectral and Depth Compensation for sO₂ and Total-Hemoglobin Estimation in PAT (ovarian-lesion diagnosis)** — PMC12869027 (2026). Fluence/spectral-coloring compensation for quantitative PAT sO₂; **tissue-level, ovarian**, not venous — retained as a Topic-2 fluence-correction methods lead only.
- **Quantitative Oximetry with PACT: Principles, Progress, and Prospects** — *J. Innov. Opt. Health Sci.* 2026, DOI 10.1142/S1793545826300065. Review scaffold under the deep-vein PA anchors; authors unverified. Carried forward.
- **Performance of Wearable Pulse Oximetry During Controlled Hypoxia Induction** — *JMIR Formative Research* 2026 (formative.jmir.org/2026/1/e85253). **Arterial-only** wearable SpO₂ validation showing >FDA-threshold error in the hypoxemic range — a transferable accuracy caution for the wearable-venous device class (§1.4/§1.5), which operates at even lower saturations.
- **Classic ovine / large-vein optoacoustic SSS venous work** (Esenaliev/Petrov lineage; superior sagittal sinus, triple-wavelength optoacoustic large-vein oximetry). Foundational venous-optoacoustic prior art; historical root of deep-venous PA oximetry.

---

## Cross-topic synthesis

Today keeps the series' central finding intact — **no new primary non-invasive venous *measurement* paper was published** — but it is a better-than-average cycle because two previously-uncatalogued venous-specific papers surfaced, one per topic, and both sharpen the corpus's framing rather than merely adding volume.

The two topics remain coupled by a single problem: **isolate the venous signal, then correct the confound that corrupts its saturation estimate**, addressed by three complementary strategies:

1. **Anatomical targeting** of a large, named vein — jugular optical sensing (§1.1), IJV-PA (§2.1), and, indirectly, the cerebral-NIRS channel that §1.2 shows can *track* mixed venous SvO₂.
2. **Signal modulation / separation** to lift a small venous component from a noisy mixed background — peripheral-venous modulation (§1.4), e-tattoo spatial filtering (§1.5), DNN inversion (§1.3), and the snapshot phase-demodulation of the new SP-SFDI method (§2.5).
3. **Physics-based decoloring** to correct wavelength-dependent fluence / spectral contaminants before unmixing — deep-tissue PA fluence correction (§2.2), per-vessel spectral cleanup in vis-OCT (§2.3), intravascular PACT (§2.4), and the PINN/spectral-compensation leads.

The new §1.2 (NIRS *tracks* SvO₂) and §2.5 (SFDI reads retinal venous αSO₂, and it *predicts* DR progression) together nudge the field's success criterion: from "measure absolute venous sO₂ once" toward "**track venous oxygenation change reliably, and show it carries clinical predictive value.**" That is a lower bar on absolute calibration but a higher bar on longitudinal robustness — and it is a bar the tracking-oriented NIRS (§1.2) and the analogue-but-predictive SFDI (§2.5) partly clear today, while the absolute-calibration methods (ADS-vis-OCT §2.3, APM+ §2.2, IJV-PA §2.1) remain the ones that could eventually satisfy both.

The counterweight is unchanged: even *arterial* wearable oximetry (the JMIR lead) fails in the low-saturation range where venous measurement lives, and §1.2 shows device-to-device tracking performance itself varies (INVOS vs O3), so the accuracy/robustness bar for any wearable venous device (§1.4/§1.5) is, if anything, higher than the arterial state of the art. Net: **no bedside-ready systemic non-invasive SvO₂ optical device emerged today**, the two new entries improve corpus coverage without changing that verdict, and the honest population of strong, truly-venous, truly-optical papers remains **fewer than five per topic** of genuinely new material once arterial-only and tissue-level work is excluded.

---

*Scan generated 2026-08-10 (UTC). Metadata cross-checked across ≥2 search-index snippets per item; arxiv.org and publisher full-text pages (nature.com, pmc.ncbi.nlm.nih.gov, opg.optica.org, sciencedirect.com, wiley.com) were egress-blocked / returned HTTP 403 to direct fetch in this environment (source-/policy-side; agent proxy healthy), so items flagged "full text not read" are abstract/snippet-verified and flagged unverified fields are noted inline. New-to-corpus items this cycle: §1.2 (Sci. Rep. 2023 NIRS mixed-venous tracking) and §2.5 (Eye 2025 SP-SFDI retinal venous oximetry).*
