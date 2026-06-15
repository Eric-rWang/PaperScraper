# Daily Venous Oxygen Research Scan — 2026-06-15

**Scan scope:** Non-invasive venous blood oxygen monitoring (SvO₂ / ScvO₂ / peripheral & cerebral venous oxygenation) + optical imaging techniques for non-invasively obtaining venous blood oxygen (photoacoustic, NIRS, diffuse optics, hyperspectral, OCT/vis-OCT, SFDI).

**Prior scans consulted for de-duplication:** `2026-06-10`, `2026-06-11`, `2026-06-14`. Papers already surfaced in those files are NOT re-ranked as fresh finds; where a landmark recurs because nothing newer exists, it is explicitly flagged **[previously surfaced]**.

**Honesty note on sparseness:** Genuinely *venous-specific* non-invasive optical work continues to publish at very low volume. The three prior scans this cycle already captured the strongest venous-specific human studies (Hill jugular optical sensor; Sun DNN + Monte Carlo IJV NIRS; Jeleff/Mespere ScvO₂ validation; Garcia-Uribe/Wang IJV photoacoustic; the heart-failure SvO₂ model; transmissive hyperspectral single-vessel mapping). Today's truly-new yield is thin — **Topic 1 produced only ~2 genuinely new items; Topic 2 produced ~3.** Rather than pad with arterial-only SpO₂ work, the remaining slots are filled with standing landmarks, clearly flagged, so the ranking stays useful. Relevance is scored strictly against *non-invasive venous (not arterial) blood oxygen*. Tissue-level StO₂/SatO₂ (mixed arterio-venous bed) papers are flagged as such.

---

## Topic 1 — Non-invasive monitoring of venous blood oxygen (SvO₂ / ScvO₂ / peripheral & cerebral venous)

> **Verdict for today:** No new dedicated *venous-specific* optical sensor paper appeared since the 06-14 scan. The two new items below are clinical-context/review pieces that frame the demand for non-invasive ScvO₂; the strongest device-level venous papers remain those previously surfaced (re-listed with flags and honest scores).

### Paper 1.1 — NEW
**Title:** Less-Invasive Hemodynamic and Tissue Perfusion Monitoring in Sepsis and Septic Shock: A Narrative Review
**Authors:** Not individually verified from the publisher landing page (fetch blocked); MDPI author block unconfirmed — *flagged.*
**Year:** 2026
**Venue:** *Journal of Clinical Medicine* (MDPI), vol. 15, no. 5, art. 2061
**Link / DOI:** https://www.mdpi.com/2077-0383/15/5/2061
**Metadata verified:** Title, journal, volume/issue/article number confirmed via search result; author list and exact DOI not confirmed — *flagged.*
**Relevance score:** 6 / 10
**Novelty:** A 2026 narrative review of the shift away from invasive hemodynamic monitoring (PA catheter, central lines) toward less-/non-invasive perfusion and oxygenation assessment in sepsis. Positions continuous, non-invasive tissue-perfusion and venous-oxygenation surrogates as the emerging standard, and discusses the well-known limitation that ScvO₂ can read paradoxically normal/high in sepsis due to impaired cellular O₂ extraction.
**Integration insights:** Useful as a current (2026) demand-side anchor: it articulates *why* a robust non-invasive ScvO₂ readout matters clinically and where it fails (microcirculatory shunting), which directly motivates vessel-resolved optical approaches (photoacoustic / vis-OCT) that can target a named vein rather than a mixed tissue bed. Not a measurement-method paper — context only.

### Paper 1.2 — NEW (adjacent / metric utility)
**Title:** Central venous oxygen saturation vs. oxygen extraction ratio in septic shock resuscitation: which metric is more informative?
**Authors:** Not verified (publisher fetch blocked) — *flagged.*
**Year:** 2026
**Venue:** *Anesthesiology and Perioperative Science* (Springer)
**Link / DOI:** https://link.springer.com/article/10.1007/s44254-026-00177-y
**Metadata verified:** Title, journal, and DOI path confirmed via search; authors/issue unconfirmed — *flagged.*
**Relevance score:** 4 / 10
**Novelty:** Compares the diagnostic informativeness of ScvO₂ against the oxygen-extraction ratio (O₂ER) as resuscitation targets. Argues O₂ER may carry information ScvO₂ alone misses.
**Integration insights:** Relevant only indirectly: it concerns *which venous-derived quantity* to compute, not how to obtain it non-invasively. Worth noting because any non-invasive optical venous-oxygen platform should output O₂ER-compatible data (i.e., paired arterial SpO₂ + venous sO₂), not ScvO₂ in isolation. Included for completeness; weak on the non-invasive-optical axis.

### Paper 1.3 — **[previously surfaced — 2026-06-10, Paper 1.1]**
**Title:** Estimation of Venous Oxygen Saturation Through Non-Invasive Optical Sensing at the Jugular Veins
**Authors:** Jordan F. Hill, Jake Campbell, J. Geoffrey Chase, Christopher G. Pretty
**Year:** 2024 · **Venue:** *Current Directions in Biomedical Engineering* 10(4):295–298 (De Gruyter)
**Link / DOI:** https://doi.org/10.1515/cdbme-2024-2072
**Relevance score:** 9 / 10 (unchanged) — still the clearest "sensor placed *over the vein*" proof-of-concept; no newer version found this cycle.
**Why re-listed:** Remains the strongest device-level venous-specific optical paper; nothing published since supersedes it. See 06-10 entry for full novelty/integration notes.

### Paper 1.4 — **[previously surfaced — 2026-06-10, Paper 1.2]**
**Title:** Quantifying Changes in Oxygen Saturation of the Internal Jugular Vein In Vivo Using Deep Neural Networks and Subject-Specific 3-D Monte Carlo Models
**Authors:** Chin-Hsuan Sun, Hao-Wei Lee, Ya-Hua Tsai, Jia-Rong Luo, Kung-Bin Sung
**Year:** 2024 · **Venue:** *Optics Letters* 49(10):2669–2672
**Link / DOI:** https://opg.optica.org/ol/abstract.cfm?uri=ol-49-10-2669
**Relevance score:** 9 / 10 (unchanged). Subject-specific Monte Carlo + DNN inversion remains the leading approach to separating IJV signal from overlying neck tissue.
**Why re-listed:** Still the best NIRS-side venous-specific method; no 2025–26 successor found.

### Paper 1.5 — **[previously surfaced — 2026-06-10, Paper 1.3]**
**Title:** New Noninvasive Method for the Assessment of Central Venous Oxygen Saturations in Critically Ill Patients (Mespere VO100, external-jugular NIRS)
**Authors:** Alexandre Jeleff, Noémie Suh, Álmos Schranc, John Diaper, Karim Bendjelid, Eduardo Schiffer
**Year:** 2023 · **Venue:** *Journal of Cardiothoracic and Vascular Anesthesia* (PMID 37827917)
**Link:** https://www.sciencedirect.com/science/article/pii/S1053077023007826
**Relevance score:** 8 / 10 (unchanged). Largest single-centre human validation of a dedicated non-invasive jugular venous oximeter to date; remains the clinical benchmark.
**Why re-listed:** No larger or newer dedicated non-invasive ScvO₂-device validation surfaced this cycle.

---

## Topic 2 — Optical imaging techniques for non-invasively obtaining venous blood oxygen

> **Verdict for today:** Three genuinely new optical-imaging items, all 2025–2026: a deep-learning PACT reconstruction advance (sO₂ imaging), a validated high-resolution hyperspectral retinal system (artery + vein sO₂), and a 2025 retinal-oximetry review. The single strongest *venous-specific* photoacoustic study (Garcia-Uribe/Wang IJV) is re-listed as a flagged landmark.

### Paper 2.1 — NEW
**Title:** A Hybrid Diffusion Model Enhances Multiparametric 3D Photoacoustic Computed Tomography (HD-PACT)
**Authors:** Jeong et al. (lead author Jeong; full list not individually re-verified) — *partially flagged.*
**Year:** 2026
**Venue:** *Advanced Science* (Wiley)
**Link / DOI:** https://doi.org/10.1002/advs.202513624 · PMID 41126760 · PMC12767131
**Metadata verified:** Title, journal, year, DOI, PMID, and PMCID all confirmed via PubMed/Wiley/PMC search hits; full author list beyond first author not individually confirmed — *flagged.*
**Relevance score:** 7 / 10
**Novelty:** A hybrid diffusion generative model that reconstructs high-quality structural, functional, and contrast-enhanced 3-D PACT from a *sparse* transducer set (256 of 1024 elements, transferable down to 128). Critically for oxygenation: the model "suppresses artifacts and restores sO₂ values," recovers subtle vessel-oxygenation changes, and generalizes to *unseen* wavelengths (730/756/796/866 nm) for spectral unmixing of sO₂ and HbT during tumor progression (hypoxia tracking) in live animals.
**Integration insights:** The headline relevance is hardware/cost reduction with preserved sO₂ fidelity — a sparse-array PACT that still yields quantitative oxygen saturation lowers the barrier to a deployable deep-vessel oximeter, the exact platform needed for non-invasive IJV/deep-vein sO₂. The cross-wavelength generalization is directly applicable to venous spectral unmixing where deoxy-Hb dominates. Caveat: demonstrated on tumor/animal models for *generic* vessel sO₂, not venous-specific human imaging — it is an enabling-technology advance, not a venous measurement per se.

### Paper 2.2 — NEW
**Title:** Development and Validation of a High-Resolution Hyperspectral Imaging System for the Retina
**Authors:** Not individually verified (PMC/EuropePMC fetch blocked, HTTP 403) — *flagged.*
**Year:** 2026
**Venue:** Journal not confirmed from landing page (indexed as PMC12997856); an earlier related system appears as PMC11086557 — *flagged.*
**Link:** https://pmc.ncbi.nlm.nih.gov/articles/PMC12997856/
**Metadata verified:** Title and PMCID confirmed via multiple search hits; year (2026) reported by search but not page-verified; authors/journal/DOI **unconfirmed** — *flagged for manual check.*
**Relevance score:** 7 / 10
**Novelty:** A snapshot hyperspectral camera + high-res RGB camera fused via pansharpening (including deep-learning methods) to reach 0.1 mm/pixel and resolve hemoglobin sO₂ plus a spectral-noise index in retinal vessels as small as ~50 µm, over milliseconds. Validated in retina phantoms for spatial resolution and spectral fidelity; clinical use produced relative SatO₂ and HbT maps (500–600 nm).
**Integration insights:** The retina is the one site where *individual veins and arteries* are routinely separable non-invasively, so retinal venous sO₂ is the cleanest optical analogue of true SvO₂. A validated, high-resolution, snapshot (motion-tolerant) hyperspectral system that resolves ~50 µm vessels is a meaningful step toward reliable, vessel-resolved venous oximetry, and the noise-index output addresses the reproducibility problem that has dogged retinal oximetry. Complements vis-OCT retinal oximetry surfaced on 06-11 and 06-14.

### Paper 2.3 — NEW (review)
**Title:** Retinal Oximetry: New Insights into Ocular and Systemic Diseases
**Authors:** Not verified (Springer fetch blocked) — *flagged.*
**Year:** 2025
**Venue:** *Graefe's Archive for Clinical and Experimental Ophthalmology* (Springer)
**Link / DOI:** https://doi.org/10.1007/s00417-025-06831-8
**Metadata verified:** Title, journal, and DOI path confirmed via search; authors/issue unconfirmed — *flagged.*
**Relevance score:** 6 / 10
**Novelty:** A current (2025) review synthesizing retinal-oximetry methods (fundus-camera, OCT-, and ophthalmoscope-based) and their disease associations, including the venous-sO₂ changes seen in branch retinal vein occlusion and diabetic retinopathy (typical normal venous sO₂ ≈ 58%, A–V difference ≈ 35%).
**Integration insights:** Good orientation map for which retinal-oximetry modality to back for venous-specific readout and what venous-sO₂ shifts are pathologically meaningful. Establishes the clinical normative venous baseline against which new imaging systems (e.g., Paper 2.2, vis-OCT) should be benchmarked. Review, not a new method.

### Paper 2.4 — **[previously surfaced — 2026-06-10, Paper 2.1]**
**Title:** Noninvasive In Vivo Photoacoustic Measurement of Internal Jugular Venous Oxygenation in Humans
**Authors:** Alejandro Garcia-Uribe, Todd N. Erpelding, Haixin Ke, Kavya Narayana Reddy, Anshuman Sharma, Lihong V. Wang
**Year:** 2023 (arXiv 2303.10775) · **Venue:** arXiv preprint — no peer-reviewed journal version found (re-checked today; still preprint) — *flagged.*
**Link:** https://arxiv.org/abs/2303.10775
**Relevance score:** 9 / 10 (unchanged). Direct US-guided photoacoustic sO₂ of the IJV in humans (mean s_ijvO₂ 72 ± 7%) — still the single most on-target venous-specific optical-imaging paper.
**Why re-listed:** Searched specifically for a 2025–26 journal version by the same group; none found. Remains the photoacoustic gold-standard reference for the venous goal.

### Paper 2.5 — Sparse-slot note (no new qualifying #5)
No additional *new* Topic-2 paper this cycle clears the relevance bar for venous-specific optical imaging without duplicating prior scans. Candidates encountered were already surfaced: the thrombosis-PACT ex-vivo study (06-11, 2.2), the Hybrid-Net spectroscopic-PACT sO₂/segmentation paper arXiv 2512.15394 (06-10, 2.4), the physics-informed-NN spectral-unmixing paper arXiv 2602.16357 (06-11, 2.3), the sulfate blood phantom paper arXiv 2512.01458 (06-14, 2.3), and the vis-OCT retinal-oximetry translation work (06-11/06-14). Per the no-padding instruction, this slot is intentionally left as a documented gap rather than filled with arterial-only or duplicate work.

---

## Cross-Topic Synthesis

1. **The fresh signal this cycle is enabling-technology, not new venous endpoints.** Both genuinely new method papers (HD-PACT, 2.1; hyperspectral retina, 2.2) improve *how well / how cheaply* optical sO₂ can be reconstructed, not a new venous target. The maturity gradient is unchanged: photoacoustic IJV imaging (2.4) and jugular optical/NIRS sensing (1.3–1.5) remain the only methods demonstrated on a *named human vein*; everything else is tissue-level or retinal-microvascular.

2. **Two distinct venous-access strategies persist.** (a) *Large named vessel* — IJV via photoacoustic (2.4) or reflectance/NIRS over the jugular (1.3–1.5), the closest analogue to invasive ScvO₂. (b) *Retinal vessels* — the only site where artery/vein sO₂ separate cleanly non-invasively, now served by higher-resolution hyperspectral (2.2) and vis-OCT (prior scans). A deployable, sparse-array PACT (2.1) could lower cost for strategy (a).

3. **Deep learning is now the connective tissue.** Monte-Carlo-personalised DNN inversion for the IJV (1.4), diffusion-model PACT reconstruction (2.1), pansharpening for hyperspectral retina (2.2), and the previously surfaced physics-informed spectral unmixing all point to the same convergence: model-based inversion that separates the venous compartment from tissue/arterial background and from fluence/spectral-coloring artifacts — the long-standing barrier to *absolute* (not trend-only) non-invasive SvO₂.

4. **Clinical pull is sharpening (sepsis).** The new sepsis-monitoring review (1.1) and the ScvO₂-vs-O₂ER paper (1.2) reinforce that the clinical target is a *continuous, non-invasive, vessel-specific* venous-oxygen readout that also supports O₂ER computation — and that ScvO₂ alone can mislead in sepsis. This argues for platforms that pair venous sO₂ with arterial SpO₂ at a resolved vessel, exactly where photoacoustic/hyperspectral/vis-OCT are heading.

5. **Honest state of the field:** low novel-publication volume for true non-invasive *venous* (not arterial, not mixed-tissue) oximetry. After three scans this cycle the strongest venous-specific human studies are already catalogued; daily fresh yield is now dominated by enabling-technology and review literature. Several 2025–26 items here carry **unverified author/journal metadata** (publisher pages returned HTTP 403) and are flagged for manual confirmation.

---

### Metadata-verification caveats (today)
- Multiple publisher/PMC pages (Wiley, Springer, MDPI, NCBI/PMC, EuropePMC) returned **HTTP 403** to automated fetch; metadata was cross-checked from search-result snippets where possible. Items with unconfirmed authors/journal/DOI are flagged inline: Papers 1.1, 1.2, 2.2, 2.3, and the author list of 2.1.
- Paper 2.4 (Garcia-Uribe/Wang IJV photoacoustic) remains a **preprint** with no located peer-reviewed version as of this scan.
