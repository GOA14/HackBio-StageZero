From FASTQ to Figure: Why Most Bioinformatics Pipelines Fail at the Last Mile

# Introduction

Bioinformatics is a field that applies computational, mathematical, and statistical tools to collect and analyze biological data. A bioinformatics pipeline is a set of algorithms that are executed in a specific or predefined order to process biological data (Roy et al., 2018). Next Generation Sequencing (NGS) is known to generate millions of short-read sequences of DNA or RNA isolated from a sample. This is why bioinformatics pipelines are very important, a system is needed whereby these reads can be analyzed accurately without having to process them individually, which is known as automation. (Mantere et al., 2019).

# Typical Steps in a Bioinformatics Pipeline

A typical pipeline for analysing raw reads starts with checking the quality of the reads, which is known as Quality Control (QC). The tool commonly used is FastQC, followed by trimming of adapters using fastp, mapping the reads to a reference genome using bwa, then variant calling, filtering, and finally visualisation (Chen et al., 2017).

# Visualization as the Final Step

Each step has its usefulness, as shown above, but after all these steps have been completed, we reach the last step, which should be considered vital; visualisation. This is the step where biological insights are obtained. One way of visualising data in some cases is by building a phylogenetic tree. This gives information about the relationship a sample has with existing ones, basically showing family relationships. Without proper visualisation, we would not be able to get this information; instead, it would just be a series of data that cannot be interpreted, despite running it through the pipeline (O'Donoghue et al., 2021).

# Why Pipelines Fail at the Last Mile ?

Despite the importance of visualisation, it is still treated as if it is not part of the pipeline. Most bioinformaticians or scientists tend to give more attention to the earlier steps because they are seen as the core of the workflow. Most of the time, effort is focused on alignment, mapping, and building reference datasets, with the mindset that once these are done, everything is complete and visualisation can be rushed. Some people even visualise separately, meaning it is not part of their pipeline at all. This is wrong and leads to poorly structured figures.

# Conclusion

Treating visualisation as not important or as not part of the pipeline, it negates the main importance of a pipeline and bioinformatics itself, which are automation and reproducibility. Automation refers to running the steps automatically without stress once the pipeline is tested and functional, while reproducibility is the ability for another user or another sample to reuse the pipeline and obtain very similar results (Ziemann et al., 2023; Baykal, 2024). When visualisation is done separately, it cannot be reproducible, especially at the final stage, and figures are the storytellers of the analysis.

In bioinformatics, R is commonly used for visualisation due to the fact that plots can be generated completely using code, making it possible to reproduce results when the pipeline is rerun Wickham, 2016). Treating visualisation as part of the pipeline, and not just as a simple task, using clear and structured code will help produce clearer, more reliable, and more reproducible results.

# REFERENCES

Baykal, P. I. (2024). Genomic reproducibility in the bioinformatics era. Genome Biology.

Chen, S., Huang, T., Zhou, Y., Han, Y., Xu, M., & Gu, J. (2017). AfterQC: Automatic filtering,

trimming, error removing and quality control for FASTQ data. BMC Bioinformatics, 18.

Djaffardjy, M. (2023). Developing and reusing bioinformatics data analysis pipelines. Computational

and Structural Biotechnology Journal.

Mantere, T., Kersten, S., & Hoischen, A. (2019). Long-read sequencing emerging in medical genetics.

Frontiers in Genetics, 10, 426.

O'Donoghue, S. I., et al. (2021). Grand challenges in bioinformatics data visualization. Frontiers in

Bioinformatics.

Roy, S., Coldren, C., Karunamurthy, A., et al. (2018). Standards and guidelines for validating next-

generation sequencing bioinformatics pipelines. Journal of Molecular Diagnostics, 20, 4-27.

Wickham, H. (2016). ggplot2: Elegant Graphics for Data Analysis. Springer.

Ziemann, M., Poulain, P., & Bora, A. (2023). The five pillars of computational reproducibility:

Bioinformatics and beyond. Briefings in Bioinformatics.
