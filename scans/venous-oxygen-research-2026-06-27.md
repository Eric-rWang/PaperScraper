# Venous Oxygen Research Scan — 2026-06-27

**Prior scans in this repository:** 2026-06-10, 06-11, 06-14, 06-16, 06-17, 06-18, 06-19, 06-21, 06-22, 06-24, 06-25. Every paper entered in those scans — plus all items in their "previously surfaced", "honorable mentions", "reviewed and excluded" and "standing leads" sections — is excluded here unless a genuinely newer version or finding warrants re-entry.

**Search window:** This is the **twelfth scan** in the series, run **two days** after 2026-06-25. Emphasis on work published or first-surfacing after 06-25, with the standard fallback to the best-available venous-specific work **not yet catalogued** anywhere in this repository. Sources searched today: PubMed/PMC, arXiv, bioRxiv/medRxiv, Optica (*Biomed. Opt. Express*, *Optics Letters*), SPIE / *J. Biomed. Opt.*, *Photoacoustics* (ScienceDirect), IEEE Xplore, Nature / *Eye* / *npj Acoustics*, Springer / Frontiers, MDPI, De Gruyter Brill, IOPscience, ClinicalTrials.gov, ResearchGate, Semantic Scholar, GitHub.

---

## ⚠️ Read this first — honest sparseness report

This was a **near-empty cycle**. Genuinely novel, non-invasive *venous*-specific work is published at low volume, and the repository's eleven prior scans have already captured essentially the entire current literature. Today's searches returned almost exclusively items that are **already catalogued**.

- **Topic 1 (venous monitoring): NO not-yet-catalogued item surfaced.** Every monitoring hit returned was already in the repository — jugular optical SvO₂ (Hill 2024), Mespere VO100 (Jeleff 2023), the peripheral-PPG / cuff-modulation / artificial-venous-pulse family (Zhang 2016/2017), the cerebral-NIRS respiration-filtered surrogate (Oh 2023), the venous-occlusion test, the preterm-neonate NIRS VOT paper (Mileder 2022, catalogued 06-24), the MRI references, the e-tattoo, hDOS, and the capnodynamic / SjvO₂ NIRS clinical trials. Topic 1 therefore carries forward its standing references with **no new entry** — a second consecutive honest empty cycle for venous *monitoring* (06-25 was also empty).

- **Topic 2 (optical imaging): ONE not-yet-catalogued item surfaced** — a **23 Jan 2026** arXiv benchmarking-framework preprint from the Anastasio group (Chen et al., 2601.17165) for DL-based PACT image reconstruction. It is a **methods/validation-infrastructure** paper, not an oximetry result, so it is entered honestly at low relevance. Two items that *looked* new on first pass were checked and found already catalogued: the **Cam et al. qPACT virtual-imaging framework** (arXiv 2510.03431 / PMC12858365) is the repository's 06-11 §2.4 entry, and the **npj Acoustics PA-detection review** (DOI 10.1038/s44384-025-00005-w) is already an 06-14 honorable mention. The convex-cone TMI paper, the ISDC *J. Biomed. Opt.* paper, Hybrid-Net, the sulfate phantoms, the PINN preprint, SP-SFDI/BioxyDR, the HSI/vis-OCT retinal systems, PAVT, and the IJV-PA proof-of-concept all re-surfaced and are **already catalogued** — not re-entered.

**Bottom line:** No new venous-monitoring paper today, and the single new optical-imaging item is enabling infrastructure rather than a venous result. The state of the field is unchanged from 06-25: the only direct human named-vein optical SvO₂ results in existence remain **Garcia-Uribe/Wang's IJV photoacoustic proof-of-concept** (sijvO₂ 72 ± 7 %, 7 volunteers) and **Hill et al.'s external-jugular optical SvO₂ sensor** (≈70–72 %, 3 subjects).

---

## Topic 1 — Non-Invasive Monitoring of Venous Blood Oxygen (SvO₂ / ScvO₂ / Peripheral Venous Oxygenation)

**No new not-yet-catalogued paper this cycle.** The strongest available venous-monitoring references — all previously surfaced and **NOT re-entered** — are carried forward:

- **Hill, Campbell, Chase & Pretty 2024** — jugular optical SvO₂ proof-of-concept; pulse-oximeter-like sensor at the external jugular vein, SvO₂ ≈ 70–72 % in 3 subjects (DOI `10.1515/cdbme-2024-2072`; scan 06-10 §1.1). **Still the repository's closest thing to a true non-invasive named-vein optical SvO₂ result.**
- **Sun et al. 2024** — IJV NIRS + subject-specific Monte Carlo + DNN (*Opt. Lett.* 49:2669; 06-10 §1.2).
- **Jeleff et al. 2023** — Mespere VO100 jugular NIRS device (PMID 37827917; 06-10 §1.3).
- **Oh et al. 2023** — cerebral-NIRS ScvO₂ surrogate via respiration-frequency filtering (DOI `10.1038/s41598-023-49078-1`; 06-10 §1.4).
- **Zachia Alan et al. 2022** — thenar StO₂ → ScvO₂ venous-occlusion (06-10 §1.5).
- **McDiarmid et al. 2026** — cardiac-MRI T₂ iSvO₂, n = 628 survival-endpoint cohort (06-11 §1.1).
- **Skow et al. 2025** — MRI susceptometry venous oximetry (06-14 §1.1).
- **Lahade et al. 2026** — wearable FD-NIRS arterio-venous transition (06-11 §1.2).
- **Tan et al. 2023** — arterial+venous optical e-tattoo (06-17 §1.1).
- **hDOS 2025** — Durduran-group automated venous-occlusion TD-NIRS+DCS platform (06-17 §1.2).
- **Zhang et al. 2016/2017** — induced-venous-fluctuation peripheral SvO₂ (`10.1186/s12938-016-0208-8`, `10.1186/s12938-017-0351-x`; 06-17 §1.3 + honorable mentions).
- **Mileder et al. 2022** — non-invasive peripheral venous saturation in 226 preterm neonates via NIRS venous-occlusion (DOI `10.3389/fped.2022.834045`; catalogued 06-24 §1.1).
- **Peripheral-venous-vs-co-oximetry validation + artificial-venous-pulse PPG family** (06-22).

**Reviewed-and-excluded today (context, no action):** the **capnodynamic** mixed-SvO₂ method (ClinicalTrials.gov NCT06632197) and the **MRI ScvO₂ validation** trial (NCT05161884) — registered trials, not published optical results; the **SjvO₂-NIRS critical-illness** trials (NCT04624009, NCT04778150) and the **Jeleff/Mespere** EJV-NIRS clinical correlation — all within the already-catalogued jugular-NIRS thread.

---

## Topic 2 — Optical Imaging Techniques for Non-Invasive Venous Blood Oxygen

### 2.1 — Benchmarking Deep Learning-Based Reconstruction Methods for Photoacoustic Computed Tomography with Clinically Relevant Synthetic Datasets *(newly catalogued — not previously surfaced)*

- **Title:** Benchmarking Deep Learning-Based Reconstruction Methods for Photoacoustic Computed Tomography with Clinically Relevant Synthetic Datasets
- **Authors:** Panpan Chen, Seonyeong Park, Gangwon Jeong, Refik Mert Cam, Umberto Villa, Mark A. Anastasio
- **Year / Venue:** **2026** (submitted 23 Jan 2026) · **arXiv preprint 2601.17165** (not yet peer-reviewed)
- **Link / DOI:** https://arxiv.org/abs/2601.17165 · https://arxiv.org/html/2601.17165
- **Relevance: 4.5 / 10** — a **methods/validation-infrastructure** paper for PACT *acoustic image reconstruction*, not an oximetry or venous result. It earns a place only as a transferable-technique lead in the deep-vein-PACT pipeline; docked heavily because it neither measures sO₂ nor addresses venous physiology directly. **Not a venous-oxygen result; tissue-/reconstruction-level, general-purpose.**
- **Novelty:** Proposes an **open-source benchmarking framework** with anatomically plausible **synthetic datasets** and standardized, *clinically meaningful* image-quality evaluation strategies for deep-learning–based acoustic-inversion methods in PACT. The paper's argument is that the rapid proliferation of DL reconstruction methods has used non-standardized data and traditional IQ metrics that "may lack clinical relevance," undermining fair comparison and reproducibility — so it supplies a common, physics-grounded testbed for *acoustic* inversion (the upstream step before any quantitative spectral/fluence inversion that yields sO₂).
- **Integration insights:** This is the **acoustic-reconstruction counterpart** to the *spectral/fluence*-inversion methods that dominate this repository's PA thread. Quantitative venous sO₂ from PACT is a two-stage problem: first recover an accurate initial-pressure / absorbed-energy map from the acoustic data (reconstruction), then unmix that map into chromophore concentrations under fluence correction (oximetry). Almost everything catalogued here — Hybrid-Net (06-10 §2.4), the convex-cone TMI paper (06-24 §2.1), the ISDC *J. Biomed. Opt.* paper (06-25 §2.1), the PINN preprint, the JIOHS review (06-17 §2.1) — attacks the *second* stage; this preprint hardens the *first*, and it comes from the **same Anastasio group** as the catalogued **qPACT virtual-imaging framework** (Cam et al., 06-11 §2.4), of which it is the natural successor (shared authors Park, Cam, Villa, Anastasio). A standardized, clinically-relevant reconstruction benchmark is precisely the validation rigor a deep-vein qPACT program (IJV at ~3 cm; femoral/IVC deeper) needs before in-vivo human trials: it lets candidate reconstructors be compared on anatomically realistic phantoms across noise and aberration before the spectral-unmixing stage is even reached. Honest caveat: it is reconstruction infrastructure, PACT-general and arterial/venous-agnostic, and reports no sO₂ — its value to this project is entirely as **upstream plumbing** for the deep-vein quantitative pipeline.
- **Verification:** Title, full author list (Chen, Park, Jeong, Cam, Villa, Anastasio), submission date (23 Jan 2026), and abstract cross-confirmed via the arXiv listing + arXiv HTML mirror; arXiv full text (abs/pdf/html) returned 403 in this environment, so claims beyond the abstract are not read on-source and the venue is flagged as **preprint, not peer-reviewed**.

---

**Previously surfaced — standing optical-imaging references (NOT re-entered):**
Garcia-Uribe/Wang IJV-PA proof-of-concept (arXiv 2303.10775; 06-10 §2.1 — re-confirmed today as **still the only direct human named-vein photoacoustic oximetry result**, sijvO₂ 72 ± 7 %); Kong et al. PACT intra-vessel flow / oxygenation-heterogeneity (PMC11161372; 06-10 §2.2, 06-22/06-24); Zhang et al. PAVT deep haemodynamics (PMC11136879 / arXiv 2209.08706; 06-10 §2.3); Shang et al. **Hybrid-Net** (arXiv 2512.15394; 06-10 §2.4); Huang et al. SFDI-net (PMC12014942; 06-10 §2.5); Liu et al. transmissive HSI single-vessel sO₂ (06-11 §2.1); Feng et al. PA thrombosis spectral-coloring correction (06-11 §2.2); Ter Martirosyan et al. SPOI-AE (06-11 §2.3); **Cam et al. qPACT virtual-imaging framework** (arXiv 2510.03431 / PMC12858365; 06-11 §2.4 — re-surfaced today, the direct predecessor of §2.1 above; not re-entered); Wu et al. vis-OCT review (06-11 §2.5); Basiri et al. SP-SFDI / BioxyDR retinal venous αSO₂ **methods** paper (06-14 §2.1) and the Sept-2025 *Eye* DR-staging clinical paper (DOI 10.1038/s41433-025-04032-5; 06-24 §2.2); Zafar et al. multispectral PAM (06-14 §2.2); Davenet et al. venous-range sulfate phantoms (arXiv 2512.01458; 06-14 §2.3); *Taiwan J. Ophthalmol.* vis-OCT translation review (06-14 §2.4); Zhang & Wang PA-for-PAD review (06-14 §2.5); BMC Ophthalmology macular venular oximetry (06-16 §2.1); Kirchner/Jaeger/Frenz MI-MS-LSD human accompanying-vein oximetry (06-16 §2.2); Quantitative PACT oximetry review (JIOHS, DOI 10.1142/S1793545826300065; 06-17 §2.1); Gu et al. vis-OCT diseased mouse models with explicit venous-sO₂ finding (PMID 41767920; 06-18 §2.1); JHU/Penn multimodal vis-OCT + PLIM (06-18 §2.2); dual-camera high-resolution HSI retina system (PMC12997856; 06-18 §2.3); Frontiers carotid-stenosis automated retinal oximetry A–V difference (PMC12527905; 06-19 §2.1); the convex-cone multispectral-PAT sO₂ paper, IEEE *TMI* (06-24 §2.1); the ISDC transvaginal-PAT sO₂/THb paper, *J. Biomed. Opt.* (DOI 10.1117/1.JBO.31.2.026002; 06-25 §2.1); the OR-PAM vascular-graph ovarian-lesion classifier, *Photoacoustics* (DOI 10.1016/j.pacs.2025.100794; 06-25 §2.2); the awake-mouse cerebral-PA oxygenation bioRxiv preprint (06-24 §2.3); the PINN optical-inversion/spectral-unmixing arXiv 2602.16357 (06-11); the "distribution-informed, wavelength-flexible" data-driven PA oximetry (arXiv 2403.14863) and NIR-II/SWIR PA decoloring (bioRxiv 2024.08.08.607178) transferable-technique leads.

**Honorable mentions / context (not ranked):**
- *Advancements in Photoacoustic Detection Techniques for Biomedical Imaging* — *npj Acoustics* (27 Mar 2025), DOI `10.1038/s44384-025-00005-w`. Reviews PA detection hardware (ultrasonic transducers + optical sensing); not venous-specific. **Already an 06-14 honorable mention** — re-confirmed today, not a new item.
- *Recent advancements in molecular photoacoustic tomography* — IOPscience (DOI `10.1088/2515-7647/adf167`) and *Advances in photoacoustic imaging reconstruction and quantitative analysis* (Springer `10.1186/s42492-025-00213-x` / arXiv 2411.02843) — general PA reviews surfaced today; PACT-general, not venous, carried as context.
- MSOT human-vasculature feasibility / forearm reactive-hyperemia work (RSNA *Radiology* 2016; MDPI *Life* 2022) — established optoacoustic artery/vein discrimination in limbs; predates the catalogued PAVT/IJV results and remains useful background for deep-limb-vein optoacoustic oximetry.

---

## Cross-Topic Synthesis

### What this scan establishes
1. **The literature has plateaued against this repository's coverage.** Two consecutive scans (06-25, 06-27) now return **no new venous-monitoring paper at all**, and 06-27 adds only a single optical-imaging item that is *infrastructure rather than result*. This is the expected shape of a low-volume, well-mined niche: the eleven prior scans captured the field, and the incoming flux is now mostly enabling methods from a handful of active groups (Anastasio/Illinois on qPACT; Zhu/WashU on clinical PAT; the retinal-oximetry community on vis-OCT/HSI/SFDI).

2. **Today's only new item reinforces the dominant trend: PA is advancing on the *upstream-pipeline* problem, not on venous endpoints.** Where 06-24/06-25 added *spectral/fluence-inversion* methods (convex-cone, ISDC), 06-27 adds the *acoustic-reconstruction* benchmarking layer beneath them. The Anastasio group is methodically building the full validation stack for quantitative PACT — phantoms (qPACT VI framework), reconstruction benchmarks (today's preprint), and the spectral-unmixing methods other groups supply — but none of it has yet been pointed at a named deep vein in a human.

3. **The venous-specific frontier is unchanged.** The only direct human named-vein optical SvO₂ results remain Garcia-Uribe/Wang (IJV-PA, 72 ± 7 %) and Hill et al. (EJV optical sensor, ≈70–72 %). The retina remains the one human bed where vessel-resolved venous saturation is routinely measured (vis-OCT, HSI, SP-SFDI), and the venous-occlusion test remains the most clinically-matured *surrogate* route (hDOS, preterm-neonate cohort).

### Persisting gaps (carried forward, unchanged and still open)
- **No 3-D in-vivo human qPACT venous sO₂** at clinical depth (IJV ~3 cm; femoral/IVC deeper). The validation infrastructure is now nearly complete (phantoms + reconstruction benchmark + unmixing/decoloring methods), but the in-vivo demonstration has not been made.
- **No continuous, vessel-specific, blood-gas-calibrated peripheral SvO₂ monitor.** The retinal methods are vessel-specific but confined to the eye; the peripheral/jugular methods are either tissue-averaged (NIRS/VOT) or single-snapshot proof-of-concept (Hill, Garcia-Uribe).
- **The translational chasm** between thin/transparent retina (where venous separation is routine) and thick/opaque peripheral beds (external jugular, basilic, cephalic, femoral) is unbridged.

### Bottom line
An honest empty-to-near-empty cycle. **Topic 1: nothing new.** **Topic 2: one new low-relevance infrastructure preprint** (Chen et al., PACT reconstruction benchmarking, arXiv 2601.17165) entered for completeness as an upstream methods lead in the deep-vein qPACT pipeline. No new direct venous-oxygen result appeared, and the field's state of the art is identical to the previous scan. Reported at face value rather than padded with arterial work.
