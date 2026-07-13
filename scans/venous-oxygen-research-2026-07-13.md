# Venous Oxygen Research Scan — 2026-07-13

**Search window:** Twenty-third scan in the series, run **one day** after 2026-07-12. Emphasis on work published or first-surfacing after 07-12, with the standard fallback to the best-available venous-specific work already catalogued. Sources searched today: PubMed/PMC, arXiv, bioRxiv/medRxiv, Optica (Biomed. Opt. Express, Optics Letters, Applied Optics), SPIE / *J. Biomed. Opt.*, *Photoacoustics* (ScienceDirect), IEEE Xplore, Nature / *Sci. Rep.* / *Nat. Biomed. Eng.*, Wiley (*Advanced Science*), MDPI (*Biosensors*), IOPscience, Springer, De Gruyter, World Scientific (*JIOHS*), ClinicalTrials.gov, ResearchGate, Semantic Scholar.

**Verification caveat:** As in every prior scan, publisher **full-text** pages — including arxiv.org, opg.optica.org, pmc.ncbi.nlm.nih.gov, sciencedirect.com, medrxiv.org and the Wiley/Nature domains — returned **HTTP 403** to direct `WebFetch` in this environment today (re-confirmed on PMC12384115 and medrxiv.org/…v1.full). Every reference below was therefore cross-checked across **at least two independent search-index snippets**; per-item notes state what was confirmed and what could not be read directly on a publisher page.

---

## ⚠️ Read this first — day summary

**One genuinely new item today; no new venous-specific *optical* work.** Today's sweep surfaced exactly **one** paper first-appearing since the last scan:

- **NEW (Topic 1):** *Leveraging Self-Supervised Learning for Non-Invasive Intra-Cardiac Magnetic Resonance Oximetry Assessment* (Chen et al., medRxiv, posted **2026-07-01**). This is an **MRI** method (T2 oximetry + cine CMR), **not optical** — but it is squarely on-topic for non-invasive **mixed/intra-cardiac venous** O₂ estimation, so it leads Topic 1 with an honest note about modality.

Everything else returned by today's searches is **previously surfaced** (jugular optical sensing, DNN+Monte-Carlo SijvO₂, PACT flow visualization, vis-OCT retinal oximetry, APM+ arterial-transferable photoacoustics, etc.). Consistent with the series' standing observation, **truly novel non-invasive venous-optical work is published at very low volume**; today reinforces that. The Topic-2 list below is therefore the best-available standing set, each item honestly flagged as previously surfaced with its relevance score unchanged.

---

## Topic 1 — Non-invasive monitoring of venous blood oxygen (SvO₂ / ScvO₂ / peripheral venous)

### 1.1 — ★ NEW — Leveraging Self-Supervised Learning for Non-Invasive Intra-Cardiac Magnetic Resonance Oximetry Assessment
- **Authors:** Jiayuan Chen, Thai-Hoang Pham, Ping Zhang, Juliet Varghese
- **Year:** 2026 (preprint posted **2026-07-01**)
- **Venue:** medRxiv (preprint, not yet peer-reviewed)
- **Link / DOI:** https://www.medrxiv.org/content/10.64898/2026.06.29.26356860v1.full — DOI `10.64898/2026.06.29.26356860`
- **Relevance:** **7/10** for non-invasive venous O₂; **3/10** for the *optical-imaging* thrust of Topic 2 (it is MRI, not optical).
- **Novelty:** A unified **self-supervised learning** framework that jointly ingests cine CMR and **T2-oximetry CMR**, pre-training ResNet and ViT encoders via contrastive learning + masked image modeling on **>48,000 cardiac images**, then fine-tuning for **O₂-saturation regression with uncertainty quantification**. Reported **MAE ≈ 3.70** (SimCLR-pretrained ResNet), a claimed **>15%** improvement over radiomics/supervised baselines. Uncertainty quantification is the standout: it gives a per-estimate confidence, which is exactly what clinical venous-O₂ trend monitoring needs.
- **Integration insights:** T2 CMR oximetry recovers **chamber-level (intra-cardiac) blood O₂ saturation**, i.e. true mixed-venous (RA/RV/PA) SvO₂ — the same physiological quantity that jugular/peripheral optical methods chase, but here as a non-invasive **reference-grade** modality. Its label-scarce SSL + uncertainty recipe is **directly portable** to the optical side of this program, where labelled in-vivo SvO₂ ground truth is the binding constraint (see the recurring DNN+Monte-Carlo jugular work in 1.3). Value as a **cross-modality validation target** and as a transferable ML methodology, not as an optical device. *Metadata (title, authors, date, DOI) confirmed across two independent search snippets; abstract not readable directly (medRxiv 403).*

### 1.2 — Estimation of Venous Oxygen Saturation Through Non-Invasive Optical Sensing at the Jugular Veins *(previously surfaced — scan 06-10 §1.1; the flagship optical-venous device paper)*
- **Authors:** (De Gruyter CDBME 2024 proceedings — jugular optical-sensing group)
- **Year:** 2024
- **Venue:** *Current Directions in Biomedical Engineering* (De Gruyter), CDBME
- **Link / DOI:** https://www.degruyterbrill.com/document/doi/10.1515/cdbme-2024-2072/html — DOI `10.1515/cdbme-2024-2072`
- **Relevance:** **9/10** — direct, non-invasive, optical, venous.
- **Novelty:** Pulse-oximeter-style optical sensor at the **external jugular vein (EJV)**; identifies the EJV waveform and returns SvO₂ estimates in the healthy 60–90% band (reported ~70–75% across small cohorts). Still the closest thing to a wearable-form-factor optical SvO₂ device in the literature.
- **Integration insights:** The reference architecture for peripheral optical SvO₂. Its open problem — calibration/validation against blood-gas gold standard — is precisely the gap that 1.1's SSL + uncertainty approach and reference-grade MRI could help close.

### 1.3 — Quantifying Changes in Oxygen Saturation of the Internal Jugular Vein In Vivo Using Deep Neural Networks and Subject-Specific 3-D Monte-Carlo Models *(previously surfaced — scan 06-10 §1.2)*
- **Year:** 2024
- **Venue:** *Optics Letters* 49(10):2669
- **Link / DOI:** https://opg.optica.org/ol/abstract.cfm?uri=ol-49-10-2669
- **Relevance:** **8/10** — non-invasive optical, internal-jugular, SijvO₂.
- **Novelty:** Models reflectance→ΔSijvO₂ with **subject-specific 3-D Monte-Carlo** forward simulation, then trains a **DNN** to invert it — sidestepping the labelled-data bottleneck via simulation.
- **Integration insights:** The simulation-to-DNN pattern is the methodological twin of 1.1's SSL approach; both attack the "no in-vivo venous labels" problem from different directions (physics-simulation vs. self-supervision). A natural pairing.

### 1.4 — Development and Validation of a Noninvasive Model of Mixed Venous Oxygen Saturation in Heart Failure *(previously surfaced — scan 07-07 §1.1)*
- **Year:** 2025
- **Venue:** cardiology / heart-failure literature (model-based SvO₂)
- **Relevance:** **7/10** — mixed-venous, non-invasive, clinically validated; not optical.
- **Novelty:** A validated **model-based** SvO₂ estimator for heart-failure populations, giving a clinical-grade non-invasive surrogate without a catheter.
- **Integration insights:** Provides the **clinical target range and validation framing** (HF cohorts) against which optical SvO₂ devices should ultimately be benchmarked. Complements 1.1's MRI reference on the clinical-outcomes axis.

### 1.5 — Non-invasively Measured Venous Oxygen Saturation as Early Marker of Impaired Oxygen Delivery in Preterm Neonates *(previously surfaced — catalogued in prior scans)*
- **Venue:** *Frontiers* / PMC (PMC8831784)
- **Link:** https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8831784/
- **Relevance:** **7/10** — NIRS venous-occlusion SvO₂ in a real patient population.
- **Novelty:** Uses NIRS-based non-invasive SvO₂ as an **early physiological marker** of impaired O₂ delivery in preterm neonates — a concrete clinical use-case for continuous venous-O₂ trending.
- **Integration insights:** Establishes clinical value (neonatal ICU) and the venous-occlusion NIRS technique that a wearable optical SvO₂ device would operationalize.

**Topic-1 honesty note:** Only **1.1** is new this cycle, and it is MRI rather than optical. No new non-invasive *optical* venous-O₂ paper appeared today.

---

## Topic 2 — Optical imaging techniques for non-invasive venous blood oxygen

*No new items today.* The standing best-available set (all previously surfaced) with unchanged scores:

### 2.1 — Noninvasive In Vivo Photoacoustic Measurement of Internal Jugular Venous Oxygenation in Humans *(previously surfaced — flagship, scan 06-10 §2.1)*
- **Year:** 2023 (arXiv 2303.10775)
- **Venue:** arXiv preprint (WashU group)
- **Link:** https://arxiv.org/abs/2303.10775
- **Relevance:** **10/10** — the single most on-target paper in the corpus: non-invasive, in-vivo, human, **internal-jugular venous** sO₂ by photoacoustics (reported ~72 ± 7%).
- **Novelty:** Demonstrates label-free PA quantification of true venous sO₂ in a named deep vein in humans, with arterial-admixture-free specificity.
- **Integration insights:** The optical-imaging anchor of the entire program. Everything in Topic 2 is measured against whether it can reach this depth/specificity non-invasively.

### 2.2 — Oxygenation Heterogeneity Facilitates Spatiotemporal Flow-Pattern Visualization Inside Human Blood Vessels Using Photoacoustic Computed Tomography *(previously surfaced)*
- **Year:** 2024 (PMC11161372)
- **Link:** https://pmc.ncbi.nlm.nih.gov/articles/PMC11161372/
- **Relevance:** **8/10** — recovers, in real time, the **parabolic laminar-flow wavefront inside a deep human vein in vivo** via multi-wavelength PA spectra.
- **Novelty:** First real-time in-vivo laminar-flow-profile recovery inside a deep vein; couples oxygenation contrast to flow dynamics.
- **Integration insights:** Extends venous PA from static sO₂ to **flow + oxygenation jointly**, informing venous-return and O₂-delivery physiology beyond a scalar SvO₂.

### 2.3 — Adaptive Spectroscopic Visible-Light OCT for Clinical Retinal Oximetry *(previously surfaced — scan 06-11 §2.2)*
- **Year:** 2023
- **Venue:** *Communications Medicine* (Nature)
- **Link:** https://www.nature.com/articles/s43856-023-00288-8
- **Relevance:** **8/10** — resolves **retinal vein** sO₂ at single-vessel scale (venous ~48% vs arterial ~92% in normals); ADS-vis-OCT removes per-vessel spectral contaminants.
- **Novelty:** ~1% bias vs blood-gas in phantoms (0–100%); ~2.1% RMSE vs pulse oximeter in human arteries; validated pathway to CRVO/DR/glaucoma.
- **Integration insights:** The most clinically mature **vessel-resolved venous** optical oximetry; the retinal vein is the accessible testbed for single-vessel venous sO₂.

### 2.4 — Arterial Blood-Mediated Deep-Tissue Photoacoustic Oximetry (APM+) *(previously surfaced — scan 07-05 §2.5; arterial-demonstrated, included under the transferable-technique clause)*
- **Authors:** Sastry et al.
- **Year:** 2026
- **Venue:** *Advanced Science* (Wiley)
- **Link / DOI:** https://advanced.onlinelibrary.wiley.com/doi/10.1002/advs.76366 — DOI `10.1002/advs.76366`
- **Relevance:** **7/10** — arterial-demonstrated but **directly transferable to venous**: uses a known-high arterial sO₂ as a local **fluence calibrator** to defeat spectral coloring, then estimates nearby-tissue sO₂ (median error **2.9%** vs **9.8%** linear unmixing).
- **Novelty:** Turns the arterial prior into an in-situ fluence reference — the core obstacle for **quantitative deep venous** PA oximetry.
- **Integration insights:** If an artery can calibrate fluence for a neighbouring region, the **same calibration should sharpen the adjacent vein's sO₂** — the most promising near-term route to quantitative deep-venous PACT.

### 2.5 — Non-Invasive Photoacoustic Imaging of Cerebral Oxygenation and Hemoglobin Content in Awake Mice *(previously surfaced — bioRxiv preprint, transferable technique)*
- **Year:** 2025 (bioRxiv, posted 2025-10-02)
- **Link:** https://www.biorxiv.org/content/10.1101/2025.10.02.679935v1.full
- **Relevance:** **6/10** — through-intact-skull PA sO₂ + tHb; cerebral (mixed vascular) rather than a named vein, but the **transcranial, label-free, awake** capability is directly relevant to non-invasive cerebral **venous** (e.g. sagittal-sinus) oximetry.
- **Novelty:** Longitudinal awake-animal PA oxygenation through intact skull — removes anesthesia confounds on hemodynamics.
- **Integration insights:** Complements the cerebral-venous PA validation lineage (sagittal-sinus piglet work); a translational stepping-stone toward non-invasive cerebral venous O₂ in humans.

**Topic-2 honesty note:** **No new optical venous-O₂ paper appeared today.** The list is the best-available standing set; each item is previously surfaced with its score carried forward unchanged.

---

## Cross-topic synthesis

1. **The binding constraint is labelled in-vivo venous ground truth, and today's one new paper attacks exactly that.** Chen et al. (1.1) bring **self-supervised pretraining + uncertainty quantification** to non-invasive oximetry — the same label-scarcity problem the optical jugular DNN work (1.3) solves with Monte-Carlo simulation. The two paradigms (self-supervision vs. physics-simulation) are complementary and both are portable to optical SvO₂. This is the clearest cross-modality methodology transfer surfaced this week, even though the paper itself is MRI.

2. **MRI is emerging as the non-invasive reference standard for the optical program.** T2/intra-cardiac CMR oximetry (1.1) measures true mixed-venous SvO₂ non-invasively and reference-grade — it is a natural **validation target** for the jugular optical sensor (1.2) and deep-venous PACT (2.1–2.2), which chronically lack a non-invasive gold standard.

3. **The fluence-calibration problem (Topic 2) and the label problem (Topic 1) are the two walls.** APM+ (2.4) shows an arterial prior can calibrate optical fluence to reach quantitative deep-tissue sO₂; applying that same calibration to the adjacent vein is the most concrete near-term path to quantitative deep **venous** photoacoustic oximetry.

4. **Sparseness confirmed, not padded.** Across full sweeps of PubMed, arXiv, bioRxiv/medRxiv, Optica, SPIE, Wiley, Nature and MDPI, only **one** item post-dated the last scan, and it is MRI. Genuinely novel non-invasive **venous-optical** work remains rare; today produced none. The strongest venous-optical results (2.1 jugular PA; 2.3 retinal-vein vis-OCT; 2.2 PACT venous flow) continue to be the anchors, and no newer work displaces them.

**Open gaps (carried forward, still open):** (a) no continuous, calibrated, wearable optical SvO₂ device validated against blood-gas; (b) no quantitative deep-venous PA sO₂ with an in-situ fluence reference in humans; (c) no non-invasive optical SvO₂ method benchmarked head-to-head against reference CMR oximetry — a study the emergence of 1.1 now makes feasible.
