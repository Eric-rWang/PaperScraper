# Venous Oxygen Research Scan — 2026-06-17

**Scan scope:** Non-invasive venous blood oxygen monitoring + optical imaging techniques for venous oxygen saturation.
**Prior scans in this repository:** 2026-06-10 (10 papers), 2026-06-11 (10 papers), 2026-06-14 (≈7 entries), 2026-06-16 (2 entries). Every paper entered in those four scans — plus all items listed in their "honorable mentions" / "reviewed and excluded" / "previously surfaced" sections — is excluded here unless a genuinely newer version or finding warrants re-entry. None did.
**Search window:** This scan ran only **one day** after the 2026-06-16 scan (which itself ran two days after a thorough 2026-06-14 sweep). Emphasis on work published or first-surfacing after 2026-06-16, with a fallback to the best-available venous-specific work **not yet catalogued** anywhere in this repository. Sources searched: PubMed/PMC, arXiv, medRxiv, Optica (Biomedical Optics Express, Optics Letters, Applied Optics), SPIE / *J. Biomed. Opt.*, *Photoacoustics*, World Scientific (*J. Innovative Optical Health Sciences*), IEEE Xplore (EMBC), Springer / *BioMedical Engineering OnLine*, Wiley, ResearchGate, Semantic Scholar, ADS, Wikidata.
**Verification caveat:** As in every prior scan, nearly all publisher and PMC/PubMed pages (Springer, World Scientific, medRxiv, Wiley, IEEE, sites.utexas.edu) returned **HTTP 403** to direct fetches today. Every entry below was therefore cross-checked across **at least two independent search-index sources**; per-entry notes state what was confirmed and what could not be read directly on a publisher page.

---

## ⚠️ Read this first — honest sparseness report

On a **one-day cadence**, in a genuinely low-volume niche, **no brand-new (post-2026-06-16) venous-specific paper surfaced today.** Rather than pad with arterial-only SpO₂ work, this scan does the honest thing: it reports the field as quiet for new publications and instead uses the cycle to **fill three real gaps in this repository's bibliography** — venous-specific works that are on-target for the project's goal but had never been catalogued in any prior scan. Two of them are older (2016, 2023) and are clearly **date-flagged**; one is genuinely recent (2025); and Topic 2 adds one genuinely **new 2026** review.

- **Topic 1** adds three newly-catalogued venous-relevant entries: a wearable **arterial+venous** optical e-tattoo (EMBC 2023), the **hDOS** hybrid diffuse-optical platform built around the venous-occlusion test (*J. Biomed. Opt.* 2025), and an early **light-absorption SvO₂** method using induced venous fluctuation (2016).
- **Topic 2** adds one new entry: a **2026 review of quantitative PACT oximetry** (the spectral-coloring / fluence problem that gates all deep venous photoacoustic sO₂).

The standing picture is unchanged from 06-14/06-16: **MRI is the absolute-reference venous calibrator, the retina is the proving ground for vessel-specific optical venous saturation, and human deep-vein optical sO₂ at clinical scale remains the unfilled prize.** No padding was added to reach five entries per topic, per the scan's honesty mandate.

---

## Topic 1 — Non-Invasive Monitoring of Venous Blood Oxygen (SvO₂ / ScvO₂ / Peripheral Venous Oxygenation)

> **Sparseness flag — no *new* (post-2026-06-16) entries.** The three entries below are venous-specific works **newly catalogued** in this repository (none appeared in any prior scan); two are date-flagged as older context, one is 2025. They are reported with honest relevance scores.

### Paper 1.1
**Title:** Towards Simultaneous Noninvasive Arterial and Venous Oxygenation Monitoring with Wearable E-Tattoo
**Authors:** Philip Tan, Emily Wang, Sangjun Tamma, Sarnab Bhattacharya, Nanshu Lu
**Year:** 2023 (presented Aug 2023; IEEE Xplore entry Dec 2023)
**Venue:** *45th Annual International Conference of the IEEE Engineering in Medicine and Biology Society (EMBC)*, Sydney
**Link / DOI:** https://pubmed.ncbi.nlm.nih.gov/38083768/ ; IEEE Xplore document 10340010 (https://ieeexplore.ieee.org/document/10340010)
**Metadata verified:** Title, author group (Tan, Wang, Tamma, Bhattacharya, Lu — UT Austin Lu Research Group), conference (EMBC 2023, Sydney), PMID (38083768), and IEEE document ID cross-confirmed across PubMed, IEEE Xplore, the Lu group's conference-papers page, and a 2024 MRS talk of the same project (MRS abstract EL05.07.03). IEEE/PMC/sites.utexas.edu pages returned 403 — exact DOI string and page numbers not directly read on source (*flagged*). No peer-reviewed **journal** version was found; the EMBC proceedings paper is the citable record.
**Relevance score:** 7 / 10
⚠️ *Older paper (2023), included because it is **not present in any prior scan** and is one of the few wearable studies that explicitly targets **venous** (SvO₂) — not just arterial — oxygenation. Date-flagged: best-available context, not new this cycle. Note this is the wrist/peripheral-vein counterpart to the same group's "Wearable Optical E-Tattoo for Deep Neck Hemodynamic Monitoring" (2023), which targets the jugular.*

**Novelty:** A soft, skin-conformal **optical e-tattoo** worn on the wrist that simultaneously records the **arterial and venous pulses**, with the explicit aim of extracting **both SaO₂ and SvO₂** from a single wearable. The paper's central contribution is identifying and characterizing — via simulation, in-vitro, and in-vivo experiments — the **arterial–venous crosstalk** that arises because the artery and vein lie in close proximity, and proposing **spatial filtering** to separate the two contributions. It explicitly frames non-invasive venous oxygenation as the unmet need (sepsis/shock are detectable only via venous O₂ content), distinguishing it from conventional arterial-only pulse oximetry.

**Integration insights:** This is the wearable-form-factor sibling of the jugular-sensor lineage already catalogued (Hill et al. 2024, prior scan 2026-06-10 §1.1; Mespere VO100, 2026-06-10 §1.3) and of the wearable FD-NIRS hardware thread (Lahade et al. 2026, 2026-06-11 §1.2). Its specific, transferable contribution is the **crosstalk characterization + spatial-filtering** strategy: every surface optical venous oximeter at a site where an artery runs alongside the vein (wrist, neck, antecubital) faces exactly this arterial-contamination problem, which the prior scans repeatedly flagged as the core limitation of tissue-level NIRS. The honest limitation is that this is a *"towards"* proof-of-concept conference paper — the SvO₂ extraction is demonstrated in principle, not validated against blood-gas co-oximetry in a cohort. It belongs in the bibliography because it is one of the few works to put **venous-selective spatial demodulation** on a soft wearable, the convergence target prior scans identified as the highest-leverage near-term path.

---

### Paper 1.2
**Title:** "hDOS": An Automated Hybrid Diffuse Optical Device for Real-Time Non-Invasive Tissue Monitoring — Precision and In Vivo Validation
**Authors:** Author list not fully verified on source (ICFO / Turgut Durduran group; Durduran confirmed as senior author — *flagged*)
**Year:** 2025 (medRxiv preprint posted 3 June 2025; journal version published November 2025)
**Venue:** *Journal of Biomedical Optics* (SPIE), 2025 — preprint: *medRxiv* 2025.06.03.25328859
**Link / DOI:** medRxiv https://doi.org/10.1101/2025.06.03.25328859 ; PMC12626046 (https://www.ncbi.nlm.nih.gov/pmc/articles/PMC12626046/)
**Metadata verified:** Title, hybrid method (time-domain NIRS + diffuse correlation spectroscopy + pulse oximetry), the **vascular-occlusion-test** development context, the 7-month critical-care deployment (~150 sessions, >200 h), the INVOS 5100C comparison, the senior author (Durduran, ICFO Barcelona), the medRxiv DOI/date, the PMC ID, and the *J. Biomed. Opt.* 2025 venue cross-confirmed across medRxiv, PMC, ResearchGate, and the author's profile. All pages returned 403 — full author list and exact volume/article number not directly read on source (*flagged*).
**Relevance score:** 5 / 10
*(Tissue-level StO₂ — NOT a direct vessel-specific SvO₂ measurement. Included as a new 2025 entry because it was purpose-built around the **venous-occlusion test (VOT)**, the standing surrogate route to venous saturation in this repository, and because it operationalizes that route in a real ICU.)*

**Novelty:** A **fully automated, self-contained hybrid diffuse-optical platform (hDOS)** that fuses **time-domain NIRS** (absolute μₐ/μₛ′ → StO₂, blood volume), **diffuse correlation spectroscopy** (microvascular blood flow), and **pulse oximetry** in one operator-independent device. Its distinguishing claims are automation and multiparametric, real-time output validated across bench test-retest, a **7-month critical-care deployment** (~150 sessions, >200 hours), and head-to-head against a commercial CW-NIRS monitor (INVOS 5100C). It was explicitly developed in the context of **vascular-occlusion tests** before being generalized to trauma/surgery/anesthesia.

**Integration insights:** The hDOS sits squarely on this repository's recurring **venous-occlusion-test thread** — Zachia Alan et al. 2022 (prior scan 2026-06-10 §1.5, thenar StO₂ → ScvO₂ during VOT), El Masry et al. 2025 (2026-06-11 §1.5, multimodal VOT benchmarking), and the FD-NIRS forearm-occlusion demonstration (2026-06-11 §1.2). During a venous occlusion the tissue bed transiently behaves as a stagnant venous reservoir, so StO₂ converges toward venous sO₂; hDOS is the most clinically-matured, automated instrument for running that protocol continuously in the ICU, and its **absolute TD-NIRS μₐ** (rather than CW relative changes) is exactly what a quantitative VOT-derived venous readout needs. The DCS flow channel is also the complement that distinguishes stagnant-venous equilibration from ongoing perfusion. Honest caveat: hDOS reports **tissue StO₂/flow**, not vessel-specific SvO₂ — it advances the *delivery vehicle* for the VOT venous surrogate, not direct venous oximetry. It is the natural hardware platform on which to test whether automated VOT can deliver a reliable peripheral-venous saturation at scale.

---

### Paper 1.3
**Title:** A New Method for Noninvasive Venous Blood Oxygen Detection
**Authors:** Xu Zhang, Meimei Zhang, Shengkun Zheng, Liqi Wang, Jilun Ye
**Year:** 2016
**Venue:** *BioMedical Engineering OnLine* (Springer/BioMed Central), vol. 15
**Link / DOI:** https://doi.org/10.1186/s12938-016-0208-8 (PMID 27436186; PMC4952148)
**Metadata verified:** Title, full 5-author list (recovered via Wikidata Q37111362 and cross-checked against PubMed), journal, year, DOI, PMID, and PMC ID cross-confirmed across PubMed, PMC, Springer, and Wikidata. The reported accuracy (RMSE ≈ 5.31, correlation r ≈ 0.72 vs. invasive reference) was confirmed in two independent search-index summaries. Springer/PMC pages returned 403 — exact article number and figures not directly read on source (*flagged*).
**Relevance score:** 6 / 10
⚠️ *Older paper (2016), included because it is **not present in any prior scan** and is a genuinely **venous-specific** non-invasive SvO₂ method (not a tissue StO₂ surrogate). Date-flagged: foundational context, not new this cycle.*

**Novelty:** A non-invasive **SvO₂ measurement based on light absorption**, in which an **external stimulation signal is applied to induce a cyclical (low-frequency) fluctuation in the vein**, creating a venous "pulse" that can be optically demodulated — directly attacking the low-SNR problem that defeats passive venous photoplethysmography (veins are normally non-pulsatile). The induced-venous-modulation approach lets a pulse-oximetry-style ratio be computed for the *venous* compartment. Validated against an invasive reference with RMSE ≈ 5.31 and r ≈ 0.72.

**Integration insights:** This is the conceptual ancestor of the **venous-modulation** family that recurs throughout this project: the respiration-frequency "spiroximetry" lead (noted 2026-06-16), the dynamic low-pressure venous-filling NIRS lineage (Yoxall/Weindling, noted 2026-06-16), and the e-tattoo's arterial/venous pulse separation (Paper 1.1 above). All share the same core idea — **manufacture or isolate a venous-specific time-varying signal** so the deoxygenated-hemoglobin ratio can be read out without arterial contamination. The 2016 method's modest accuracy (r ≈ 0.72) quantifies how far passive/active surface optics sat from clinical-grade venous oximetry a decade ago, providing a useful baseline against which the newer wearable (Paper 1.1) and photoacoustic vessel-specific results (IJV-PA, prior scan 2026-06-10 §2.1) should be read. A closely related follow-up — *"Proof of concept non-invasive estimation of peripheral venous oxygen saturation,"* *BioMedical Engineering OnLine* 2017, DOI 10.1186/s12938-017-0351-x — is noted as an additional venous-specific reference (see honorable mentions).

---

**Previously surfaced — standing venous-monitoring references (NOT re-entered):**
- **Jeleff et al. 2023**, Mespere VO100 jugular NIRS vs invasive ScvO₂, 79 ICU patients — prior scan 2026-06-10 §1.3.
- **Hill, Campbell, Chase & Pretty 2024**, optical SvO₂ at the external jugular vein — prior scan 2026-06-10 §1.1.
- **Sun et al. 2024**, IJV SijvO₂ via NIRS + subject-specific Monte Carlo + DNN — prior scan 2026-06-10 §1.2.
- **McDiarmid et al. 2026**, cardiac-MRI T₂ iSvO₂, 628-patient HF cohort — prior scan 2026-06-11 §1.1.
- **Skow et al. 2025**, MRI susceptometry-based venous oximetry during exercise — prior scan 2026-06-14 §1.1.
- **Lahade et al. 2026**, wearable FD-NIRS (ASIC), forearm-occlusion arterio-venous transition — prior scan 2026-06-11 §1.2.

**Re-confirmed methodological leads (still no new 2025–2026 publication):** near-infrared "spiroximetry" (respiration-frequency-filtered venous NIRS); dynamic low-pressure venous-filling NIRS (Yoxall/Weindling lineage). Both venous-specific in principle; carried forward as leads, not entered.

---

## Topic 2 — Optical Imaging Techniques for Non-Invasive Venous Blood Oxygen

> **Sparseness flag — one new entry this cycle.** No vessel-specific venous *primary* optical study published after 2026-06-16 surfaced. The single new entry is a 2026 review that directly addresses the quantitative-accuracy problem gating all deep venous photoacoustic sO₂.

### Paper 2.1
**Title:** Quantitative Oximetry with Photoacoustic Computed Tomography: Principles, Progress, and Prospects
**Authors:** Author list not verified on source (*flagged* — World Scientific page returned 403)
**Year:** 2026
**Venue:** *Journal of Innovative Optical Health Sciences* (World Scientific)
**Link / DOI:** https://doi.org/10.1142/S1793545826300065
**Metadata verified:** Title, journal, and DOI cross-confirmed across the World Scientific listing and two independent search-index summaries; the DOI stem (S1793545**826**...) and the journal's volume sequencing place this in the **2026** volume. The publisher page returned 403 — **author list, volume/issue, and page numbers could not be read on source (flagged).**
**Relevance score:** 6 / 10
*(Review, not primary venous data; PACT sO₂ is inherently vessel-resolved — an artery and an adjacent vein are separable by spectrum — so the techniques surveyed are directly transferable to venous oximetry. Included as the only genuinely new 2026 optical-imaging item this cycle.)*

**Novelty:** A 2026 synthesis of **quantitative PACT oximetry** organized around the field's central obstacle: the **spatiotemporal heterogeneity of optical fluence** that produces the **spectral-coloring effect** and corrupts sO₂ at depth. It systematically classifies the correction strategies into five families — **photon-transport modeling, acoustic-spectrum-based self-calibration, multimodality fusion, statistical inference, and learning-based approaches** — and assesses progress and remaining prospects for each.

**Integration insights:** This review is the conceptual umbrella over essentially the entire photoacoustic thread this repository has tracked. Its five correction families map directly onto catalogued primary work: **photon-transport modeling** ↔ subject-specific Monte Carlo (Sun et al. 2024, 2026-06-10 §1.2) and the qPACT virtual-imaging framework (Cam et al. 2025, 2026-06-11 §2.4); **self-calibration / internal-chromophore correction** ↔ Feng et al.'s spectral-coloring correction (2026-06-11 §2.2); **statistical / learning-based inversion** ↔ Hybrid-Net (2026-06-10 §2.4), SPOI-AE (2026-06-11 §2.3), eMSOT and MI-LSD (2026-06-16 honorable mentions / Paper 2.2). Because venous saturations (~60–75%) sit precisely in the range where spectral-coloring and unmixing errors are most consequential, a state-of-the-art map of how the field corrects fluence is directly load-bearing for the project's goal of **deep-vein optical sO₂** (the IJV at ~3 cm; femoral/IVC deeper). It also pairs naturally with the venous-range sulfate phantoms (Davenet et al. 2026, prior scan 2026-06-14 §2.3): the review says *how* to correct, the phantoms say *how to validate* the correction at venous saturations. Honest caveat: this is a review and PACT-general, not venous-exclusive primary data.

---

**Previously surfaced — standing optical venous-imaging references (NOT re-entered):** Garcia-Uribe/Wang IJV-PA (2026-06-10 §2.1); Kong et al. PACT intra-vessel flow (2026-06-10 §2.2); Zhang et al. PAVT deep hemodynamics (2026-06-10 §2.3); Liu et al. transmissive HSI single-vessel sO₂ (2026-06-11 §2.1); Feng et al. PA thrombosis oximetry (2026-06-11 §2.2); Wu et al. and the *Taiwan J. Ophthalmol.* vis-OCT reviews (2026-06-11 §2.5, 2026-06-14 §2.4); Basiri et al. SP-SFDI retinal venous αSO₂ (2026-06-14 §2.1); Zafar et al. multispectral PAM (2026-06-14 §2.2); BMC Ophthalmology macular venular oximetry (2026-06-16 §2.1); Kirchner/Jaeger/Frenz MI-MS-LSD human accompanying-vein oximetry (2026-06-16 §2.2); eMSOT (Tzoumas et al. 2016, honorable mention).

**Honorable mentions (verified, venous-relevant, not ranked — context only):**
- **Zhang, Zhang, Zheng, Wang, Ye et al. 2017**, *"Proof of concept non-invasive estimation of peripheral venous oxygen saturation"* — *BioMedical Engineering OnLine* 16, DOI 10.1186/s12938-017-0351-x. Venous-specific follow-up to Paper 1.3; not previously catalogued.
- **"Comparison of non-invasive peripheral venous saturations with venous blood co-oximetry"** — PMC5655584. Validation-flavored venous-specific reference; older, context only.

---

## Cross-Topic Synthesis

### What this scan actually establishes
On a **one-day cadence**, the venous-specific non-invasive oxygen literature **did not produce new publications** — the correct and expected outcome for a niche field scanned daily, and itself a signal worth recording. The value added this cycle is **bibliographic completeness**: four venous-relevant works that were genuinely on-target yet absent from this repository have now been catalogued, with two older items honestly date-flagged.

1. **A wearable venous-selective optical sensor enters the record (Paper 1.1).** The Lu-group e-tattoo is the soft-wearable embodiment of the arterial-contamination problem every prior scan flagged: it *characterizes* arterial–venous crosstalk and proposes spatial filtering — the demodulation problem that any wrist/neck venous oximeter must solve. It is the form-factor convergence target sitting between the jugular sensors (Hill 2024) and the wearable FD-NIRS hardware (Lahade 2026).
2. **The venous-occlusion-test route gets a clinical-grade instrument (Paper 1.2).** hDOS operationalizes the VOT surrogate (Zachia Alan 2022; El Masry 2025) in an automated, multiparametric, ICU-deployed device with absolute TD-NIRS μₐ plus DCS flow — exactly the measurement stack a quantitative VOT-derived venous readout needs.
3. **An early venous-modulation method anchors the lineage (Paper 1.3).** The 2016 induced-venous-fluctuation light-absorption method is the ancestor of the "manufacture a venous-specific signal" idea (spiroximetry, dynamic venous filling, e-tattoo pulse separation); its r ≈ 0.72 quantifies how far surface optics sat from clinical venous oximetry a decade ago.
4. **The PACT accuracy problem gets a 2026 map (Paper 2.1).** The new review consolidates the fluence/spectral-coloring correction landscape that gates every deep venous photoacoustic sO₂ result this project tracks, and pairs with the venous-range phantoms (Davenet 2026) as the "how to correct / how to validate" couple.

### Persisting gaps (carried forward, unchanged and still open)
- **No new in-vivo human venous-PA sO₂ result.** The 2023 IJV-PA proof-of-concept remains the only direct human named-vein photoacoustic oximetry result; clinical-scale validation does not exist.
- **The MRI validation-scale gap still dominates.** Two MRI venous-SvO₂ methods (T₂ iSvO₂; susceptometry) are blood-gas-validated at cohort scale; no optical method approaches that bar. The e-tattoo and 2016 method are proof-of-concept / r ≈ 0.72, respectively.
- **Vessel-specific venous separation is proven only in the retina (and thin/murine tissue).** No 2025–2026 feasibility study extends single-vessel venous separation to an accessible systemic vein in thick human tissue.
- **VOT venous surrogate now has a vehicle (hDOS) but still no vessel-specificity.** The open question — can automated VOT deliver a reliable peripheral-venous saturation at scale? — is now testable on a clinical platform.

### Bottom line
An honestly **empty cycle for new publications**, used to close four real bibliographic gaps. The single genuinely-new 2026 item (PACT-oximetry review) and the new-to-repo 2025 hDOS platform reinforce — without altering — the standing picture: **MRI is the absolute-reference calibrator, the retina is the proving ground, the venous-occlusion test is the practical surrogate, and human deep-vein optical sO₂ at clinical scale remains the unfilled prize.** No arterial-only padding was added to reach five entries per topic.
