# A Gillis lab guide to papers in functional genomics (and beyond)
 What we talk about when we talk about ... 

## Co-expression 
|      Nickname(s)     |     Citation  and URL     |     Main    Takeaways/Comments     |     Keywords     |
| ---------------------|--------------------------------|------------------------------------|------------------ |
|    The   Eisen Paper                            |    Eisen,   M.B., Spellman, P.T., Brown, P.O., and Botstein, D. (1998). Cluster analysis   and display of genome-wide expression patterns. Proceedings of the National   Academy of Sciences of the United States of America 95, 14863-14868.                                                                                                              http://www.pnas.org/content/95/25/14863                                            |    -         in expression data, genes cluster according to their   function = can infer functions for unannotated genes   -                                                                                                                                                |    Coexpression,   microarray, gene function                                    |
|    Paul’s   coexpression meta-analysis Paper    |    Lee,   H.K., Hsu, A.K., Sajdak, J., Qin, J., and Pavlidis, P. (2004). Coexpression   analysis of human genes across many microarray data sets. Genome research   14, 1085-1094.                                                                                                                                                                         https://www.ncbi.nlm.nih.gov/pubmed/15173114                                       |    -         confirmation of coexpression in multiple data sets is   correlated with functional relatedness   -         cluster analysis of the aggregate network reveals   functionally coherent groups of genes                                                           |    Paul,   coexpression, meta-analysis, microarray, human, GO                   |
|                                                 |    Gaiteri   C, Ding Y, French B, Tseng GC, Sibille E. Beyond modules and hubs: the   potential of gene coexpression networks for investigating molecular   mechanisms of complex brain disorders. Genes, brain, and behavior.   2014;13(1):13-24. Epub 2013/12/11. doi: 10.1111/gbb.12106. PubMed PMID:   24320616; PubMed Central PMCID: PMCPMC3896950   https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3896950                               |    -         Review on sources of co-expression and use in brain   specific analyses                                                                                                                                                                                        |    Co-expression,   brainspan, brain                                            |
|    That   Speed Paper                           |    Freytag   S, Gagnon-Bartsch J, Speed TP, Bahlo M. Systematic noise degrades gene   co-expression signals but can be corrected. BMC Bioinformatics.   2015;16(1):309. doi: 10.1186/s12859-015-0745-3                                                                                                                                                     https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-015-0745-3     |    -         Assessment of the effects of RUV on gene coexpression    -         Claims that RUV corrected data is better in generating   good coexpression networks    -         but true effect of removing variation is not always clear   (biology versus technical)     |    Gene   co-expression, Data cleaning, Removal of unwanted variation (RUV)     |



## RNA-seq 
|     Nickname(s)     |     Citation  and URL     |     Main    Takeaways/Comments     |     Keywords     |
|---------------------|--------------------------------|------------------------------------|------------------|
|    MAQC   paper                      |    SEQC/MAQC-III   Consortium. A comprehensive assessment of RNA-seq accuracy, reproducibility   and information content by the Sequencing Quality Control Consortium. Nat   Biotech. 2014;32(9):903-14. doi: 10.1038/nbt.2957                                      https://www.nature.com/articles/nbt.2957                                       |    -         Low expressing genes are unreliable in RNA-seq due to   technical and methodological biases    -         Filter away bottom third of genes (low expressing) and   fold changes > 2    -         STAR performs well         |    RNA-seq,   biases, expression, STAR    |
|    SEQC   collection                 |                                                                                                                                                                                                                                                                     https://www.nature.com/collections/ppgrhzcwpf                                            |                                                                                                                                                                                                                                         |                                           |
|    STAR   paper                      |    Dobin   A, Davis CA, Schlesinger F, Drenkow J, Zaleski C, Jha S, et al. STAR:   ultrafast universal RNA-seq aligner. Bioinformatics. 2013;29(1):15-21. doi:   10.1093/bioinformatics/bts635. PubMed PMID: PMC3530905                                             https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3530905/                          |    -         STAR is awesome/useful/practical and fast.   -         Also, funny ROC.                                                                                                                                                    |    STAR,   software, RNA-seq alignment    |
|    MAD   scores paper                |    Teng   M, Love MI, Davis CA, Djebali S, Dobin A, Graveley BR, et al. A benchmark for   RNA-seq quantification pipelines. Genome Biology. 2016;17(1):74. doi:   10.1186/s13059-016-0940-1                                                                         https://genomebiology.biomedcentral.com/articles/10.1186/s13059-016-0940-1     |    -         Correlations are a bad metric when dynamic range is high   (eg. RNA-seq expression data)                                                                                                                                   |    Metrics,   expression, benchmarking    |
|    The   Leek Batch Effects Paper    |    Leek,   J.T., Scharpf, R.B., Bravo, H.C., Simcha, D., Langmead, B., Johnson, W.E.,   Geman, D., Baggerly, K., and Irizarry, R.A. (2010). Tackling the widespread   and critical impact of batch effects in high-throughput data. Nat Rev Genet   11, 733-739.    https://www.ncbi.nlm.nih.gov/pubmed/20838408                                   |    -         Batch effects are common and pernicious in high   throughput biological data                                                                                                                                               |    Batch   effects, Irizarry              |
|   Perils of batch correction 1 (Jaffe)     |    Jaffe, A.E., et al., Practical impacts of genomic data “cleaning” on biological discovery using surrogate variable analysis. BMC Bioinformatics, 2015. 16(1): p. 1-10.  https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-015-0808-5                              |    -	It’s easy to remove real signal if you aren’t careful with your batch correction                                                                                                                                                |    Batch   effects              |
|   Perils of batch correction 2 (Nygaard)     |    Nygaard, V., Rødland, E.A. & Hovig, E. Methods that remove batch effects while retaining group differences may lead to exaggerated confidence in downstream analyses. Biostatistics (Oxford, England) 17, 29-39 (2015). https://academic.oup.com/biostatistics/article/17/1/29/1744261                         |    -		It’s easy to over-estimate confidence after batch correction, particularly with unbalanced experimental designs                                                                                                                                                  |    Batch   effects              |

## Single cell 
|     Nickname(s)     |     Citation and URL    |     Main    Takeaways/Comments     |     Keywords     |
|---------------------|--------------------------------|------------------------------------|------------------|
|    Monocle                                                      |    Trapnell,   C., Cacchiarelli, D., Grimsby, J., Pokharel, P., Li, S., Morse, M., Lennon,   N.J., Livak, K.J., Mikkelsen, T.S., and Rinn, J.L. (2014). The dynamics and   regulators of cell fate decisions are revealed by pseudotemporal ordering of   single cells. Nat Biotech 32, 381-386.   https://www.nature.com/articles/nbt.2859  |    -         cells can ordered in ‘pseudotime’ for developmental   trajectory inference                                                                                                  |    Single cell,   pseudotime                                   |
|    The Hicks Paper                                              |    Hicks,   S.C., Townes, F.W., Teng, M., and Irizarry, R.A. (2017). Missing data and   technical variability in single-cell RNA-sequencing experiments.   Biostatistics (Oxford, England). https://www.ncbi.nlm.nih.gov/pubmed/29121214   |    -         there are huge batch effects in single cell RNA-seq   data which can be misinterpreted as biological variability   -         PC1 is usually correlated with the number of genes   detected per cell     |    Batch effects, single   cell, Irizarry                      |
|    Single cell   experimental design                            |    Tung, P.-Y., Blischak, J.D., Hsiao, C.J., Knowles,   D.A., Burnett, J.E., Pritchard, J.K., and Gilad, Y. (2017). Batch effects and   the effective design of single-cell gene expression studies. Scientific   Reports 7, 39921.   https://www.nature.com/articles/srep39921                                                              |    -         higher correlation of samples from the same individual   within batches than across    -         ERCCs are affected by biological variation in batches   so can’t be used to get rid of technical variation   -         Recommend combining individuals in one technical   replicate as a way to save money   -         75 cells with 1.5 million reads is sufficient                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |    Batch effects, single   cell, experimental design           |
|    The Macosko paper;   The Drop-seq paper; The retina paper    |    Macosko, E.Z., Basu, A., Satija, R., Nemesh,   J., Shekhar, K., Goldman, M., Tirosh, I., Bialas, A.R., Kamitaki, N.,   Martersteck, E.M., et al. (2015). Highly Parallel Genome-wide Expression   Profiling of Individual Cells Using Nanoliter Droplets. Cell 161, 1202-1214.   https://www.cell.com/abstract/S0092-8674(15)00549-8                |    -         first demonstration of Drop-seq    -         39 cell type clusters identified using 7 replicates   (multiple animals per replicate)   -         first to use tSNE and projection (of held-out cells)   onto the reduced dimensional space    -         first to use Louvain clustering in single cell RNA-seq   (had previously been used for cytof by Dana Pe’er’s group)   -         lots of interesting stuff to go through in the   supplement                                                                                                                                                                                                                                                                                                                                                                                                                                                          |    Single cell,   drop-seq, tSNE, clustering, replicability    |
|    The Shekhar paper;   The bipolar cell paper                  |    Shekhar, K., et al. (2016). "Comprehensive   Classification of Retinal Bipolar Neurons by Single-Cell   Transcriptomics." Cell 166(5): 1308-1323.e1330.         https://www.cell.com/cell/abstract/S0092-8674(16)31007-8                                                                                                                                 |    -         Drop-seq and Smart-seq2, two Cre-driver lines   -         Random forest classifier from clusters, re-classified data   from Macosko    -         More cells with few genes is better than few cells with   many genes for defining clusters   -         Tried many different dimensionality reduction and   clustering techniques                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |    Single cell, drop-seq                                       |
|    The Heimberg paper                                           |    Heimberg, G., et al. (2016). "Low Dimensionality   in Gene Expression Data Enables the Accurate Extraction of Transcriptional   Programs from Shallow Sequencing." Cell Syst 2(4): 239-250   https://www.cell.com/fulltext/S2405-4712(16)30109-0                                                                                                    |    -         Shallow sequencing is sufficient for cell typing because   cell types differ across many genes that co-vary                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |    Single cell, theory,   dimensionality                       |
|    RNA velocity                                                 |    La Manno, G., et al. (2018). "RNA velocity of   single cells." Nature 560(7719): 494      https://www.nature.com/articles/s41586-018-0414-6                                                                                                                                                                                                       |    -         The fraction of unspliced to spliced mRNA for certain   genes provides temporal information about cell differentiation (expansion of Zeisel   2011)   -         Requires kNN smoothing (5-10 samples)   -         Commentary from Pachter and Svennson here: https://doi.org/10.1016/j.molcel.2018.09.026                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |    Single cell, trajectory,   pseudotime                       |
|    The Soneson/Robinson   DE paper                              |    Soneson, C. and M. D. Robinson (2018). "Bias,   robustness and scalability in single-cell differential expression   analysis." Nat Methods 15(4): 255-261.  https://www.nature.com/articles/nmeth.4612                                                                                                                                     |    -         T-test and Mann-Whitney are better for scDE than tests   with more distributional assumptions                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |    Single cell, DE, comparative   assessment                   |
|    The Soneson/Robinson   clustering paper                      |    Duò, A., et al. (2018). "A systematic performance   evaluation of clustering methods for single-cell RNA-seq data [version 2;   referees: 2 approved]." F1000Research 7(1141).   https://f1000research.com/articles/7-1141/v1                                                                                                                |    -         Clustering algorithms have different results   -         Seurat and SC3 generally good. Seurat very stable   across different gene selection strategies (high expression, HVG, M3Drop)   -         Combining two methods into an ensemble did not improve   the performance compared to the best of the individual methods   -         “We also investigated whether the number of detected   features per cell differed between the clusters, using a Kruskal-Wallis test.   No strong association was found for the simulated data sets indicating that   there is low inherent bias in the clustering algorithms. For most of the real   data sets, we found highly significant differences in the number of detected   features between cells in different clusters. However, it is unclear whether   this represents a technical effect or a biological difference between the   cell populations.”    |    Single cell, clustering,   comparative assessment           |



## Human genetics 
|     Nickname(s)     |     Citation  and URL     |     Main    Takeaways/Comments     |     Keywords     |
|---------------------|--------------------------------|------------------------------------|------------------|
|    AJHG   skew paper                      |    Amos-Landgraf   JM, Cottle A, Plenge RM, Friez M, Schwartz CE, Longshore J, et al. X   Chromosome–Inactivation Patterns of 1,005 Phenotypically Unaffected Females.   American Journal of Human Genetics. 2006;79(3):493-9. PubMed PMID: PMC1559535       http://www.cell.com/ajhg/fulltext/S0002-9297(07)62748-7                                    |    -         Skew ratios within a population of women are normally   distributed    -         First “large” scale XCI analysis using the AR   X-inactivation assay (HUMARA)                                                                                                                                                                                                 |    X-inactivation,   X-skew, tissue dependent                 |
|    MacArthur   XCI paper                  |    Tukiainen T, Villani A-C, Yen A, Rivas MA,   Marshall JL, Satija R, et al. Landscape of X chromosome inactivation across   human tissues. Nature. 2017;550:244. doi: 10.1038/nature24265                                                                  https://www.nature.com/articles/nature24265                                                |    -         Assessment of GTEx data for XCI and incomplete   inactivation (escapers)    -         First “large” scale use of RNA-seq data for XCI                                                                                                                                                                                                                          |    Dosage   compensation, GTEx, X-inactivation, X-escapers    |
|    GWAs                                   |    Hirschhorn JN, Daly MJ. Genome-wide   association studies for common diseases and complex traits. Nature Reviews   Genetics. 2005;6:95. doi: 10.1038/nrg1521                                                                                              https://www.nature.com/articles/nrg1521                                                    |    -         Key paper on the thoughts/ideas behind genome wide   association studies for complex disorders                                                                                                                                                                                                                                                                 |    GWAs,   SNPs, LD                                           |
|    Disease   networks (Barabasi paper)    |    Goh K-I, Cusick ME, Valle D, Childs B, Vidal   M, Barabási A-L. The human disease network. Proceedings of the National   Academy of Sciences. 2007;104(21):8685-90. doi: 10.1073/pnas.0701361104.                                                         http://www.pnas.org/content/104/21/8685.long                                                         |                                                                                                                                                                                                                                                                                                                                                                             |                                                               |
|    Polygenic   risk scores                |    The International Schizophrenia C. Common   polygenic variation contributes to risk of schizophrenia and bipolar   disorder. Nature. 2009;460:748. doi: 10.1038/nature08185                                                                               https://www.nature.com/articles/nature08185                                                |    -         Scores to explain distributed risk of disease                                                                                                                                                                                                                                                                                                                  |    GWAs,   risk scores                                        |
|    Wigler   paper                         |    Ronemus M, Iossifov I, Levy D, Wigler M. The   role of de novo mutations in the genetics of autism spectrum disorders.   Nature Reviews Genetics. 2014;15:133. doi: 10.1038/nrg3585                                                                       https://www.nature.com/articles/nrg3585                                                    |    -         De novo mutations                                                                                                                                                                                                                                                                                                                                              |    Autism,   de novo, recurrence                              |
|    Ivan’s   paper                         |    Iossifov I, O’Roak BJ, Sanders SJ, Ronemus M,   Krumm N, Levy D, et al. The contribution of de novo coding mutations to   autism spectrum disorder. Nature. 2014;515(7526):216-21. doi:   10.1038/nature13908. PubMed PMID: PMC4313871                    https://www.nature.com/articles/nature13908                                                |    -         Recurrent genes in autism   -         LGD (likely gene disruptive)                                                                                                                                                                                                                                                                                             |    Autism,   de novo, recurrence                              |
|    PGC   paper                            |    Schizophrenia Working Group of the Psychiatric   Genomics C. Biological insights from 108 schizophrenia-associated genetic   loci. Nature. 2014;511:421. doi: 10.1038/nature13595                                                                         https://www.nature.com/articles/nature13595                                                |    -         Schizophrenia loci are still mostly in non-coding regions   of the genome                                                                                                                                                                                                                                                                                      |    Schizophrenia,   GWAs                                      |
|    ExAC   paper                           |    Lek M, Karczewski KJ, Minikel EV, Samocha KE,   Banks E, Fennell T, et al. Analysis of protein-coding genetic variation in   60,706 humans. Nature. 2016;536:285. doi: 10.1038/nature19057                                                                https://www.nature.com/articles/nature19057                                                |    -         Background variation in the human population   -         Knockout variants via depletion   -         PLI scores for genes    (probability of being loss-of-function (LoF) intolerant)                                                                                                                                                                          |    Variant   scores, WES                                      |
|    RVIS   paper                           |    Petrovski S, Wang Q, Heinzen EL, Allen AS,   Goldstein DB. Genic Intolerance to Functional Variation and the   Interpretation of Personal Genomes. PLOS Genetics. 2013;9(8):e1003709. doi:   10.1371/journal.pgen.1003709                                 http://journals.plos.org/plosgenetics/article/citation?id=10.1371/journal.pgen.1003709     |    -         Scores for variation intolerance   -         Precedes the ExAC PLI scores    -         genes responsible for Mendelian diseases are significantly   more intolerant to functional genetic variation than genes that do not cause   any known disease, but with striking variation in intolerance among genes   causing different classes of genetic disease    |    Variant   scores, WES                                      |


## Network analysis 
|     Nickname(s)     |     Citation  and URL     |     Main    Takeaways/Comments     |     Keywords     |
|---------------------|--------------------------------|------------------------------------|------------------|
|    The   first WGCNA Paper                  |    Zhang, B., and Horvath, S. (2005). A general   framework for weighted gene co-expression network analysis. Statistical   applications in genetics and molecular biology 4, Article17.           https://www.ncbi.nlm.nih.gov/pubmed/16646834                                      |    -         Argue for weighted networks over binary networks   -         Weighted networks lead to more cohesive modules                                                                                                                                                                                                                                                                                                                 |    Coexpression,   network analysis, clustering, WGCNA                  |
|    The   Dynamic Tree Cutting Paper         |    Langfelder, P., Zhang, B., and Horvath, S.   (2008). Defining clusters from a hierarchical cluster tree: the Dynamic Tree   Cut package for R. Bioinformatics (Oxford, England) 24, 719-720.    https://www.ncbi.nlm.nih.gov/pubmed/18024473                                      |    -         dynamic tree cutting can yield more intuitive clusters   than picking a cut height on a dendrograms                                                                                                                                                                                                                                                                                                                          |    Clustering,   WGCNA, R, Bioconductor                                 |
|    The   WGCNA Module Preservation Paper    |    Langfelder, P., Luo, R., Oldham, M.C., and   Horvath, S. (2011). Is My Network Module Preserved and Reproducible? PLOS   Computational Biology 7, e1001057.                                     http://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1001057     |    -         Applying cluster stability/validation methods to gene   networks   -         “We   find that it is advantageous to aggregate multiple preservation statistics   into summary preservation statistics”   -         “Cluster validation statistics may not be appropriate when   modules are not defined as clusters. In general, assessing module preservation is a different task from   assessing cluster preservation.”    |    Clustering,   replicability, network analysis, WGCNA, metrics        |

## Machine learning 
|     Nickname(s)     |     Citation  and URL     |     Main    Takeaways/Comments     |     Keywords     |
|---------------------|--------------------------------|------------------------------------|------------------|
|    Hand   paper                |    Hand DJ. Classifier technology and the   illusion of progress. Statistical science. 2006:1-14                                                                                                                                                                             https://arxiv.org/pdf/math/0606441.pdf                                       |    -         simple methods are often surprisingly effective     |    Machine   learning                                        |
|    GeneMania   / MouseFunc     |    Peña-Castillo, L., Tasan, M., Myers, C.L.,   Lee, H., Joshi, T., Zhang, C., Guan, Y., Leone, M., Pagnani, A., Kim, W.K.,   et al. (2008). A critical assessment of Mus musculus gene function   prediction using integrated genomic evidence. Genome biology 9, S2-S2.    https://genomebiology.biomedcentral.com/articles/10.1186/gb-2008-9-s1-s2     |    -         Gene function prediction is hard                    |    Machine   learning, gene function, critical assessment    |
|    CAFA                        |    Radivojac P, Clark WT, Oron TR, Schnoes AM,   Wittkop T, Sokolov A, et al. A large-scale evaluation of computational   protein function prediction. Nature Methods. 2013;10:221. doi:   10.1038/nmeth.2340                                                                https://www.nature.com/articles/nmeth.2340                                   |    -         BLAST works okay compared to “naïve” methods        |    Competitions,   machine learning                          |

## Gene set enrichment analysis 
|     Nickname(s)     |     Citation  and URL     |     Main    Takeaways/Comments     |     Keywords     |
|---------------------|--------------------------------|------------------------------------|------------------|
|    Goeman   2007                                          |    Goeman, J.J., and Buhlmann, P. (2007).   Analyzing gene expression data in terms of gene sets: methodological issues.   Bioinformatics (Oxford, England) 23, 980-987.                                                https://academic.oup.com/bioinformatics/article-abstract/23/8/980/198511     |    -         For enrichment analysis, sample permutation and gene   permutation have different underlying assumptions   -         Gene permutation does not take coexpression into account,   making p-values easily misinterpreted/”anti-conservative”   -         Competitive gene set testing “creates an unnecessary rift   between single gene testing and gene set testing”    |    Functional   enrichment, commentary                                       |
|    Irizarry’s   Enrichment Paper (The Anti-GSEA Paper)    |    Irizarry, R.A., Wang, C., Zhou, Y., and   Speed, T.P. (2009). Gene set enrichment analysis made simple. Statistical   methods in medical research 18, 565-575.                                                       https://www.ncbi.nlm.nih.gov/pubmed/20048385                                 |    -         GSEA is unnecessarily complicated                                                                                                                                                                                                                                                                                                                                       |    Functional   enrichment, expression analysis, Irizarry, simple methods    |
|    Tamayo   2012                                          |    Tamayo, P., Steinhardt, G., Liberzon, A., and   Mesirov, J.P. (2016). The limitations of simple gene set enrichment analysis   assuming gene independence. Statistical methods in medical research 25,   472-487.    https://www.ncbi.nlm.nih.gov/pubmed/23070592                                 |    -         Gene coexpression invalidates simple gene set enrichment   approaches                                                                                                                                                                                                                                                                                                   |    Coexpression,   functional enrichment                                     |

## Statistics 
|     Nickname(s)     |     Citation  and URL     |     Main    Takeaways/Comments     |     Keywords     |
|---------------------|--------------------------------|------------------------------------|------------------|
|    FDR                          |    Noble   WS. How does multiple testing correction work? Nature biotechnology.   2009;27(12):1135-7. doi: 10.1038/nbt1209-1135. PubMed PMID: PMC2907892.                                                                        https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2907892/                      |                                                                                                                                                                                                                                                                                                                                                                                      |    Multiple   test correction                          |
|    The   Gap Statistic Paper    |    Tibshirani, R., Walther, G., and Hastie, T.   (2001). Estimating the number of clusters in a data set via the gap   statistic. Journal of the Royal Statistical Society: Series B (Statistical   Methodology) 63, 411-423.    https://statweb.stanford.edu/~gwalther/gap                       |    -         Propose the ‘gap statistic’ for estimating the number of   clusters in a set of data    -         “The technique uses the output of any clustering algorithm,   comparing the change in within-cluster dispersion with   that expected under an appropriate reference null distribution.”                                                                               |    Clustering,   Tibshirani, metrics                   |
|    Tibshirani   2005            |    Tibshirani, R., and Walther, G. (2005).   Cluster validation by prediction strength. Journal of Computational and   Graphical Statistics 14, 511-528.                                                                         http://statweb.stanford.edu/~gwalther/predictionstrength.pdf     |    -         “This article   proposes a new quantity for assessing the number of groups or clusters in a   dataset. The key idea is to view clustering as a supervised classification   problem, in which we must also estimate the “true” class labels. The   resulting “prediction strength” measure assesses how many groups can be   predicted from the data, and how well.”     |    Clustering,   Tibshirani, replicability, metrics    |

