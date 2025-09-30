# CombineSVsTITAN
Combining filtered SVs with TITAN copy number results to plot chromosome or Zoom plots

If using the CombineSV repo to combine Structural Variant calls from different callers (Svaba, MANAT, Gridss2), this edited pipeline can be used to combine the SVs with TITAN copy number output for further downstream analysis. These analyses include
Zoom Plots
Chromosome Plots 
Circos Plots

Example command for running this script: 
Rscript combineJasmineTITAN.R --id sample_id --svaba_funcs svaba_utils.R  --svabaVCF **combineSV_file.txt** --titanBinFile TITANfile.titan.ichor.cna.txt --titanSegFile TITANfile.titan.ichor.seg.noSNPs.txt --genomeBuild hg38 --genomeStyle UCSC --minSPAN 0 --minInversionSPAN 1000 --outDir Output_Directory --outputSVFile OutputSVfile.mergedTitan.sv.txt --outputCNFile OutputCopyNumberFile.mergedTitan.cn.txt --outputBedpeFile OutputBEDfile.mergedTitan.sv.bedpe
