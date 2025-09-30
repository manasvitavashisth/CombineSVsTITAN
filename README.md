# CombineSVsTITAN
Combining filtered SVs with TITAN copy number results to plot chromosome or Zoom plots

If using the CombineSV repo to combine Structural Variant calls from different callers (Svaba, MANAT, Gridss2), this edited pipeline can be used to combine the SVs with TITAN copy number output for further downstream analysis. These analyses include
Zoom Plots
Chromosome Plots 
Circos Plots

Example command for running this script: 
Rscript /fh/fast/ha_g/projects/ProstateTAN/analysis_CN-SV/JASMINE/code/combineJasmineTITAN.R --id 19-048_cfPL_39_WGS --svaba_funcs /fh/fast/ha_g/projects/ProstateTAN/analysis_CN-SV/JASMINE/code/svaba_utils.R  --svabaVCF /fh/fast/ha_g/projects/ProstateTAN/analysis_CN-SV/SV/output/TwoOverlap/19-048_cfPL_39_WGS_TwoOverlap_chr.txt --titanBinFile /fh/fast/ha_g/projects/ProstateTAN/analysis_CN-SV/optimalTITAN/19-048_cfPL_39_WGS_cluster1.titan.ichor.cna.txt --titanSegFile /fh/fast/ha_g/projects/ProstateTAN/analysis_CN-SV/optimalTITAN/19-048_cfPL_39_WGS_cluster1.titan.ichor.seg.noSNPs.txt --genomeBuild hg38 --genomeStyle UCSC --minSPAN 0 --minInversionSPAN 1000 --outDir /fh/fast/ha_g/projects/ProstateTAN/analysis_CN-SV/SV/output/TwoOverlap/19-048_cfPL_39_WGS --outputSVFile /fh/fast/ha_g/projects/ProstateTAN/analysis_CN-SV/SV/output/TwoOverlap/19-048_cfPL_39_WGS/19-048_cfPL_39_WGS.mergedTitan.sv.txt --outputCNFile /fh/fast/ha_g/projects/ProstateTAN/analysis_CN-SV/SV/output/TwoOverlap/19-048_cfPL_39_WGS/19-048_cfPL_39_WGS.mergedTitan.cn.txt --outputBedpeFile /fh/fast/ha_g/projects/ProstateTAN/analysis_CN-SV/SV/output/TwoOverlap/19-048_cfPL_39_WGS/19-048_cfPL_39_WGS.mergedTitan.sv.bedpe
