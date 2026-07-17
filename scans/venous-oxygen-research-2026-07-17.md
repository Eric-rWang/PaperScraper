# Venous Oxygen Research Scan — 2026-07-17

**Search window:** Twenty-fifth scan in the series, run **two days** after 2026-07-15 (no scan on 07-16). Emphasis on work published or first-surfacing after 07-15, with the standard fallback to the best-available venous-specific work already catalogued. Sources searched today: PubMed/PMC, arXiv, bioRxiv/medRxiv, Optica (Biomed. Opt. Express, Optics Letters, Applied Optics), SPIE / *J. Biomed. Opt.*, *Photoacoustics* (ScienceDirect), IEEE Xplore, Nature / *Sci. Rep.* / *Eye*, Wiley (*Advanced Science*, *J. Biophotonics*), MDPI, Springer, De Gruyter, ClinicalTrials.gov, ResearchGate, Semantic Scholar, ADS.

**Verification caveat:** As in every prior scan, publisher **full-text** pages — including arxiv.org, pmc.ncbi.nlm.nih.gov, opg.optica.org, advanced.onlinelibrary.wiley.com and the Nature/Eye domains — returned **HTTP 403** to direct `WebFetch` in this environment today (re-confirmed on arXiv `2512.15394`, `2602.00283`). Every reference below was therefore cross-checked across **at least two independent search-index snippets** (Google Scholar-style result blocks + ADS/ResearchGate/PMC listings); per-item notes state what was confirmed and what could not be read directly on a publisher page.

---

## ⚠️ Read this first — day summary

**No new venous-specific *primary* paper today.** Consistent with the series' standing observation, truly novel non-invasive **venous**-optical work is published at very low volume, and today's sweep produced no new SvO₂/ScvO₂ demonstration. However, the sweep did surface **two genuinely new technique/methodology preprints** — not in any prior scan file — that sit on the **optical/photoacoustic** side (Topic 2) and are **transferable** to the venous-oximetry inverse problem:

- **NEW — APRECOT** (arXiv:2606.16835, June 2026, Ntziachristos/Jüstel group, TU Munich/iThera): anatomical-prior-conditioned reconstruction of **MSOT** images that jointly segments tissue and recovers **bulk chromophore (oxygenation) composition** — a direct attack on the ill-posed fluence problem that limits quantitative PA venous sO₂.
- **NEW — Novel Differential Pathlength Factor (DPF) model** (arXiv:2602.00283, submitted 2026-01-30): Monte-Carlo-derived, distance- and property-dependent DPF models that reduce modified-Beer-Lambert errors in **continuous-wave NIR diffuse optical imaging** — the quantitative foundation under every transcutaneous-NIRS jugular/peripheral venous method in this catalogue.

Both are **tissue/technique-level**, not true SvO₂, and are scored accordingly. Everything else returned by the sweep is **previously surfaced** or out-of-scope: the Alqahtani jugular optical sensor (De Gruyter CDBME), the IJV DNN + Monte-Carlo work (Optics Letters), Mespere VO100 jugular NIRS, the McDiarmid MRI iSvO₂ model, the SSL intra-cardiac MR oximetry preprint, the IJV-PA anchor, APM+ (radial-vein sO₂ in humans), PACT venous-flow work, vis-OCT / hyperspectral retinal oximetry, Hybrid-Net (arXiv:2512.15394, Dec 2025, already surfaced), and the sulfate-phantom paper. No new primary venous demonstration — only new **transferable machinery**.

---

## Topic 1 — Non-invasive monitoring of venous blood oxygen (SvO₂ / ScvO₂ / peripheral venous)

*No new items today.* The standing best-available set (all previously surfaced) with scores carried forward. This topic remains the sparse one: no primary non-invasive venous-O₂ measurement paper first-surfaced since 2026-07-15.

### 1.1 — Estimation of Venous Oxygen Saturation Through Non-Invasive Optical Sensing at the Jugular Veins *(previously surfaced — scan 06-10 §1.1; flagship optical-venous device paper)*
- **Authors:** Alqahtani et al.
- **Year / Venue:** 2024 · *Current Directions in Biomedical Engineering* 10(2) (De Gruyter; CDBME-2024-2072)
- **Link / DOI:** https://doi.org/10.1515/cdbme-2024-2072
- **Relevance:** **8/10** — true, non-invasive, optical, venous (but n=3, no invasive co-oximetry reference).
- **Novelty:** A pulse-oximeter-style optical sensor over the external jugular vein isolates the EJV waveform and returns SvO₂ estimates (~70–72 %) within the healthy 60–90 % band — still the closest thing to a wearable-form-factor optical SvO₂ device in the literature.
- **Integration insights:** The superficial/low-cost optical analogue of the deep IJV-PA anchor (§2.1); together they bracket the venous-optical problem from the shallow and deep ends. Its open problem — calibration against a blood-gas gold standard — is exactly what the APM+ artery-as-reference approach (§2.2) and MRI reference oximetry (§1.4) aim to close. *Metadata cross-confirmed via De Gruyter listing + ResearchGate; full text 403 (flagged).*

### 1.2 — Quantifying Changes in Oxygen Saturation of the Internal Jugular Vein In Vivo Using Deep Neural Networks and Subject-Specific 3-D Monte-Carlo Models *(previously surfaced — scan 06-10 §1.2)*
- **Authors:** (multi-author; NIRS + DNN group)
- **Year / Venue:** 2024 · *Optics Letters* 49(10):2669
- **Link / DOI:** https://opg.optica.org/ol/abstract.cfm?uri=ol-49-10-2669
- **Relevance:** **7/10** — IJV-specific, non-invasive, inverse-modeling for venous saturation *change*.
- **Novelty:** Multi-channel NIRS + DNNs trained on subject-specific 3-D Monte-Carlo forward models recover ΔSijvO₂ non-invasively, tying measured reflectance to a physically-modelled forward problem — sidestepping the labelled-data bottleneck via simulation.
- **Integration insights:** The inverse-modeling / fluence-correction leg of the program; the physics-simulation twin of the self-supervised-learning approach in §1.3. **Directly touched by today's NEW DPF-model preprint (§2.5):** the accuracy of this DNN-on-Monte-Carlo pipeline is bounded by the pathlength/fluence assumptions the DPF paper reformulates. *Cross-confirmed via Optica listing + Semantic Scholar; full text 403 (flagged).*

### 1.3 — Leveraging Self-Supervised Learning for Non-Invasive Intra-Cardiac Magnetic Resonance Oximetry Assessment *(previously surfaced — scan 07-13 §1.1; MRI, not optical)*
- **Authors:** Jiayuan Chen, Thai-Hoang Pham, Ping Zhang, Juliet Varghese
- **Year / Venue:** 2026 (preprint posted 2026-07-01) · medRxiv
- **Link / DOI:** https://www.medrxiv.org/content/10.64898/2026.06.29.26356860v1.full — DOI `10.64898/2026.06.29.26356860`
- **Relevance:** **7/10** for non-invasive venous O₂; **3/10** for the optical thrust of Topic 2 (MRI, not optical).
- **Novelty:** Self-supervised pre-training (contrastive + masked image modeling) on >48,000 cardiac images, then fine-tuning for O₂-saturation regression **with uncertainty quantification** (MAE ≈ 3.70; claimed >15 % improvement over baselines). Recovers chamber-level (intra-cardiac) blood O₂ — true mixed-venous SvO₂ — non-invasively and reference-grade.
- **Integration insights:** The label-scarce SSL + uncertainty recipe is **directly portable** to the optical side, where labelled in-vivo SvO₂ ground truth is the binding constraint (cf. §1.2). Value as a cross-modality **validation target** and transferable ML methodology. *Metadata confirmed across two search snippets; abstract not readable (medRxiv 403).*

### 1.4 — Development and Validation of a Noninvasive Model of Mixed Venous Oxygen Saturation in Heart Failure (imaging-derived iSvO₂) *(previously surfaced — scan 07-07 §1.1)*
- **Authors:** McDiarmid et al.
- **Year / Venue:** 2025/2026 · *JACC: Advances*
- **Link / DOI:** https://doi.org/10.1016/j.jacadv.2025.102484 · PMC12869880 · PMID 41609283
- **Relevance:** **7/10** — true mixed-venous, non-invasive, clinically validated (MRI, not optical).
- **Novelty:** 628-patient validation of an imaging-derived mixed-venous SvO₂ from the RV/LV blood-pool T₂ ratio on cardiac MRI (R = 0.82 vs invasive SvO₂), anchored to right-heart catheterization and an independent predictor of mortality/HF-hospitalization.
- **Integration insights:** Sets the **absolute-accuracy and outcome-relevance benchmark** any optical SvO₂ method must match, in exactly the population (heart failure) where a cheap continuous optical surrogate would be most valuable. Its internal-reference (RV vs LV) logic recurs on the optical side as artery-vs-vein calibration (§2.2). *Cross-confirmed via JACC/ScienceDirect + PMC + PubMed; full text 403 (flagged).*

### 1.5 — A New Non-Invasive Method for the Assessment of Central Venous Oxygen Saturation (Mespere VO100 jugular NIRS) *(previously surfaced — scan 06-10 §1.3)*
- **Authors:** (critical-care cohort study)
- **Year / Venue:** 2023 · *J. Cardiothoracic and Vascular Anesthesia* (S1053-0770(23)00782-6)
- **Link / DOI:** https://www.sciencedirect.com/science/article/pii/S1053077023007826 · PMID 37827917
- **Relevance:** **7/10** — non-invasive NIRS surrogate for ScvO₂, clinical cohort.
- **Novelty:** Validates transcutaneous jugular NIRS (Mespere VO100) against invasive ScvO₂ in critically ill patients, reporting strong linear correlation with low bias/percentage error.
- **Integration insights:** The most clinically-mature non-invasive venous-NIRS device line — the practical baseline on bias and limits-of-agreement any optical/PA method must beat. **Its accuracy floor is set by exactly the CW-NIRS pathlength assumptions the NEW DPF model (§2.5) targets.** *Cross-confirmed via ScienceDirect + PubMed 37827917; full text 403 (flagged).*

**Standing context (not scored in the top-5):** jugular transcutaneous NIRS in pediatric cardiac surgery (r = 0.91 vs ScvO₂, bias 2.92 %; PMC7491293), respiration-frequency-selected NIRS for cerebral SvO₂ (PMC4126245 / PMID 24439329), capnodynamic mixed-venous SvO₂ (NCT06632197; PMID 34609659), and the preterm-neonate NIRS venous-occlusion series — all previously catalogued, none updated this cycle.

---

## Topic 2 — Optical imaging techniques for non-invasively obtaining venous blood oxygen (PA/PACT, NIRS, DOI/DOT, hyperspectral, vis-OCT, SFDI)

Two **new** transferable-technique preprints this cycle (§2.4, §2.5), slotted below the standing venous-specific anchors.

### 2.1 — Noninvasive In Vivo Photoacoustic Measurement of Internal Jugular Venous Oxygenation in Humans *(previously surfaced — scan 06-10 §2.1; the Topic-2 anchor)*
- **Authors:** (PA/US group; arXiv:2303.10775)
- **Year / Venue:** 2023 · arXiv preprint / SPIE lineage (cf. 2014 SPIE 8943E..1MG)
- **Link / DOI:** https://arxiv.org/abs/2303.10775
- **Relevance:** **9/10** — true, non-invasive, optical/PA, deep **named-vein** (IJV) sO₂ in humans. The single most on-target paper in the corpus.
- **Novelty:** Combined photoacoustic + ultrasound imaging computes hemoglobin sO₂ of the internal jugular vein in vivo, non-invasively, in real time — the reference demonstration that deep venous PA oximetry is physically achievable in humans.
- **Integration insights:** The deep-vein anchor that everything else is measured against; APM+ (§2.2), APRECOT (§2.4), and the DPF model (§2.5) are all, in different ways, attempts to make this kind of measurement quantitative and fluence-robust without an ultrasound co-registration crutch. *Metadata cross-confirmed via arXiv + ADS; full text 403 (flagged).*

### 2.2 — Arterial Blood-Mediated Deep-Tissue Photoacoustic Oximetry (APM+): in-vivo human radial-vein sO₂ *(previously surfaced — upgraded 07-15 §2.2)*
- **Authors:** Sastry et al.
- **Year / Venue:** 2026 · *Advanced Science* (Wiley)
- **Link / DOI:** https://doi.org/10.1002/advs.76366
- **Relevance:** **8/10** — a bona-fide non-invasive optical/PA venous-oximetry demonstration in humans (radial-vein median sO₂ 72.3 %, IQR 8.9 %, n=8 healthy adults).
- **Novelty:** Uses the neighbouring radial **artery** as an in-situ fluence calibrator to circumvent spectral coloring, then reports the adjacent **vein's** sO₂ in the physiological 60–80 % band — the artery-as-reference trick made to work in vivo.
- **Integration insights:** The clearest worked example of internal-reference calibration on the optical side, mirroring the RV/LV reference logic of the MRI iSvO₂ model (§1.4). The fluence-calibration problem it solves locally is the same one APRECOT (§2.4) attacks globally with anatomical priors. *Metadata cross-confirmed via Wiley + arXiv oximetry search snippets; full text 403 (flagged).*

### 2.3 — Oxygenation Heterogeneity Facilitates Spatiotemporal Flow-Pattern Visualization Inside Human Blood Vessels Using Photoacoustic Computed Tomography *(previously surfaced — scan 06-11 §2.2)*
- **Authors:** (PACT group)
- **Year / Venue:** 2024/2025 · PACT human-vessel study
- **Link / DOI:** (PACT venous-flow paper; see scan 06-11 for DOI) — cross-referenced via PMC/ADS
- **Relevance:** **7/10** — non-invasive PACT resolving intravascular oxygenation heterogeneity in human veins.
- **Novelty:** Shows that oxygenation gradients inside a vessel can be used as endogenous contrast to visualize flow patterns, implicitly demonstrating spatially-resolved venous sO₂ within a single vessel lumen.
- **Integration insights:** Argues venous sO₂ is not a single number but a spatial field — relevant to how APRECOT's bulk-chromophore reconstruction (§2.4) and any wearable device should sample a vein. *Cross-confirmed via prior-scan record + search snippet; full text 403 (flagged).*

### 2.4 — ★ NEW — Conditioning Deep Anatomical Prior Knowledge for Reconstruction of Multispectral Optoacoustic Tomography Images (APRECOT) *(newly catalogued this cycle — transferable technique, not venous-specific)*
- **Authors:** Sarah Franceschin, Lukas Imanuel Scheel-Platz, Philipp Haim, Guillaume Zahnd, Vasilis Ntziachristos, Dominik Jüstel
- **Year / Venue:** 2026 (arXiv preprint posted June 2026) · arXiv:2606.16835 (TU Munich / Helmholtz Munich / iThera Medical)
- **Link / DOI:** https://arxiv.org/abs/2606.16835
- **Relevance:** **5/10** — MSOT reconstruction methodology; **not** a venous measurement, but squarely aimed at the quantitative-oxygenation inverse problem that gates PA venous sO₂. In-silico proof-of-concept only.
- **Novelty:** APRECOT conditions reconstruction on **probabilistic anatomical priors** to *jointly* segment tissues and recover their **bulk chromophore (oxygenation) composition**, tackling the ill-posed, fluence-dependent MSOT inverse problem head-on. Reports strongly improved bulk-chromophore accuracy vs reference methods on in-silico data; framed explicitly as a step toward an MSOT mode that "directly provides clinically relevant information such as tissue oxygenation."
- **Integration insights:** Where APM+ (§2.2) fixes fluence *locally* with an arterial reference, APRECOT tries to fix it *globally* with anatomical structure priors — a complementary attack on the same barrier that keeps deep PA venous sO₂ from being quantitative. If it generalises from in-silico to in-vivo forearm/neck anatomy (artery+vein pairs), it is directly on-path to quantitative venous oximetry without an in-situ arterial calibrator. Watch for an in-vivo follow-up. *Authors, title, and abstract cross-confirmed via arXiv listing + search snippet; full text 403 (flagged). Still in-silico — flagged as not yet experimentally validated.*

### 2.5 — ★ NEW — A Novel Differential Pathlength Factor (DPF) Model for Near-Infrared Diffuse Optical Imaging *(newly catalogued this cycle — transferable technique, not venous-specific)*
- **Authors:** (arXiv:2602.00283; NIR diffuse-optics group — author list not fully readable, flagged)
- **Year / Venue:** 2026 (arXiv preprint submitted 2026-01-30) · arXiv:2602.00283
- **Link / DOI:** https://arxiv.org/abs/2602.00283
- **Relevance:** **5/10** — CW-NIRS/DOI quantitation methodology; **tissue-level**, not venous sO₂, but underpins every transcutaneous-NIRS venous method in Topic 1.
- **Novelty:** Derives, from Monte-Carlo simulation, **two distance- and optical-property-dependent DPF models** (one ideal, one experimentally practical) and benchmarks them against standard constant-DPF formulations. Shows existing DPF definitions introduce **large modified-Beer-Lambert errors — worst at small source–detector separations in reflectance mode**, precisely the geometry of compact/wearable NIRS venous sensors.
- **Integration insights:** The quantitative floor under the jugular-NIRS device line (Mespere VO100 §1.5, pediatric NIRSijv) and the DNN-on-Monte-Carlo IJV work (§1.2). A better DPF directly tightens the bias/limits-of-agreement those methods report — the exact metric they must improve to displace an invasive catheter. Low headline relevance because it never measures a vein, but high **leverage** on the accuracy of methods that do. *Title, submission date, and abstract cross-confirmed via arXiv HTML/PDF listing + ResearchGate; full text 403 and author list not verified (flagged).*

**Standing context (not scored in the top-5 this cycle):** Adaptive spectroscopic **vis-OCT** retinal oximetry (ADS-vis-OCT; 1 % phantom bias, 2.1 % vs pulse-oximeter; PMC10126115) and the hyperspectral retinal-oximetry line remain the strongest **true artery-and-vein optical sO₂** demonstrations, but in the retinal microvasculature rather than a systemic vein — all previously surfaced, unchanged today. **Hybrid-Net** (Deep-Learning-Driven Quantitative Spectroscopic PA Imaging, arXiv:2512.15394, Dec 2025) and the **sulfate blood-phantom** paper (arXiv:2512.01458) were re-returned but are already catalogued. The "blood stethoscope" optoacoustic patch and PA-TEE mixed-venous items are likewise previously surfaced.

---

## Cross-topic synthesis

**1. Today's signal is machinery, not measurement.** Zero new venous-specific primary papers, but two new preprints that both attack the *same single barrier* from opposite ends: **spectral coloring / fluence uncertainty** in optical oximetry. APRECOT (§2.4) attacks it in **photoacoustic** reconstruction with global anatomical priors; the DPF model (§2.5) attacks it in **diffuse-optical/NIRS** quantitation with better pathlength physics. This is the through-line of the entire corpus — the IJV-PA anchor, APM+, the DNN+Monte-Carlo IJV work, and the jugular-NIRS devices all live or die on how well fluence/pathlength is handled — and both new items are direct upstream investments in that.

**2. The three calibration strategies are now clearly separable.** (a) *Physical internal reference* — APM+'s neighbouring artery (§2.2), the MRI RV/LV ratio (§1.4). (b) *Learned/simulation prior* — the DNN+Monte-Carlo IJV work (§1.2), SSL intra-cardiac MR (§1.3), and now APRECOT's probabilistic anatomy (§2.4). (c) *Better forward physics* — the new DPF model (§2.5). A convincing wearable venous oximeter will likely need two of the three; no single-paper method yet combines them.

**3. The sparseness verdict holds, and honestly.** Topic 1 (true SvO₂) produced nothing new for the fourth consecutive scan cycle; the top-5 there is a stable, previously-surfaced set spanning optical (jugular sensor, jugular-NIRS) and reference-grade MRI/capnodynamic methods. Topic 2's genuine novelty this cycle is **both technique-level and in-silico/methodological** — real progress on the enabling problem, but not a new human venous measurement. Neither new item should be over-read as a venous-oximetry result; they are scored 5/10 precisely because their venous relevance is *indirect but high-leverage*.

**4. Persisting gaps (carried forward, still open):** (i) no non-invasive optical/PA SvO₂ method has been validated against invasive co-oximetry in a large cohort with published limits-of-agreement (the Alqahtani sensor is n=3; APM+ is n=8 healthy); (ii) no method yet fuses an internal reference + learned prior + corrected forward physics; (iii) the retinal vis-OCT/hyperspectral line has the best *true venous* optical accuracy but in a vessel bed not representative of systemic/central venous status. Today moved the needle on (ii)'s building blocks, not on (i) or (iii).

---

*Scan generated 2026-07-17 (UTC). Two new items catalogued (§2.4 APRECOT, §2.5 DPF model); all other entries previously surfaced and carried forward with scores unchanged. Publisher full-text access was 403-blocked in this environment; every reference was cross-checked across ≥2 independent search-index snippets, with per-item verification notes and flags above.*
