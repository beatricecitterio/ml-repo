# **Predicting TP53 Mutations in Cancerous Cell Lines** 
_Project for ML Lab by Beatrice Citterio, Clara Montemurro, Martina Serandrei._

The aim of this project is to study how mutations of TP53 can be predicted from genetic expression and how, in turn, these mutations affect the gene expression. 

The project is divided into two main tasks: binary classification (predict mutation) and multi class classification (predict mutation type). We perform both tasks on two different datasets. The first one has been downloaded from CCLE and it contains the genetic expression of several cell lines from different tumors. For each cell line, we were able to retrieve whether TP53 was mutated or not and the type of mutation.

The second dataset was constructed from datasets of different tumor types from TCGA, combined together and then filtered on TP53 mutations. The resulting dataset was much more noisy than the one from CCLE, thus we had to perform a broader exploratory analysis and cleaning.

The repository is structured as follows:
- in results_ccle and results_multiclass we saved plots from training of models, EDA and outlier detection
- ccle_binary_classification.ipynb contains exploratory data analysis on CCLE data, PCA, clustering, outliers detection and finally the classification model: we first tried several models, then performed hyperparameter tuning on the one that worked better. The performance of the model on the whole data was then confronted to the performance on target genes only and on highly differential genes
- ccle_multiclass_classification.ipynb contains prediction of mutation type on CCLE cell lines
- DEGs_filtered_sorted.csv contains the output of differential expression
- differential_expression_analysis.ipynb contain the analysis on which genes vary the most between mutated and non mutated cells
- tcga_binary_classification.ipynb contains binary classification on TCGA data
- tcga_filt.csv is the final output of the thorough cleaning performed on TCGA data