# Genome-wide association and genomic prediction for Fe and Zn concentration and Fe bioavailability in a yellow bean collection of dry beans

## Abstract
Dry bean is a nutrient-dense food targeted in biofortification programs to increase seed iron and zinc levels. 
The underlying assumption of breeding for higher mineral content is that enhanced iron and zinc levels will 
deliver health benefits to the consumers of these biofortified foods. This study characterized a diversity 
panel of 295 genotypes comprising the Yellow Bean Collection (YBC) for seed Fe and Zn concentration, 
Fe bioavailability (FeBio), and seed yield across two years in two field locations. The genetic architecture 
of each trait was elucidated via genome-wide association studies (GWAS) and the efficacy of genomic prediction (GP) 
was assessed. Moreover, 82 yellow breeding lines were evaluated for seed Fe and Zn concentrations as well as seed yield, 
serving as a prediction set for GP models. Large phenotypic variability was identified in all traits evaluated, and variations 
of up to 2.8 and 13.7-fold were observed for Fe concentration and FeBio, respectively. Prediction accuracies in the YBC ranged 
from a low of 0.12 for Fe concentration, to a high of 0.72 for FeBio, and an accuracy improvement of 0.03 was observed when a QTN, 
identified through GWAS, was used as a fixed effect for FeBio. This study provides evidence of the lack of correlation between 
FeBio estimated in vitro and Fe concentration and highlights the potential of GP in accurately predicting FeBio in yellow beans, 
offering a cost-effective alternative to the traditional assessment of using Caco2 cell methodologies.

https://doi.org/10.3389/fgene.2024.1330361 

## Organization of this repository
### Scripts:
1. R script for analyzing correlations, generating figures, conducting variance component analysis, performing GWAS, PCA, and kinship, and evaluating phenotypes of families and seed color.
2. R script for running SSI and RKHS models on the training dataset for Yield, Fe, and Zn in MI and NE for the years 2018-2019.
3. R script for running SSI and RKHS models with QTN information to the training dataset for FeBio in MI over 2018-2019.
4. R script for running SSI and RKHS models on the prediction set utilizing the entire YBC.
5. R script for running SSI and RKHS models on the prediction set using the Andean accessions from the YBC.

### Data:

- YBC_GWASAssistedGP.RData: R List containing the Phenotype, Genotype, Hapmap, and SNPs positions.
- YBC_phenotype_Color_CT.csv: CSV file containing agronomic, mineral traits collected in this study, and cooking time, seed type, population structure, and gene pool information collected by Sadohara et al., 2021 (https://doi.org/10.1002/tpg2.20173) and Sadohara et al., 2022 (https://doi.org/10.1007/s10722-021-01323-0).
- Raw Sequencing Data available at https://www.ncbi.nlm.nih.gov/bioproject/1061170
