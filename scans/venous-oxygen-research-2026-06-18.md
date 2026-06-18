# Venous Oxygen Research Scan — 2026-06-18

**Scan scope:** Non-invasive venous blood oxygen monitoring + optical imaging techniques for venous oxygen saturation.
**Prior scans in this repository:** 2026-06-10 (10 papers), 2026-06-11 (10 papers), 2026-06-14 (≈7 entries), 2026-06-16 (2 entries), 2026-06-17 (4 entries). Every paper entered in those five scans — plus all items listed in their "honorable mentions" / "reviewed and excluded" / "previously surfaced" sections — is excluded here unless a genuinely newer version or finding warrants re-entry. None did.
**Search window:** This scan ran **one day** after the 2026-06-17 scan, which itself ran one day after 2026-06-16 and three days after a thorough 2026-06-14 sweep. Emphasis on work published or first-surfacing after 2026-06-17, with a fallback to the best-available venous-specific work **not yet catalogued** anywhere in this repository. Sources searched: PubMed/PMC, arXiv, bioRxiv/medRxiv, Optica (Biomedical Optics Express, Optics Letters, Applied Optics), SPIE / *J. Biomed. Opt.* / *Neurophotonics*, *Photoacoustics*, Springer / *BioMedical Engineering OnLine*, Nature, ScienceDirect, IOVS/ARVO, ClinicalTrials.gov, ResearchGate, Semantic Scholar, ADS.
**Verification caveat:** As in every prior scan, essentially all PMC/PubMed, Nature, Springer, SPIE, Optica-fulltext and bioRxiv pages returned **HTTP 403** to direct fetches today. Every entry below was therefore cross-checked across **at least two independent search-index sources**; per-entry notes state what was confirmed and what could not be read directly on a publisher page.

---

## ⚠️ Read this first — honest sparseness report

This is the **sixth consecutive daily scan** of a genuinely low-volume niche, run one day after 06-17. As in the preceding three single-day cycles, **no brand-new (post-2026-06-17) venous-specific paper surfaced today.** Rather than pad with arterial-only SpO₂ work, this scan does the honest thing:

- **Topic 1 (systemic non-invasive venous monitoring): reported as empty for new entries.** Every result returned was already catalogued in a prior scan (jugular NIRS, Mespere VO100, spiroximetry, the venous-occlusion test, the MRI references, the e-tattoo, the 2016/2017 venous-modulation methods). One genuinely *new* item appeared — but it is a **clinical trial**, not a publication — and is recorded below as a lead.
- **Topic 2 (optical imaging): three venous-attributed primary papers, newly catalogued.** All three are from the **retinal vis-OCT / hyperspectral lineage** this repository tracks as the "proving ground," none appeared in any prior scan, and one (Gu et al.) reports an **explicit venous-sO₂ disease finding**. Two are 2025 (date-flagged); one is a very recently-indexed 2026 item. They are reported with honest relevance scores.

The standing picture is unchanged from 06-14 → 06-17: **MRI is the absolute-reference venous calibrator, the retina is the proving ground for vessel-specific optical venous saturation, the venous-occlusion test is the practical surrogate, and human deep-vein optical sO₂ at clinical scale remains the unfilled prize.** No padding was added to reach five entries per topic, per the scan's honesty mandate.

---

## Topic 1 — Non-Invasive Monitoring of Venous Blood Oxygen (SvO₂ / ScvO₂ / Peripheral Venous Oxygenation)

> **Sparseness flag — no new entries this cycle.** No venous-specific non-invasive *monitoring* paper published or first-surfacing after 2026-06-17 met the bar. Searches re-returned only (a) papers already entered in prior scans and (b) pre-2024 methodological references already noted as leads. Topic 1 is therefore reported honestly as empty for new publications this cycle.

**Previously surfaced — standing venous-monitoring references (NOT re-entered):**
- **Hill, Campbell, Chase & Pretty 2024**, optical SvO₂ sensing at the external jugular vein — *Curr. Dir. Biomed. Eng.* 10(4):295–298 (DOI 10.1515/cdbme-2024-2072). Prior scan **2026-06-10 §1.1**.
- **Sun et al. 2024**, IJV SijvO₂ via NIRS + subject-specific Monte Carlo + DNN — *Optics Letters* 49(10):2669–2672. Prior scan **2026-06-10 §1.2**.
- **Jeleff et al. 2023**, Mespere VO100 jugular NIRS vs invasive ScvO₂, 79 ICU patients — *J. Cardiothorac. Vasc. Anesth.* (PMID 37827917). Prior scan **2026-06-10 §1.3**.
- **Oh et al. 2023**, cerebral-NIRS surrogate tracking of mixed SvO₂ — *Sci. Rep.* (DOI 10.1038/s41598-023-49078-1). Prior scan **2026-06-10 §1.4**.
- **Zachia Alan et al. 2022**, thenar StO₂ → ScvO₂ during the venous-occlusion test — *Critical Care Science* (DOI 10.5935/0103-507X.20220023-en). Prior scan **2026-06-10 §1.5**.
- **McDiarmid et al. 2026**, cardiac-MRI T₂ iSvO₂, 628-patient HF cohort — *JACC: Advances* 5(1):102484. Prior scan **2026-06-11 §1.1**.
- **Skow et al. 2025**, MRI susceptometry-based venous oximetry during exercise — *Am. J. Physiol. Heart Circ. Physiol.* 328(6) (DOI 10.1152/ajpheart.00134.2025). Prior scan **2026-06-14 §1.1**.
- **Lahade et al. 2026**, wearable FD-NIRS (ASIC), forearm-occlusion arterio-venous transition — *Biomed. Opt. Express* 17(2):555–571 (DOI 10.1364/BOE.585068). Prior scan **2026-06-11 §1.2**.
- **Tan et al. 2023**, wearable arterial+venous optical e-tattoo (EMBC 2023, PMID 38083768). Prior scan **2026-06-17 §1.1**.
- **"hDOS" 2025** (Durduran group), automated hybrid diffuse-optical platform built around the venous-occlusion test — *J. Biomed. Opt.* 2025 / medRxiv 2025.06.03.25328859. Prior scan **2026-06-17 §1.2**.
- **Zhang et al. 2016**, light-absorption SvO₂ via induced venous fluctuation — *BioMed. Eng. OnLine* 15 (DOI 10.1186/s12938-016-0208-8). Prior scan **2026-06-17 §1.3**.
- **Zhang et al. 2017**, proof-of-concept non-invasive peripheral SvO₂ — *BioMed. Eng. OnLine* 16 (DOI 10.1186/s12938-017-0351-x). Prior scan 2026-06-17 honorable mention.

**Re-confirmed methodological leads (still no new 2025–2026 publication):** near-infrared "spiroximetry" (respiration-frequency-filtered venous NIRS; the substantive papers remain 2002/2013/2014, PMC3786737 / PMID 24439329); dynamic low-pressure venous-filling NIRS (Yoxall/Weindling lineage, PMID 10938779). Both venous-specific in principle; carried forward as leads, not entered.

**New lead this cycle (not a publication — recorded for the next cycle):**
- **ClinicalTrials.gov NCT01891188** — *"Using Near-Infrared Spectroscopy (NIRS) Monitor to Noninvasively Evaluate Hepatic Venous Saturation"* — record **updated January 2026**, investigating the correlation between hepatic regional StO₂ (NIRS) and hepatic venous oxygen saturation (SvHO₂) with newer NIRS sensors. This is a *venous-specific* non-invasive validation effort at a previously-untracked site (hepatic vein), but no results paper exists yet. Flagged as a lead to chase, not an entry. (A separately-found 2026-active trial, **NCT07279701**, uses NIRS only to *locate* veins for cannulation — not oximetry — and is noted only to exclude it.)

---

## Topic 2 — Optical Imaging Techniques for Non-Invasive Venous Blood Oxygen

> **Sparseness flag — no genuinely *new* (post-2026-06-17) primary study surfaced.** The three entries below are venous-attributed optical-imaging works **newly catalogued** in this repository (none appeared in any prior scan). All three sit in the retinal vis-OCT / hyperspectral lineage already identified as the field's proving ground; two are 2025 (date-flagged) and one is a 2026-indexed system paper. Reported with honest relevance scores.

### Paper 2.1
**Title:** Visible Light Optical Coherence Tomography for Assessing Retinal Structure and Function in Diseased Mouse Models
**Authors:** Qianyue Gu, Wenbo Xiu, Songzhi Wu, Kaiwen Li, Baihan Li, Zhenfei Tang, Chenlu Yan, Xiaogang Wang, Chong He, Fang Lu, Zhao Wang
**Year:** 2025 (BOE vol. 16 = 2025; **very recent PubMed indexing — see caveat**)
**Venue:** *Biomedical Optics Express* (Optica), vol. 16, no. 5, pp. 2077–2092
**Link / DOI:** PubMed PMID 41767920 ; canonical Optica path https://opg.optica.org/boe/abstract.cfm?uri=boe-16-5-2077
**Metadata verified:** Title, full 11-author list (Gu, Xiu, Wu, K. Li, B. Li, Tang, Yan, X. Wang, He, Lu, Z. Wang — the **Zhao Wang** vis-OCT group, the same group as the vis-OCT review catalogued in prior scan 2026-06-11 §2.5), journal (*Biomed. Opt. Express*), volume/issue/pages (16(5):2077–2092), PMID, and the venous-sO₂ disease findings cross-confirmed across PubMed and two independent search-index summaries. **Caveat (flagged):** the PMID (41767920) is anomalously high for a May-2025 paper, indicating **recent (≈2026) PubMed indexing of a 2025 article** — this is why it first surfaces now and was absent from prior scans. Optica/PubMed pages returned 403; exact DOI suffix and figures not read directly on source.
**Relevance score:** 7 / 10
*(Vessel-resolved retinal oximetry with an **explicit venous-saturation disease finding**; murine and retinal — so venous-attributed tissue/vessel sO₂, not a named systemic vein or blood-gas-calibrated SvO₂. Strongest new-to-repo Topic-2 entry because the headline result is specifically venous.)*

**Novelty:** A high-definition vis-OCT platform integrating high-resolution structural imaging, **GPU-accelerated computing**, and **automated retinal-layer segmentation**, delivering simultaneous 3-D structure, **blood flow**, and **oxygen-saturation** measurement in live mice. Its distinguishing contribution is the application to **diseased models** — retinitis pigmentosa (RP) and glaucoma vs. wild-type — with a clear vessel-resolved oximetry readout. The central functional finding is directly venous: both disease models showed **decreased retinal arteriovenous and total blood flow, increased *venous* oxygen saturation, and a reduced arteriovenous (A–V) oxygen-saturation difference** — i.e., reduced oxygen extraction consistent with lower metabolic demand in degenerating retina.

**Integration insights:** This is the **primary-research counterpart** to the vis-OCT *review* already catalogued from the same lab (Wu et al. 2025, prior scan 2026-06-11 §2.5) and the *Taiwan J. Ophthalmol.* translation review (2026-06-14 §2.4). It is a concrete data point in the project's recurring thesis that the retina is the one human-translatable bed where **vessel-specific venous saturation** is routinely measured optically, and it operationalizes the **A–V difference / oxygen-extraction-fraction** readout that is the physiologically meaningful venous endpoint (rising venous sO₂ + shrinking A–V gap = falling extraction). The same "increased venous sO₂, reduced A–V difference" signature reported here for glaucoma echoes the glaucoma finding synthesized in the vis-OCT review, and it is methodologically convergent with the SP-SFDI retinal venous αSO₂ result (Basiri et al., 2026-06-14 §2.1) and the BMC macular venular-oximetry study (2026-06-16 §2.1) — three optical modalities now reporting retinal *venous* saturation as a disease biomarker. Honest limitations: murine retina (thin, transparent; the translational gap to thick opaque peripheral beds is unchanged), and the readout is vessel/tissue sO₂ rather than a blood-gas-calibrated systemic SvO₂.

---

### Paper 2.2
**Title:** Multimodal Retinal Imaging by Visible Light Optical Coherence Tomography and Phosphorescence Lifetime Ophthalmoscopy in the Mouse Eye
**Authors:** Author list not fully verified on source (Johns Hopkins University / University of Pennsylvania collaboration; *flagged*)
**Year:** 2025
**Venue:** *Neurophotonics* (SPIE), vol. 12, no. 3, article 035015 — preprint: *bioRxiv* 2025.05.29.656845
**Link / DOI:** https://doi.org/10.1117/1.NPh.12.3.035015 ; PMID 41019609 ; PMC12476265 ; preprint https://www.biorxiv.org/content/10.1101/2025.05.29.656845v1
**Metadata verified:** Title, journal (*Neurophotonics*), volume/issue/article (12(3):035015), year (2025), PMID (41019609), PMC ID (PMC12476265), bioRxiv DOI, the JHU/Penn attribution, and the method (vis-OCT + **PLIM-SLO**, with **Oxyphor 2P** retro-orbital probe for intravascular pO₂) cross-confirmed across the SPIE Neurophotonics listing, PMC, bioRxiv, PubMed, and an EurekAlert/SPIE news release. Pages returned 403 — **full author list and exact figures not read directly on source (flagged).**
**Relevance score:** 5 / 10
⚠️ *Older-than-this-cycle (2025) and murine; included because it is **not present in any prior scan** and pairs a vessel-resolved vis-OCT sO₂ channel with a gold-standard **intravascular pO₂** reference (phosphorescence lifetime) — directly relevant to validating optical venous oximetry. Date-flagged: best-available new-to-repo context, not new this cycle.*

**Novelty:** A **multimodal** retinal platform that co-registers **vis-OCT** (structure + Doppler flow + spectroscopic sO₂) with **phosphorescence lifetime imaging ophthalmoscopy (PLIM-SLO)** using the **Oxyphor 2P** probe to recover **absolute intravascular oxygen partial pressure (pO₂)** down to the **capillary** level in live mice (high-definition 10 kHz raster + 100 kHz Doppler circular protocols). The key contribution is delivering **structure + flow + two independent oxygen readouts (optical sO₂ and phosphorescence pO₂)** in one instrument, enabling cross-validation of the optical saturation estimate against a physically distinct oxygen measurement.

**Integration insights:** This paper supplies something the project's bibliography lacked: an **optical-vs-reference oxygen cross-validation within a single eye**. Phosphorescence-lifetime pO₂ is an absolute, model-independent oxygen measurement, so co-registering it with vis-OCT sO₂ is the retinal analogue of the validation design the project repeatedly flags as missing for systemic optical venous oximetry (cf. the MRI absolute-reference thread, McDiarmid 2026 / Skow 2025). Because it resolves **capillary and venous-side** oxygenation, it informs the oxygen-extraction physiology that any venous-saturation endpoint depends on, and it complements Paper 2.1 (same retinal proving ground, different oxygen contrast). Honest caveats: murine, retinal, requires an **injected exogenous probe** (PLIM is not label-free, so it is a *validation/reference* tool rather than a translatable non-invasive venous monitor), and it reports pO₂/sO₂ in the retinal microvasculature rather than a named systemic vein.

---

### Paper 2.3
**Title:** Development and Validation of a High-Resolution Hyperspectral Imaging System for the Retina
**Authors:** Author list not verified on source (*flagged* — PMC page returned 403)
**Year:** 2026 (very recent PubMed/PMC indexing — see caveat)
**Venue:** Venue not confirmed on source (*flagged*); SPIE conference precursor exists (*"A dual-camera high-resolution hyperspectral imaging system for the retina,"* Proc. SPIE 13410, 134100A, 2025, DOI 10.1117/12.3047906)
**Link / DOI:** PMID 41858558 ; PMC12997856 (https://pmc.ncbi.nlm.nih.gov/articles/PMC12997856/)
**Metadata verified:** Title, PMID (41858558), PMC ID (PMC12997856), and the method (snapshot hyperspectral camera + high-resolution RGB camera + beamsplitter + imaging endoscope; **deep-learning pansharpening** to recover high-resolution HSI; vessel-size and oxygenation measurement validated in retinal **phantoms** then **in vivo in mice**) cross-confirmed across PMC and two independent search-index summaries, plus the 2025 SPIE conference precursor. **Journal name, publication year, and full author list could NOT be confirmed on source (flagged); the anomalously high PMID/PMC IDs indicate ≈2026 indexing.**
**Relevance score:** 4 / 10
*(Vessel-resolved retinal **hyperspectral** oximetry, but it reports a generic vessel "oxygenation rate" — **not** an explicit artery-vs-vein separation in the summaries available — and is a **system/validation** paper in phantoms + mice. Lowest of the three: venous-relevant by modality, but not demonstrably venous-specific in its reported results.)*

**Novelty:** A **dual-camera hyperspectral retinal imager** (snapshot HSI fused with high-resolution RGB via **deep-learning pansharpening**) that recovers high-spatial-resolution spectral maps for simultaneous extraction of **retinal vessel diameter and oxygenation**. The novelty is the engineering pipeline — combining a low-spatial-resolution snapshot spectral camera with a high-resolution RGB channel and learned pansharpening to overcome the classic HSI resolution-vs-spectral-bands trade-off — validated against a retinal phantom and then in anesthetized mice.

**Integration insights:** This is the **hyperspectral sibling** of the vis-OCT retinal work above and of the transmissive-HSI single-vessel oximetry paper already catalogued (Liu et al., prior scan 2026-06-11 §2.1). It strengthens the multimodal retinal-oximetry picture (vis-OCT, SP-SFDI, fundus spectral oximetry, and now high-resolution HSI all targeting vessel-resolved retinal saturation), and its **deep-learning pansharpening** approach is a transferable idea for any wide-field optical oximeter that must trade spatial resolution against spectral sampling. Honest caveats: the available summaries describe a generic vessel "oxygenation rate" rather than an explicit **venous** readout, the demonstration is in phantoms and mouse retina, and core metadata (journal, year, authors) could not be verified on source — so this is included as **completeness-oriented, modality-relevant context**, with a deliberately low venous-specific relevance score.

---

**Previously surfaced — standing optical venous-imaging references (NOT re-entered):** Garcia-Uribe/Wang IJV-PA (2026-06-10 §2.1); Kong et al. PACT intra-vessel flow (2026-06-10 §2.2); Zhang et al. PAVT deep hemodynamics (2026-06-10 §2.3); Shang et al. Hybrid-Net (2026-06-10 §2.4); Huang et al. SFDI-net (2026-06-10 §2.5); Liu et al. transmissive HSI single-vessel sO₂ (2026-06-11 §2.1); Feng et al. PA thrombosis oximetry (2026-06-11 §2.2); Ter Martirosyan et al. SPOI-AE (2026-06-11 §2.3); Cam et al. qPACT virtual-imaging framework (2026-06-11 §2.4); Wu et al. vis-OCT review (2026-06-11 §2.5); Basiri et al. SP-SFDI retinal venous αSO₂ (2026-06-14 §2.1); Zafar et al. multispectral PAM (2026-06-14 §2.2); Davenet et al. venous-range sulfate phantoms (2026-06-14 §2.3); *Taiwan J. Ophthalmol.* vis-OCT translation review (2026-06-14 §2.4); Zhang & Wang PA-for-PAD review (2026-06-14 §2.5); BMC Ophthalmology macular venular oximetry (2026-06-16 §2.1); Kirchner/Jaeger/Frenz MI-MS-LSD human accompanying-vein oximetry (2026-06-16 §2.2); eMSOT (Tzoumas et al. 2016, honorable mention); Quantitative PACT oximetry review (2026-06-17 §2.1).

**Honorable mentions (verified, context only, not ranked):**
- *Distribution-informed and wavelength-flexible data-driven photoacoustic oximetry* — arXiv:2403.14863 (2024), PMC11151660. Learned-oximetry method (LSTM, wavelength-flexible) descending from LSD-qPAI / MI-LSD; not venous-specific. Re-confirmed today; previously noted as a lead in 2026-06-16.
- *A dual-camera high-resolution hyperspectral imaging system for the retina* — Proc. SPIE 13410, 134100A (2025), DOI 10.1117/12.3047906. The conference precursor to Paper 2.3.

---

## Cross-Topic Synthesis

### What this scan actually establishes
On a **one-day cadence** in a low-volume niche, the venous-specific non-invasive oxygen literature **again produced no new publications** — the correct and expected outcome, now observed for the fourth consecutive short-cycle scan, and itself a signal worth recording. The value added this cycle is **bibliographic completeness in the retinal optical thread**:

1. **A venous-specific vis-OCT disease finding enters the record (Paper 2.1).** Gu et al. (Zhao Wang group) is the primary-research complement to the vis-OCT review already catalogued from the same lab. Its headline is squarely venous: in RP and glaucoma mouse models, **venous sO₂ rises and the arteriovenous oxygen-extraction gap narrows** — the exact A–V/OEF physiology that defines a meaningful venous endpoint. It joins SP-SFDI and BMC macular oximetry as a third optical modality reporting retinal *venous* saturation as a disease biomarker.
2. **An optical-vs-reference oxygen cross-validation is now catalogued (Paper 2.2).** The JHU/Penn multimodal vis-OCT + phosphorescence (PLIM) platform co-registers a label-free optical sO₂ with an absolute, physically independent intravascular pO₂ in the same eye — the retinal analogue of the absolute-reference validation design (MRI for systemic veins) the project keeps flagging as missing for optical venous oximetry.
3. **The retinal hyperspectral toolkit gains a resolution-recovery method (Paper 2.3).** A deep-learning-pansharpened dual-camera HSI retinal imager extends the multimodal retinal-oximetry picture, though its reported readout is generic vessel oxygenation rather than explicit venous separation (hence its low score and unverified core metadata).

### Persisting gaps (carried forward, unchanged and still open)
- **No new in-vivo human venous-PA sO₂ result.** The 2023 IJV-PA proof-of-concept remains the only direct human named-vein photoacoustic oximetry result; clinical-scale validation still does not exist.
- **The MRI validation-scale gap still dominates.** Two MRI venous-SvO₂ methods (T₂ iSvO₂; susceptometry) are blood-gas-validated at cohort scale; no optical method approaches that bar. This cycle's optical additions are murine and retinal.
- **Vessel-specific venous separation remains proven only in the retina (and thin/murine tissue).** All three new entries reinforce the retina-as-proving-ground thesis; none extends single-vessel venous separation to an accessible systemic vein in thick human tissue.
- **A new validation idea, still only in the eye.** Paper 2.2's optical-sO₂-vs-phosphorescence-pO₂ co-registration is exactly the kind of head-to-head an optical *systemic* venous oximeter needs — but it requires an injected probe and is demonstrated only in mouse retina. The systemic, label-free, blood-gas-validated equivalent is still unpublished.
- **Topic 1's only forward motion is a trial, not a paper.** The hepatic-vein NIRS trial (NCT01891188, updated Jan 2026) is the one *new* venous-specific monitoring effort surfaced this cycle, at a previously-untracked site; no results exist yet.

### Bottom line
An honestly **empty cycle for new publications**, used to close three real bibliographic gaps in the retinal optical-oximetry thread. The strongest addition (Gu et al. vis-OCT, Paper 2.1) is genuinely venous in its finding; the other two are validation-method (PLIM cross-reference) and modality (HSI) context. Nothing this cycle alters the standing picture: **MRI is the absolute-reference calibrator, the retina is the proving ground, the venous-occlusion test is the practical surrogate, and human deep-vein optical sO₂ at clinical scale remains the unfilled prize.** No arterial-only padding was added to reach five entries per topic, per the scan's honesty mandate.
