# Methods Resources
Resources that cover methods and procedures for bioinformatics, statistics, and
machine learning.

## Bioinformatics
| Resource  | Description |
|-----------|-------------|
| [High Throughput Sequencing - StatQuest](https://www.youtube.com/playlist?list=PLblh5JKOoLUJo2Q6xK4tZElbIvAACEykp) | Josh Starmer explains RNASeq, ChiPSeq, DESeq2, PCA, Expression Heatmaps, RPKM/FPKM/TPM and more        |
| [RNASeq RPKM vs FPKM vs TPM](https://haroldpimentel.wordpress.com/2014/05/08/what-the-fpkm-a-review-rna-seq-expression-units/)          |  Reviews different RNASeq units common in the literature |
| [RNASeq Between Sample Normalization](https://haroldpimentel.wordpress.com/2014/12/08/in-rna-seq-2-2-between-sample-normalization/)          | Why FPKM and TPM aren't comparable between samples and library normalization is needed |
| [Single-Cell RNASeq Data in R](https://osca.bioconductor.org) | Tutorial explaining how to use Bioconductor packages to efficiently manipulate single cell data |
| [Broad Single-Cell RNASeq Tutorial](https://broadinstitute.github.io/2019_scWorkshop/) | 2019 Broad workshop on how to analyze sc-RNAseq data |
| [Computational Genomics with R](http://compgenomr.github.io/book/) | Great introduction to different areas of bioinformatics using R |
| [RNA-Seq Differential Expression Walkthrough](https://hbctraining.github.io/DGE_workshop_salmon/schedule/) | Harvard Broad workshop that covers the entire DEG workflow: sample QC, count normalization, DE analysis, visualization, and functional analysis. |
| [Microarray Data Analysis](http://bioinformatics-core-shared-training.github.io/microarray-analysis/) | Workshop covering microarray DE analysis for GEO data using `limma`. |
| [FastQC Plots: Good vs Bad Plots](https://rtsf.natsci.msu.edu/genomics/tech-notes/fastqc-tutorial-and-faq/) | Tutorial describing how to interpret `FastQC` plots with examples of good and bad data |
| [CoMutPlotter: Visualize Mutation Data](http://tardis.cgu.edu.tw/comutplotter/) | Online tool to visualize mutation heatmaps and include clinical characteristics for a sequencing cohort |
| [Check RNASeq Strandedness](https://fishycat.netlify.com/en/2017/08/strandness_in_rnaseq/) | Use different RNASeq alignment programs to check if RNASeq data is stranded or unstranded |
| [RNASeq Strandedness Explanation](https://chipster.csc.fi/manual/library-type-summary.html) | Explains unstranded vs stranded vs reverse stranded and how to use RSeQC to check the strandedness of FASTQ data |


## Statistics
| Resource  | Description |
|-----------|-------------|
| [StatQuest](https://www.youtube.com/playlist?list=PLblh5JKOoLUJo2Q6xK4tZElbIvAACEykp) | Khan Academy style videos by Josh Starmer on distributions, parameters, linear models, machine learning, bioinformatics, and R |
| [Statistical Tests Are Linear Models](https://lindeloev.github.io/tests-as-linear/) | Common statistical tests such as the t-test and ANOVA are just specialized forms of linear models |
| [Flexible Imputation For Missing Data](https://stefvanbuuren.name/fimd/) | Statistical aspects of missing data. Covers MCAR/MAR/MNAR assumptions, complete-case analysis, and MICE imputation methods |
| [Modern Statistics For Modern Biology](https://www-huber.embl.de/msmb/index.html) | Intro statistics for bioinformatics applications. Covers distributions, PCA, hypothesis testing, RNASeq analysis, machine learning, experimental design |
| [Biostatistics For Biomedical Research](http://hbiostat.org/doc/bbr.pdf) | Intro biostatistics, regression models, randomized controlled trials (RCTs), observational studies, diagnosis, statistical pitfalls, high dimensional modeling |
| [Statistical Problems to Avoid](http://biostat.mc.vanderbilt.edu/wiki/Main/ManuscriptChecklist) | Common statistical issues to think about in the design, analysis, and publication of research |
| [Common Statistical Misconceptions](https://discourse.datamethods.org/t/reference-collection-to-push-back-against-common-statistical-myths/1787) | List of statistical misconceptions with sources to disprove each misconception | 
| [Regression Modeling Strategies](http://hbiostat.org/doc/rms.pdf) | Comprehensive dive into regression modeling covers linear, logistic, and ordinal regression as well as survival analysis with lots of case studies |
| [Communicating Frequentist Results](https://discourse.datamethods.org/t/language-for-communicating-frequentist-results-about-treatment-effects/934) | Proper way to describe treatment effects according to frequentist theory |
| [Bayesian Re-analysis of Toss Up Clinical Trial](https://discourse.datamethods.org/t/andromeda-shock-or-how-to-intepret-hr-0-76-95-ci-0-55-1-02-p-0-06/1349) | How to interpret clinical trials that slightly miss p < .05 cutoff and bayesian methods to re-analyze trials | 
| [Statistics Glossary](http://hbiostat.org/doc/glossary.pdf) | Glossary of Statistical Terms |
| [Observed Power should be avoided](https://discourse.datamethods.org/t/observed-power-and-other-power-issues/731) | Issues with observed power overestimating the study's true power, misleading researchers |
| [Observed Power Simulation Study](https://lesslikely.com/statistics/observed-power-magic/) | Simulation study showing problems with observed power | 
| [Criticisms of ROC curves for medical decision-making](https://discourse.datamethods.org/t/sensitivity-specificity-and-roc-curves-are-not-needed-for-good-medical-decision-making/1152) | Problems with using ROC curves to evaluate the quality of medical decision-making models |
| [Table 1 P-values in RCTs](https://discourse.datamethods.org/t/should-we-ignore-covariate-imbalance-and-stop-presenting-a-stratified-table-one-for-randomized-trials/547) | Baseline differences should not be tested in RCTs as differences are already due to chance from randomization |
| [Pseudo R^2 Explanation](https://stats.idre.ucla.edu/other/mult-pkg/faq/general/faq-what-are-pseudo-r-squareds/) | Intuitive explanation behind OLS R^2 and generalizes this intuition to pseduo R^2 measures for binary outcomes |
| [GLMs Explained](https://newonlinecourses.science.psu.edu/stat504/node/216/) | Introduction to Generalized Linear Models (GLMs) |
| [Multicollinearity and Omitted Variable Bias](https://are.berkeley.edu/courses/EEP118/current/handouts/OVB%20versus%20Multicollinearity_eep118_sp15.pdf) | Distinction between collinearity and omitted variable bias |
| [Cox PH Diagnostics](https://www.ics.uci.edu/~dgillen/STAT255/Handouts/lecture10.pdf) | Guide to checking Cox PH regression assumptions |
| [Dealing with Unbalanced Datasets](https://github.com/matloff/regtools/blob/master/UnbalancedClasses.md) | Why resampling techniques should be avoided when analyzing datasets with unbalanced outcomes |
| [Statistical Rethinking with `brms`](https://bookdown.org/content/4857/) | Uses `brms` and `tidyverse` code instead of base R |
| [Interpretting P-Value Histogram](http://varianceexplained.org/statistics/interpreting-pvalue-histogram/) | How to interpret results from running several statistical tests before adjusting for multiple comparisons|



## Machine Learning
| Resource  | Description |
|-----------|-------------|
| [ML Resources](https://sgfin.github.io/learning-resources/) | Tons of resources on all areas of machine learning including theory, practice, causal inference, DL, NLP, and RL |

## Visualization
| Resource  | Description |
|-----------|-------------|
| [Data Visualization with ggplot2](http://socviz.co/index.html#preface) | Theory and practice of data visualization using `ggplot2` | 
| [ggplot2 Categorical Heatmaps](https://stackoverflow.com/questions/12998372/heatmap-like-plot-but-for-categorical-variables) | How to plot heatmaps showing categorical variable in `ggplot2`|
| [Dynamite Plots Should Be Avoided](https://simplystatistics.org/2019/02/21/dynamite-plots-must-die/) | Why dynamite plots should be discarded and replaced with boxplots or violin plots|
| [Colorspace Color Library](https://cran.r-project.org/web/packages/colorspace/vignettes/colorspace.html) | More color options with `colorspace` R package |
