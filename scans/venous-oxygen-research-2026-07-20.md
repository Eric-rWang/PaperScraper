# Venous Oxygen Research Scan — 2026-07-20

**Search window:** Twenty-sixth scan in the series, run **three days** after 2026-07-17 (no scans on 07-18, 07-19). Emphasis on work published or first-surfacing after 07-17, with the standard fallback to the best-available venous-specific work already catalogued. Sources searched today: PubMed/PMC, arXiv, bioRxiv/medRxiv, Optica (Biomed. Opt. Express, Optics Letters, Applied Optics), SPIE / *J. Biomed. Opt.*, IOP (*Phys. Med. Biol.*, *J. Phys. Photonics*), *Photoacoustics* (ScienceDirect), IEEE Xplore, Nature / *Sci. Rep.* / *Eye*, Wiley (*Advanced Science*, *J. Biophotonics*), MDPI, Springer, De Gruyter, ClinicalTrials.gov, ResearchGate, Semantic Scholar, ADS.

**Verification caveat:** As in every prior scan, publisher **full-text** pages — including arxiv.org (abs + /html), pmc.ncbi.nlm.nih.gov, opg.optica.org, iopscience.iop.org and the Wiley/Nature domains — returned **HTTP 403** to direct `WebFetch` in this environment today (re-confirmed on arXiv `2602.16357` abs + html, and on IOP `2515-7647/ae6ae4`). Every reference below was therefore cross-checked across **at least two independent search-index snippets** (Google Scholar-style result blocks + ADS/ResearchGate/PMC/PuSH listings); per-item notes state what was confirmed and what could not be read directly on a publisher page.

---

## ⚠️ Read this first — day summary

**No new venous-specific *primary* paper today.** Consistent with the series' standing observation, truly novel non-invasive **venous**-optical work is published at very low volume, and today's sweep produced no new SvO₂/ScvO₂ demonstration. However, the sweep surfaced **three genuinely new technique/methodology papers** — none in any prior scan file — all on the **optical/photoacoustic** side (Topic 2), all attacking the **fluence / spectral-coloring** barrier that gates quantitative optical venous oximetry, and all therefore **transferable** to (but not themselves) venous sO₂:

- **NEW — SPOI-AE** (arXiv:2602.16357, 2026-02-18, **Emelianov group**): a physics-informed autoencoder that performs **optical inversion + spectral unmixing** of spectroscopic-PA images *without assuming linearity*, returning optical parameters, chromophore concentrations, and tissue %sO₂. From the same lab as the IJV-PA venous anchor (§2.1).
- **NEW — ISDC** (J. Biomed. Opt. 31(2):026002, 2026-02-04, **Quing Zhu group, WashU**): an **integrated spectral + depth compensation** method that corrects both wavelength-dependent spectral distortion and depth-dependent attenuation to improve sO₂/tHb quantitation in clinical **photoacoustic tomography**; validated on phantoms and 82 ovarian lesions.
- **NEW — Time-resolved diffuse-optics simulator validation** (arXiv:2511.09587 → *Phys. Med. Biol.* 10.1088/1361-6560/ae7bad, **Ren/Charbon group**): systematic experimental validation of MMC / NIRFASTer / Toast++ forward models against a **32×32 SPAD** time-resolved dataset — the forward-model floor beneath every NIRS/DOI venous method.

All three are **tissue/technique-level**, not true SvO₂, and are scored accordingly. Everything else returned by the sweep is **previously surfaced** or out-of-scope: the Alqahtani jugular optical sensor (De Gruyter CDBME), the IJV DNN + Monte-Carlo work (Optics Letters), Mespere VO100 jugular NIRS, the McDiarmid MRI iSvO₂ model, the SSL intra-cardiac MR oximetry preprint, the IJV-PA anchor, APM+ (radial-vein sO₂ in humans), PACT venous-flow work, vis-OCT / hyperspectral retinal oximetry, APRECOT (arXiv:2606.16835, surfaced 07-17), the new DPF model (arXiv:2602.00283, surfaced 07-17), Hybrid-Net (arXiv:2512.15394), and the sulfate-phantom paper (arXiv:2512.01458). No new primary venous demonstration — only new **transferable machinery**.

---

## Topic 1 — Non-invasive monitoring of venous blood oxygen (SvO₂ / ScvO₂ / peripheral venous)

*No new items today.* The standing best-available set (all previously surfaced) with scores carried forward. This topic remains the sparse one: no primary non-invasive venous-O₂ measurement paper first-surfaced since 2026-07-15, now a fifth consecutive scan cycle with no new Topic-1 primary work.

### 1.1 — Estimation of Venous Oxygen Saturation Through Non-Invasive Optical Sensing at the Jugular Veins *(previously surfaced — scan 06-10 §1.1; flagship optical-venous device paper)*
- **Authors:** Alqahtani et al.
- **Year / Venue:** 2024 · *Current Directions in Biomedical Engineering* 10(2) (De Gruyter; CDBME-2024-2072)
- **Link / DOI:** https://doi.org/10.1515/cdbme-2024-2072
- **Relevance:** **8/10** — true, non-invasive, optical, venous (but n=3, no invasive co-oximetry reference).
- **Novelty:** A pulse-oximeter-style optical sensor over the external jugular vein isolates the EJV waveform and returns SvO₂ estimates (~70–72 %) within the healthy 60–90 % band — still the closest thing to a wearable-form-factor optical SvO₂ device in the literature.
- **Integration insights:** The superficial/low-cost optical analogue of the deep IJV-PA anchor (§2.1); together they bracket the venous-optical problem from the shallow and deep ends. Its open problem — calibration against a blood-gas gold standard — is exactly what the SPOI-AE unmixing (§2.4) and ISDC fluence-correction (§2.5) approaches aim to make quantitative. *Metadata cross-confirmed via De Gruyter listing + ResearchGate 387159780; full text 403 (flagged).*

### 1.2 — Quantifying Changes in Oxygen Saturation of the Internal Jugular Vein In Vivo Using Deep Neural Networks and Subject-Specific 3-D Monte-Carlo Models *(previously surfaced — scan 06-10 §1.2)*
- **Authors:** (multi-author; NIRS + DNN group)
- **Year / Venue:** 2024 · *Optics Letters* 49(10):2669
- **Link / DOI:** https://opg.optica.org/ol/abstract.cfm?uri=ol-49-10-2669
- **Relevance:** **7/10** — IJV-specific, non-invasive, inverse-modeling for venous saturation *change*.
- **Novelty:** Multi-channel NIRS + DNNs trained on subject-specific 3-D Monte-Carlo forward models recover ΔSijvO₂ non-invasively, tying measured reflectance to a physically-modelled forward problem — sidestepping the labelled-data bottleneck via simulation.
- **Integration insights:** The inverse-modeling leg of the program. **Directly touched by today's NEW diffuse-optics simulator-validation work (§2.6):** the accuracy of this DNN-on-Monte-Carlo pipeline is bounded by exactly the forward-model fidelity (MMC and relatives) that §2.6 benchmarks against real SPAD data. *Cross-confirmed via Optica listing + Semantic Scholar; full text 403 (flagged).*

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
- **Integration insights:** The most clinically-mature non-invasive venous-NIRS device line — the practical baseline on bias and limits-of-agreement any optical/PA method must beat. Its accuracy floor is set by the same CW-NIRS pathlength/forward-model assumptions the new DPF model (07-17 §2.5) and the diffuse-optics simulator validation (§2.6) target. *Cross-confirmed via ScienceDirect + PubMed 37827917; full text 403 (flagged).*

**Standing context (not scored in the top-5):** jugular transcutaneous NIRS in pediatric cardiac surgery (r = 0.91 vs ScvO₂, bias 2.92 %; PMC7491293), respiration-frequency-selected NIRS for cerebral SvO₂ (PMC4126245 / PMID 24439329), NIRS cerebral-oximetry tracking of mixed-venous SvO₂ (Sci. Rep. 2023, s41598-023-49078-1), capnodynamic mixed-venous SvO₂ (NCT06632197; PMID 34609659), and the preterm-neonate NIRS venous-occlusion series (PMC8831784) — all previously catalogued, none updated this cycle.

---

## Topic 2 — Optical imaging techniques for non-invasively obtaining venous blood oxygen (PA/PACT, NIRS, DOI/DOT, hyperspectral, vis-OCT, SFDI)

Three **new** transferable-technique papers this cycle (§2.4 SPOI-AE, §2.5 ISDC, §2.6 diffuse-optics simulator validation), slotted below the standing venous-specific anchors.

### 2.1 — Noninvasive In Vivo Photoacoustic Measurement of Internal Jugular Venous Oxygenation in Humans *(previously surfaced — scan 06-10 §2.1; the Topic-2 anchor)*
- **Authors:** (PA/US group, Emelianov lab; arXiv:2303.10775)
- **Year / Venue:** 2023 · arXiv preprint / SPIE lineage
- **Link / DOI:** https://arxiv.org/abs/2303.10775
- **Relevance:** **9/10** — true, non-invasive, optical/PA, deep **named-vein** (IJV) sO₂ in humans. The single most on-target paper in the corpus.
- **Novelty:** Combined photoacoustic + ultrasound imaging computes hemoglobin sO₂ of the internal jugular vein in vivo, non-invasively, in real time — the reference demonstration that deep venous PA oximetry is physically achievable in humans.
- **Integration insights:** The deep-vein anchor everything else is measured against. Notably, today's NEW **SPOI-AE** (§2.4) comes from the *same lab (Emelianov)* — it is the natural quantitative-unmixing engine to bolt onto this IJV-PA measurement to remove its dependence on an ultrasound co-registration crutch. *Metadata cross-confirmed via arXiv + ADS; full text 403 (flagged).*

### 2.2 — Arterial Blood-Mediated Deep-Tissue Photoacoustic Oximetry (APM+): in-vivo human radial-vein sO₂ *(previously surfaced — upgraded 07-15 §2.2)*
- **Authors:** Sastry et al.
- **Year / Venue:** 2026 · *Advanced Science* (Wiley)
- **Link / DOI:** https://doi.org/10.1002/advs.76366
- **Relevance:** **8/10** — a bona-fide non-invasive optical/PA venous-oximetry demonstration in humans (radial-vein median sO₂ 72.3 %, IQR 8.9 %, n=8 healthy adults).
- **Novelty:** Uses the neighbouring radial **artery** as an in-situ fluence calibrator to circumvent spectral coloring, then reports the adjacent **vein's** sO₂ in the physiological 60–80 % band — the artery-as-reference trick made to work in vivo.
- **Integration insights:** The clearest worked example of internal-reference calibration on the optical side. Where APM+ fixes fluence with a *physical* arterial reference, SPOI-AE (§2.4) and ISDC (§2.5) attempt to fix the *same* spectral-coloring problem *computationally* — the two families are complementary and, in principle, stackable. *Metadata cross-confirmed via Wiley + arXiv oximetry search snippets; full text 403 (flagged).*

### 2.3 — Oxygenation Heterogeneity Facilitates Spatiotemporal Flow-Pattern Visualization Inside Human Blood Vessels Using Photoacoustic Computed Tomography *(previously surfaced — scan 06-11 §2.2)*
- **Authors:** (PACT group)
- **Year / Venue:** 2024/2025 · PACT human-vessel study
- **Link / DOI:** (PACT venous-flow paper; see scan 06-11 for DOI) — cross-referenced via PMC/ADS
- **Relevance:** **7/10** — non-invasive PACT resolving intravascular oxygenation heterogeneity in human veins.
- **Novelty:** Shows that oxygenation gradients inside a vessel can be used as endogenous contrast to visualize flow patterns, implicitly demonstrating spatially-resolved venous sO₂ within a single vessel lumen.
- **Integration insights:** Argues venous sO₂ is a spatial field, not a single number — relevant to how the pixel-wise SPOI-AE unmixing (§2.4) and depth-resolved ISDC (§2.5) should sample a vein. *Cross-confirmed via prior-scan record + search snippet; full text 403 (flagged).*

### 2.4 — ★ NEW — Optical Inversion and Spectral Unmixing of Spectroscopic Photoacoustic Images with Physics-Informed Neural Networks (SPOI-AE) *(newly catalogued this cycle — transferable technique, not venous-specific)*
- **Authors:** Sarkis Ter Martirosyan, Xinyue Huang, David Qin, Anthony Yu, Stanislav Emelianov (Georgia Institute of Technology / Emory)
- **Year / Venue:** 2026 (arXiv preprint posted 2026-02-18) · arXiv:2602.16357
- **Link / DOI:** https://arxiv.org/abs/2602.16357
- **Relevance:** **6/10** — spectroscopic-PA optical-inversion methodology; **not** a venous measurement, but from the exact lab and imaging modality (PA) behind the IJV-PA venous anchor (§2.1), and squarely on the sO₂-quantitation critical path. Highest new-item relevance this cycle because of that direct lineage.
- **Novelty:** The **Spectroscopic Photoacoustic Optical Inversion Autoencoder (SPOI-AE)** is a *physics-informed* autoencoder that jointly solves the sPA **optical-inversion** and **spectral-unmixing** problems **without assuming a linear** absorption-to-signal relationship — the linearity assumption that breaks conventional linear-unmixing sO₂ estimates in deep/heterogeneous tissue. It reconstructs input sPA pixels better than conventional algorithms while returning *biologically coherent* estimates of optical parameters, chromophore concentrations, and tissue %sO₂.
- **Integration insights:** This is the computational engine the IJV-PA anchor (§2.1) currently lacks — a way to turn multiwavelength PA signal into calibrated venous sO₂ without a co-registered ultrasound fluence crutch or a neighbouring-artery reference (APM+, §2.2). If validated in vivo on a forearm/neck artery–vein pair, it is directly on-path to quantitative venous PA oximetry. Same fluence/spectral-coloring barrier as APRECOT (07-17 §2.4), attacked with a nonlinear autoencoder rather than anatomical priors. *Authors (5), title, and SPOI-AE abstract cross-confirmed via arXiv listing + search snippet; full text 403 on both abs and /html (flagged). In-silico / reconstruction-level — no in-vivo venous validation yet (flagged).*

### 2.5 — ★ NEW — Integrated Spectral and Depth Compensation (ISDC) for Oxygen Saturation and Total Hemoglobin Estimation in Photoacoustic Tomography *(newly catalogued this cycle — transferable technique, clinical PAT, not venous-specific)*
- **Authors:** Lukai Wang, Yixiao Lin, Haolin Nie, Jinhua Xu, Sanskar Thakur, Quing Zhu (Washington University in St. Louis)
- **Year / Venue:** 2026 (published 2026-02-04) · *Journal of Biomedical Optics* 31(2):026002
- **Link / DOI:** https://doi.org/10.1117/1.JBO.31.2.026002 · PMC12869027
- **Relevance:** **6/10** — clinical PAT fluence-correction methodology validated on real patient data; **tissue/lesion-level** sO₂, not venous, but the most experimentally-grounded new fluence-correction paper this cycle.
- **Novelty:** ISDC corrects **both** wavelength-dependent **spectral distortion** (via Monte-Carlo-derived spectral compensation) **and** depth-dependent fluence attenuation (depth-wise correction) to improve sO₂ and total-hemoglobin quantitation in photoacoustic tomography. Validated on phantoms of known optical properties and applied to **clinical PAT data from 82 ovarian lesions** (67 benign, 15 malignant) — a rare case of a fluence-correction method tested at clinical scale rather than only in silico.
- **Integration insights:** The depth-plus-spectral compensation is exactly the correction any **deep venous** PA measurement (IJV at several cm, §2.1) needs, because venous sO₂ error grows with depth-dependent spectral coloring. Complements SPOI-AE (§2.4, learned nonlinear inversion) and APM+ (§2.2, physical arterial reference) as the *analytical/Monte-Carlo* member of the fluence-correction family — and, unlike the two in-silico items, it is already validated on human tissue. *Authors (6), venue, DOI, and clinical-cohort details cross-confirmed via PMC12869027 + PubMed snippets; full text 403 (flagged). Not a venous measurement — ovarian lesion application (flagged).*

### 2.6 — ★ NEW — Systematic Validation of Time-Resolved Diffuse Optical Simulators via Non-Contact SPAD-Based Measurements *(newly catalogued this cycle — forward-model foundation, not venous-specific)*
- **Authors:** Weijia Zhao, Linlin Li, Kaiqi Kuang, Yang Lin, Claudio Bruschini, Jiaming Cao, Ting Li, Edoardo Charbon, Wuwei Ren
- **Year / Venue:** 2025/2026 · arXiv:2511.09587 (posted Nov 2025) → *Physics in Medicine & Biology* (10.1088/1361-6560/ae7bad)
- **Link / DOI:** https://arxiv.org/abs/2511.09587 · https://doi.org/10.1088/1361-6560/ae7bad
- **Relevance:** **5/10** — diffuse-optics **forward-model** validation; tissue-level, never measures a vein, but underpins every NIRS/DOI venous method in Topic 1.
- **Novelty:** Rigorously benchmarks three widely-used open-source diffusion/Monte-Carlo simulators (**MMC, NIRFASTer, Toast++**) against **time-resolved experimental data** from a **32×32 SPAD array** across 16 standardized phantoms of varying μₐ/μₛ′, in a *non-contact, oblique-illumination* configuration that prior validations neglected — quantifying where each simulator's photon-propagation model diverges from measurement.
- **Integration insights:** The DNN-on-Monte-Carlo IJV work (§1.2) and every subject-specific-forward-model NIRS venous method inherit their accuracy ceiling from exactly these simulators; knowing where MMC/NIRFASTer/Toast++ break (and by how much) directly bounds the achievable bias/limits-of-agreement of simulation-trained venous NIRS. The non-contact/oblique geometry is also the geometry of a wearable venous-NIRS patch. Low headline relevance, high **leverage** — the ground-truth check under the inverse models. *Authors (9), title, simulator list, and SPAD-array details cross-confirmed via arXiv + IOPscience + Cool Papers snippets; full text 403 (flagged). Forward-model validation only — no sO₂/venous measurement (flagged).*

**Standing context (not scored in the top-5 this cycle):** Adaptive spectroscopic **vis-OCT** retinal oximetry (ADS-vis-OCT; repeat-measurement SD ≈ 2.3 % in veins; PMC10126115 / Nature Comms Med s43856-023-00288-8) and the hyperspectral retinal-oximetry line remain the strongest **true artery-and-vein optical sO₂** demonstrations, but in the retinal microvasculature rather than a systemic vein — all previously surfaced, unchanged today. **APRECOT** (arXiv:2606.16835) and the **DPF model** (arXiv:2602.00283) were catalogued last cycle (07-17). **Hybrid-Net** (arXiv:2512.15394) and the **sulfate blood-phantom** paper (arXiv:2512.01458) were re-returned but are already catalogued. A 2026 IOP review, "Advances in fully integrated wearable near-infrared spectroscopy: hardware innovations and biomedical applications" (*J. Phys. Photonics*, 10.1088/2515-7647/ae6ae4), was surfaced but is a hardware review, not a venous measurement — noted, not scored (metadata partly unverified, 403).

---

## Cross-topic synthesis

**1. The fluence-correction family now has four distinct members — and today added two.** Every serious attempt at quantitative optical venous sO₂ lives or dies on handling wavelength-dependent fluence / spectral coloring, and the corpus now cleanly separates four attacks on it: (a) **physical internal reference** — APM+'s neighbouring artery (§2.2); (b) **anatomical priors** — APRECOT (07-17 §2.4); (c) **learned nonlinear inversion** — today's **SPOI-AE** (§2.4); (d) **analytical spectral+depth compensation** — today's **ISDC** (§2.5). ISDC is the only one of the four already validated on human tissue at clinical scale (82 lesions), and SPOI-AE is the only one from the same lab as the human IJV-PA venous anchor. That lineage makes SPOI-AE the single most watch-worthy new item.

**2. Beneath the correction methods sits a forward-model floor — and today someone measured it.** The DNN/Monte-Carlo IJV work (§1.2), APRECOT, and simulation-trained NIRS all assume their light-transport simulators are faithful. §2.6 is the first item in the corpus to *systematically test that assumption* against time-resolved SPAD data for MMC/NIRFASTer/Toast++ in a non-contact geometry. This is unglamorous but load-bearing: it bounds how good any simulation-trained venous method can get.

**3. Zero new venous *measurement* — the fifth consecutive dry cycle for Topic 1.** No new primary non-invasive venous SvO₂/ScvO₂ paper has first-surfaced since 07-15. The Topic-1 top-5 is a stable, previously-surfaced set spanning optical (jugular sensor, jugular-NIRS) and reference-grade MRI/capnodynamic methods. Today's three new items are all Topic-2, all technique/foundation-level, none a venous measurement — scored 5–6/10 precisely because their venous relevance is *indirect but high-leverage*. This is honest sparseness, not padding.

**4. Persisting gaps (carried forward, still open):** (i) no non-invasive optical/PA SvO₂ method has been validated against invasive co-oximetry in a large cohort with published limits-of-agreement (Alqahtani n=3; APM+ n=8 healthy); (ii) no single method yet fuses an internal reference + learned prior + corrected forward physics — though today's SPOI-AE (learned) + ISDC (analytical) + §2.6 (validated forward model) are the building blocks that could be composed; (iii) the retinal vis-OCT/hyperspectral line has the best *true venous* optical accuracy but in a vessel bed not representative of systemic/central venous status. Today moved the needle on (ii)'s components, not on (i) or (iii).

---

*Scan generated 2026-07-20 (UTC). Three new items catalogued (§2.4 SPOI-AE, §2.5 ISDC, §2.6 diffuse-optics simulator validation); all other entries previously surfaced and carried forward with scores unchanged. Publisher full-text access was 403-blocked in this environment; every reference was cross-checked across ≥2 independent search-index snippets, with per-item verification notes and flags above.*
