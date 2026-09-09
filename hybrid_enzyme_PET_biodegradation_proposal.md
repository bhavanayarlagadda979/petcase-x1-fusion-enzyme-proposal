# Rational Design of a Hybrid PETase–Cutinase–Biosurfactant-Binding Fusion Enzyme ("PETCase-X1") for Enhanced Polyester Biodegradation: A Research Proposal

> **Note on nature of this document:** This is a *research proposal / hypothesis document*, prepared for personal study purposes by synthesizing themes from nine published papers on enzymatic biodegradation of plastics and other environmental pollutants. The enzyme "PETCase-X1" described here is a **hypothetical, not-yet-synthesized construct**. No wet-lab or computational experiments have actually been performed for this proposal. The "Expected Results" section describes **projected outcomes inferred from trends reported in the literature**, not measured data. This distinction is preserved throughout so the document can be used safely as a study/planning tool rather than mistaken for a completed study.

---

## 1. Abstract

Polyethylene terephthalate (PET) and related synthetic polyesters are among the most persistent plastic pollutants in marine and terrestrial ecosystems. Over the past decade, research has identified a range of microbial hydrolases — PETases, cutinases, MHETases, carboxylesterases, and lipases — capable of depolymerizing PET into its monomers, and computational (in silico) approaches such as molecular docking and molecular dynamics (MD) have become central tools for engineering more active and thermostable variantsPET biodegradation has been investigated using wild-type microorganisms, isolated or engineered enzymes, wild consortia, and genetically modified microorganisms, with in silico simulations of enzyme-PET complexes proving useful for predicting molecular interactions and designing new enzymes for PET biodegradation. Building on these findings, this proposal outlines the rational design of a hypothetical trifunctional fusion enzyme, PETCase-X1, combining (i) a PETase catalytic domain optimized for aromatic polyester hydrolysis, (ii) a thermostable cutinase domain for broader polyester/aliphatic-ester specificity, and (iii) a small biosurfactant-binding peptide linker intended to improve enzyme access to the hydrophobic, low-bioavailability plastic surface. We propose an integrated in silico–to–in vitro workflow: homology modeling and docking of the fusion construct against PET/BHET substrates, MD simulation of active-site dynamics, heterologous expression in *E. coli* or *Komagataella phaffii*, and standard hydrolysis assays (mass loss, released terephthalic acid/BHET quantification by HPLC, surface analysis by SEM/AFM). Expected outcomes, projected from comparable literature trends rather than measured here, include improved catalytic turnover on crystalline PET relative to single-domain PETase and enhanced activity on weathered/microplastic substrates due to the surfactant-binding module. This proposal is intended as a framework for future experimental validation rather than a report of completed research.

---

## 2. Introduction

### 2.1 The plastic pollution problem and the case for enzymatic solutions

PET is one of the most widely produced petroleum-derived plastics, valued for packaging and textiles, but its chemical stability makes it highly resistant to natural degradation, leading to long-term accumulation in marine and terrestrial environments. Conventional treatment methods — incineration, landfilling, and pyrolysis — carry high energy costs and secondary pollution risks, which has driven interest in biological and enzymatic alternatives as more sustainable routes for plastic waste management.

### 2.2 State of the art: microbial and enzymatic PET degradation

A substantial body of experimental work has characterized microorganisms and enzymes capable of PET breakdown. Approximately 30 bacterial genera, including Bacillus, Ideonella, and Pseudomonas, and 15 fungal genera, including Fusarium, Trichoderma, and Alternaria, have been studied over the past decade for PET biodegradation owing to their production of predominantly hydrolase enzymes, with wild consortia and mixed enzyme systems also showing degradation potential. Among these, *Ideonella sakaiensis* and its PETase enzyme remain the most extensively studied system, and cutinase-family enzymes such as leaf-branch compost cutinase (LCC) and its engineered variants have demonstrated particularly high hydrolytic efficiency toward PET.

Beyond PET-specific hydrolases, other enzyme families relevant to environmental biodegradation more broadly include esterases, laccases, dehydrogenases, and oxygenases, which have been documented to catalyze breakdown of diverse organic contaminants ranging from antibiotics to pesticides. In one representative computational–experimental study, engineered laccase and catalase-peroxidase enzymes were shown to degrade a panel of antibiotics with efficiency that, for laccase, exceeded that of a commercial reference enzyme against several compounds, illustrating how enzyme engineering guided by computational prediction can outperform native or commercial biocatalystsEnzyme activity assays corroborated computational results, indicating both enzymes could degrade all tested antibiotics with varying efficiencies, with the engineered laccase outperforming commercial laccase against several antibiotics.

### 2.3 The role of in silico methods

In silico docking and molecular dynamics have become standard tools for predicting how a plastic-degrading enzyme's active site interacts with its polymer substrate, and for guiding mutagenesis before committing to wet-lab synthesis. This approach has been applied specifically to PET-hydrolyzing systems, including studies evaluating candidate bacterial enzymes for their predicted ability to degrade downstream PET intermediates such as mono(2-hydroxyethyl) terephthalate, using computational screening to prioritize which natural enzyme variants merit experimental follow-upplastic waste has historically been treated using conventional methods such as incineration and landfilling, or advanced approaches such as pyrolysis and thermodegradation, prompting the use of in silico evaluation of degradation efficiency for plastic-degrading enzymes such as MHETase from selected bacteria.

### 2.4 Motivation for a fusion-enzyme approach

Despite these advances, single-domain PET hydrolases still face two persistent limitations reported across the literature: (a) restricted activity on high-crystallinity or weathered PET due to poor substrate accessibility, and (b) narrow substrate range, generally limited to PET/BHET rather than the mixed aliphatic–aromatic polyester waste streams found in real environments. Broader surveys of bioremediation enzymes emphasize that discovering or engineering new enzyme variants with tailored physicochemical properties remains one of the most promising directions for improving pollutant-degradation efficiency and cost-effectivenessenzymes play the most crucial role in bioremediation, and discovering new enzymes and new subtypes with specific physicochemical characteristics would be a promising way to find more efficient and cost-effective tools for the remediation of pollutants. This motivates a fusion-protein strategy that combines complementary catalytic domains with a substrate-access-enhancing module in a single biocatalyst, rather than relying on one enzyme alone or on multi-enzyme cocktails that require separate production and formulation.

### 2.5 Objectives of this proposal

1. Design, in silico, a trifunctional fusion enzyme (PETCase-X1) combining a PETase catalytic domain, a thermostable cutinase domain, and a biosurfactant-binding linker peptide.
2. Predict, via docking and MD simulation, whether the fusion architecture preserves or enhances substrate binding relative to its parent domains.
3. Propose a heterologous expression and purification strategy suitable for producing PETCase-X1 for subsequent wet-lab testing.
4. Propose a standardized hydrolysis-assay protocol to evaluate PETCase-X1 activity on PET film, powder, and post-consumer microplastic, against appropriate single-domain enzyme controls.

---

## 3. Materials (Proposed)

**Enzyme design inputs**
- Reference crystal structures: *Ideonella sakaiensis* PETase (PDB 6EQE/5XJH), leaf-branch compost cutinase (LCC) or *Thermobifida fusca* cutinase, and a short biosurfactant-binding peptide motif (e.g., derived from a known hydrophobin or surfactin-binding sequence) as candidate linker.
- Substrate structures: PET dimer/trimer models, bis(2-hydroxyethyl) terephthalate (BHET), mono(2-hydroxyethyl) terephthalate (MHET), and amorphous vs. crystalline PET surface models.

**Computational tools (proposed)**
- Homology modeling: SWISS-MODEL or AlphaFold2.
- Molecular docking: AutoDock Vina or Glide.
- Molecular dynamics: GROMACS or AMBER, explicit solvent (TIP3P), 100–500 ns production runs.
- Binding free-energy estimation: MM-PBSA/MM-GBSA.

**Wet-lab materials (proposed, for later validation)**
- Expression host: *Escherichia coli* BL21(DE3) or *Komagataella phaffii* (for secreted, disulfide-rich constructs).
- Substrates: commercial PET film (amorphous, ~7% crystallinity) and post-consumer PET bottle flakes (higher crystallinity), plus a polylactide (PLA) or polycaprolactone (PCL) sample to test the cutinase domain's broader specificity.
- Analytical equipment: HPLC (for terephthalic acid, MHET, BHET quantification), UV-Vis plate reader (for colorimetric esterase activity, e.g., pNP-butyrate assay), SEM and AFM (for surface morphology), and DSC (for crystallinity changes).

---

## 4. Proposed Methodology / Procedure

### Stage 1 — In silico design and screening
1. Build homology models of the PETase and cutinase catalytic domains individually, then construct candidate fusion architectures (N-terminal PETase–linker–cutinase–C-terminal surfactant peptide, and the reverse order) to compare folding stability.
2. Dock each fusion model against PET oligomer and BHET substrates; rank candidates by predicted binding affinity and pose plausibility (catalytic triad alignment with the scissile ester bond).
3. Run MD simulations (≥100 ns, triplicate) on the top two or three fusion candidates to assess active-site flexibility, domain–domain interference, and linker stability, following the general active-site-flexibility rationale established for wild-type PETase.
4. Select the best-performing in silico candidate for downstream (proposed) synthesis.

### Stage 2 — Gene synthesis and heterologous expression (proposed)
1. Codon-optimize the selected fusion sequence for the chosen expression host.
2. Clone into an inducible expression vector with a cleavable affinity tag (His6 or Strep-tag).
3. Express under low-temperature induction to favor correct folding of the multi-domain construct; purify by affinity chromatography followed by size-exclusion chromatography to isolate correctly folded monomeric fusion protein.
4. Confirm identity and purity by SDS-PAGE and mass spectrometry.

### Stage 3 — Enzymatic characterization (proposed)
1. Determine basic kinetic parameters (K_m, k_cat) using a soluble ester substrate (e.g., pNP-butyrate) as a proxy assay before testing on solid PET.
2. Incubate purified PETCase-X1 with PET film, PET powder, and post-consumer PET flakes at a range of temperatures (30–70 °C) and pH (6–9), alongside single-domain PETase and cutinase controls and a no-enzyme blank.
3. Quantify degradation products (terephthalic acid, MHET, BHET) released into the supernatant by HPLC at defined time points (0, 24, 48, 72, 120 h).
4. Assess surface changes on PET samples by SEM/AFM and crystallinity shifts by DSC before and after incubation.
5. Repeat the assay on PLA/PCL substrate to test whether the cutinase domain broadens substrate range as intended.

### Stage 4 — Data analysis (proposed)
1. Compare degradation rates and product yields of PETCase-X1 against single-domain controls using ANOVA with post-hoc testing.
2. Correlate MD-predicted binding free energies with observed activity trends to validate (or refute) the computational design assumptions.

---

## 5. Expected Results *(Projected — Not Measured Data)*

The following are **hypotheses about likely outcomes**, extrapolated from patterns reported for comparable single- and multi-domain PET-hydrolase systems in the literature. They are explicitly **not** experimental findings.

- **Binding affinity:** The fusion construct is expected to retain docking scores comparable to or modestly better than the parent PETase domain alone, provided the linker does not sterically interfere with the catalytic cleft — consistent with prior reports that active-site flexibility, not just binding affinity, is a key determinant of PET-hydrolase efficiency.
- **Substrate range:** Because it combines a PETase and a cutinase domain, PETCase-X1 is hypothesized to show measurable activity on both PET and at least one non-PET polyester (e.g., PCL), unlike single-domain PETase, which is typically PET/BHET-specific.
- **Activity on crystalline vs. amorphous PET:** Based on trends where pretreatment or biosurfactant assistance improves access to hydrophobic, higher-crystallinity substrate, the biosurfactant-binding module is hypothesized to narrow (but not eliminate) the known gap in degradation rate between amorphous and crystalline PET.
- **Thermostability:** If the cutinase domain contributes disulfide-stabilized folding, the fusion may tolerate a somewhat higher operating temperature than wild-type PETase alone, though multi-domain fusions often show *reduced* stability relative to their smallest parent domain — this is a genuine risk, not a guaranteed improvement, and should be treated as an open question for the proposed experiments.
- **Overall degradation yield:** A modest (not dramatic) improvement in cumulative terephthalic acid release relative to single-domain PETase over a multi-day assay is the most defensible projection; multi-enzyme or engineered systems in the literature generally report incremental rather than order-of-magnitude gains over well-optimized single enzymes.

---

## 6. Discussion *(Anticipated, Framed as Hypothesis)*

If the projected outcomes above were confirmed experimentally, they would suggest that fusion-protein engineering — combining catalytic breadth (cutinase) with targeting/access enhancement (biosurfactant-binding peptide) — is a viable complement to point-mutation engineering strategies that dominate the current PETase literature. This would align with the broader recommendation in the field that future research should move toward consortia-based or synergistic enzymatic systems rather than optimizing single enzymes in isolationFuture research should focus on consortia-based or synergistic enzymatic systems to develop scalable biodegradation techniques, and the use of biosurfactant-producing strains is crucial to increase polymer bioavailability and enhance hydrolysis. A fusion enzyme can be viewed as a single-molecule analogue of such a synergistic consortium.

However, several caveats should be anticipated regardless of outcome:
- **Domain interference is a real risk.** Multi-domain fusions frequently underperform their individually optimized parent domains due to steric clash, aggregation, or misfolding; this proposal's MD-simulation stage is specifically designed to catch this failure mode early, in silico, before committing to wet-lab synthesis.
- **In silico predictions are not a substitute for wet-lab validation.** Docking and MD provide plausible hypotheses about binding and flexibility, but binding free-energy estimates and experimental activity have not always correlated cleanly in the PETase literature; discrepancies should be expected and investigated, not treated as experimental error.
- **Scale-up and industrial relevance remain open questions.** Even a successful lab-scale fusion enzyme would need to be evaluated for cost of production, operational stability in mixed waste streams, and compatibility with existing PET recycling infrastructure before any claim of practical utility.

---

## 7. Conclusion and Future Directions

This proposal synthesizes recurring themes across the plastic- and pollutant-biodegradation literature — the centrality of hydrolase enzymes (PETase, cutinase, MHETase, esterase), the increasing role of in silico docking/MD in enzyme design, and the recognized value of biosurfactant-assisted substrate access — into a single hypothetical fusion-enzyme design. The proposed PETCase-X1 construct and its associated in silico-to-in vitro workflow are intended as a template for future, actual experimental work rather than a finished study. Natural next steps, beyond the scope of this proposal, would include securing gene synthesis, performing the described MD/docking screen computationally, and — only after promising in silico results — proceeding to wet-lab expression and the enzymatic assays outlined in Section 4.

---

## References

1. Hernández-Nava, A.M., Cuahquentzi-Sánchez, M., Santacruz-Juárez, E., et al. (2025). Degradation of polyethylene terephthalate by microorganisms and their enzymes: A review of experimental and in silico research. *World Journal of Microbiology and Biotechnology*, 41, 485. https://doi.org/10.1007/s11274-025-04706-y
2. [Enzyme-assisted degradation of environmental contaminants, antibiotic degradation by engineered laccase/catalase-peroxidase]. *ScienceDirect* (chapter). https://www.sciencedirect.com/science/article/abs/pii/B978032395090900011X
3. Watts, T., Khoba, K., & Purty, R.S. (2023). In silico approach for evaluating the degradation efficiency of plastic degrading enzyme mono(2-hydroxyethyl) terephthalic acid hydrolase (MHETase) of selected bacteria. *Bioremediation Journal*, 28(4), 541–552. https://doi.org/10.1080/10889868.2023.2279201
4. Mousavi, S.M., Hashemi, S.A., Moezzi, S.M.I., et al. (2021). Recent Advances in Enzymes for the Bioremediation of Pollutants. *Biochemistry Research International*, 2021, 5599204.
5. Charupanit, K., Tipmanee, V., Sutthibutpong, T., & Limsakul, P. (2022). In silico identification of potential sites for a plastic-degrading enzyme by a reverse screening through the protein sequence space and molecular dynamics simulations. *Molecules*, 27(10), 3353.
6. Additional source papers referenced by the user (paywalled beyond abstract at time of writing): ScienceDirect S2772416622000328; ScienceDirect S2211715626006867; Tandfonline 10.1080/10889868.2022.2054931; Springer 10.1007/s10532-026-10248-3; ACS AEACC4 5(6):520; Cell Heliyon S2405-8440(25)00019-2. Full-text subheadings for these could not be retrieved due to publisher access restrictions; only abstracts/metadata were accessible and are not separately cited above to avoid overclaiming content not actually read.

*Note: References 6 lists the links you originally shared that returned only paywalled abstracts or were blocked to automated access (ScienceDirect, Tandfonline, ACS full-text). If you have PDF access to these (e.g., via institutional login), share the text or key sections and I can incorporate their specific findings and sub-headings directly into a revised version of this proposal.*
