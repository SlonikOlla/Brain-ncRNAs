# Frozen analysis contract

## RNA
- Genome: GRCh38.p14
- Annotation: GENCODE Human Release 50
- Salmon: 2.7.0, decoy-aware selective alignment
- GSE163044 library: ISR
- GSE286147 library: IU
- tximport: 1.34.0
- DESeq2: 1.46.0
- Gene filter: row-summed counts >= 10
- Significance: Benjamini-Hochberg FDR < 0.05
- Strong effect: |log2FC| >= 1

## Primary contrasts
- GSE163044: neocortex minus posterior brainstem; model `~ embryo + region`
- GSE286147 D2: aNE minus pNE
- GSE286147 D4: `~ lineage + medium + lineage:medium`

## Replicated lncRNAs
Stringent replicated candidates were lncRNAs with FDR < 0.05 and |log2FC| >= 1 in both primary datasets and the same fold-change direction. This yielded 15 concordant lncRNAs.

## Final cis analysis
- Operational neighborhood: protein-coding genes within ±1 Mb of each of the 15 lncRNAs.
- 335 candidate lncRNA-coding pairs.
- Strong replicated coupling: same direction and |Spearman rho| >= 0.5 in both RNA systems.
- 29 pairs, 12/15 lncRNAs, 26 unique coding partners.
- |rho| >= 0.5 is an effect-size criterion, not a significance threshold.
- Developmental-state residualization reduced the strong cross-system set to 12.
- Matched-control analysis did not produce BH-significant candidate-level enrichment.

## Final ATAC analysis
- fastp 0.23.4
- Bowtie2 2.5.4: `--very-sensitive -I 10 -X 2000`
- samblaster 0.1.26
- SAMtools 1.22.1
- BEDTools 2.31.0
- featureCounts/Subread 2.0.6
- edgeR 4.6.3, robust quasi-likelihood framework
- D2 ATAC is a temporally matched sensitivity/context analysis.
- D4 provides the stronger accessibility evidence.
- Directional stability/concordance is not interpreted as causality or peak-level significance.
