# Final Nibi sync required before public tag

The recovered frozen archive contains the real production code/results available at the earlier project checkpoint. The following later-stage production material must be copied verbatim from:

`/scratch/vasilisa/forebrain_hindbrain_ncrna`

before declaring the GitHub repository final.

## cis_analysis
- GENCODE_v50_gene_coordinates.tsv
- 15_lncRNA_cis_protein_coding_1Mb.tsv
- GSE163044_15_lncRNA_cis_correlations.tsv
- GSE286147_15_lncRNA_cis_correlations.tsv
- 29_strong_replicated_cis_pairs_FROZEN.tsv
- 15_lncRNA_controls_radius075.tsv
- matched_control_cis_coupling.tsv
- 15_lncRNA_matched_control_test.tsv
- 15_lncRNA_cis_residual_correlations.tsv
- exact scripts that generated these files

## GSE286146
- metadata/D2_ATAC_runs.tsv
- metadata/D4_ATAC_runs.tsv
- D2/D4 preprocessing scripts
- D2_ATAC_edgeR_QC.R and downstream candidate/LOO scripts
- D4 factorial edgeR scripts
- 29_strong_cis_ATAC_peak_LOO_robustness.tsv
- 29_strong_cis_pairs_ATAC_LOO_summary.tsv
- D4_15_lncRNA_genebody_ATAC_candidate_summary.tsv
- D4_15_lncRNA_promoter_ATAC_three_regions.tsv
- D4_29_strong_cis_ATAC_three_regions_summary.tsv
- D4_29_strong_cis_partner_peaks_with_ID.tsv
- other exact candidate-overlap tables used in the manuscript

## integration
Add the later files:
- GSE286147_GSE286146_15_lncRNA_D4_RNA_ATAC.tsv
- GSE286147_GSE286146_29_cis_pairs_D4_RNA_ATAC.tsv
- D4_RNA_ATAC_key_results.txt
- exact scripts that generated them

Do not reconstruct these production scripts from remembered command fragments; copy the versions actually run on Nibi.
