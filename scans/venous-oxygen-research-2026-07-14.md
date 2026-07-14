# Venous Oxygen Research Scan — 2026-07-14

**Search window:** Twenty-fourth scan in the series, run **one day** after 2026-07-13. Emphasis on work published or first-surfacing after 07-13, with the standard fallback to the best-available venous-specific work already catalogued. Sources searched today: PubMed/PMC, arXiv, bioRxiv/medRxiv, Optica (Biomed. Opt. Express, Optics Letters, Applied Optics, Optics Express), SPIE / *J. Biomed. Opt.*, *Photoacoustics* (ScienceDirect), IEEE Xplore, Nature / *Sci. Rep.*, Wiley (*Advanced Science*, *J. Biophotonics*), MDPI (*Biosensors*, *Sensors*), IOPscience, Springer, De Gruyter, ClinicalTrials.gov, ResearchGate, Semantic Scholar, QuantumZeitgeist.

**Verification caveat:** As in every prior scan, publisher **full-text** pages — including arxiv.org, opg.optica.org, pmc.ncbi.nlm.nih.gov, sciencedirect.com and the Wiley/Nature domains — returned **HTTP 403** to direct `WebFetch` in this environment today (re-confirmed on arxiv.org/abs/2510.27487). Every reference below was therefore cross-checked across **at least two independent search-index snippets**; per-item notes state what was confirmed and what could not be read directly on a publisher page.

---

## ⚠️ Read this first — day summary

**Two genuinely new items today, and one of them is a rare true venous-optical paper.** Today's sweep surfaced two papers not previously catalogued in this series:

- **NEW (Topic 1, flagship):** *Automatic photoacoustic monitoring of perinatal brain hypoxia with superior sagittal sinus detection* (Jiang et al., *J. Biomed. Opt.* **30(7):076004**, posted **2025-07-11**). This is a **transcranial photoacoustic** method that measures oxyhemoglobin saturation at the **superior sagittal sinus (SSS)** — a large cerebral **vein** — making it a genuinely on-topic non-invasive **venous-optical** paper, not an arterial surrogate. It leads Topic 1.
- **NEW (Topic 2):** *Towards robust quantitative photoacoustic tomography via learned iterative methods* (Manninen, Gröhl, Lucka et al., arXiv **2510.27487**, posted Oct 2025). A qPAT reconstruction-methodology paper — technique, not venous-specific — that directly bears on the fluence-correction bottleneck all photoacoustic sO₂ (arterial *and* venous) work must solve.

Everything else returned today is **previously surfaced** (jugular optical sensing, DNN+Monte-Carlo SijvO₂, self-supervised MRI oximetry, APM arterial-mediated deep-tissue PA oximetry, vis-OCT retinal oximetry, Hybrid-Net spectroscopic PA, ovarian-lesion PAT spectral/depth compensation). Consistent with the series' standing observation, **truly novel non-invasive venous-optical work is published at very low volume**; today is a comparatively good day (one true venous-optical item), but it does not change the overall picture. Lists below combine today's new items with the best-available standing set, each older item honestly flagged as previously surfaced with its relevance score unchanged.

---

## Topic 1 — Non-invasive monitoring of venous blood oxygen (SvO₂ / ScvO₂ / cerebral & peripheral venous)

### 1.1 — ★ NEW — Automatic photoacoustic monitoring of perinatal brain hypoxia with superior sagittal sinus detection
- **Authors:** Baichuan Jiang, Ernest Graham, Mathias Unberath, Russell H. Taylor, Raymond C. Koehler, Jeeun Kang, Emad M. Boctor (Johns Hopkins University / JHMI)
- **Year:** 2025 (published **2025-07-11**)
- **Venue:** *Journal of Biomedical Optics* **30(7):076004** (SPIE)
- **Link / DOI:** https://doi.org/10.1117/1.JBO.30.7.076004 — PMC: https://pmc.ncbi.nlm.nih.gov/articles/PMC12245645/
- **Relevance:** **9/10** for non-invasive venous O₂ — the SSS is a true cerebral vein, so this measures venous-side sO₂ non-invasively and optically. First-surfacing in this series today.
- **Novelty:** Validates **transcranial photoacoustic** oxyhemoglobin-saturation measurement at the **superior sagittal sinus** in the neonatal piglet brain and, critically, **automates the PA workflow** — automatic detection/tracking of the SSS target so the system can run **fully autonomous, continuous** perinatal monitoring rather than requiring an operator to hand-place the acoustic window. The automation (SSS auto-detection via the imaging pipeline) is the genuinely new contribution over the group's earlier fixed-target SSS validation work.
- **Integration insights:** This is exactly the archetype the program is chasing on the optical side — a **non-invasive optical readout of a specific vein's O₂ saturation**, here the cerebral venous compartment that reflects global cerebral O₂ extraction. The autonomous-targeting piece is directly transferable to the peripheral/jugular optical-SvO₂ devices in 1.3–1.4: those methods' open problem is reliably locating and holding on the venous target, which is precisely what this SSS auto-detection addresses. Pairs naturally with the DNN+Monte-Carlo jugular inversion (1.3) as the "acquire the vein → invert to SvO₂" two-step. *Metadata (title, authors, venue, DOI, date) confirmed across two independent search snippets; full text not readable directly (PMC/SPIE 403).*

### 1.2 — Leveraging Self-Supervised Learning for Non-Invasive Intra-Cardiac Magnetic Resonance Oximetry Assessment *(previously surfaced — scan 07-13 §1.1)*
- **Authors:** Jiayuan Chen, Thai-Hoang Pham, Ping Zhang, Juliet Varghese
- **Year:** 2026 (preprint posted 2026-07-01)
- **Venue:** medRxiv (preprint, not peer-reviewed)
- **Link / DOI:** https://www.medrxiv.org/content/10.64898/2026.06.29.26356860v1.full — DOI `10.64898/2026.06.29.26356860`
- **Relevance:** **7/10** for non-invasive venous O₂; **3/10** for the optical thrust (it is MRI, not optical).
- **Novelty:** Self-supervised (contrastive + masked-image-modeling) pre-training on >48,000 cardiac images, fine-tuned for **O₂-saturation regression with uncertainty quantification** (MAE ≈ 3.70). Recovers chamber-level (intra-cardiac) mixed-venous SvO₂ non-invasively.
- **Integration insights:** A **reference-grade** non-invasive mixed-venous O₂ target and a label-scarce ML recipe (SSL + per-estimate uncertainty) that is directly portable to the optical side, where in-vivo SvO₂ labels are the binding constraint. Cross-modality validation target for optical devices.

### 1.3 — Estimation of Venous Oxygen Saturation Through Non-Invasive Optical Sensing at the Jugular Veins *(previously surfaced — scan 06-10 §1.1; the flagship optical-venous device paper)*
- **Year:** 2024
- **Venue:** *Current Directions in Biomedical Engineering* (De Gruyter), CDBME
- **Link / DOI:** https://www.degruyterbrill.com/document/doi/10.1515/cdbme-2024-2072/html — DOI `10.1515/cdbme-2024-2072`
- **Relevance:** **9/10** — direct, non-invasive, optical, venous.
- **Novelty:** Pulse-oximeter-style optical sensor at the **external jugular vein**; identifies the EJV waveform and returns SvO₂ estimates in the healthy 60–90% band. Closest thing to a wearable-form-factor optical SvO₂ device in the literature.
- **Integration insights:** The reference architecture for peripheral optical SvO₂. Its open problem — calibration against blood-gas gold standard, plus reliable venous-target acquisition — is exactly what today's SSS auto-detection (1.1) and the reference-grade MRI (1.2) help close.

### 1.4 — Quantifying Changes in Oxygen Saturation of the Internal Jugular Vein In Vivo Using Deep Neural Networks and Subject-Specific 3-D Monte-Carlo Models *(previously surfaced — scan 06-10 §1.2)*
- **Year:** 2024
- **Venue:** *Optics Letters* 49(10):2669
- **Link / DOI:** https://opg.optica.org/ol/abstract.cfm?uri=ol-49-10-2669
- **Relevance:** **8/10** — non-invasive optical, internal-jugular, SijvO₂.
- **Novelty:** Models reflectance→ΔSijvO₂ with **subject-specific 3-D Monte-Carlo** forward simulation, then trains a **DNN** to invert it — sidestepping the labelled-data bottleneck via simulation.
- **Integration insights:** The simulation-to-DNN inversion is the methodological twin of 1.2's SSL approach and pairs with 1.1's acquisition automation to form a complete jugular-SvO₂ pipeline.

### 1.5 — Non-invasively Measured Venous Oxygen Saturation as Early Marker of Impaired Oxygen Delivery in Preterm Neonates *(previously surfaced — catalogued in prior scans)*
- **Venue:** *Frontiers in Pediatrics* / PMC (PMC8831784)
- **Link:** https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8831784/
- **Relevance:** **7/10** — NIRS venous-occlusion SvO₂ in a real patient population.
- **Novelty:** Uses NIRS-based non-invasive SvO₂ as an **early physiological marker** of impaired O₂ delivery in preterm neonates — a concrete clinical use-case for continuous venous-O₂ trending.
- **Integration insights:** Establishes clinical value (neonatal ICU) and the venous-occlusion NIRS technique a wearable optical SvO₂ device would operationalize. Note the neonatal overlap with today's new SSS-PA paper (1.1) — both target the newborn brain/venous compartment, one via NIRS, one via photoacoustics.

---

## Topic 2 — Optical imaging techniques for non-invasively obtaining venous blood oxygen

### 2.1 — ★ NEW — Towards robust quantitative photoacoustic tomography via learned iterative methods
- **Authors:** Anssi Manninen (Univ. of Oulu), Janek Gröhl (UMC Göttingen / MPI-NAT), Felix Lucka (CWI), et al.
- **Year:** 2025 (arXiv preprint, posted October 2025)
- **Venue:** arXiv (preprint) — **2510.27487**
- **Link / DOI:** https://arxiv.org/abs/2510.27487
- **Relevance:** **6/10** for venous O₂ specifically — this is a **technique/reconstruction** paper, not venous-targeted, but qPAT sO₂ (arterial *and* venous) is its downstream purpose; **8/10** as a Topic-2 optical-imaging method.
- **Novelty:** Combines **model-based iterative reconstruction** with learned components ("learned iterative methods") to make quantitative PAT robust with **limited training data** — the standing weakness of purely data-driven qPAT sO₂ estimators, which overfit to their simulated training distribution and degrade on real, heterogeneous tissue. Hybridizing physics (the PAT forward operator) with learning is aimed squarely at generalization.
- **Integration insights:** Every photoacoustic venous-sO₂ method — including today's SSS-PA paper (1.1) and the APM arterial-mediated approach (2.3) — ultimately depends on correcting for unknown, wavelength-dependent optical **fluence** to turn measured pressure into true sO₂. This paper attacks that inversion generically and with data-efficiency, so a robust learned-iterative qPAT backbone would directly improve the accuracy of any deep-tissue venous sO₂ readout. Methodologically it is the "physics + learning" counterpart to the Monte-Carlo+DNN jugular work (1.4). *Title/authors/ID confirmed across arxiv listing + QuantumZeitgeist summary; abstract not readable directly (arxiv 403).*

### 2.2 — Arterial Blood-Mediated Deep-Tissue Photoacoustic Oximetry (APM⁺) *(previously surfaced — scan 06-30 & later)*
- **Authors:** Sastry et al.
- **Year:** 2026
- **Venue:** *Advanced Science* (Wiley)
- **Link / DOI:** https://advanced.onlinelibrary.wiley.com/doi/10.1002/advs.76366 — DOI `10.1002/advs.76366`
- **Relevance:** **7/10** — deep-tissue PA oximetry; arterial-anchored but explicitly used to **estimate venous sO₂**, so directly transferable.
- **Novelty:** Uses the **arterial photoacoustic measurement (APM)** as an in-situ fluence reference to recover deep-tissue sO₂, including a route to **venous** sO₂ — turning the arterial signal into a self-calibration for the harder venous target.
- **Integration insights:** Its arterial-as-reference calibration is a concrete answer to the fluence problem that 2.1 attacks generically; the two are complementary (physical reference vs. learned reconstruction). Directly informs deep venous sO₂ recovery where no surface waveform is available.

### 2.3 — Deep Learning-Driven Quantitative Spectroscopic Photoacoustic Imaging (Hybrid-Net) for Segmentation and Oxygen Saturation Estimation *(previously surfaced — scan 06-14 & later)*
- **Year:** 2025 (arXiv 2512.15394)
- **Venue:** arXiv (preprint)
- **Link:** https://arxiv.org/abs/2512.15394
- **Relevance:** **6/10** — spectroscopic PA sO₂ + vessel segmentation; not venous-specific but vessel-resolved.
- **Novelty:** A single network (**Hybrid-Net**) jointly segments vessels and estimates sO₂, coupling structure and function so fluence-affected estimates can be regularized per-vessel.
- **Integration insights:** Vessel-type segmentation is a prerequisite to labeling a vessel arterial vs. **venous**; joint segmentation+sO₂ is the natural front-end for an automated venous-sO₂ PA pipeline (cf. 1.1's SSS auto-detection).

### 2.4 — Adaptive Spectroscopic Visible-Light OCT for Clinical Retinal Oximetry *(previously surfaced — catalogued in prior scans)*
- **Venue:** *Biomedical Optics Express* / PMC (PMC10126115)
- **Link:** https://www.ncbi.nlm.nih.gov/pmc/articles/PMC10126115/
- **Relevance:** **7/10** — resolves **retinal venous** sO₂ (~72%) distinctly from arterial (~95%), with ~1% bias vs blood-gas after spectral-contaminant removal.
- **Novelty:** Adaptive removal of spectral contaminants lets vis-OCT recover accurate sO₂ across 0–100%, separating arterial and **venous** vessels label-free in one modality (oximetry + angiography + flowmetry).
- **Integration insights:** The clearest existing demonstration of **vessel-resolved venous** optical oximetry in humans; the spectral-contaminant framework is portable to any spectroscopic optical sO₂ method needing to isolate the venous signal.

### 2.5 — Integrated Spectral and Depth Compensation for Oxygen Saturation and Total Hemoglobin Estimation in Photoacoustic Tomography (ovarian lesions) *(previously surfaced — scan 07-09 & later)*
- **Year:** 2026 (*J. Biomed. Opt.*, Feb 2026)
- **Venue:** *Journal of Biomedical Optics* / PMC (PMC12869027)
- **Link:** https://www.ncbi.nlm.nih.gov/pmc/articles/PMC12869027/
- **Relevance:** **6/10** — depth/spectral fluence compensation for PAT sO₂; disease-application (ovarian), not venous-targeted.
- **Novelty:** Couples **spectral** and **depth** compensation to correct wavelength- and depth-dependent fluence in PAT sO₂/tHb estimation — a concrete instance of the correction problem 2.1 generalizes.
- **Integration insights:** Depth compensation matters specifically for **deep veins**, where fluence attenuation is severe; the method is transferable to a deep venous-sO₂ target even though it was demonstrated on lesions.

---

## Cross-topic synthesis

Today's two new items sharpen a theme that has recurred across the whole series: **the barrier to non-invasive venous optical oximetry is no longer "can we see a vein" but "can we quantify its sO₂ robustly and autonomously."** The new SSS-photoacoustic paper (1.1) contributes the **acquisition/automation** half — reliably and autonomously locating a specific vein (the superior sagittal sinus) and tracking it for continuous monitoring — while the new learned-iterative qPAT paper (2.1) contributes the **quantification** half — data-efficient, physics-anchored reconstruction that turns measured pressure into trustworthy sO₂ despite unknown fluence. Read together, they map onto the two persistent gaps this program tracks:

1. **Target the vein, not the artery.** vis-OCT (2.4) already separates retinal venous from arterial sO₂ vessel-by-vessel; Hybrid-Net (2.3) and the SSS auto-detector (1.1) generalize "find and label the venous target" to deeper, larger vessels. Vessel-type identity is the gate that keeps venous work from collapsing into arterial SpO₂.

2. **Solve fluence to get true sO₂.** This is now attacked from three converging directions — a **physical arterial reference** (APM⁺, 2.2), **explicit spectral+depth compensation** (2.5), and **learned-iterative reconstruction** (2.1) — while the Monte-Carlo+DNN jugular work (1.4) and the self-supervised MRI oximetry recipe (1.2) address the same underlying "no in-vivo venous labels" problem from the data side.

**Honesty note on volume:** even on a comparatively productive day, only **one** of today's two new items is genuinely venous-specific-and-optical (1.1); the other (2.1) is enabling methodology. The rest of both lists is the standing best-available set, unchanged. Truly novel non-invasive venous-optical work continues to appear at low volume, and the highest-leverage near-term move remains **combining an established venous-target acquisition front-end (jugular optical sensing / SSS-PA) with a robust fluence-corrected quantification back-end (learned-iterative or arterial-referenced qPAT), validated against a reference-grade non-invasive venous standard (T2-CMR oximetry).**
