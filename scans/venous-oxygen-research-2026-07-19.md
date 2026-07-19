# Venous Oxygen Research Scan — 2026-07-19

**Search window:** Twenty-sixth scan in the series, run **two days** after 2026-07-17 (no scan on 07-18). Emphasis on work published or first-surfacing after 07-17, with the standard fallback to the best-available venous-specific work already catalogued. Sources searched today: PubMed/PMC, arXiv (physics.med-ph, eess.IV), bioRxiv/medRxiv, Optica (Biomed. Opt. Express, Optics Letters, Applied Optics), SPIE / *J. Biomed. Opt.*, *Photoacoustics* (ScienceDirect), IEEE Xplore, Nature / *Sci. Rep.* / *Eye*, Wiley (*Advanced Science*, *J. Biophotonics*), MDPI, Springer, De Gruyter, *J. Clin. Monit. Comput.*, *BioMedical Engineering OnLine*, ClinicalTrials.gov, ResearchGate, Semantic Scholar, ADS.

**Verification caveat:** As in every prior scan, publisher **full-text** pages — including arxiv.org, pmc.ncbi.nlm.nih.gov, opg.optica.org, link.springer.com, advanced.onlinelibrary.wiley.com and the Nature/Eye domains — returned **HTTP 403** to direct `WebFetch` in this environment today (re-confirmed on arXiv `2403.14863`, PMC `PMC5655584`). Every reference below was therefore cross-checked across **at least two independent search-index snippets** (Google Scholar-style result blocks + PubMed/PMC/ResearchGate/Springer listings); per-item notes state what was confirmed and what could not be read directly on a publisher page.

---

## ⚠️ Read this first — day summary

**No new venous-specific *primary* paper published since 2026-07-17, and no new technique preprint either.** APRECOT (arXiv:2606.16835) and the DPF-model preprint (arXiv:2602.00283) catalogued on 07-17 remain the most recent genuinely-new items; today's sweep surfaced nothing published after them. Consistent with the series' standing observation, truly novel non-invasive **venous**-optical work is published at very low volume.

**One genuinely-uncatalogued venous-specific method family surfaced today — older, but new to this catalogue and honestly additive (not padding):** the **Belhaj / Kyriacou / Phillips / Langford PPG peripheral-venous oximetry** line (*J. Clin. Monit. Comput.* 2016/2017; *BioMed. Eng. OnLine* 2017; foundational Nitzan work). This is a **true non-invasive peripheral venous sO₂ method validated against venous blood co-oximetry** — the direct methodological ancestor of the wearable E-tattoo venous work already in the catalogue, and better-referenced (co-oximetry gold standard, larger n) than the flagship Alqahtani jugular sensor (n=3). It is catalogued below as **§1.2 (newly catalogued, published 2016/2017 — not previously surfaced)** and honestly scored.

Everything else returned by the sweep is **previously surfaced** or out-of-scope: the Alqahtani jugular optical sensor (De Gruyter CDBME), the IJV DNN + Monte-Carlo work (Optics Letters), Mespere VO100 jugular NIRS, the McDiarmid MRI iSvO₂ model, the SSL intra-cardiac MR oximetry preprint, the IJV-PA anchor, APM+ (radial-vein sO₂ in humans), PACT venous-flow work, vis-OCT / hyperspectral retinal oximetry, APRECOT, the DPF model, Hybrid-Net (arXiv:2512.15394), the sulfate-phantom paper, SFDI-net, and the "distribution-informed data-driven PA oximetry" preprint (arXiv:2403.14863, 2024 — noted in standing context, not venous). No new primary venous demonstration this cycle.

---

## Topic 1 — Non-invasive monitoring of venous blood oxygen (SvO₂ / ScvO₂ / peripheral venous)

One newly-catalogued (older) venous-specific method (§1.2); the rest of the standing best-available set carried forward with scores. No primary non-invasive venous-O₂ measurement paper was *published* since 2026-07-17.

### 1.1 — Estimation of Venous Oxygen Saturation Through Non-Invasive Optical Sensing at the Jugular Veins *(previously surfaced — scan 06-10 §1.1; flagship optical-venous device paper)*
- **Authors:** Alqahtani et al.
- **Year / Venue:** 2024 · *Current Directions in Biomedical Engineering* 10(2) (De Gruyter; CDBME-2024-2072)
- **Link / DOI:** https://doi.org/10.1515/cdbme-2024-2072
- **Relevance:** **8/10** — true, non-invasive, optical, venous (but n=3, no invasive co-oximetry reference).
- **Novelty:** A pulse-oximeter-style optical sensor over the external jugular vein isolates the EJV waveform and returns SvO₂ estimates (~70–75 %; reported per-subject 70.4–75.3 %) within the healthy 60–90 % band — still the closest thing to a wearable-form-factor optical SvO₂ device in the literature.
- **Integration insights:** The superficial/low-cost optical analogue of the deep IJV-PA anchor (§2.1); together they bracket the venous-optical problem from the shallow and deep ends. Its open problem — calibration against a blood-gas gold standard — is exactly what the newly-catalogued PPG-vs-co-oximetry work (§1.2) partly closes at the peripheral (hand) site, and what MRI reference oximetry (§1.5) and APM+ (§2.2) close at deep sites. *Metadata cross-confirmed via De Gruyter listing + ResearchGate; full text 403 (flagged).*

### 1.2 — ★ NEW (catalogued this cycle) — Comparison of Non-Invasive Peripheral Venous Saturations with Venous Blood Co-Oximetry *(published 2016/2017 — not previously surfaced in any prior scan)*
- **Authors:** A. M. Belhaj, J. P. Phillips, P. A. Kyriacou, R. M. Langford
- **Year / Venue:** 2016 (online) / 2017 · *Journal of Clinical Monitoring and Computing* 31(6)
- **Link / DOI:** https://doi.org/10.1007/s10877-016-9959-9 · PMC5655584 · PMID 27873173
- **Relevance:** **7/10** — a genuine **non-invasive peripheral venous** sO₂ method, and — unusually for this catalogue — **validated directly against venous blood co-oximetry** (the correct gold standard), not merely against the healthy physiological band.
- **Novelty:** PPG-derived peripheral venous saturations (SpvO₂) from the dorsum of the hand were compared against co-oximetry of venous blood in two cohorts — healthy spontaneously-breathing volunteers and mechanically-ventilated anaesthetised patients. Reports **moderate correlation r = 0.81** in volunteers with **mean bias +5.65 % and wide limits of agreement (±14.3 %)** — an honest, sobering accuracy figure for the induced-venous-modulation PPG approach. Companion "proof-of-concept" paper (Shafqat/Kyriacou lineage, *BioMed. Eng. OnLine* 2017, DOI 10.1186/s12938-017-0351-x) describes the method: use the artery–vein compliance difference to make venous blood artificially pulsatile, then apply pulse-oximetry-style ratio-of-ratios math to the venous component.
- **Integration insights:** This is the **direct methodological ancestor of the wearable E-tattoo arterial+venous work** already catalogued (scan 06-17 §1.1 / 07-01), and its published limits-of-agreement set the **realistic accuracy floor** any wearable venous PPG/optical device must beat. Its co-oximetry validation is exactly the reference-standard step the Alqahtani jugular sensor (§1.1, n=3, no co-oximetry) still lacks — making the two complementary (Alqahtani = better site/waveform isolation; Belhaj = better reference standard). Fills a real gap in the Topic-1 catalogue. *Authors, venue, DOI, PMID and the r = 0.81 / +5.65 ± 14.3 % figures cross-confirmed via PubMed 27873173 + Springer listing + PMC5655584 snippet; full text 403 (flagged).*

### 1.3 — Quantifying Changes in Oxygen Saturation of the Internal Jugular Vein In Vivo Using Deep Neural Networks and Subject-Specific 3-D Monte-Carlo Models *(previously surfaced — scan 06-10 §1.2)*
- **Authors:** (multi-author; NIRS + DNN group)
- **Year / Venue:** 2024 · *Optics Letters* 49(10):2669
- **Link / DOI:** https://opg.optica.org/ol/abstract.cfm?uri=ol-49-10-2669
- **Relevance:** **7/10** — IJV-specific, non-invasive, inverse-modeling for venous saturation *change*.
- **Novelty:** Multi-channel NIRS + DNNs trained on subject-specific 3-D Monte-Carlo forward models recover ΔSijvO₂ non-invasively, tying measured reflectance to a physically-modelled forward problem — sidestepping the labelled-data bottleneck via simulation.
- **Integration insights:** The inverse-modeling / fluence-correction leg of the program; its accuracy is bounded by exactly the pathlength/fluence assumptions the DPF-model preprint (§2 standing context) reformulates. Recovers *change* rather than absolute sO₂ — the complement to §1.2's absolute (but noisy) co-oximetry-referenced estimate. *Cross-confirmed via Optica listing + Semantic Scholar; full text 403 (flagged).*

### 1.4 — A New Non-Invasive Method for the Assessment of Central Venous Oxygen Saturation (Mespere VO100 jugular NIRS) *(previously surfaced — scan 06-10 §1.3)*
- **Authors:** (critical-care cohort study)
- **Year / Venue:** 2023 · *J. Cardiothoracic and Vascular Anesthesia* (S1053-0770(23)00782-6)
- **Link / DOI:** https://www.sciencedirect.com/science/article/pii/S1053077023007826 · PMID 37827917
- **Relevance:** **7/10** — non-invasive NIRS surrogate for ScvO₂, clinical cohort.
- **Novelty:** Validates transcutaneous jugular NIRS (Mespere VO100) against invasive ScvO₂ in critically ill patients, reporting strong linear correlation with low bias/percentage error.
- **Integration insights:** The most clinically-mature non-invasive venous-NIRS device line — the practical baseline on bias and limits-of-agreement any optical/PA method (and the PPG method in §1.2) must beat. Its accuracy floor is set by exactly the CW-NIRS pathlength assumptions the DPF model targets. *Cross-confirmed via ScienceDirect + PubMed 37827917; full text 403 (flagged).*

### 1.5 — Development and Validation of a Noninvasive Model of Mixed Venous Oxygen Saturation in Heart Failure (imaging-derived iSvO₂) *(previously surfaced — scan 07-07 §1.1)*
- **Authors:** McDiarmid et al.
- **Year / Venue:** 2025/2026 · *JACC: Advances*
- **Link / DOI:** https://doi.org/10.1016/j.jacadv.2025.102484 · PMC12869880 · PMID 41609283
- **Relevance:** **7/10** — true mixed-venous, non-invasive, clinically validated (MRI, not optical).
- **Novelty:** 628-patient validation of an imaging-derived mixed-venous SvO₂ from the RV/LV blood-pool T₂ ratio on cardiac MRI (R = 0.82 vs invasive SvO₂), anchored to right-heart catheterization and an independent predictor of mortality/HF-hospitalization.
- **Integration insights:** Sets the **absolute-accuracy and outcome-relevance benchmark** any optical SvO₂ method must match, in exactly the population (heart failure) where a cheap continuous optical surrogate would be most valuable. Its internal-reference (RV vs LV) logic recurs on the optical side as artery-vs-vein calibration (§2.2). *Cross-confirmed via JACC/ScienceDirect + PMC + PubMed; full text 403 (flagged).*

**Standing context (not scored in the top-5 this cycle):** the SSL intra-cardiac MR oximetry preprint (medRxiv, 2026-07-01; MAE ≈ 3.70, true mixed-venous, non-optical — carried from scan 07-13 §1.1), jugular transcutaneous NIRS in pediatric cardiac surgery (r = 0.91 vs ScvO₂, bias 2.92 %; PMC7491293), respiration-frequency-selected NIRS for cerebral SvO₂ (PMC4126245 / PMID 24439329), capnodynamic mixed-venous SvO₂ (NCT06632197; PMID 34609659), the IDO₂ delivery index, and the preterm-neonate NIRS venous-occlusion series — all previously catalogued, none updated this cycle.

---

## Topic 2 — Optical imaging techniques for non-invasively obtaining venous blood oxygen (PA/PACT, NIRS, DOI/DOT, hyperspectral, vis-OCT, SFDI)

**No new technique paper this cycle.** The standing anchors are carried forward with scores; the most recent genuinely-new items remain APRECOT and the DPF model (both catalogued 07-17), listed here in standing context.

### 2.1 — Noninvasive In Vivo Photoacoustic Measurement of Internal Jugular Venous Oxygenation in Humans *(previously surfaced — scan 06-10 §2.1; the Topic-2 anchor)*
- **Authors:** (PA/US group; arXiv:2303.10775)
- **Year / Venue:** 2023 · arXiv preprint / SPIE lineage
- **Link / DOI:** https://arxiv.org/abs/2303.10775
- **Relevance:** **9/10** — true, non-invasive, optical/PA, deep **named-vein** (IJV) sO₂ in humans (average IJV sO₂ 72 ± 7 %). The single most on-target paper in the corpus.
- **Novelty:** Combined photoacoustic + ultrasound imaging computes hemoglobin sO₂ of the internal jugular vein in vivo, non-invasively, in real time — the reference demonstration that deep venous PA oximetry is physically achievable in humans.
- **Integration insights:** The deep-vein anchor everything else is measured against; APM+ (§2.2), APRECOT, and the DPF model are all attempts to make this kind of measurement quantitative and fluence-robust without an ultrasound co-registration crutch. *Metadata cross-confirmed via arXiv + ADS; full text 403 (flagged).*

### 2.2 — Arterial Blood-Mediated Deep-Tissue Photoacoustic Oximetry (APM+): in-vivo human radial-vein sO₂ *(previously surfaced — upgraded 07-15 §2.2)*
- **Authors:** Sastry et al.
- **Year / Venue:** 2026 · *Advanced Science* (Wiley)
- **Link / DOI:** https://doi.org/10.1002/advs.76366
- **Relevance:** **8/10** — a bona-fide non-invasive optical/PA venous-oximetry demonstration in humans (radial-vein median sO₂ 72.3 %, IQR 8.9 %, n=8 healthy adults; phantom median error 2.9 % vs 9.8 % for linear unmixing).
- **Novelty:** Uses the neighbouring radial **artery** as an in-situ fluence calibrator to circumvent spectral coloring, then reports the adjacent **vein's** sO₂ in the physiological 60–80 % band — the artery-as-reference trick made to work in vivo.
- **Integration insights:** The clearest worked example of internal-reference calibration on the optical side, mirroring the RV/LV reference logic of the MRI iSvO₂ model (§1.5). The fluence-calibration problem it solves locally is the same one APRECOT attacks globally with anatomical priors. *Metadata cross-confirmed via Wiley + arXiv oximetry search snippets; full text 403 (flagged).*

### 2.3 — Oxygenation Heterogeneity Facilitates Spatiotemporal Flow-Pattern Visualization Inside Human Blood Vessels Using Photoacoustic Computed Tomography *(previously surfaced — scan 06-11 §2.2)*
- **Authors:** (PACT group)
- **Year / Venue:** 2024/2025 · PACT human-vessel study
- **Link / DOI:** (PACT venous-flow paper; see scan 06-11 for DOI) — cross-referenced via PMC/ADS
- **Relevance:** **7/10** — non-invasive PACT resolving intravascular oxygenation heterogeneity in human veins.
- **Novelty:** Shows oxygenation gradients inside a vessel can be used as endogenous contrast to visualize flow patterns, implicitly demonstrating spatially-resolved venous sO₂ within a single vessel lumen.
- **Integration insights:** Argues venous sO₂ is not a single number but a spatial field — relevant to how any wearable device and any bulk-chromophore reconstruction should sample a vein. *Cross-confirmed via prior-scan record + search snippet; full text 403 (flagged).*

### 2.4 — Adaptive Spectroscopic Visible-Light OCT for Clinical Retinal Oximetry (ADS-vis-OCT) *(previously surfaced — scan 06-11 §2.2)*
- **Authors:** (vis-OCT oximetry group)
- **Year / Venue:** 2023 · PMC10126115
- **Link / DOI:** https://pmc.ncbi.nlm.nih.gov/articles/PMC10126115/
- **Relevance:** **7/10** — the strongest **true artery-and-vein** optical sO₂ demonstration, in the retinal microvasculature (retinal-vein sO₂ ~48–72 % depending on study; ex-vivo phantom bias ~1 % vs blood-gas, ~2.1 % vs pulse-oximeter in vivo).
- **Novelty:** Adaptively removes spectral contaminants per-vessel, letting vis-OCT recover absolute sO₂ under each vessel's unique conditions — the most accurate optical venous sO₂ figures in the corpus, albeit in a retinal vessel bed.
- **Integration insights:** Demonstrates that per-vessel adaptive spectral correction can push optical venous sO₂ to blood-gas-level accuracy — a template for the systemic-vein problem, though the retinal bed is not representative of central/systemic venous status. *Cross-confirmed via PMC + PubMed listings; full text 403 (flagged).*

### 2.5 — Conditioning Deep Anatomical Prior Knowledge for Reconstruction of Multispectral Optoacoustic Tomography Images (APRECOT) *(previously surfaced — newly catalogued 07-17 §2.4; transferable technique, not venous-specific, in-silico only)*
- **Authors:** Sarah Franceschin, Lukas Imanuel Scheel-Platz, Philipp Haim, Guillaume Zahnd, Vasilis Ntziachristos, Dominik Jüstel
- **Year / Venue:** 2026 (arXiv preprint, June 2026) · arXiv:2606.16835 (TU Munich / Helmholtz Munich / iThera Medical)
- **Link / DOI:** https://arxiv.org/abs/2606.16835
- **Relevance:** **5/10** — MSOT reconstruction methodology; not a venous measurement, but aimed squarely at the quantitative-oxygenation inverse problem that gates PA venous sO₂. In-silico proof-of-concept only.
- **Novelty:** Conditions reconstruction on probabilistic anatomical priors to jointly segment tissues and recover their bulk chromophore (oxygenation) composition, attacking the ill-posed, fluence-dependent MSOT inverse problem directly; strongly improved bulk-chromophore accuracy on in-silico data.
- **Integration insights:** Where APM+ (§2.2) fixes fluence *locally* with an arterial reference, APRECOT tries to fix it *globally* with anatomical structure priors — a complementary attack on the same barrier keeping deep PA venous sO₂ from being quantitative. Watch for an in-vivo follow-up on forearm/neck artery+vein anatomy. *Authors/title/abstract cross-confirmed via arXiv listing + search snippet; full text 403 (flagged). Still in-silico — flagged as not yet experimentally validated.*

**Standing context (not scored in the top-5 this cycle):** the **DPF-model** preprint (arXiv:2602.00283, 2026 — CW-NIRS pathlength quantitation, catalogued 07-17 §2.5, underpins every transcutaneous-NIRS venous method above), **Hybrid-Net** (Deep-Learning-Driven Quantitative Spectroscopic PA Imaging, arXiv:2512.15394, Dec 2025), the **sulfate blood-phantom** metrology paper (arXiv:2512.01458), the high-resolution **hyperspectral retinal imaging** system (PMC12997856, 2026), **SFDI-net** deep-learning spatial-frequency-domain skin oxygenation (PMC12014942), the flexible optoacoustic "blood stethoscope" patch, PA-TEE mixed-venous monitoring, and **"Distribution-informed and wavelength-flexible data-driven photoacoustic oximetry"** (arXiv:2403.14863, 2024 — a wavelength-flexible learned PA-oximetry technique surfaced in today's sweep; transferable but **not venous-specific** and not new, so held in context rather than scored). All previously surfaced or out-of-scope; none updated this cycle.

---

## Cross-topic synthesis

**1. The signal today is a catalogue gap closed, not a new publication.** No venous-specific or technique paper has appeared since 07-17. But the sweep filled a real hole in Topic 1: the **Belhaj/Kyriacou PPG peripheral-venous line (§1.2)** — a true non-invasive venous method **validated against venous co-oximetry**, with published limits of agreement (r = 0.81, bias +5.65 ± 14.3 %). It is the missing reference-standard bookend to the Alqahtani jugular optical sensor (§1.1), which has better waveform isolation but only n=3 and no blood-gas reference. Together they now define the peripheral-venous-optical problem from both the *device* and the *validation* ends.

**2. The through-line remains fluence / pathlength / spectral coloring.** Every scored optical method — the IJV-PA anchor (§2.1), APM+ (§2.2), vis-OCT (§2.4), the IJV DNN+Monte-Carlo work (§1.3), the jugular-NIRS devices (§1.4) — lives or dies on how well fluence/pathlength is handled, and the newest technique preprints (APRECOT, DPF) are direct upstream investments in exactly that. The PPG method (§1.2) sidesteps fluence entirely by working in the ratio-of-ratios regime — which is why it is robust enough to reach co-oximetry validation but too coarse (±14 % LoA) to displace a catheter.

**3. Three calibration strategies, still separable.** (a) *Physical internal reference* — APM+'s neighbouring artery (§2.2), the MRI RV/LV ratio (§1.5), and the PPG artery-vs-vein compliance contrast (§1.2). (b) *Learned/simulation prior* — the DNN+Monte-Carlo IJV work (§1.3), the SSL intra-cardiac MR preprint, APRECOT's probabilistic anatomy. (c) *Better forward physics* — the DPF model. A convincing wearable venous oximeter will likely need two of the three; no single-paper method yet combines them.

**4. The sparseness verdict holds, honestly.** Topic 1's true-SvO₂ literature produced nothing *newly published* for the fifth consecutive scan cycle; today's addition is an older-but-uncatalogued paper, not fresh work. Topic 2's genuine novelty remains the two 07-17 technique preprints, both technique-level and (for APRECOT) in-silico. **Persisting gaps, carried forward and still open:** (i) no non-invasive optical/PA SvO₂ method has been validated against invasive co-oximetry in a *large* cohort with tight limits of agreement (Alqahtani n=3; APM+ n=8 healthy; Belhaj ±14 % LoA); (ii) no method yet fuses an internal reference + learned prior + corrected forward physics; (iii) the retinal vis-OCT/hyperspectral line has the best *true venous* optical accuracy but in a vessel bed not representative of systemic/central venous status. Today moved the needle on (i)'s *documentation* (the Belhaj co-oximetry benchmark), not on (ii) or (iii).

---

*Scan generated 2026-07-19 (UTC). One older venous-specific paper newly catalogued (§1.2 Belhaj/Kyriacou PPG-vs-co-oximetry); no new publications since 2026-07-17; all other entries previously surfaced and carried forward with scores unchanged. Publisher full-text access was 403-blocked in this environment; every reference was cross-checked across ≥2 independent search-index snippets, with per-item verification notes and flags above.*
