# PMA
Supplementary data for "Is the Protein Model Assignment problem under linked branch lengths NP-hard?"

This package contains the three partitioned and formerly published source data sets in the archaea bacteria and eukaryotes folders. Each of these folders contains subfolders 1 to 50 for the subsamples. The subsamples have been removed to reduce size (to reconstruct the data samples run bash ./01_reconstruct_samples.sh).


01_reconstruct_samples.sh	script to reconstruct the data samples

02_compute_pma.sh		conduct exhausitive and naive model assignment

03_compute_ml.sh		conduct maximum likelihood inference using naive and exhaustive PMA
04_compute_rf.sh		compute the RF distances between the inferred trees
05_evaluate.sh			summarize assignment differences and compute average rf-diastances (creates model_diffs.txt, summary.txt, and rf_dists.txt)
archaea				archaeatic data and data sub-samples
bacteria			bacteria data and data sub-samples
bin				necessary binaries and scripts
eukaryotes			eukaryotic data and data sub-samples
model_diffs.txt			contains the difference in PMA for each data sample
summary.txt			contains overall summary of differeing PMA and RF-distance
rf_dists.txt			contains the rf-distances of the fully optimized ML tree for data samples where naive and exhaustive PMA are different
README				this file
