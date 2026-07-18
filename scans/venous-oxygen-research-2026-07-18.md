# Venous Oxygen Research Scan — 2026-07-18

**Search window:** Twenty-sixth scan in the series, run **one day** after 2026-07-17. Emphasis on work published or first-surfacing after 07-17, with the standard fallback to the best-available venous-specific work already catalogued. Sources searched today: PubMed/PMC, arXiv, bioRxiv/medRxiv, Optica (Biomed. Opt. Express, Optics Letters, Applied Optics), SPIE / *J. Biomed. Opt.*, *Photoacoustics* (ScienceDirect), IEEE Xplore, Nature / *Sci. Rep.* / *Eye*, Wiley (*Advanced Science*, *J. Biophotonics*), MDPI, Springer, De Gruyter, World Scientific (JIOHS), ClinicalTrials.gov, ResearchGate, Semantic Scholar, ADS.

**Verification caveat:** As in every prior scan, publisher **full-text** pages — including arxiv.org (re-confirmed today: `WebFetch` on arXiv `2607.07996` returned **HTTP 403 Forbidden**), pmc.ncbi.nlm.nih.gov, opg.optica.org, advanced.onlinelibrary.wiley.com, nature.com and the De Gruyter domains — remain **inaccessible to direct fetch** in this environment. Every reference below was therefore cross-checked across **at least two independent search-index snippets** (Google Scholar–style result blocks + arXiv listing / ResearchGate / PMC / Semantic Scholar). Per-item notes state what was confirmed and what could not be read directly on a publisher page.

---

## ⚠️ Read this first — day summary

**No new venous-specific *primary* paper today.** Consistent with the series' standing observation, truly novel non-invasive **venous**-optical work is published at very low volume, and today's one-day sweep produced no new SvO₂/ScvO₂/venous-imaging demonstration. The sweep did surface **two genuinely new arXiv preprints** (both first-appearing this cycle, neither in any prior scan file), but both are **arterial-only SpO₂ / PPG signal-processing** work:

- **NEW — SpO₂ Predictor-Guided Stage-Wise Time-Frequency Reconstruction of Low-Quality Dual-Wavelength PPG** (arXiv:2607.07996, July 2026): a reconstruction pipeline that repairs motion-/contact-corrupted red+IR PPG before SpO₂ estimation.
- **NEW — Low-Rate Wrist SpO₂ Estimation under Micro-Perturbations** (arXiv:2607.08001, July 2026): motion-aware beat selection + perfusion-index-guided calibration for weak-perfusion wrist PPG.

Per the task rule ("exclude arterial-only SpO₂ work unless its technique is directly transferable to venous — if so, include it and say why"), the stronger of the two (§2.4) is included and scored **honestly low (4/10)** because its *technique* — recovering a usable oxygenation ratio from a low-quality, weakly-pulsatile PPG signal — is exactly the signal-conditioning problem faced by the pulsatile-venous methods in this catalogue (the external-jugular EJV optical sensor and the artery/vein compliance-modulation SpvO₂ approach). The second (§2.5 standing context) is closely related. Neither measures a vein.

Everything else returned by the sweep is **previously surfaced** or out-of-scope: the Alqahtani jugular optical sensor, the IJV DNN + Monte-Carlo work, Mespere VO100 jugular NIRS, the McDiarmid MRI iSvO₂ model, the SSL intra-cardiac MR oximetry preprint, the IJV-PA anchor, APM+, PACT venous-flow work, APRECOT (arXiv:2606.16835), the DPF-model preprint (arXiv:2602.00283), the PINN spectral-unmixing preprint (arXiv:2602.16357), Hybrid-Net (arXiv:2512.15394), the sulfate-phantom paper (arXiv:2512.01458), the JIOHS PACT-oximetry review (S1793545826300065), the CHEST "emerging technology" review, the Sci. Rep. SFDI multimodal-comparison paper, the ML-VO₂ wearable-PPG paper, and the vis-OCT / hyperspectral retinal-oximetry line. No new primary venous demonstration this cycle.

---

## Topic 1 — Non-invasive monitoring of venous blood oxygen (SvO₂ / ScvO₂ / peripheral venous)

*No new items today.* The standing best-available set (all previously surfaced) with scores carried forward. This remains the sparse topic: **no primary non-invasive venous-O₂ measurement paper has first-surfaced since 2026-07-15** — now the fifth consecutive scan cycle without a new Topic-1 primary.

### 1.1 — Estimation of Venous Oxygen Saturation Through Non-Invasive Optical Sensing at the Jugular Veins *(previously surfaced — scan 06-10 §1.1; flagship optical-venous device paper)*
- **Authors:** Alqahtani et al.
- **Year / Venue:** 2024 · *Current Directions in Biomedical Engineering* 10(2) (De Gruyter; CDBME-2024-2072)
- **Link / DOI:** https://doi.org/10.1515/cdbme-2024-2072
- **Relevance:** **8/10** — true, non-invasive, optical, venous (but n=3, no invasive co-oximetry reference).
- **Novelty:** A pulse-oximeter-style optical sensor over the external jugular vein isolates the EJV waveform and returns SvO₂ estimates (71.1 %, 72.2 %, 70.4 %) within the healthy 60–90 % band — still the closest thing to a wearable-form-factor optical SvO₂ device in the literature.
- **Integration insights:** The superficial/low-cost optical analogue of the deep IJV-PA anchor (§2.1); together they bracket the venous-optical problem from the shallow and deep ends. Its open problem — calibration against a blood-gas gold standard — is exactly what the APM+ artery-as-reference approach (§2.2) and MRI reference oximetry (§1.4) aim to close. **Directly relevant to today's NEW PPG-reconstruction preprint (§2.4):** the EJV waveform this sensor extracts is precisely the kind of weak, easily-corrupted pulsatile signal that §2.4's reconstruction pipeline is designed to salvage. *Metadata cross-confirmed via De Gruyter listing + ResearchGate (publication 387159780); full text not directly fetchable (flagged).*

### 1.2 — Quantifying Changes in Oxygen Saturation of the Internal Jugular Vein In Vivo Using Deep Neural Networks and Subject-Specific 3-D Monte-Carlo Models *(previously surfaced — scan 06-10 §1.2)*
- **Authors:** (multi-author; NIRS + DNN group)
- **Year / Venue:** 2024 · *Optics Letters* 49(10):2669
- **Link / DOI:** https://opg.optica.org/ol/abstract.cfm?uri=ol-49-10-2669
- **Relevance:** **7/10** — IJV-specific, non-invasive, inverse-modeling for venous saturation *change*.
- **Novelty:** Multi-channel NIRS + DNNs trained on subject-specific 3-D Monte-Carlo forward models recover ΔSijvO₂ non-invasively, tying measured reflectance to a physically-modelled forward problem — sidestepping the labelled-data bottleneck via simulation.
- **Integration insights:** The inverse-modeling / fluence-correction leg of the program; the physics-simulation twin of the self-supervised-learning approach in §1.3. Its accuracy is bounded by the pathlength/fluence assumptions the standing DPF-model preprint (arXiv:2602.00283) reformulates. *Cross-confirmed via Optica listing + Semantic Scholar; full text not directly fetchable (flagged).*

### 1.3 — Leveraging Self-Supervised Learning for Non-Invasive Intra-Cardiac Magnetic Resonance Oximetry Assessment *(previously surfaced — scan 07-13 §1.1; MRI, not optical)*
- **Authors:** Jiayuan Chen, Thai-Hoang Pham, Ping Zhang, Juliet Varghese
- **Year / Venue:** 2026 (preprint posted 2026-07-01) · medRxiv
- **Link / DOI:** https://www.medrxiv.org/content/10.64898/2026.06.29.26356860v1.full — DOI `10.64898/2026.06.29.26356860`
- **Relevance:** **7/10** for non-invasive venous O₂; **3/10** for the optical thrust of Topic 2 (MRI, not optical).
- **Novelty:** Self-supervised pre-training (contrastive + masked image modeling) on >48,000 cardiac images, then fine-tuning for O₂-saturation regression **with uncertainty quantification** (MAE ≈ 3.70; claimed >15 % improvement over baselines). Recovers chamber-level (intra-cardiac) blood O₂ — true mixed-venous SvO₂ — non-invasively and reference-grade.
- **Integration insights:** The label-scarce SSL + uncertainty recipe is **directly portable** to the optical side, where labelled in-vivo SvO₂ ground truth is the binding constraint (cf. §1.2). Value as a cross-modality **validation target** and transferable ML methodology. *Metadata confirmed across two search snippets; abstract not directly readable (flagged).*

### 1.4 — Development and Validation of a Noninvasive Model of Mixed Venous Oxygen Saturation in Heart Failure (imaging-derived iSvO₂) *(previously surfaced — scan 07-07 §1.1)*
- **Authors:** McDiarmid et al.
- **Year / Venue:** 2025/2026 · *JACC: Advances*
- **Link / DOI:** https://doi.org/10.1016/j.jacadv.2025.102484 · PMC12869880 · PMID 41609283
- **Relevance:** **7/10** — true mixed-venous, non-invasive, clinically validated (MRI, not optical).
- **Novelty:** 628-patient validation of an imaging-derived mixed-venous SvO₂ from the RV/LV blood-pool T₂ ratio on cardiac MRI (R = 0.82 vs invasive SvO₂), anchored to right-heart catheterization and an independent predictor of mortality/HF-hospitalization.
- **Integration insights:** Sets the **absolute-accuracy and outcome-relevance benchmark** any optical SvO₂ method must match, in exactly the population (heart failure) where a cheap continuous optical surrogate would be most valuable. Its internal-reference (RV vs LV) logic recurs on the optical side as artery-vs-vein calibration (§2.2). *Cross-confirmed via JACC/ScienceDirect + PMC + PubMed; full text not directly fetchable (flagged).*

### 1.5 — A New Non-Invasive Method for the Assessment of Central Venous Oxygen Saturation (Mespere VO100 jugular NIRS) *(previously surfaced — scan 06-10 §1.3)*
- **Authors:** (critical-care cohort study)
- **Year / Venue:** 2023 · *J. Cardiothoracic and Vascular Anesthesia* (S1053-0770(23)00782-6)
- **Link / DOI:** https://www.sciencedirect.com/science/article/pii/S1053077023007826 · PMID 37827917
- **Relevance:** **7/10** — non-invasive NIRS surrogate for ScvO₂, clinical cohort.
- **Novelty:** Validates transcutaneous jugular NIRS (Mespere VO100) against invasive ScvO₂ in critically ill patients, reporting strong linear correlation with low bias/percentage error; supports using SjvO₂ as a non-invasive surrogate of ScvO₂.
- **Integration insights:** The most clinically-mature non-invasive venous-NIRS device line — the practical baseline on bias and limits-of-agreement any optical/PA method must beat. Its accuracy floor is set by the CW-NIRS pathlength assumptions the standing DPF-model preprint targets. *Cross-confirmed via ScienceDirect + PubMed 37827917; full text not directly fetchable (flagged).*

**Standing context (not scored in the top-5):** jugular transcutaneous NIRS in pediatric cardiac surgery (r = 0.91 vs ScvO₂, bias 2.92 %; PMC7491293), respiration-frequency-selected NIRS for cerebral SvO₂ (PMC4126245 / PMID 24439329), capnodynamic mixed-venous SvO₂ (NCT06632197; PMID 34609659), the preterm-neonate NIRS venous-occlusion series (PMC8831784), and the CHEST 2025 "Emerging Technology for Noninvasively Measuring Oxygen Saturations" review (S0012-3692(25)05393-0) — all previously catalogued, none updated this cycle.

---

## Topic 2 — Optical imaging techniques for non-invasively obtaining venous blood oxygen (PA/PACT, NIRS, DOI/DOT, hyperspectral, vis-OCT, SFDI)

One **new** transferable-technique preprint this cycle (§2.4), slotted below the standing venous-specific anchors and scored honestly low; a closely-related second new preprint is noted in standing context.

### 2.1 — Noninvasive In Vivo Photoacoustic Measurement of Internal Jugular Venous Oxygenation in Humans *(previously surfaced — scan 06-10 §2.1; the Topic-2 anchor)*
- **Authors:** (PA/US group; arXiv:2303.10775)
- **Year / Venue:** 2023 · arXiv preprint / SPIE lineage (cf. 2014 SPIE 8943E..1MG)
- **Link / DOI:** https://arxiv.org/abs/2303.10775
- **Relevance:** **9/10** — true, non-invasive, optical/PA, deep **named-vein** (IJV) sO₂ in humans. The single most on-target paper in the corpus.
- **Novelty:** Combined dual-wavelength photoacoustic + ultrasound imaging computes hemoglobin sO₂ of the internal jugular vein in vivo, non-invasively, in real time (re-confirmed today: sijvO₂ ≈ 72 ± 7 % in seven healthy volunteers) — the reference demonstration that deep venous PA oximetry is physically achievable in humans.
- **Integration insights:** The deep-vein anchor that everything else is measured against; APM+ (§2.2), APRECOT, and the DPF model are all, in different ways, attempts to make this kind of measurement quantitative and fluence-robust without an ultrasound co-registration crutch. *Metadata cross-confirmed via arXiv + ADS + Science.gov topic page; full text not directly fetchable (flagged).*

### 2.2 — Arterial Blood-Mediated Deep-Tissue Photoacoustic Oximetry (APM+): in-vivo human radial-vein sO₂ *(previously surfaced — upgraded 07-15 §2.2)*
- **Authors:** Sastry et al.
- **Year / Venue:** 2026 · *Advanced Science* (Wiley)
- **Link / DOI:** https://doi.org/10.1002/advs.76366
- **Relevance:** **8/10** — a bona-fide non-invasive optical/PA venous-oximetry demonstration in humans (radial-vein median sO₂ 72.3 %, IQR 8.9 %, n=8 healthy adults).
- **Novelty:** Uses the neighbouring radial **artery** as an in-situ fluence calibrator to circumvent spectral coloring, then reports the adjacent **vein's** sO₂ in the physiological 60–80 % band. Phantom/ex-vivo median estimation error 2.9 % vs 9.8 % for linear unmixing — the artery-as-reference trick made to work in vivo.
- **Integration insights:** The clearest worked example of internal-reference calibration on the optical side, mirroring the RV/LV reference logic of the MRI iSvO₂ model (§1.4). The fluence-calibration problem it solves locally is the same one APRECOT attacks globally with anatomical priors. *Metadata cross-confirmed via Wiley + arXiv oximetry search snippets; full text not directly fetchable (flagged).*

### 2.3 — Oxygenation Heterogeneity Facilitates Spatiotemporal Flow-Pattern Visualization Inside Human Blood Vessels Using Photoacoustic Computed Tomography *(previously surfaced — scan 06-11 §2.2)*
- **Authors:** (PACT group)
- **Year / Venue:** 2024/2025 · PACT human-vessel study
- **Link / DOI:** (PACT venous-flow paper; see scan 06-11 for DOI) — cross-referenced via PMC/ADS
- **Relevance:** **7/10** — non-invasive PACT resolving intravascular oxygenation heterogeneity in human veins.
- **Novelty:** Shows that oxygenation gradients inside a vessel can be used as endogenous contrast to visualize flow patterns, implicitly demonstrating spatially-resolved venous sO₂ within a single vessel lumen.
- **Integration insights:** Argues venous sO₂ is not a single number but a spatial field — relevant to how any wearable device should sample a vein, and to how bulk-chromophore reconstruction methods should model a lumen. *Cross-confirmed via prior-scan record + search snippet; full text not directly fetchable (flagged).*

### 2.4 — ★ NEW — SpO₂ Predictor-Guided Stage-Wise Time-Frequency Reconstruction of Low-Quality Dual-Wavelength PPG for Oxygen Saturation Estimation *(newly catalogued this cycle — arterial SpO₂, included as a transferable technique)*
- **Authors:** (arXiv:2607.07996; PPG/pulse-oximetry signal-processing group — author list not readable on the 403-blocked listing, flagged)
- **Year / Venue:** 2026 (arXiv preprint, July 2026) · arXiv:2607.07996
- **Link / DOI:** https://arxiv.org/abs/2607.07996
- **Relevance:** **4/10** — arterial SpO₂, **not** a venous measurement; included because the *signal-conditioning technique* is directly transferable to pulsatile-venous optical oximetry. Method/algorithm paper, no venous data.
- **Novelty:** A **stage-wise time-frequency reconstruction** pipeline, *guided by an SpO₂ predictor*, that repairs low-quality red+IR PPG corrupted by motion, unstable skin contact, and variable optical coupling — restoring the pulsatile/baseline ratio (R-value) that downstream SpO₂ estimation depends on. Rather than discarding bad segments, it reconstructs a usable signal before the ratio is computed.
- **Integration insights:** **Why it's in-scope:** the two non-arterial optical methods in this catalogue that rely on a *pulsatile* signal — the external-jugular EJV optical sensor (§1.1) and the artery/vein-compliance-modulation SpvO₂ approach — both extract a venous waveform that is intrinsically weaker and more artifact-prone than an arterial finger PPG. A predictor-guided reconstruction that rescues a degraded ratio is exactly the front-end those methods need to move from n=3 feasibility toward robust wearable use. It does nothing for the fluence/spectral-coloring problem that dominates the *photoacoustic* venous methods (§2.1–2.3) — its leverage is specifically on the PPG-style pulsatile-venous branch. Scored 4/10 because the transfer is plausible and useful but unproven on venous signals. *Title and abstract framing cross-confirmed via arXiv listing + Semantic Scholar snippet; full text 403 and author list not verified (flagged).*

### 2.5 — vis-OCT / hyperspectral retinal oximetry line *(previously surfaced — standing true-venous optical anchor; no update this cycle)*
- **Representative work:** Adaptive spectroscopic **vis-OCT** retinal oximetry (ADS-vis-OCT; PMC10126115) and the high-resolution hyperspectral retinal-imaging system (PMC12997856, accepted Feb 2026 / published Mar 2026).
- **Year / Venue:** 2023–2026 · Optica (Biomed. Opt. Express / Optics Letters) and PMC.
- **Link / DOI:** https://pmc.ncbi.nlm.nih.gov/articles/PMC10126115/ · https://pmc.ncbi.nlm.nih.gov/articles/PMC12997856/
- **Relevance:** **7/10** — genuine **true artery-and-vein** optical sO₂ (retinal veins ≈ 72 % vs arteries ≈ 95 %), but in the retinal microvasculature, not a systemic/central vein.
- **Novelty:** vis-OCT resolves sO₂ down to single retinal vessels; ADS-vis-OCT agrees with a blood-gas machine to ~1 % bias in phantoms and ~2.1 % RMSE vs pulse oximeter for retinal arteries in humans. The 2026 hyperspectral system extracts vessel diameter and oxygenation simultaneously at high resolution.
- **Integration insights:** The strongest evidence that non-contact optical instruments can separate arterial from venous sO₂ at the single-vessel level and compute oxygen extraction — the capability a systemic venous oximeter ultimately needs, transplanted to a vessel bed that is optically accessible but not representative of central venous status. *Previously surfaced across multiple prior scans; unchanged today.*

**Standing context (not scored in the top-5 this cycle):**
- **★ NEW (arterial, standing) — Low-Rate Wrist SpO₂ Estimation under Micro-Perturbations Using Motion-Aware Beat Selection and Perfusion-Guided Calibration** (arXiv:2607.08001, July 2026). Newly surfaced this cycle; **arterial wrist SpO₂**, sibling to §2.4. Uses accelerometer data to select low-motion beats and the **perfusion index as a calibration-state indicator** to adapt the R–SpO₂ relationship across subjects. Transferable to the *weak-perfusion* regime that any wrist/limb venous optical sensor operates in; kept in standing context (score would be ~3–4/10) to avoid double-counting the same PPG-signal-quality theme as §2.4. *Title/abstract cross-confirmed via arXiv listing; full text 403 (flagged).*
- Standing PA/DOI technique preprints unchanged this cycle: **APRECOT** (anatomical-prior MSOT reconstruction, arXiv:2606.16835), the **DPF-model** CW-NIRS pathlength preprint (arXiv:2602.00283), the **PINN** spectral-unmixing preprint (arXiv:2602.16357), **Hybrid-Net** (arXiv:2512.15394), the **sulfate blood-phantom** paper (arXiv:2512.01458), and the **JIOHS** review "Quantitative oximetry with photoacoustic computed tomography" (S1793545826300065).
- Standing device/comparison work unchanged: the **SFDI** multimodal tissue-oxygenation comparison (Sci. Rep. s41598-025-15767-2), and the **ML-VO₂** multiwavelength-PPG wearable (PMC12024819).

---

## Cross-topic synthesis

**1. Today's only new signal is PPG signal-quality, on the arterial side.** Both genuinely-new items this cycle (§2.4, §2.5-standing) attack the same narrow problem — recovering a trustworthy oxygenation ratio from a **degraded, weakly-pulsatile PPG** (motion, contact, low perfusion). Neither measures a vein. They matter to this program only through **transfer**: the pulsatile-venous branch of the catalogue (the EJV optical sensor §1.1 and the compliance-modulation SpvO₂ method) lives on exactly the kind of weak, artifact-prone waveform these papers learn to rescue. This is a different lever from the fluence/spectral-coloring problem that dominates the photoacoustic branch — worth tracking, but not over-reading.

**2. The two enabling-problem families remain cleanly separable.** (a) *Fluence / spectral coloring* in deep PA and diffuse optics — addressed by APM+ (internal arterial reference, §2.2), APRECOT (anatomical priors), the DPF model (forward-physics), and the PINN unmixing preprint. (b) *Pulsatile-signal quality* in PPG-style venous oximetry — addressed, for the first time in this corpus, by today's §2.4 / §2.5-standing. A wearable venous oximeter that uses a pulsatile readout will need a solution from family (b); one that uses a spectroscopic/PA readout needs family (a). No single paper yet spans both.

**3. The sparseness verdict holds, and honestly.** Topic 1 (true SvO₂) produced nothing new for the **fifth consecutive scan cycle**; its top-5 is a stable, previously-surfaced set spanning optical (jugular sensor, jugular-NIRS) and reference-grade MRI/capnodynamic methods. Topic 2's only novelty this cycle is **arterial and algorithmic**, included solely on transferability and scored 4/10 accordingly. This is a low-volume day, reported as such — no arterial padding beyond the two items whose *technique* has a defensible venous application.

**4. Persisting gaps (carried forward, still open):** (i) no non-invasive optical/PA SvO₂ method has been validated against invasive co-oximetry in a large cohort with published limits-of-agreement (the Alqahtani sensor is n=3; APM+ is n=8 healthy); (ii) no method yet fuses an internal reference + learned prior + corrected forward physics into one venous measurement; (iii) the retinal vis-OCT/hyperspectral line has the best *true venous* optical accuracy but in a vessel bed not representative of systemic/central venous status. Today added a fourth watch-item — (iv) robust front-end signal conditioning for weak pulsatile-venous PPG — but moved the needle on none of (i)–(iii).

---

*Scan generated 2026-07-18 (UTC). One new item scored in the top-5 (§2.4, arXiv:2607.07996, arterial SpO₂ included on transferability); one further new preprint noted in standing context (arXiv:2607.08001). All other entries previously surfaced and carried forward with scores unchanged. Publisher full-text access (incl. arXiv) was 403-blocked in this environment; every reference was cross-checked across ≥2 independent search-index snippets, with per-item verification notes and flags above.*
