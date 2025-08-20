> id: https://www.nature.com/articles/s41588-025-02293-0

> link: https://www.nature.com/articles/s41588-025-02293-0

> title: A comparison of 27 Arabidopsis thaliana genomes and the path toward an unbiased characterization of genetic polymorphism

# A comparison of 27 Arabidopsis thaliana genomes and the path toward an unbiased characterization of genetic polymorphism
_Published on Tue, 19 Aug 2025 00:00:00 GMT_

Abstract
--------

Making sense of whole-genome polymorphism data is challenging, but it is essential for overcoming the biases in SNP data. Here we analyze 27 genomes of _Arabidopsis thaliana_ to illustrate these issues. Genome size variation is mostly due to tandem repeat regions that are difficult to assemble. However, while the rest of the genome varies little in length, it is full of structural variants, mostly due to transposon insertions. Because of this, the pangenome coordinate system grows rapidly with sample size and ultimately becomes 70% larger than the size of any single genome, even for _n_ = 27. Finally, we show how short-read data are biased by read mapping. SNP calling is biased by the choice of reference genome, and both transcriptome and methylome profiling results are affected by mapping reads to a reference genome rather than to the genome of the assayed individual.

### Similar content being viewed by others

![](https://media.springernature.com/w215h120/springer-static/image/art%3A10.1038%2Fs41588-024-01715-9/MediaObjects/41588_2024_1715_Fig1_HTML.png)

### [A pan-genome of 69 _Arabidopsis thaliana_ accessions reveals a conserved genome structure throughout the global species range](https://www.nature.com/articles/s41588-024-01715-9?fromPaywallRec=false)

Article Open access 11 April 2024

![](https://media.springernature.com/w215h120/springer-static/image/art%3A10.1038%2Fs41467-023-42029-4/MediaObjects/41467_2023_42029_Fig1_HTML.png)

### [The pan-genome and local adaptation of _Arabidopsis thaliana_](https://www.nature.com/articles/s41467-023-42029-4?fromPaywallRec=false)

Article Open access 06 October 2023

![](https://media.springernature.com/w215h120/springer-static/image/art%3A10.1038%2Fs41437-024-00688-z/MediaObjects/41437_2024_688_Fig1_HTML.png)

### [Dual-trait genomic analysis in highly stratified _Arabidopsis thaliana_ populations using genome-wide association summary statistics](https://www.nature.com/articles/s41437-024-00688-z?fromPaywallRec=false)

Article 31 May 2024

Main
----

The last 25 years have witnessed an explosion of genetic polymorphism data, fueled by Human Genome Project-inspired collaborations and the development of massively parallel technologies for sequencing and genotyping. Such data allow us to study population history, selection and genetic architecture of traits, as well as the evolution of the genome itself. However, our current view of genetic polymorphism has been shaped by technologies that attempt to align short sequence fragments to a reference genome to detect sites that differ. As a result, our knowledge of genome variation has remained incomplete and biased towards simple variants in regions that are easy to align—a small fraction of the genome in many species. A further source of bias arises from the use of a single reference genome.

All this is beginning to change now that long reads are making it possible to assemble high-quality, full-length chromosomal sequences from population samples. During the last couple of years, nearly complete genomes have been produced for large numbers of eukaryotic species, including yeast, animals (including fruit flies, humans and cichlids) and many plants, including rice, tomato, soybean, grapevine, wheat, barley, maize, millet, _Brassica oleracea_, _Eucalyptus_, _Populus_ and _Marchantia_ sp.—as well as _Arabidopsis thaliana_[1](https://www.nature.com/articles/s41588-025-02293-0#ref-CR1 "Gallone, B. et al. Domestication and divergence of Saccharomyces cerevisiae beer yeasts. Cell 166, 1397–1410 (2016)."),[2](https://www.nature.com/articles/s41588-025-02293-0#ref-CR2 "Istace, B. et al. De novo assembly and population genomic survey of natural yeast isolates with the Oxford Nanopore MinION sequencer. GigaScience 6, 1–13 (2017)."),[3](https://www.nature.com/articles/s41588-025-02293-0#ref-CR3 "Peter, J. et al. Genome evolution across 1,011 Saccharomyces cerevisiae isolates. Nature 556, 339–344 (2018)."),[4](https://www.nature.com/articles/s41588-025-02293-0#ref-CR4 "Walkowiak, S. et al. Multiple wheat genomes reveal global variation in modern breeding. Nature 588, 277–283 (2020)."),[5](https://www.nature.com/articles/s41588-025-02293-0#ref-CR5 "Alonge, M. et al. Major impacts of widespread structural variation on gene expression and crop improvement in tomato. Cell 182, 145–161 (2020)."),[6](https://www.nature.com/articles/s41588-025-02293-0#ref-CR6 "Jayakodi, M. et al. The barley pan-genome reveals the hidden legacy of mutation breeding. Nature 588, 284–289 (2020)."),[7](https://www.nature.com/articles/s41588-025-02293-0#ref-CR7 "Hufford, M. B. et al. De novo assembly, annotation, and comparative analysis of 26 diverse maize genomes. Science 373, 655–662 (2021)."),[8](https://www.nature.com/articles/s41588-025-02293-0#ref-CR8 "Liu, Y. et al. Pan-Genome of wild and cultivated soybeans. Cell 182, 162–176 (2020)."),[9](https://www.nature.com/articles/s41588-025-02293-0#ref-CR9 "Qin, P. et al. Pan-genome analysis of 33 genetically diverse rice accessions reveals hidden genomic variations. Cell 184, 3542–3558 (2021)."),[10](https://www.nature.com/articles/s41588-025-02293-0#ref-CR10 "Ebert, P. et al. Haplotype-resolved diverse human genomes and integrated analysis of structural variation. Science 372, eabf7117 (2021)."),[11](https://www.nature.com/articles/s41588-025-02293-0#ref-CR11 "Rech, G. E. et al. Population-scale long-read sequencing uncovers transposable elements associated with gene expression variation and adaptive signatures in Drosophila. Nat. Commun. 13, 1948 (2022)."),[12](https://www.nature.com/articles/s41588-025-02293-0#ref-CR12 "Zhou, Y. et al. Graph pangenome captures missing heritability and empowers tomato breeding. Nature 606, 527–534 (2022)."),[13](https://www.nature.com/articles/s41588-025-02293-0#ref-CR13 "Li, R. et al. A sheep pangenome reveals the spectrum of structural variations and their effects on tail phenotypes. Genome Res. 33, 463–477 (2023)."),[14](https://www.nature.com/articles/s41588-025-02293-0#ref-CR14 "Ferguson, S. et al. Plant genome evolution in the genus Eucalyptus is driven by structural rearrangements that promote sequence divergence. Genome Res. 34, 606–619 (2024)."),[15](https://www.nature.com/articles/s41588-025-02293-0#ref-CR15 "Liao, W.-W. et al. A draft human pangenome reference. Nature 617, 312–324 (2023)."),[16](https://www.nature.com/articles/s41588-025-02293-0#ref-CR16 "Wlodzimierz, P. et al. Cycles of satellite and transposon evolution in Arabidopsis centromeres. Nature 618, 557–565 (2023)."),[17](https://www.nature.com/articles/s41588-025-02293-0#ref-CR17 "He, Q. et al. A graph-based genome and pan-genome variation of the model plant Setaria. Nat. Genet. 55, 1232–1242 (2023)."),[18](https://www.nature.com/articles/s41588-025-02293-0#ref-CR18 "Shi, T. et al. The super-pangenome of Populus unveils genomic facets for its adaptation and diversification in widespread forest trees. Mol. Plant 17, 725–746 (2024)."),[19](https://www.nature.com/articles/s41588-025-02293-0#ref-CR19 "Kang, M. et al. The pan-genome and local adaptation of Arabidopsis thaliana. Nat. Commun. 14, 6259 (2023)."),[20](https://www.nature.com/articles/s41588-025-02293-0#ref-CR20 "Cochetel, N. et al. A super-pangenome of the North American wild grape species. Genome Biol. 24, 290 (2023)."),[21](https://www.nature.com/articles/s41588-025-02293-0#ref-CR21 "Beaulieu, C. et al. The Marchantia polymorpha pangenome reveals ancient mechanisms of plant adaptation to the environment. Nat. Genet. 57, 729–740 (2025)."),[22](https://www.nature.com/articles/s41588-025-02293-0#ref-CR22 "Li, X. et al. Large-scale gene expression alterations introduced by structural variation drive morphotype diversification in Brassica oleracea. Nat. Genet. 56, 517–529 (2024)."),[23](https://www.nature.com/articles/s41588-025-02293-0#ref-CR23 "Lian, Q. et al. A pan-genome of 69 Arabidopsis thaliana accessions reveals a conserved genome structure throughout the global species range. Nat. Genet. 56, 982–991 (2024)."),[24](https://www.nature.com/articles/s41588-025-02293-0#ref-CR24 "Kileeg, Z., Wang, P. & Mott, G. A. Chromosome-scale assembly and annotation of eight Arabidopsis thaliana ecotypes. Genome Biol. Evol. 16, evae169 (2024)."),[25](https://www.nature.com/articles/s41588-025-02293-0#ref-CR25 "Quah, F. X. et al. Lake Malawi cichlid pangenome graph reveals extensive structural variation driven by transposable elements. Genome Res. 35, 1094–1107 (2025)."),[26](https://www.nature.com/articles/s41588-025-02293-0#ref-CR26 "Schloissnig, S. et al. Long-read sequencing and structural variant characterization in 1,019 samples from the 1000 Genomes Project. Preprint at bioRxiv 
https://doi.org/10.1101/2024.04.18.590093
(2024)."),[27](https://www.nature.com/articles/s41588-025-02293-0#ref-CR27 "Jiao, C. et al. Pan-genome bridges wheat structural variations with habitat and breeding. Nature 637, 384–393 (2025)."). Impressive as these studies are, they have also highlighted the difficulty in making sense of whole-genome polymorphism data, primarily because sequence alignment is not unambiguous. Pangenome graphs[28](https://www.nature.com/articles/s41588-025-02293-0#ref-CR28 "Eizenga, J. M. et al. Pangenome graphs. Annu. Rev. Genomics Hum. Genet. 21, 139–162 (2020)."),[29](https://www.nature.com/articles/s41588-025-02293-0#ref-CR29 "Garrison, E. et al. Building pangenome graphs. Nat. Methods 21, 2008–2012 (2024).") may provide elegant and computationally efficient ways of representing such data, but they do not solve this fundamental problem. To compare genomes and interpret their differences properly, we require a modeling framework that reflects the mutational mechanisms and recombination history that gave rise to these differences, but such a framework is still largely missing.

Here we illustrate this problem by analyzing the genomes of 27 natural inbred accessions of _A. thaliana_, chosen to cover the global genetic diversity of the species. Our focus is on obtaining an unbiased picture of polymorphism in the more easily alignable chromosome arms and comparing it to existing data built over almost two decades[30](https://www.nature.com/articles/s41588-025-02293-0#ref-CR30 "Nordborg, M. et al. The pattern of polymorphism in Arabidopsis thaliana. PLoS Biol. 3, e196 (2005)."),[31](https://www.nature.com/articles/s41588-025-02293-0#ref-CR31 "Clark, R. M. et al. Common sequence polymorphisms shaping genetic diversity in Arabidopsis thaliana. Science 317, 338–342 (2007)."),[32](https://www.nature.com/articles/s41588-025-02293-0#ref-CR32 "Atwell, S. et al. Genome-wide association study of 107 phenotypes in Arabidopsis thaliana inbred lines. Nature 465, 627–631 (2010)."),[33](https://www.nature.com/articles/s41588-025-02293-0#ref-CR33 "Horton, M. W. et al. Genome-wide patterns of genetic variation in worldwide Arabidopsis thaliana accessions from the RegMap panel. Nat. Genet. 44, 212–216 (2012)."),[34](https://www.nature.com/articles/s41588-025-02293-0#ref-CR34 "1001 Genomes Consortium. 1,135 genomes reveal the global pattern of polymorphism in Arabidopsis thaliana. Cell 166, 481–491 (2016)."). To provide an unbiased picture of the ‘gene-ome’, that is, the collection of genes across multiple genomes, we complement our genome assemblies with transcriptomes from multiple tissues for the entire sample. In addition, we seek to lay the foundation for a community resource that will eventually comprise complete genomes for the thousands of natural inbred accessions that are publicly available for this model plant, thus connecting whole-genome polymorphism data to experimentally accessible germplasm and knowledge of a wide range of morphological, life-history, physiological and molecular phenotypes, as well as precise collection information ([https://1001genomes.org/](https://1001genomes.org/)).

Results
-------

### The organization of genome variation

We selected 27 accessions to cover global genetic variation of the species based on the original 1001 Genomes Project[34](https://www.nature.com/articles/s41588-025-02293-0#ref-CR34 "1001 Genomes Consortium. 1,135 genomes reveal the global pattern of polymorphism in Arabidopsis thaliana. Cell 166, 481–491 (2016)."), and additional samples from eastern Asia[35](https://www.nature.com/articles/s41588-025-02293-0#ref-CR35 "Zou, Y.-P. et al. Adaptation of Arabidopsis thaliana to the Yangtze River basin. Genome Biol. 18, 239 (2017)."), Africa[36](https://www.nature.com/articles/s41588-025-02293-0#ref-CR36 "Durvasula, A. et al. African genomes illuminate the early history and transition to selfing in Arabidopsis thaliana. Proc. Natl Acad. Sci. USA 114, 5213–5218 (2017).") and Madeira[37](https://www.nature.com/articles/s41588-025-02293-0#ref-CR37 "Fulgione, A., Koornneef, M., Roux, F., Hermisson, J. & Hancock, A. M. Madeiran Arabidopsis thaliana reveals ancient long-range colonization and clarifies demography in Eurasia. Mol. Biol. Evol. 35, 564–574 (2017).") (Fig. [1a](https://www.nature.com/articles/s41588-025-02293-0#Fig1)). The genomes were sequenced using PacBio continuous long reads (CLRs) and assembled as described in [Methods](https://www.nature.com/articles/s41588-025-02293-0#Sec13) and Supplementary Note [3](https://www.nature.com/articles/s41588-025-02293-0#MOESM1)—‘The organization of genome variation’).

**Fig. 1: Genome assemblies and size variation across 27 _A. thaliana_ accessions.**

[![figure 1](https://media.springernature.com/full/springer-static/image/art%3A10.1038%2Fs41588-025-02293-0/MediaObjects/41588_2025_2293_Fig1_HTML.png)](https://www.nature.com/articles/s41588-025-02293-0/figures/1)

**a**, Origin of the sequenced accessions with colors indicating ‘Admixture’ group[34](https://www.nature.com/articles/s41588-025-02293-0#ref-CR34 "1001 Genomes Consortium. 1,135 genomes reveal the global pattern of polymorphism in Arabidopsis thaliana. Cell 166, 481–491 (2016)."). The reference accession Col-0 (6909) lacks reliable collection data (but hails from Central Europe based on genotype as well as historical records). Please note that 22005 and 22006 appear as a single point as they are geographically close and belong to the same admixture group. Maps were generated using public domain data from the Natural Earth project via the R package rnaturalearth. **b**, Histogram of genome sizes estimated from _k_\-mers in PCR-free short reads with total assembly sizes superimposed (values to the left of ‘zero’). Most of the variation in genome size can be attributed to unassembled regions (values to the right of ‘zero’). **c**, The amount of centromeric, 5S rDNA and 45S rDNA repeats, estimated from PCR-free short reads with a BLAST-based approach. **d**, Correlation between genome size and each of the three major satellite repeats. Their estimated amounts jointly explain up to 92% (_P_ < 2.2 × 10−16) of total genome size variation (for details, see Supplementary Note [3](https://www.nature.com/articles/s41588-025-02293-0#MOESM1)—‘Estimation of satellite repeats’). The linear regression lines with shaded 95% confidence intervals exclude accession 6981 (Ws-2; indicated with a triangle) because of its very high centromeric repeat content.

Like many plants, _A. thaliana_ has experienced recent episodes of transposable elements (TE) activity, leading to nearly identical sequences inserted across each genome[38](https://www.nature.com/articles/s41588-025-02293-0#ref-CR38 "Quadrana, l. The Arabidopsis thaliana mobilome and its impact at the species level. eLife 5, e15716 (2016)."). These make short-read alignments difficult, but our CLR reads were long enough to bridge such insertions, allowing us to assemble the gene-dense chromosome arms with ease. However, extensive tracts of identical or near-identical tandem repeats, such as centromere satellites and rDNA, consistently break our assemblies (Supplementary Figs. [1](https://www.nature.com/articles/s41588-025-02293-0#MOESM1) and [2](https://www.nature.com/articles/s41588-025-02293-0#MOESM1)). Of note, centromeres can now be assembled using PacBio HiFi reads[16](https://www.nature.com/articles/s41588-025-02293-0#ref-CR16 "Wlodzimierz, P. et al. Cycles of satellite and transposon evolution in Arabidopsis centromeres. Nature 618, 557–565 (2023)."), whereas 45S rDNA clusters remain challenging[39](https://www.nature.com/articles/s41588-025-02293-0#ref-CR39 "Fultz, D., McKinlay, A., Enganti, R. & Pikaard, C. S. Sequence and epigenetic landscapes of active and silent nucleolus organizer regions in Arabidopsis. Sci. Adv. 9, eadj4509 (2023).").

Our assemblies are all ~120 Mb in size, whereas the full genomes are estimated to range from 135 to 155 Mb (Fig. [1b](https://www.nature.com/articles/s41588-025-02293-0#Fig1)), consistent with previous results[40](https://www.nature.com/articles/s41588-025-02293-0#ref-CR40 "Schmuths, H., Meister, A., Horres, R. & Bachmann, K. Genome size variation among accessions of Arabidopsis thaliana. Ann. Bot. 93, 317–321 (2004)."),[41](https://www.nature.com/articles/s41588-025-02293-0#ref-CR41 "Long, Q. et al. Massive genomic variation and strong selection in Arabidopsis thaliana lines from Sweden. Nat. Genet. 45, 884–890 (2013)."). This genome size variation appears to be almost entirely due to variation in centromeric and rDNA repeats (Fig. [1b–d](https://www.nature.com/articles/s41588-025-02293-0#Fig1)), with the importance of 45S rDNA variation having been appreciated before[41](https://www.nature.com/articles/s41588-025-02293-0#ref-CR41 "Long, Q. et al. Massive genomic variation and strong selection in Arabidopsis thaliana lines from Sweden. Nat. Genet. 45, 884–890 (2013)."). While individual TE families can vary greatly in size across accessions (Supplementary Fig. [3](https://www.nature.com/articles/s41588-025-02293-0#MOESM1)), we confirm that the cumulative effect of all TEs on genome size variation appears to be small in _A. thaliana_[41](https://www.nature.com/articles/s41588-025-02293-0#ref-CR41 "Long, Q. et al. Massive genomic variation and strong selection in Arabidopsis thaliana lines from Sweden. Nat. Genet. 45, 884–890 (2013).")—contrary to the major role they have in interspecific variation[42](https://www.nature.com/articles/s41588-025-02293-0#ref-CR42 "Kidwell, M. G. Transposable elements and the evolution of genome size in eukaryotes. Genetica 115, 49–63 (2002)."),[43](https://www.nature.com/articles/s41588-025-02293-0#ref-CR43 "Bista, I. et al. Genomics of cold adaptations in the Antarctic notothenioid fish radiation. Nat. Commun. 14, 3412 (2023).").

### Detecting structural variation

In agreement with others[23](https://www.nature.com/articles/s41588-025-02293-0#ref-CR23 "Lian, Q. et al. A pan-genome of 69 Arabidopsis thaliana accessions reveals a conserved genome structure throughout the global species range. Nat. Genet. 56, 982–991 (2024)."), we find the chromosome arms were not only similar in length across accessions but also largely syntenic (Fig. [2a](https://www.nature.com/articles/s41588-025-02293-0#Fig2)). Thirteen Mb-scale rearrangements were readily apparent in whole-genome alignments (WGAs). These include the previously described 1.2-Mb paracentric inversion associated with a heterochromatic knob on chromosome 4 (refs. [44](https://www.nature.com/articles/s41588-025-02293-0#ref-CR44 "Zapata, L. et al. Chromosome-level assembly of Arabidopsis thaliana Ler reveals the extent of translocation and inversion polymorphisms. Proc. Natl Acad. Sci. USA 113, E4052–60 (2016)."),[45](https://www.nature.com/articles/s41588-025-02293-0#ref-CR45 "Fransz, P. et al. Molecular, genetic and evolutionary analysis of a paracentric inversion in Arabidopsis thaliana. Plant J. 88, 159–178 (2016)."); Extended Data Fig. [1](https://www.nature.com/articles/s41588-025-02293-0#Fig9) and Supplementary Table [2](https://www.nature.com/articles/s41588-025-02293-0#MOESM5)), and a very large reciprocal translocation in accession 22001 from the Yangtze River region (Supplementary Fig. [4](https://www.nature.com/articles/s41588-025-02293-0#MOESM1)). For convenience, we treat this latter rearrangement as if it had not happened in the analysis below, and refer to the modified assembly as 22001m (Supplementary Note [3](https://www.nature.com/articles/s41588-025-02293-0#MOESM1)—‘Reciprocal translocation in 22001’).

**Fig. 2: Distribution of variation on chromosome 1.**

[![figure 2](https://media.springernature.com/full/springer-static/image/art%3A10.1038%2Fs41588-025-02293-0/MediaObjects/41588_2025_2293_Fig2_HTML.png)](https://www.nature.com/articles/s41588-025-02293-0/figures/2)

**a**, WGA illustrates that the genomes are structurally conserved away from centromeric regions. Chromosomes are aligned from both ends to emphasize the contiguity of the arms, with the unassembled centromeric regions indicated in yellow and inversions in pink. Oscillating gray shades highlight homologous regions (the periodicity of the gradients reflects repeated use of the color scheme and has no biological meaning). **b**, The density of pangenome graph bubbles, reflecting higher diversity in pericentromeric regions and at ~20 Mb, where an ancestral centromere was lost through chromosome fusion[41](https://www.nature.com/articles/s41588-025-02293-0#ref-CR41 "Long, Q. et al. Massive genomic variation and strong selection in Arabidopsis thaliana lines from Sweden. Nat. Genet. 45, 884–890 (2013)."). Synteny level refers to the average sharing of links between nodes across the 27 genomes in 300-kb blocks. **c**, Distribution of nucleotide diversity based on SNPs called from a multiple alignment. Blue dots represent values of diversity in 200-kb windows. The red line is a smoothed fit to these points, with the standard error shown. The dark blue area corresponds to the centromeric region, with the lighter blue area highlighting the pericentromeric area and the lightest blue the ancestral lost centromere[41](https://www.nature.com/articles/s41588-025-02293-0#ref-CR41 "Long, Q. et al. Massive genomic variation and strong selection in Arabidopsis thaliana lines from Sweden. Nat. Genet. 45, 884–890 (2013)."). For chromosomes 2–5, see Extended Data Fig. [1](https://www.nature.com/articles/s41588-025-02293-0#Fig9).

Large-scale rearrangements aside, a comprehensive characterization of structural variants (SVs; by which we mean any alteration that causes variation in length, orientation or local context of sequence) remains difficult. The characterization of SVs is a fundamentally different problem from SNP calling. The latter can be viewed as a technical issue—namely, how to distinguish SNPs from sequencing errors—but SV calling remains challenging even with flawless chromosomal sequences. The reason is that the SVs identified between genomes depend on the alignment method and parameters used, and there is no obvious ground truth. Therefore, we pursued two complementary approaches: a new whole-genome multiple-alignment pipeline, Pannagram[46](https://www.nature.com/articles/s41588-025-02293-0#ref-CR46 "Igolkina, A. A., Bezlepsky, A. D. & Nordborg, M. Pannagram: unbiased pangenome alignment and the mobilome calling. Preprint at bioRxiv 
https://doi.org/10.1101/2025.02.07.637071
(2025)."), and the pangenome graph builder (PGGB)[29](https://www.nature.com/articles/s41588-025-02293-0#ref-CR29 "Garrison, E. et al. Building pangenome graphs. Nat. Methods 21, 2008–2012 (2024)."). A discussion and comparison of these methods can be found in Supplementary Note [4](https://www.nature.com/articles/s41588-025-02293-0#MOESM1). We emphasize that the differences between two algorithms designed to perform different tasks should not be interpreted as bias, and that, as noted above, there is no definitive ground truth. However, because Pannagram produces easily interpretable SVs along with convenient pangenome coordinates, and PGGB SVs cover all Pannagram SVs, we based our further SV analyses on the Pannagram data.

### Characterization of SVs

SVs come in many types and sizes, reflecting diverse mutational mechanisms. We will focus on length variants, which are by far the most numerous (for example, we identified fewer than a hundred inversions). We further divide them into bi-allelic presence/absence polymorphisms, consistent with simple insertion/deletion (indel) mutations (sSV), and more complex multi-allelic polymorphisms (cSV). We primarily consider the former, as they are easier to interpret and constitute the majority (over 80% overall), especially in the chromosome arms (Extended Data Fig. [2](https://www.nature.com/articles/s41588-025-02293-0#Fig10)).

We identified 532,178 sSVs, affecting over 37.5 Mb in total—with the length distribution being heavily skewed towards short variants (Fig. [3](https://www.nature.com/articles/s41588-025-02293-0#Fig3)). To gain further insight into the nature of these polymorphisms, we consider sSVs between 15 and 20,000 bp length, because shorter variants are more sensitive to the choice of alignment parameters, and larger ones are too few for statistical treatment. The frequency distribution for the presence allele of sSVs was consistent with sSVs mostly being due to rare insertions or rare deletions. Specifically, long presence alleles tend to be rare, and short ones common, suggesting that sSVs are mainly caused by long insertions and short deletions. Both types are also more likely to occur in intergenic regions than in genic regions, and they are more often observed in introns than in exons, consistent with purifying selection removing many of them (Extended Data Fig. [2](https://www.nature.com/articles/s41588-025-02293-0#Fig10)).

**Fig. 3: The allele frequency distribution of SVs.**

[![figure 3](https://media.springernature.com/full/springer-static/image/art%3A10.1038%2Fs41588-025-02293-0/MediaObjects/41588_2025_2293_Fig3_HTML.png)](https://www.nature.com/articles/s41588-025-02293-0/figures/3)

**a**, The frequency distribution of the presence alleles of all sSVs grouped by variant length (in bp). The height of the gray block (left) is equivalent to the height of the complete panel (right). **b**, The proportion of length classes of sSVs in each frequency bin. Colors correspond to those in **a**.

Of particular note are 108 organellar insertions, almost all of them singletons or doubletons, ranging from a few hundred bp to entire organellar genomes (Supplementary Fig. [7](https://www.nature.com/articles/s41588-025-02293-0#MOESM1)).

### SVs and annotated TEs

Active TEs produce SVs of diverse natures, including both insertions and deletions, and serve as templates for various mutational processes, such as double-stranded break repair[47](https://www.nature.com/articles/s41588-025-02293-0#ref-CR47 "Puchta, H. The repair of double-strand breaks in plants: mechanisms and consequences for genome evolution. J. Exp. Bot. 56, 1–14 (2005)."). We classified the presence alleles of 17,447 sSVs of length ≥100 bp based on their BLAST-identified coverage by ~35,000 annotated TE sequences, spanning ~15% of the _A. thaliana_ reference genome (Fig. [1b](https://www.nature.com/articles/s41588-025-02293-0#Fig1)). In total, over 60% of sSVs showed some overlap with TE annotation, confirming a strong connection between our sSVs and TEs (Fig. [4b](https://www.nature.com/articles/s41588-025-02293-0#Fig4)).

**Fig. 4: The role of TEs in bi-allelic indels.**

[![figure 4](https://media.springernature.com/full/springer-static/image/art%3A10.1038%2Fs41588-025-02293-0/MediaObjects/41588_2025_2293_Fig4_HTML.png)](https://www.nature.com/articles/s41588-025-02293-0/figures/4)

**a**, Categories of overlap between the presence allele of sSVs and annotated TE sequences. **b**, Number of sSVs in each TE-content category described in **a**. Colors correspond to **a**—gray, no TE content. **c**,**d**, Histograms of presence frequency showing annotated TE content as a function of frequency, either raw counts (**c**) or relative to TE-related SVs (**d**). **e**, Distribution of the length of presence alleles in different categories. For an analysis broken down by TE superfamily (Supplementary Fig. [12](https://www.nature.com/articles/s41588-025-02293-0#MOESM1)).

Likely insertions (presence allele in 1–3 accessions) tend to be longer than likely deletions (absence allele in 1–3 accessions). As shown in Fig. [4c,d](https://www.nature.com/articles/s41588-025-02293-0#Fig4), likely insertions also correspond more often to complete TEs, consistent with recent TE activity, whereas likely deletions more often correspond to incomplete TEs, suggesting that they are decaying elements.

As expected, sSVs corresponding to complete TEs are enriched for particular lengths (specifically around 5 kb), reflecting activity of complete TEs (Fig. [4e](https://www.nature.com/articles/s41588-025-02293-0#Fig4)). Similar patterns of enrichment were also found for sSVs in all other categories except for those corresponding to TE fragments. This supports recent reports that active TEs are far from perfectly annotated[48](https://www.nature.com/articles/s41588-025-02293-0#ref-CR48 "Jaegle, B. et al. Extensive sequence duplication in Arabidopsis revealed by pseudo-heterozygosity. Genome Biol. 24, 44 (2023)."),[49](https://www.nature.com/articles/s41588-025-02293-0#ref-CR49 "Borredá, C., Leduque, B., Colot, V. & Quadrana, L. Transposable element products, functions, and regulatory networks in Arabidopsis. Preprint at bioRxiv 
https://doi.org/10.1101/2024.04.02.587720
(2024).").

### The mobile-ome

Mobile elements that have been active in the history of our sample of genomes will have generated segregating insertions and deletions with similar sequences at different locations in the genomes. We can use this property to look directly for mobile elements without relying on TE annotation. We will refer to the set of such elements as the mobile-ome, noting that our usage differs somewhat from that of others[38](https://www.nature.com/articles/s41588-025-02293-0#ref-CR38 "Quadrana, l. The Arabidopsis thaliana mobilome and its impact at the species level. eLife 5, e15716 (2016)."). To identify the mobile-ome, we used Pannagram to cluster all presence alleles from sSVs based on sequence similarity and represented the output as a graph of nestedness, where nodes represent sequences, and connected components are expected to correspond to distinct TE superfamilies or families. We note that several similar approaches have recently been proposed[50](https://www.nature.com/articles/s41588-025-02293-0#ref-CR50 "Sierra, P. & Durbin, R. Identification of transposable element families from pangenome polymorphisms. Mob. DNA 15, 13 (2024)."),[51](https://www.nature.com/articles/s41588-025-02293-0#ref-CR51 "Saidi, S., Blaison, M., del Pilar Rodríguez-Ordóñez, M., Confais, J. & Quesneville, H. panREPET: a reference-free pipeline for detecting shared Transposable Elements from pan-genomes to retrace their dynamics in a species. Preprint at bioRxiv 
https://doi.org/10.1101/2024.06.17.598857
(2025)."),[52](https://www.nature.com/articles/s41588-025-02293-0#ref-CR52 "Groza, C., Chen, X., Wheeler, T. J., Bourque, G. & Goubert, C. A unified framework to analyze transposable element insertion polymorphisms using graph genomes. Nat. Commun. 15, 8915 (2024).").

Almost all sSVs that corresponded to complete TEs are included in the graph, consistent with their being part of the mobile-ome (Fig. [5a](https://www.nature.com/articles/s41588-025-02293-0#Fig5)). Among other TE-related sSVs, approximately 70% are linked to the graph and are thus also related to the mobile-ome, presumably reflecting a mixture of incompletely annotated TE families, complex insertion behaviors and deletions within active TE families.

**Fig. 5: The graph structure of sSVs.**

[![figure 5](https://media.springernature.com/full/springer-static/image/art%3A10.1038%2Fs41588-025-02293-0/MediaObjects/41588_2025_2293_Fig5_HTML.png)](https://www.nature.com/articles/s41588-025-02293-0/figures/5)

**a**, The number of sSVs included (or not) in the graph of nestedness as a function of TE content. **b**, Graph illustrating the nestedness of sSVs, including only presence alleles with nonzero TE content. Each node represents a set of mutually nested sequences, using a similarity threshold of 0.85, with node size reflecting the number of included sequences. Nodes are colored by TE content as shown in **a**. **c**, Same graph as in **b**, but colored by TE superfamilies, as shown in the center on top. Note that the algorithm used no prior knowledge of TE superfamilies. A large, dominant component connecting all TE superfamilies is also seen in a graph built using the entire _A. thaliana_ TE annotation, suggesting that our sSVs and the reference annotation have comparable properties (Extended Data Fig. [4](https://www.nature.com/articles/s41588-025-02293-0#Fig12)). **d**, A graph of nestedness for sSVs without TE content, colored by open reading frame content based on protein BLAST, as shown on the right.

To understand the relationship between annotated TEs, we filtered out sequences without TE content and merged sequences with high similarity into larger nodes. The resulting subgraph consists of one dominant component along with numerous smaller ones (Fig. [5b](https://www.nature.com/articles/s41588-025-02293-0#Fig5)). As expected, there are multiple large nodes corresponding to complete TEs, but we also see large nodes corresponding to sequences ostensibly containing complete TEs or TE fragments, demonstrating that many of these sequences are in fact part of the mobile-ome (Extended Data Fig. [3](https://www.nature.com/articles/s41588-025-02293-0#Fig11)). Coloring the nodes by TE superfamily reveals that, while the smaller components mostly can be attributed to single TE families, the dominant component contains members of all known TE superfamilies (Fig. [5c](https://www.nature.com/articles/s41588-025-02293-0#Fig5)). Possible reasons include TEs inserting into existing TEs and closely related sequences being mis-annotated as belonging to different superfamilies (for example, Supplementary Fig. [13](https://www.nature.com/articles/s41588-025-02293-0#MOESM1)). Further evidence for the incompleteness of the TE annotation comes from small graph components that contain large nodes of longer elements that have only partial TE content (Supplementary Figs. [14](https://www.nature.com/articles/s41588-025-02293-0#MOESM1) and [15](https://www.nature.com/articles/s41588-025-02293-0#MOESM1)).

In the set of sSVs without TE content, the majority (74%) are unique and hence not connected in the graph. Among the remaining 26%, we observed 238 connected components with ≥3 nodes, similar in structure to those corresponding to single TE families, and thus presumably corresponding to previously unannotated TEs (Fig. [5d](https://www.nature.com/articles/s41588-025-02293-0#Fig5)). Of these, 97 are obviously TE-like, encoding TE proteins from _A. thaliana_ or other species. A few of them show evidence of horizontal gene transfer, as they exhibit greater protein similarity to species outside a panel of five Brassicaceae species (for example, Supplementary Fig. [16](https://www.nature.com/articles/s41588-025-02293-0#MOESM1)). However, we also found putative new mobile element families that lack clear protein-coding (PC) potential. They form relatively large components in the graph (Fig. [5d](https://www.nature.com/articles/s41588-025-02293-0#Fig5), purple islands), indicating that they are not rare. They are not low complexity, and some are exclusive to _A. thaliana_ (see Supplementary Fig. [17](https://www.nature.com/articles/s41588-025-02293-0#MOESM1) for an example).

Annotated TEs in _A. thaliana_ are generally epigenetically silenced. However, most studies have relied on a single reference genome, making it difficult to distinguish active from inactive TEs. Our mobile-ome data identifies segregating insertions corresponding to recently active TE families, and we can also consider the age of insertions, which should be proportional to their population frequency.

We investigated silencing in sSVs by remapping the existing methylation data[53](https://www.nature.com/articles/s41588-025-02293-0#ref-CR53 "Kawakatsu, T. et al. Epigenomic diversity in a global collection of Arabidopsis thaliana accessions. Cell 166, 492–505 (2016).") to our genome assemblies ([Methods](https://www.nature.com/articles/s41588-025-02293-0#Sec13)), and the results supported our conclusions above (Supplementary Fig. [18](https://www.nature.com/articles/s41588-025-02293-0#MOESM1)). sSVs corresponding to TEs or TE fragments are generally highly methylated, while other categories are more variable, consistent with a subset of these sSVs corresponding to highly methylated un- or mis-annotated TEs. For sSVs corresponding to complete TEs, methylation increases with frequency, indicating that older insertions are more highly methylated. Across all categories, sSVs that are part of the graph of nestedness are highly methylated, consistent with silencing targeting the mobile-ome.

Expression patterns from existing RNA-seq data[54](https://www.nature.com/articles/s41588-025-02293-0#ref-CR54 "Kornienko, A. E., Nizhynska, V., Molla Morales, A., Pisupati, R. & Nordborg, M. Population-level annotation of lncRNAs in Arabidopsis reveals extensive expression variation associated with transposable element-like silencing. Plant Cell 36, 85–111 (2023).") agree with the methylation data: sequences in sSVs corresponding to complete TEs are barely expressed (except in pollen, where some TE expression is known to occur[55](https://www.nature.com/articles/s41588-025-02293-0#ref-CR55 "Pachamuthu, K. & Borges, F. Epigenetic control of transposons during plant reproduction: from meiosis to hybrid seeds. Curr. Opin. Plant Biol. 75, 102419 (2023).")), while the behavior of sequences in other sSVs is more variable (Supplementary Fig. [19](https://www.nature.com/articles/s41588-025-02293-0#MOESM1)).

### The gene-ome

To investigate the variation in the portion of the genome containing PC genes—the ‘gene-ome’—with minimal reference bias, we annotated each genome independently using sequence-based gene modeling and RNA-seq data from four tissues[54](https://www.nature.com/articles/s41588-025-02293-0#ref-CR54 "Kornienko, A. E., Nizhynska, V., Molla Morales, A., Pisupati, R. & Nordborg, M. Population-level annotation of lncRNAs in Arabidopsis reveals extensive expression variation associated with transposable element-like silencing. Plant Cell 36, 85–111 (2023).") ([Methods](https://www.nature.com/articles/s41588-025-02293-0#Sec13)). After including 1,789 TAIR10 genes that were not re-identified in our study and filtering out low-confidence genes ([Methods](https://www.nature.com/articles/s41588-025-02293-0#Sec13); Supplementary Note [6](https://www.nature.com/articles/s41588-025-02293-0#MOESM1)—‘Details about reconciling annotations and gene filtering’), the final annotation contained 34,153 genes, with 28,138 classified as bona fide PC and 5,674 as TE (Fig. [6a](https://www.nature.com/articles/s41588-025-02293-0#Fig6) and Supplementary Note [6](https://www.nature.com/articles/s41588-025-02293-0#MOESM1)—‘Genes and TEs’). Of these, 2,661 PC and 565 TE genes were not previously annotated (for a detailed analysis of new genes, see Supplementary Note [6](https://www.nature.com/articles/s41588-025-02293-0#MOESM1)—‘New genes’).

**Fig. 6: Analysis of the gene-ome.**

[![figure 6](https://media.springernature.com/full/springer-static/image/art%3A10.1038%2Fs41588-025-02293-0/MediaObjects/41588_2025_2293_Fig6_HTML.png)](https://www.nature.com/articles/s41588-025-02293-0/figures/6)

**a**, The 34,153 annotated genes categorized based on whether they correspond to the TAIR10 annotation and whether they are TEs or PC (based on sequence similarity and TE-like protein domains; Extended Data Fig. [5a](https://www.nature.com/articles/s41588-025-02293-0#Fig13)). **b**, Genes categorized based on locus presence frequency across the 27 genomes. For TE presence frequency distribution and a comparison with published results[23](https://www.nature.com/articles/s41588-025-02293-0#ref-CR23 "Lian, Q. et al. A pan-genome of 69 Arabidopsis thaliana accessions reveals a conserved genome structure throughout the global species range. Nat. Genet. 56, 982–991 (2024)."), please see Extended Data Fig. [5b](https://www.nature.com/articles/s41588-025-02293-0#Fig13),[c](https://www.nature.com/articles/s41588-025-02293-0#Fig13). **c**, Synteny comparison with _A. lyrata_. For TEs, see Extended Data Fig. [5d](https://www.nature.com/articles/s41588-025-02293-0#Fig13). **d**, Ancestral status of genes of TAIR10 and newly annotated genes (‘position + sequence’ means that both gene sequence and syntenic position are conserved). **e**, Ancestral status of genes by presence frequency. **f**, Distribution of genes and TEs along chromosome 5, grouped by frequency (top) and ancestral status (bottom). For all chromosomes, see Extended Data Fig. [5h](https://www.nature.com/articles/s41588-025-02293-0#Fig13),[i](https://www.nature.com/articles/s41588-025-02293-0#Fig13). **g**, Functional domains of annotated genes, based on comparisons with UniProtKB. **h**, Functional domains of PC genes grouped by ancestral status. In **g** and **h**, genes not matching a functional category have been excluded; for plots including these and breakdowns by presence frequency, see Extended Data Fig. [6e–g](https://www.nature.com/articles/s41588-025-02293-0#Fig14). **i**,**j**, Expression (in 9-leaf rosettes) and H3K9me2/H3K27me3 levels (in mature leaves) by gene frequency (**i**) and ancestral status (**j**). Data shown[54](https://www.nature.com/articles/s41588-025-02293-0#ref-CR54 "Kornienko, A. E., Nizhynska, V., Molla Morales, A., Pisupati, R. & Nordborg, M. Population-level annotation of lncRNAs in Arabidopsis reveals extensive expression variation associated with transposable element-like silencing. Plant Cell 36, 85–111 (2023).") are for accession 6024; for other accessions, as well as DNA methylation and 24-nt sRNA coverage, see Extended Data Fig. [6](https://www.nature.com/articles/s41588-025-02293-0#Fig14). Box plots show the median (center line), the 25th and 75th percentiles (box bounds) and the smallest and largest values within 1.5× the interquartile range (whiskers); outliers beyond this range are not plotted. Expression and H3K9me2/H3K27me3 were compared between frequency/ancestry gene categories using a two-sided Wilcoxon rank-sum test. The number of genes in each category is shown above the top box plot. No multiple-comparison corrections were performed.

Focusing on gene-locus presence–absence variation, we found that 13% of genes were segregating in the population of 27 accessions (Fig. [6b](https://www.nature.com/articles/s41588-025-02293-0#Fig6)). This variation could reflect deletions of ancestral genes or insertions of new genes specific to _A. thaliana_. To resolve this, we used _Arabidopsis lyrata_ as an outgroup (Fig. [6c](https://www.nature.com/articles/s41588-025-02293-0#Fig6)). This analysis revealed a striking difference between TAIR10 genes and previously unannotated genes: while the former are generally ancestral, the latter are not (Fig. [6d](https://www.nature.com/articles/s41588-025-02293-0#Fig6)). There was also a clear difference between segregating and fixed genes: as expected, most of the latter are ancestral, but the vast majority of the segregating genes are not (Fig. [6e](https://www.nature.com/articles/s41588-025-02293-0#Fig6)). Thus, although we may have underestimated the fraction of ancestral genes by relying on the _A. lyrata_ annotation, our results suggest that segregating ancestral deletions are rare.

Segregating genes are more common near centromeres, while fixed genes are more common in the arms (Fig. [6f](https://www.nature.com/articles/s41588-025-02293-0#Fig6); _χ_2 test, _P_ < 0.0005 across chromosomes). Syntenic ancestral genes are also enriched in the arms, while other categories are evenly distributed across the genome. As expected, high-frequency TE insertions are more common near centromeres, consistent with stronger purifying selection in the arms[38](https://www.nature.com/articles/s41588-025-02293-0#ref-CR38 "Quadrana, l. The Arabidopsis thaliana mobilome and its impact at the species level. eLife 5, e15716 (2016).").

New PC genes were enriched in defense and zinc-finger genes, while TAIR10 genes were enriched in housekeeping functions such as transcriptional regulation and membrane proteins (Fig. [6g](https://www.nature.com/articles/s41588-025-02293-0#Fig6); for details of functional annotation, see Supplementary Note [6](https://www.nature.com/articles/s41588-025-02293-0#MOESM1)—‘Genes and TEs’). A similar difference was found between ancestral and nonancestral genes (Fig. [6h](https://www.nature.com/articles/s41588-025-02293-0#Fig6)), as well as between fixed and segregating genes (Extended Data Fig. [5e](https://www.nature.com/articles/s41588-025-02293-0#Fig13),[f](https://www.nature.com/articles/s41588-025-02293-0#Fig13)). New TE genes were strikingly more enriched for TE-function proteins than already annotated TEs (Fig. [6g](https://www.nature.com/articles/s41588-025-02293-0#Fig6)), suggesting that the former are more likely to be active TEs—as expected given that they are actually segregating.

Finally, fixed genes are far more highly expressed than segregating genes (Fig. [6i](https://www.nature.com/articles/s41588-025-02293-0#Fig6)). Indeed, genes absent in only one or two accessions tend to be almost silent in the remaining accessions (Extended Data Fig. [6](https://www.nature.com/articles/s41588-025-02293-0#Fig14)). Epigenetic silencing behaves similarly, with both gene-like Polycomb silencing (H3K27me3) and TE-like silencing (H3K9me2 and DNA methylation) being substantially higher for segregating genes (Fig. [6i](https://www.nature.com/articles/s41588-025-02293-0#Fig6)). Likewise, nonancestral genes have reduced expression and increased silencing compared to ancestral genes (Fig. [6j](https://www.nature.com/articles/s41588-025-02293-0#Fig6) and Extended Data Fig. [6](https://www.nature.com/articles/s41588-025-02293-0#Fig14)).

### The pangenome

The term ‘pangenome’ is currently applied with a variety of meanings, from the original use in prokaryotes to describe the observation that genomes from different strains of the same species vary enormously in gene content[56](https://www.nature.com/articles/s41588-025-02293-0#ref-CR56 "Tettelin, H. et al. Genome analysis of multiple pathogenic isolates of Streptococcus agalactiae: implications for the microbial ‘pan-genome’. Proc. Natl Acad. Sci. USA 102, 13950–13955 (2005)."), to the human genetics ambition of representing all polymorphism in a single ‘pangenome graph’[15](https://www.nature.com/articles/s41588-025-02293-0#ref-CR15 "Liao, W.-W. et al. A draft human pangenome reference. Nature 617, 312–324 (2023)."),[28](https://www.nature.com/articles/s41588-025-02293-0#ref-CR28 "Eizenga, J. M. et al. Pangenome graphs. Annu. Rev. Genomics Hum. Genet. 21, 139–162 (2020)."). We will discuss the utility of these concepts further below—here we simply consider how the known pangenome grows with sample size and why.

All components of variation considered in this paper grow with sample size, but at different rates: the mobile-ome grows faster than the full genome and the gene-ome more slowly, consistent with the latter being under stronger purifying selection (Fig. [7a](https://www.nature.com/articles/s41588-025-02293-0#Fig7)). All components increase faster than the logarithmic growth expected under neutrality in a constant population and more slowly than the linear growth expected in an exponentially growing population[57](https://www.nature.com/articles/s41588-025-02293-0#ref-CR57 "Balding, D., Moltke, I. & Marioni, J. (eds.) Handbook of Statistical Genomics, Vol. 1, 145–175 (Wiley, 2019).").

**Fig. 7: The growth of the pangenome.**

[![figure 7](https://media.springernature.com/full/springer-static/image/art%3A10.1038%2Fs41588-025-02293-0/MediaObjects/41588_2025_2293_Fig7_HTML.png)](https://www.nature.com/articles/s41588-025-02293-0/figures/7)

**a**, The dependence on sample size for the union (‘pan’) and intersection (‘core’) sequence length, separately for the full genome, the mobile-ome and the gene-ome (for saturation by sSV length and normalized views, see Extended Data Fig. [7](https://www.nature.com/articles/s41588-025-02293-0#Fig15)). **b**, Pangenome versus reference genome coordinates. The pericentromeric region (light blue) shows a higher ‘dilution’ of the spatial coordinates due to the increased number of SVs in this region, but please note that the slope is never 1, reflecting their ubiquity. The centromeric region is dark blue (for other chromosomes, see Extended Data Fig. [7](https://www.nature.com/articles/s41588-025-02293-0#Fig15)). **c**, The contribution of sSVs of different lengths to differences between pairs of genomes. Numbers are counts of sSVs. Shorter sSVs are more numerous, but longer and rarer sSVs contribute more to total length variation.

The growth of the pangenome is reflected in the coordinate system and is not uniform along each chromosome because most of the variation is found in centromeric regions (Fig. [7b](https://www.nature.com/articles/s41588-025-02293-0#Fig7)). Already with 27 accessions, the pangenome chromosomes are 63–76% longer than the TAIR10 chromosomes.

### Missing polymorphism

As part of the 1001 Genomes Project, we previously ‘resequenced’ 1,135 accessions using short reads[34](https://www.nature.com/articles/s41588-025-02293-0#ref-CR34 "1001 Genomes Consortium. 1,135 genomes reveal the global pattern of polymorphism in Arabidopsis thaliana. Cell 166, 481–491 (2016)."). We were well aware that the data were both incomplete and error-prone: we only called SNPs and short SVs, and only an average of 84% of the reference genome was covered by short reads from any particular accession.

With our whole-genome polymorphism data, we are now in a position to assess how much variation was previously missed. In the 1001 Genomes data, a pair of accessions differed, on average, at ~440,000 SNPs. In our Pannagram alignment, the corresponding number ranges from 600,000 to 800,000 SNPs, depending on how SNPs are defined ([Methods](https://www.nature.com/articles/s41588-025-02293-0#Sec13)). In other words, we previously missed 25–45% of the SNP variation. In addition, WGAs of two genomes reveal, on average, ~190,000 SVs (of length <10 kb) covering a total of over ~12.5 Mb of sequence—approximately 10% of each assembled genome (Fig. [7c](https://www.nature.com/articles/s41588-025-02293-0#Fig7)).

We investigated the causes of the missing SNPs by calling SNPs for our 27 genomes using the PCR-free, high-coverage short reads that were generated for this study and comparing the results to those from pairwise WGA of complete assemblies (Fig. [8a](https://www.nature.com/articles/s41588-025-02293-0#Fig8)). The main reason for missing SNPs from short reads comes from not making calls in regions that are not reliably covered by reads due to mapping problems. The extent of such regions depends on the mapping parameters used; however, less conservative read mapping will generally come at the cost of higher error rates. In our test SNP-calling with PCR-free data, we were able to reduce the fraction of missing SNPs to below 20%, but our false discovery rate (FDR) was then close to 7%. Consistent with a trade-off between conservative and aggressive read mapping, bona fide SNP-calling errors, be they false positives or false negatives, were overwhelmingly due to read mismapping. Rampant pseudoheterozygosity caused by segregating duplications that are absent from the reference genome is particularly worrisome[48](https://www.nature.com/articles/s41588-025-02293-0#ref-CR48 "Jaegle, B. et al. Extensive sequence duplication in Arabidopsis revealed by pseudo-heterozygosity. Genome Biol. 24, 44 (2023).") (pseudoheterozygosity is easy to distinguish from residual heterozygosity in inbred lines; only one of our accessions had very limited amounts of the latter). Differences in local sequence alignment between algorithms also contributed to discrepancies, whereas traditional base-calling errors had an insignificant role (Supplementary Fig. [27](https://www.nature.com/articles/s41588-025-02293-0#MOESM1)).

**Fig. 8: Read mapping and reference bias.**

[![figure 8](https://media.springernature.com/full/springer-static/image/art%3A10.1038%2Fs41588-025-02293-0/MediaObjects/41588_2025_2293_Fig8_HTML.png)](https://www.nature.com/articles/s41588-025-02293-0/figures/8)

**a**, To investigate SNP-calling errors, SNPs were identified from pairwise WGA as well as by designating one genome as a reference and calling SNPs using short reads from the other (next generation sequencing (NGS); see Supplementary Note [7](https://www.nature.com/articles/s41588-025-02293-0#MOESM1) for details). Numbers are averages across all accession pairs (±s.d.). From the point of view of WGA, each site can either be aligned or not. Conversely, from the point of view of NGS, each site in the reference genome can be covered by sample reads or not. Arrows pointing right refer to WGA SNPs, which we assume to be correct; arrows pointing left refer to NGS SNPs. WGA SNPs are TPs if also called by NGS, FNs if missed by NGS and uncalled if in regions not covered by NGS reads. Conversely, NGS SNPs are TPs if also found in the WGA and FPs if not. FPs come in two flavors: those that correspond to bona fide non-SNPs in the WGA and those that correspond to regions that were not aligned. Heterozygous calls in completely inbred lines are obviously FPs and are treated separately. **b**, SNP-calling error rates depend on the relationship between the reference and the sampled genome. Each line is the regression of SNP-calling errors for a different choice of reference genome (identified by color). FNR, false negative rate. **c**, Correlation between expression- and methylation-level estimates derived from mapping reads to the TAIR10 genome and the genome of the sampled individual. Sample sizes for each data type also apply to **d** and **e**. **d**, Percentage of genes for which expression or methylation levels differ by more than 30% or 50%, respectively, when mapping reads to the TAIR10 reference rather than their ‘own’ genome. **e**, Enrichment of copy-number variable genes among those with discordant expression- or methylation-level estimates. Box plots show the median plus the 25th and 75th percentiles, with whiskers covering the smallest and largest values within 1.5× the interquartile range. The percentage of copy-number variable (CNV) genes was compared between wrongly and correctly estimated genes across available samples using a two-sided Wilcoxon test. TPs, true positives; FPs, false positives; FNs, false negatives.

### Reference bias

Mapping short reads to a reference genome can cause reference bias; that is, the results will depend on which genome is used as a reference. Starting with SNP calling, we found that all SNP error rates depend both on the reference genome and on the relatedness between the reference and the sampled genome, often in unpredictable ways (Fig. [8b](https://www.nature.com/articles/s41588-025-02293-0#Fig8)). Because many population genetic analyses rely on SNPs to estimate the relatedness between samples, this is troubling, and the consequences of nonrandomly varying levels of bias in samples for downstream analyses such as genome-wide association study or demographic inference merit further investigation.

Reference bias may also affect analysis using standard omics techniques that quantify molecular phenotypes by mapping short reads to a reference genome. We investigated this problem for transcriptome and methylome profiling by comparing the results of mapping RNA-seq and bisulfite sequencing (BS-seq) reads to the TAIR10 reference as well as to the genome of the accession being studied. Expression estimates between the two approaches were strongly correlated on average (Fig. [8c](https://www.nature.com/articles/s41588-025-02293-0#Fig8)), but a subset of genes diverged markedly (Fig. [8d](https://www.nature.com/articles/s41588-025-02293-0#Fig8)). These were strongly enriched for copy-number variable genes (Fig. [8e](https://www.nature.com/articles/s41588-025-02293-0#Fig8)). Methylome profiling was even more sensitive to the choice of genome for mapping—not surprisingly given that methylation in _A. thaliana_ predominantly targets highly variable TEs[48](https://www.nature.com/articles/s41588-025-02293-0#ref-CR48 "Jaegle, B. et al. Extensive sequence duplication in Arabidopsis revealed by pseudo-heterozygosity. Genome Biol. 24, 44 (2023)."). A scan for differentially methylated regions in 100-bp windows across the genome revealed that profiling methylation by mapping reads to the TAIR10 reference rather than to each sample’s own genome produced a large number of spurious differentially methylated regions (Supplementary Fig. [32](https://www.nature.com/articles/s41588-025-02293-0#MOESM1)). How serious this problem is will depend on the application, but it seems clear that it must be considered.

Discussion
----------

Over the last several years, population samples of more-or-less complete eukaryotic genomes have been appearing at an increasing rate, and there has been much excitement over the (variously defined) ‘pangenome’, especially in plants[58](https://www.nature.com/articles/s41588-025-02293-0#ref-CR58 "Schreiber, M., Jayakodi, M., Stein, N. & Mascher, M. Plant pangenomes for crop improvement, biodiversity and evolution. Nat. Rev. Genet. 25, 563–577 (2024)."). At the same time, it has become abundantly clear that a principled characterization of all the differences between individual genomes is very difficult. The problem is not a technical one, because even with perfect chromosomal sequences, we have to decide how to align them and how to interpret the differences. For complex structural variation, especially in highly diverged regions[59](https://www.nature.com/articles/s41588-025-02293-0#ref-CR59 "Cork, J. M. & Purugganan, M. D. High-diversity genes in the Arabidopsis genome. Genetics 170, 1897–1911 (2005)."), this is not trivial, and there is no obvious ‘gold standard’ by which to evaluate algorithms. Furthermore, the ultimate reason for comparing genomes matters. If we are interested in using the pattern of polymorphism to answer questions about evolutionary history and mutational mechanisms, we must employ models that reflect actual historical events. In contrast, if the goal is simply to develop easily usable genetic markers, it may be irrelevant whether there is any correspondence between designated variants and the molecular processes that generated them.

With these caveats in mind, we tried two different approaches: Pannagram[46](https://www.nature.com/articles/s41588-025-02293-0#ref-CR46 "Igolkina, A. A., Bezlepsky, A. D. & Nordborg, M. Pannagram: unbiased pangenome alignment and the mobilome calling. Preprint at bioRxiv 
https://doi.org/10.1101/2025.02.07.637071
(2025)."), a whole-genome multiple-alignment pipeline, and PGGB[15](https://www.nature.com/articles/s41588-025-02293-0#ref-CR15 "Liao, W.-W. et al. A draft human pangenome reference. Nature 617, 312–324 (2023)."),[29](https://www.nature.com/articles/s41588-025-02293-0#ref-CR29 "Garrison, E. et al. Building pangenome graphs. Nat. Methods 21, 2008–2012 (2024)."), a tool primarily developed for human genomes. This is relevant because _A. thaliana_ genomes have higher levels of polymorphism, stronger population structure and many recently active TEs—all of which complicate graph building and interpretation. For these reasons, as well as general convenience, we based most of our analysis on the Pannagram output.

It has long been clear that SVs contribute substantially to polymorphism[60](https://www.nature.com/articles/s41588-025-02293-0#ref-CR60 "Morgante, M. et al. Gene duplication and exon shuffling by helitron-like transposons generate intraspecies diversity in maize. Nat. Genet. 37, 997–1002 (2005)."),[61](https://www.nature.com/articles/s41588-025-02293-0#ref-CR61 "Marques-Bonet, T., Ryder, O. A. & Eichler, E. E. Sequencing primate genomes: what have we learned? Annu. Rev. Genomics Hum. Genet. 10, 355–386 (2009)."). In addition to massive variation in tandem repeat regions (Fig. [1](https://www.nature.com/articles/s41588-025-02293-0#Fig1)), the readily alignable chromosome arms (Fig. [2](https://www.nature.com/articles/s41588-025-02293-0#Fig2)) are highly polymorphic, with two accessions differing at ~191,000 SVs covering ~12.5 Mb on average. Although we also uncover massive amounts of new SNP variation, this still means that at least an order of magnitude more nucleotide sites are affected by SVs than by SNPs. The allele frequency distribution of SVs suggests purifying selection, as well as a mutational process involving the insertion of longer segments coupled with the deletion of shorter segments. This is consistent with TE activity, and the overwhelming majority of presence–absence variants longer than 100 bp involve annotated TE sequences. As expected in an organism with active TEs[38](https://www.nature.com/articles/s41588-025-02293-0#ref-CR38 "Quadrana, l. The Arabidopsis thaliana mobilome and its impact at the species level. eLife 5, e15716 (2016)."),[62](https://www.nature.com/articles/s41588-025-02293-0#ref-CR62 "Stuart, T. et al. Population scale mapping of transposable element diversity reveals links to gene regulation and epigenomic variation. eLife 5, e20777 (2016)."), we found thousands of examples of what appear to be recent insertions of presumably complete TEs. Many of these correspond perfectly to annotated TEs, but many do not, demonstrating that our understanding of the mobile-ome remains highly incomplete[49](https://www.nature.com/articles/s41588-025-02293-0#ref-CR49 "Borredá, C., Leduque, B., Colot, V. & Quadrana, L. Transposable element products, functions, and regulatory networks in Arabidopsis. Preprint at bioRxiv 
https://doi.org/10.1101/2024.04.02.587720
(2024).").

Turning to the gene-ome, we note that the term ‘pangenome’ was originally invented to describe the rather fluid genomes of prokaryotes[56](https://www.nature.com/articles/s41588-025-02293-0#ref-CR56 "Tettelin, H. et al. Genome analysis of multiple pathogenic isolates of Streptococcus agalactiae: implications for the microbial ‘pan-genome’. Proc. Natl Acad. Sci. USA 102, 13950–13955 (2005)."),[63](https://www.nature.com/articles/s41588-025-02293-0#ref-CR63 "McInerney, J. O., McNally, A. & O’Connell, M. J. Why prokaryotes have pangenomes. Nat. Microbiol. 2, 17040 (2017)."). The overall picture in _A. thaliana_ is clearly very different: the gene-ome is highly conserved, with 87% of genes detected in all 27 genomes, and the number of segregating genes growing considerably more slowly with sample size than other types of variation (Fig. [7](https://www.nature.com/articles/s41588-025-02293-0#Fig7)). We distinguish between two types of segregating genes: a minority with homologs in the closely related _A. lyrata_ and a majority without (Fig. [6](https://www.nature.com/articles/s41588-025-02293-0#Fig6)). The former, which correspond either to gene duplications or segregating deletions of ancestral genes, tend to be expressed at substantially higher levels than the latter, which often were characterized by TE-like epigenetic silencing.

Finally, we demonstrate that algorithms for SNP calling, transcriptome profiling and methylation profiling that rely on mapping short-read data to a reference genome can be highly biased—a problem that is likely to be worse in organisms with larger and more polymorphic genomes than _A. thaliana_. Additionally, outcrossing makes problems such as pseudoheterozygosity due to cryptic duplications far more difficult to detect[48](https://www.nature.com/articles/s41588-025-02293-0#ref-CR48 "Jaegle, B. et al. Extensive sequence duplication in Arabidopsis revealed by pseudo-heterozygosity. Genome Biol. 24, 44 (2023)."),[64](https://www.nature.com/articles/s41588-025-02293-0#ref-CR64 "Ranade, K. et al. High-throughput genotyping with single nucleotide polymorphisms. Genome Res. 11, 1262–1268 (2001)."). While it is still impractical to completely abandon the use of SNP calling based on short reads in favor of whole-genome polymorphism data, we note that a recent study that adopted this approach to estimate demographic parameters in _A. thaliana_ reported that parameter estimates changed by two orders of magnitude[65](https://www.nature.com/articles/s41588-025-02293-0#ref-CR65 "Osmond, M. M. & Coop, G. Estimating dispersal rates and locating genetic ancestors with genome-wide genealogies. eLife 13, e72177 (2024)."). Using at least a sample of diverse, high-quality genomes for read mapping should greatly help quantify the biases.

In conclusion, we recall the prediction made in ref. [66](https://www.nature.com/articles/s41588-025-02293-0#ref-CR66 "Chakravarti, A. Population genetics—making sense out of sequence. Nat. Genet. 21, 56–60 (1999).") at the dawn of the SNP era that models would be needed to ‘make sense out of sequence’—and that this would lead to ‘a rejuvenation of population genetics’. The advent of unbiased whole-genome polymorphism data will have a similar effect. Most obviously, our understanding of TE dynamics will be revolutionized by our ability to see segregating TE insertions, reflecting recent activity. While interspecific genome comparisons can reveal that bursts of activity have occurred, they lack the resolution to understand their dynamics and cannot readily distinguish active TEs from the accumulated layers of dead and decaying TE sequences that litter most genomes.

More subtly, to make sense of complex polymorphisms, we need to understand the history of mutations that gave rise to them. The problem is analogous to phylogenetic analysis, where the estimated relationship between species is used to deduce the history of complex traits—what evolved first and what evolved multiple times? In the present context, we need to estimate local coalescent trees (the so-called Ancestral Recombination Graph[67](https://www.nature.com/articles/s41588-025-02293-0#ref-CR67 "Lewanski, A. L., Grundler, M. C. & Bradburd, G. S. The era of the ARG: an introduction to ancestral recombination graphs and their significance in empirical evolutionary genomics. PLoS Genet. 20, e1011110 (2024)."),[68](https://www.nature.com/articles/s41588-025-02293-0#ref-CR68 "Nielsen, R., Vaughn, A. H. & Deng, Y. Inference and applications of ancestral recombination graphs. Nat. Rev. Genet. 26, 47–58 (2024).")) and use them to infer the sequence of mutational and recombination events that gave rise to the sampled sequences. At the same time, this analysis must be informed by a better understanding of the molecular mechanisms that cause structural variation. Although a considerable literature on phylogeny-guided statistical alignment exists[69](https://www.nature.com/articles/s41588-025-02293-0#ref-CR69 "Novák, A., Miklós, I., Lyngsø, R. & Hein, J. StatAlign: an extendable software package for joint Bayesian estimation of alignments and evolutionary trees. Bioinformatics 24, 2403–2404 (2008)."),[70](https://www.nature.com/articles/s41588-025-02293-0#ref-CR70 "Chatzou, M. et al. Multiple sequence alignment modeling: methods and applications. Brief. Bioinform. 17, 1009–1023 (2016)."),[71](https://www.nature.com/articles/s41588-025-02293-0#ref-CR71 "Katoh, K. (ed.) in Multiple Sequence Alignment: Methods and Protocols 17–37 (Springer, 2021)."),[72](https://www.nature.com/articles/s41588-025-02293-0#ref-CR72 "Redelings, B. D. BAli-Phy version 3: model-based co-estimation of alignment and phylogeny. Bioinformatics 37, 3032–3034 (2021)."),[73](https://www.nature.com/articles/s41588-025-02293-0#ref-CR73 "Kille, B., Balaji, A., Sedlazeck, F. J., Nute, M. & Treangen, T. J. Multiple genome alignment in the telomere-to-telomere assembly era. Genome Biol. 23, 182 (2022)."), methods for doing this on a whole-genome scale, using an appropriate population genetic framework[57](https://www.nature.com/articles/s41588-025-02293-0#ref-CR57 "Balding, D., Moltke, I. & Marioni, J. (eds.) Handbook of Statistical Genomics, Vol. 1, 145–175 (Wiley, 2019).") and incorporating knowledge about molecular mechanisms, are missing.

In this context, it is important to remember that alignment-based methods developed for humans often do not work well in other species for a variety of reasons, including much higher levels of polymorphism and TE activity. _A. thaliana_ genomes are not unusual in these respects. In species like maize, where intergenic space is essentially unalignable even between relatively closely related agricultural varieties[60](https://www.nature.com/articles/s41588-025-02293-0#ref-CR60 "Morgante, M. et al. Gene duplication and exon shuffling by helitron-like transposons generate intraspecies diversity in maize. Nat. Genet. 37, 997–1002 (2005)."), the idea of representing a whole-genome multiple alignment as a graph that captures all variation may be neither practicable nor useful[74](https://www.nature.com/articles/s41588-025-02293-0#ref-CR74 "Song, B., Buckler, E. S. & Stitzer, M. C. New whole-genome alignment tools are needed for tapping into plant diversity. Trends Plant. Sci. 29, 355–369 (2023).").

Methods
-------

### DNA extraction and sequencing

For long-read sequencing, we began with 3-week-old plants grown in soil that had been transferred to darkness for 24–48 h before harvesting to reduce the starch content. A total of 20–30 g of flash-frozen rosette tissue, pooled from individuals, was ground in liquid nitrogen with a pestle and mortar. Nuclei were isolated as described for accession Ey15-2 (ref. [75](https://www.nature.com/articles/s41588-025-02293-0#ref-CR75 "Rabanal, F. A. et al. Pushing the limits of HiFi assemblies reveals centromere diversity between two Arabidopsis thaliana genomes. Nucleic Acids Res. 50, 12309–12327 (2022).")), and high-molecular-weight (HMW) DNA purified with Genomic-tips 100G (Qiagen, 10243) following the manufacturer’s instructions. Ten micrograms of HMW DNA were sheared with either Megaruptor 3 (Diagenode, B06010003) or a FINE-JECT 26G× 1″ needle (0.45 × 25 mm; 14-13651) to ca. 75 kb, and used as input for long-read library preparation with the SMRTbell Express Template Preparation Kit 2.0 (Pacific Biosciences, 101-693-800). These libraries were size-selected with the BluePippin system (Sage Science) with a 30 kb cutoff in a 0.75% DF Marker U1 high-pass 30–40 kb vs3 gel cassette (Biozym, BLF7510). Libraries for accessions 9981 (Angit-1; CS76366) and 10002 (TueWal-2; CS76405) were sequenced on a Sequel II system (Pacific Biosciences), and the others on a Sequel I system.

To prepare PCR-free libraries for short-read sequencing, the genomic DNA was fragmented to 250–350 bp using a Covaris S2 Focused Ultrasonicator (Covaris). The libraries were prepared according to the manufacturer’s instructions with either the TruSeq DNA PCR-free kit (Illumina, 20015962) or the NxSeq AmpFREE Low DNA Library kit (Lucigen, 14000-2). In total, libraries for 89 accessions (including the main 27 for which we assembled their genomes) were sequenced in paired-end mode on a HiSeq 3000 system (Illumina).

The ultra-HMW DNA extraction and sample preparation for optical maps were performed as described[75](https://www.nature.com/articles/s41588-025-02293-0#ref-CR75 "Rabanal, F. A. et al. Pushing the limits of HiFi assemblies reveals centromere diversity between two Arabidopsis thaliana genomes. Nucleic Acids Res. 50, 12309–12327 (2022)."),[76](https://www.nature.com/articles/s41588-025-02293-0#ref-CR76 "Ou, S. et al. Effect of sequence depth and length in long-read assembly of the maize inbred NC358. Nat. Commun. 11, 2288 (2020).") at Corteva Agriscience using the Direct Label and Stain technology (Bionano Genomics).

### Assembly

The CLR subreads were assembled with Canu v1.71 (ref. [77](https://www.nature.com/articles/s41588-025-02293-0#ref-CR77 "Koren, S. et al. Canu: scalable and accurate long-read assembly via adaptive k-mer weighting and repeat separation. Genome Res. 27, 722–736 (2017).")). Since accessions 9981 and 10002 had been sequenced at higher coverage on a Sequel II instrument, only about 200× genome coverage worth of reads were used for assembly. We performed two rounds of polishing on the resulting contigs of all assemblies—first with the CLR subreads and Arrow v2.3.2 ([https://github.com/PacificBiosciences/gcpp](https://github.com/PacificBiosciences/gcpp)), and then with PCR-free short reads and Pilon v1.22 (ref. [78](https://www.nature.com/articles/s41588-025-02293-0#ref-CR78 "Walker, B. J. et al. Pilon: an integrated tool for comprehensive microbial variant detection and genome assembly improvement. PLoS ONE 9, e112963 (2014).")).

For scaffolding, we generated hybrid scaffolds with optical maps for eight accessions (Supplementary Table [1](https://www.nature.com/articles/s41588-025-02293-0#MOESM4)) using Bionano Access v1.5 and [Bionano Solve](https://bionanogenomics.com/support/software-downloads) v3.6. The assembly was performed in pre-assembly mode with parameters nonhaplotype and no-CMPR-cut, without extend-split. Based on what we learned from these hybrid assemblies, we set the parameters for in silico scaffolding of the other genomes. We scaffolded contigs >150 kb with RagTag v1.1.1 (ref. [79](https://www.nature.com/articles/s41588-025-02293-0#ref-CR79 "Alonge, M. et al. Automated assembly scaffolding using RagTag elevates a new tomato system for high-throughput genome editing. Genome Biol. 23, 258 (2022)."); scaffold -q 60 -f 10000 -I 0.6 -remove-small) using the TAIR10 reference with hard-masked centromeres, rDNAs, telomeres and nuclear insertions of organelles to prevent misplacement of contigs due to reference bias[75](https://www.nature.com/articles/s41588-025-02293-0#ref-CR75 "Rabanal, F. A. et al. Pushing the limits of HiFi assemblies reveals centromere diversity between two Arabidopsis thaliana genomes. Nucleic Acids Res. 50, 12309–12327 (2022)."). All scaffolded assemblies were manually curated to specifically discard low-confidence centromere satellite-rich contigs or to invert contigs with satellite repeats at their edges, indicative of their correct orientation. These edits were implemented in the AGP files, which were converted to FASTA format with the RagTag agp2fa function[79](https://www.nature.com/articles/s41588-025-02293-0#ref-CR79 "Alonge, M. et al. Automated assembly scaffolding using RagTag elevates a new tomato system for high-throughput genome editing. Genome Biol. 23, 258 (2022)."). To detect traces of residual heterozygosity, we aligned the original long reads to their corresponding chromosome scaffolds using pbmm2 v1.3.0 with the parameters align -sort -log-level DEBUG -preset SUBREAD -min-length 5000. Unmapped reads, as well as secondary and supplementary alignments, were filtered out using samtools v1.9 (view -b -F 2308 Chr1 Chr2 Chr3 Chr4 Chr5). The resulting BAM file was then analyzed with NucFreq v0.1 (-minobed 2) to assess genome-wide coverage of primary and secondary alleles[80](https://www.nature.com/articles/s41588-025-02293-0#ref-CR80 "Vollger, M. R. et al. Long-read sequence and assembly of segmental duplications. Nat. Methods 16, 88–94 (2019)."). AGP files, both before and after manual curation, as well as NucFreq plots, are available in the GitHub repository of this project.

### Repeat annotation

Repetitive elements were annotated as described[75](https://www.nature.com/articles/s41588-025-02293-0#ref-CR75 "Rabanal, F. A. et al. Pushing the limits of HiFi assemblies reveals centromere diversity between two Arabidopsis thaliana genomes. Nucleic Acids Res. 50, 12309–12327 (2022)."). We ran RepeatMasker v4.0.9 (-cutoff 200 -nolow -gff -xsmall) using a custom library that included various consensus sequences for the CEN178 (ref. [81](https://www.nature.com/articles/s41588-025-02293-0#ref-CR81 "Maheshwari, S., Ishii, T., Brown, C. T., Houben, A. & Comai, L. Centromere location in Arabidopsis is unaltered by extreme divergence in CENH3 protein sequence. Genome Res. 27, 471–478 (2017).")), 5S rDNA[82](https://www.nature.com/articles/s41588-025-02293-0#ref-CR82 "Simon, L. et al. Genetic and epigenetic variation in 5S ribosomal RNA genes reveals genome dynamics in Arabidopsis thaliana. Nucleic Acids Res. 46, 3019–3033 (2018)."), 45S rDNA[83](https://www.nature.com/articles/s41588-025-02293-0#ref-CR83 "Rabanal, F. A. et al. Unstable inheritance of 45S rRNA genes in Arabidopsis thaliana. G3 7, 1201–1209 (2017).") and telomere repeats. We annotated tRNAs with tRNAscan-SE v2.0.6 (ref. [84](https://www.nature.com/articles/s41588-025-02293-0#ref-CR84 "Chan, P. P. & Lowe, T. M. tRNAscan-SE: searching for tRNA genes in genomic sequences. Methods Mol. Biol. 1962, 1–14 (2019).")) and TEs with Extensive de novo TE Annotator v1.9.7 (ref. [85](https://www.nature.com/articles/s41588-025-02293-0#ref-CR85 "Ou, S. et al. Benchmarking transposable element annotation methods for creation of a streamlined, comprehensive pipeline. Genome Biol. 20, 275 (2019)."); –step all –sensitive 1 –anno 1), a pipeline that combines several TE annotation tools (LTRharvest, LTR\_FINDER, LTR\_retriever, TIR-Learner, HelitronScanner and TEsorter)[86](https://www.nature.com/articles/s41588-025-02293-0#ref-CR86 "Ellinghaus, D., Kurtz, S. & Willhoeft, U. LTRharvest, an efficient and flexible software for de novo detection of LTR retrotransposons. BMC Bioinformatics 9, 18 (2008)."),[87](https://www.nature.com/articles/s41588-025-02293-0#ref-CR87 "Ou, S. & Jiang, N. LTR_retriever: a highly accurate and sensitive program for identification of long terminal repeat retrotransposons. Plant Physiol. 176, 1410–1422 (2018)."),[88](https://www.nature.com/articles/s41588-025-02293-0#ref-CR88 "Xu, Z. & Wang, H. LTR_FINDER: an efficient tool for the prediction of full-length LTR retrotransposons. Nucleic Acids Res. 35, W265–W268 (2007)."),[89](https://www.nature.com/articles/s41588-025-02293-0#ref-CR89 "Ou, S. & Jiang, N. LTR_FINDER_parallel: parallelization of LTR_FINDER enabling rapid identification of long terminal repeat retrotransposons. Mob. DNA 10, 48 (2019)."),[90](https://www.nature.com/articles/s41588-025-02293-0#ref-CR90 "Su, W., Gu, X. & Peterson, T. TIR-Learner, a new ensemble method for TIR transposable element annotation, provides evidence for abundant new transposable elements in the maize genome. Mol. Plant 12, 447–460 (2019)."),[91](https://www.nature.com/articles/s41588-025-02293-0#ref-CR91 "Shi, J. & Liang, C. Generic repeat finder: a high-sensitivity tool for genome-wide de novo repeat detection. Plant Physiol. 180, 1803–1815 (2019)."),[92](https://www.nature.com/articles/s41588-025-02293-0#ref-CR92 "Xiong, W., He, L., Lai, J., Dooner, H. K. & Du, C. HelitronScanner uncovers a large overlooked cache of helitron transposons in many plant genomes. Proc. Natl Acad. Sci. USA 111, 10263–10268 (2014)."),[93](https://www.nature.com/articles/s41588-025-02293-0#ref-CR93 "Zhang, R.-G. et al. TEsorter: an accurate and fast method to classify LTR-retrotransposons in plant genomes. Hortic. Res. 9, uhac017 (2022)."). Finally, to understand the causes of contig breaks, we determined the type of repetitive element closest to each contig edge, considering the first 2 kb from each edge in contigs >10 kb.

### Pannagram

Pannagram is a toolkit designed for reference-free pangenome alignment, annotation and analysis, as well as for generating diagrams[46](https://www.nature.com/articles/s41588-025-02293-0#ref-CR46 "Igolkina, A. A., Bezlepsky, A. D. & Nordborg, M. Pannagram: unbiased pangenome alignment and the mobilome calling. Preprint at bioRxiv 
https://doi.org/10.1101/2025.02.07.637071
(2025).").

We represent the WGA as a matrix of corresponding positions, where rows represent accessions and columns represent homologous positions. The construction of the alignment is done in a reference-free manner (see below). However, to visualize the alignment in genome browsers, columns must be sorted in some manner, for example, to correspond to the TAIR10 sequence order. Then, columns of the pangenome are used as positions in the pangenome coordinate system.

To perform reference-free WGA, we developed a three-step pipeline. First, we use several accessions as references and build draft pairwise alignments between each and all other accessions. This process results in several reference-based matrices of corresponding positions. Next, we intersect these matrices, selecting only those columns that are present in all reference-biased matrices, which produces reliable and reference-independent correspondences. In the final step, we resolve unaligned sequences between blocks of corresponding positions using multiple sequence alignment tools. Once the reference-free alignment is complete, it can be sorted according to the desired order of accessions. In our case, we employ an alphabetical order, with the TAIR10 genome first.

For the pairwise alignments between a reference genome (not necessarily TAIR10) and another accession, the focal accession genome is divided into blocks of 5,000 bp, and each block is then mapped to the corresponding chromosomes of the reference genome using BLAST, with exactly one best hit retained for each block through this process. Next, the BLAST hits that are not in close proximity to each other in both genomes are removed. An additional BLAST search is performed to align corresponding unaligned sequences between remaining hits.

To resolve any unaligned blocks after the reference-randomization procedure, MAFFT[94](https://www.nature.com/articles/s41588-025-02293-0#ref-CR94 "Katoh, K., Misawa, K., Kuma, K.-I. & Miyata, T. MAFFT: a novel method for rapid multiple sequence alignment based on fast Fourier transform. Nucleic Acids Res. 30, 3059–3066 (2002).") is used. Blocks longer than 30 kb cannot be aligned within a reasonable time using MAFFT, so they are considered to be highly diverged. We found the final unaligned regions to be primarily associated with centromeric regions, rDNA clusters, telomeres and complex regions of multiple and long insertions and deletions, which are regions that are not of primary interest in this paper.

Given the WGA, SNPs can simply be output as sequence differences. However, sequence differences can arise from ambiguities in local alignment and do not necessarily correspond to SNPs (Supplementary Note [7](https://www.nature.com/articles/s41588-025-02293-0#MOESM1)). If we consider all sequence differences as SNPs, a pair of accessions differs at over 800,000 positions on average; however, if we restrict ourselves to isolated sequence differences, the number shrinks to 600,000.

### Pangenome graph

#### Graph construction

We constructed genome graphs for each of the five chromosomes using the PGGB pipeline[29](https://www.nature.com/articles/s41588-025-02293-0#ref-CR29 "Garrison, E. et al. Building pangenome graphs. Nat. Methods 21, 2008–2012 (2024)."). First, we prepared the assemblies by splitting them into chromosomes and removing all unplaced contigs. To enforce linearity for simpler analysis and comparison, we used a modified version of accession 22001 with the genome rearranged to a consensus pan-genomic order (suffix: ‘f’). We added the TAIR10 reference genome to the graph to enable anchoring and presentation of results in a reference framework.

We executed the PGGB pipeline (downloaded on 25 January 2024) with the following parameters: -s 10000 -p 90 -n 27. PGGB consists of the following three methods: an all-against-all alignment with wfmash (v0.12.4-5-g0b191bb), graph induction using seqwish (v0.7.9-2-gf44b402) and two rounds of pangenome ordering (odgi v0.8.3-26-gbc7742ed) followed by normalization with smoothxg (v0.7.2-11-g9970e0d). The graph was used for analyzing the pangenome and synteny, as well as detecting variation using vg deconstruct[95](https://www.nature.com/articles/s41588-025-02293-0#ref-CR95 "Garrison, E. et al. Variation graph toolkit improves read mapping by representing genetic variation in the reference. Nat. Biotechnol. 36, 875–879 (2018).").

#### Similarity

We exploited graph properties to classify different levels of similarity between genomes. Nodes traversed in all accessions are labeled as core, nodes traversed in only one accession are private and all other nodes (>1 and <28 traversals) are shell (soft). Please note that nodes can be traversed multiple times by the same genome, which affects the total number of core nodes. Because each node contains a specific sequence, node count can easily be converted to the actual amount of sequence and respective genomic location.

#### Synteny windows

Every node in the graph can be translated to its exact position for each path. This direct connection allows us to create sliding window approaches for each sample/path using graph-based statistics. Here we used nonoverlapping windows of 300 kb and calculated the average similarity (see above) of these regions. This was performed for each graph and path independently and the results were represented in a heat map.

#### Saturation analysis

A saturation analysis was performed using a bootstrapping approach. In each iteration, we removed a specific number of paths from our graph and performed the same pangenome categorization as above (‘Similarity’). In addition, we added the total pangenome, which describes the total amount of sequence (core + shell + private sequence). We performed 20 different (unique) combinations for each size (number of genomes).

#### Deconstructing the graph

To achieve full insights into graph variation and cover all bubbles in the graph, VG deconstruct was run multiple times with each accession reference path once (vg deconstruct -a -e). After, the reported VCF (v1.54.0 ‘Parafada’) files were converted to a BED file with all important information provided. In addition, each chromosome was merged, and the genotype information was concluded and added. Bubbles were identified by the start and end positions, and all traversals within these bubbles were also reported. Scripts can be found in the repository.

sSVs and cSVs in the graphs were defined as follows:

-   All SVs represent indels, having one very small traversal (deletion) and a large one containing the SV sequence (insertion).
    
-   Bubbles were identified as sSVs if the bubble was shared by all accessions in the graph (here 28), and as cSVs if not. Traversals covering the insertion are at least 15 bp long and must exhibit high similarity (95% sequence). The deletion part of the bubble should be small, at most 5% of the length of the inserted sequence.
    
-   Most cSVs correspond to bubbles that have a complex structure and/or are sub-bubbles of larger bubbles.
    

#### General pangenome

To perform a reference-free pangenome analysis, we used genome graphs built separately for each chromosome. The complete graph contains 18.3 million nodes and 20.9 million edges, with a total size of 225 Mb, and has a mean compression rate of 6.75% across all chromosomes. Similar to other genome-wide analyses in this study, the large-scale reciprocal translocation in accession 22001 was masked to maximize linearity and increase resolution in the variation graph.

### The mobile-ome

The mobile-ome refers to the collection of insertions and deletions that are likely to have occurred recently and are therefore not fixed in our sample. We hypothesize that each mobile event results in an SV, specifically a presence–absence polymorphism at the location of the insertion or deletion. Consequently, our initial approach involves extracting all presence–absence SVs and systematically decomposing them step by step. To distinguish between simple bi-allelic presence–absence polymorphisms (indels) and cSV, we analyzed the lengths of alleles within the SVs. We distinguish two types based on the similarity threshold _s_, with _s_ = 0.9 in our case. We consider a simple indel as one that contains alleles of two length types—those that are shorter than (1 − _s_) of the SV length (absence allele) and those that are longer than _s_ of the SV length (presence allele). The distinction between simple and complex presence–absence polymorphisms is partially a computational construct to filter SVs and simplify further analysis. Simple indels and complex presence–absence polymorphisms form a continuum, and by relaxing the similarity threshold (_s_ < 0.9, in our case), some complex SVs become classified as simple indels. Additionally, there is a natural bias towards complex presence–absence polymorphisms. Consider a scenario with a simple presence–absence polymorphism where an indel occurs within the presence allele. If the presence allele was initially observed in only one accession, then the new event does not reclassify the initial region as not belonging to the simple presence–absence polymorphisms category. However, if the presence allele was observed in multiple accessions, the new event is likely to be reclassified as complex presence–absence polymorphisms. To simplify and clarify the analysis, we considered only the simple polymorphisms. To determine the known portion of the mobile-ome within indels, we conducted BLAST searches using pangenome consensus sequences of indels against known _A. thaliana_ TEs, as well as against themselves. The indels that exhibited some similarity to known TEs were divided into the following groups: is complete—significant similarity to known TEs and can be classified as TEs themselves; contains complete—contained regions with similarity to known TEs, but also additional sequences; is fragment—contained only partially sequenced with similarity to known TEs; and contains fragment—partial coverage by BLAST hits of TE segments, but also additional sequences unrelated to known TEs.

We consider all these indels as parts of the mobile-ome. Indels without similarity to known TEs but showing nested similarities within the indel data set (where one sequence is a subsequence of another) were considered as potential candidates for new mobile-ome elements. To investigate their potential function, we obtained all six open reading frames within each of these indels. From each translated sequence, we selected either all continuous stretches without stop codons that were longer than 100 codons or the longest stretch that exceeded 30 codons without a stop. Subsequently, we performed a BLAST search using the obtained amino acid sequences against the NCBI protein database and classified the potential proteins into four categories. If the BLAST results for an sSV contained keywords related to TE, we assigned the sequence to the TE-like category. These keywords were ‘transcriptase’, ‘reverse’, ‘transpos’, ‘gag-’, ‘pol-’, ‘integrase’, ‘gag/pol’, ‘gagpol’, ‘retrovirus’, ‘RNA-directed DNA polymerase’ and ‘RNA-dependent DNA polymerase’. sSVs that only had BLAST hits with descriptions such as ‘hypothetical protein’, ‘unnamed protein product’, ‘uncharacterized protein’, ‘predicted protein’, ‘PREDICTED:’, ‘putative protein’ and ‘unknown’ were categorized as ‘undefined proteins’. Indels without any BLAST hits were classified as ‘no protein’. In all other cases, sSV was categorized as a ‘defined protein.’

### Gene annotation

#### Preliminary annotation

Gene annotation was mainly based on Augustus (v3.3.3)[96](https://www.nature.com/articles/s41588-025-02293-0#ref-CR96 "Stanke, M., Diekhans, M., Baertsch, R. & Haussler, D. Using native and syntenically mapped cDNA alignments to improve de novo gene finding. Bioinformatics 24, 637–644 (2008)."). Augustus-predicted gene models were trained using parameters obtained from ‘hints’ from three different sources. First, we ran BUSCO (v4.0.1)[97](https://www.nature.com/articles/s41588-025-02293-0#ref-CR97 "Seppey, M., Manni, M. & Zdobnov, E. M. BUSCO: assessing genome assembly and annotation completeness. Methods Mol. Biol. 1962, 227–245 (2019).") with \-m genome option. Second, the _A. thaliana_ reference gene annotation was projected onto each genome using Liftoff[98](https://www.nature.com/articles/s41588-025-02293-0#ref-CR98 "Shumate, A. & Salzberg, S. L. Liftoff: accurate mapping of gene annotations. Bioinformatics 37, 1639–1643 (2021).") with the -exclude\_partial and -copies options. Third, the RNA-seq data for each accession were used—wiggle hints were generated using bam2wig and wig2hints, and EST hints were generated using bam2hints (all three tools provided by Augustus). Augustus was run with the following nondefault parameters:

-   –softmasking 1
    
-   –species=BUSCO\_retraining
    
-   –gff3=on
    
-   –extrinsicCfgFile=Custom\_Config
    
-   –hintsfile=Liftoff\_hints
    

For every accession, the GFF3 output of Augustus was run through the Augustus-provided tool getAnno.pl to translate gene annotations into protein sequences. Finally, for each annotation, the Augustus output was combined and evaluated using augustus\_GFF3\_to\_EVM\_GFF3.pl (provided by EVidenceModeler[99](https://www.nature.com/articles/s41588-025-02293-0#ref-CR99 "Haas, B. J. et al. Automated eukaryotic gene structure annotation using EVidenceModeler and the program to assemble spliced alignments. Genome Biol. 9, R7 (2008).")).

In addition to the Augustus-generated annotations, we used two types of independent evidence for gene models: from the SNAP de novo annotation tool[100](https://www.nature.com/articles/s41588-025-02293-0#ref-CR100 "Campbell, M. S. et al. MAKER-P: a tool kit for the rapid creation, management, and quality control of plant genome annotations. Plant Physiol. 164, 513–524 (2014).") and Cufflinks transcriptome assemblies[101](https://www.nature.com/articles/s41588-025-02293-0#ref-CR101 "Trapnell, C. et al. Differential gene and transcript expression analysis of RNA-seq experiments with TopHat and Cufflinks. Nat. Protoc. 7, 562–578 (2012)."). Annotations produced by Augustus, SNAP and Cufflinks were combined and then subdivided into 1-Mb windows with 1-kb overlap using partition\_EVM\_input.pl (provided by EVidenceModeler). We ran EVidenceModeler with annotation GFF files, the assembly fasta file, the partitions and a weight matrix. We chose weights for each input based on their ability to recreate the Araport11 gene annotation. Running EVidenceModeler produced the final annotation compilation for each accession. We retained only the longest isoform for each gene using gffread[102](https://www.nature.com/articles/s41588-025-02293-0#ref-CR102 "Pertea, G. & Pertea, M. GFF utilities: GffRead and GffCompare. F1000Res. 9, ISCB Comm J-304 (2020).").

#### Reconciling annotations

To enable comparison between the independent annotations, we used the pangenome coordinate system, reconciling discrepancies using majority voting (Supplementary Note [6](https://www.nature.com/articles/s41588-025-02293-0#MOESM1)—‘Details about reconciling annotations and gene filtering’). Additionally, we compared the sequences of each gene across different accessions. If a gene showed significant variation because it was located in regions heavily influenced by SVs, we excluded it from the analysis. In total, 3,438 genes in our annotation were the result of splitting preliminary annotations and 1,020 were the result of merges. Lastly, we added 1,789 TAIR10 genes that had not been detected by our annotation pipeline (the likely reason for which is that our RNA-seq data only covered four tissues/stages) to our annotation. For these genes, the same pangenome coordinate approach was used to map the TAIR10 annotation of the 1,789 added genes into their annotations in other genomes. Our approach generated a total of 34,153 putative genes. For the details of annotation reconciliation and filtering, see Supplementary Note [6](https://www.nature.com/articles/s41588-025-02293-0#MOESM1)—‘Details about reconciling annotations and gene filtering’.

#### Ancestry analysis

All PC sequences from all accessions were compared using DIAMOND’s blastp module[103](https://www.nature.com/articles/s41588-025-02293-0#ref-CR103 "Buchfink, B., Reuter, K. & Drost, H.-G. Sensitive protein alignments at tree-of-life scale using DIAMOND. Nat. Methods 18, 366–368 (2021).") (version 2.0.11) against the _A. lyrata_ MN47 proteome (version 2, GenBank: GCA\_944990045.1), and the best hit was considered as the _A. lyrata_ homolog. To avoid bias due to mis-annotated genes in the _A. lyrata_ proteome, we further applied Liftoff v1.63 (ref. [98](https://www.nature.com/articles/s41588-025-02293-0#ref-CR98 "Shumate, A. & Salzberg, S. L. Liftoff: accurate mapping of gene annotations. Bioinformatics 37, 1639–1643 (2021).")) to annotate all _A. thaliana_ genes from all accessions on _A. lyrata_ MN47 (v2, [https://doi.org/10.6084/m9.figshare.22285444.v1](https://doi.org/10.6084/m9.figshare.22285444.v1)) and _A. lyrata_ NT1 (v2, [https://doi.org/10.6084/m9.figshare.22293196.v1](https://doi.org/10.6084/m9.figshare.22293196.v1)) assemblies. Next, each annotation group from _A. thaliana_ was assigned to the _A. lyrata_ homolog (by LiftOff or proteome similarity) that was common to at least 50% of its members, sharing at least 80% identity and covering at least 80% of the _A. thaliana_ coding sequence. _A. thaliana_ annotation groups were defined to be ancestrally relative to the _A. lyrata_ gene if they were part of a colinear segment of at least two genes. To that end, all _A. thaliana_ genes were ordered according to their relative position in the pangenome coordinate system. Each pair of consecutive genes in _A. thaliana_ was assigned to the same colinear segment as its homologs in _A. lyrata_ if the homologs were separated by fewer than six genes. The ancestral state was defined as ‘similar’ for cases where the genes from _A. lyrata_ and _A. thaliana_ were not part of the same colinear segment but shared at least 80% sequence identity over at least 80% of the length _A. thaliana_ gene. Further details are available in [Supplementary Note 6](https://www.nature.com/articles/s41588-025-02293-0#MOESM1)—under ‘Genes and TEs’ for TE analysis and ‘New genes’ for the origin of new genes.

### Expression analysis

#### RNA-seq read mapping and gene expression calculation

Raw RNA-seq reads from 7-day-old seedlings, 9-leaf rosettes, flowers and pollen[54](https://www.nature.com/articles/s41588-025-02293-0#ref-CR54 "Kornienko, A. E., Nizhynska, V., Molla Morales, A., Pisupati, R. & Nordborg, M. Population-level annotation of lncRNAs in Arabidopsis reveals extensive expression variation associated with transposable element-like silencing. Plant Cell 36, 85–111 (2023).") were aligned either to the TAIR10 reference genome or the corresponding accession accession genome using STAR v2.7.1 (ref. [104](https://www.nature.com/articles/s41588-025-02293-0#ref-CR104 "Dobin, A. et al. STAR: ultrafast universal RNA-seq aligner. Bioinformatics 29, 15–21 (2013).")) with the following custom options:

-   –alignIntronMax 6000
    
-   –alignMatesGapMax 6000
    
-   –outFilterIntronMotifs RemoveNoncanonical
    
-   –outFilterMismatchNoverReadLmax 0.1
    
-   –outFilterMismatchNmax 999
    
-   –outFilterMismatchNoverLmax 0.3
    
-   –outFilterMultimapNmax 1
    
-   –alignSJoverhangMin 8
    
-   –outSAMattributes NH HI AS nM NM MD jM jI XS
    

Read alignment statistics are provided in Supplementary Table [4](https://www.nature.com/articles/s41588-025-02293-0#MOESM7). Expression levels were assessed using featurecounts from Subread v2.0.1 (ref. [105](https://www.nature.com/articles/s41588-025-02293-0#ref-CR105 "Liao, Y., Smyth, G. K. & Shi, W. featureCounts: an efficient general purpose program for assigning sequence reads to genomic features. Bioinformatics 30, 923–930 (2014).")) on each RNA-seq sample with either the TAIR10 gene annotation or the accession-specific annotations from this study. The entire locus, including exons and introns, was used for expression estimates. Expression levels were normalized by calculating TPMs, which represent the number of read counts divided by the gene length in kilobases, and then dividing the total number of counts per kilobase for all genes by 1 million.

#### Mapping to TAIR10 versus the own genome

To determine whether the gene expression calculation was consistent between RNA-seq mapping in TAIR10 versus accession-specific genomes, we focused on the annotation groups with a one-to-one correspondence with an Araport11 gene. For each RNA-seq sample, we obtained the Pearson’s correlation coefficient between the number of exonic counts obtained from TAIR10 mapping and accession-specific mapping. We also determined the number of genes that were correctly or wrongly estimated using TAIR10 mapping. We called a gene ‘wrong’ if the counts in TAIR10 and the counts in its own genome differed by more than 30% (Ncounts\_min/Ncounts\_max ≤ 0.7). Only genes with at least six counts in either calculation were analyzed.

### Chromatin immunoprecipitation followed by sequencing analysis

We used chromatin immunoprecipitation followed by sequencing (ChIP–seq) data from 6 accessions and sRNA-seq data from 14 accessions[54](https://www.nature.com/articles/s41588-025-02293-0#ref-CR54 "Kornienko, A. E., Nizhynska, V., Molla Morales, A., Pisupati, R. & Nordborg, M. Population-level annotation of lncRNAs in Arabidopsis reveals extensive expression variation associated with transposable element-like silencing. Plant Cell 36, 85–111 (2023)."). We used STAR[104](https://www.nature.com/articles/s41588-025-02293-0#ref-CR104 "Dobin, A. et al. STAR: ultrafast universal RNA-seq aligner. Bioinformatics 29, 15–21 (2013).") to map ChIP–seq reads with these nondefault options:

-   –alignIntronMax 5
    
-   –outFilterMismatchNmax 10
    
-   –outFilterMultimapNmax 1
    
-   –alignEndsType EndToEnd
    
-   –twopassMode Basic
    

The ChIP–seq data were log2\-normalized to input using bamCompare (deeptools package[106](https://www.nature.com/articles/s41588-025-02293-0#ref-CR106 "Ramírez, F. et al. deepTools2: a next generation web server for deep-sequencing data analysis. Nucleic Acids Res. 44, W160–W165 (2016).")) using

-   –operation log2
    
-   –effectiveGenomeSize 119481543
    
-   –ignoreDuplicates
    
-   –outFileFormat bedgraph
    

The ChIP–seq coverage was estimated using bedtools map-mean[107](https://www.nature.com/articles/s41588-025-02293-0#ref-CR107 "Quinlan, A. R. & Hall, I. M. BEDTools: a flexible suite of utilities for comparing genomic features. Bioinformatics 26, 841–842 (2010)."). The ChIP–seq coverage was further normalized to obtain value range similarity across accessions. For this, we applied quantile-normalization using an _R_ function:

-   function(x) { (x-quantile(x,.20)) / (quantile(x,.80) - quantile(x,.20)) }
    

which equalized the 20% and 80% quantile values of each ChIP–seq sample. After quantile-normalization, the replicated samples were averaged.

### sRNA-seq analysis

We used sRNA-seq data for 14 accessions[54](https://www.nature.com/articles/s41588-025-02293-0#ref-CR54 "Kornienko, A. E., Nizhynska, V., Molla Morales, A., Pisupati, R. & Nordborg, M. Population-level annotation of lncRNAs in Arabidopsis reveals extensive expression variation associated with transposable element-like silencing. Plant Cell 36, 85–111 (2023)."). To process the sRNA-seq data, we trimmed the reads using cutadapt[108](https://www.nature.com/articles/s41588-025-02293-0#ref-CR108 "Martin, M. Cutadapt removes adapter sequences from high-throughput sequencing reads. EMBnet J. 17, 10–12 (2011)."): cutadapt -a AACTGTAGGCACCATCAAT –minimum-length 18. We then used STAR[104](https://www.nature.com/articles/s41588-025-02293-0#ref-CR104 "Dobin, A. et al. STAR: ultrafast universal RNA-seq aligner. Bioinformatics 29, 15–21 (2013).") with the following nondefault options to map sRNA-seq reads to the corresponding genome:

-   –runRNGseed 12345
    
-   –alignEndsType Extend5pOfRead1
    
-   –alignIntronMax 5000 –alignSJDBoverhangMin 1
    
-   –outReadsUnmapped Fastx –outSAMmultNmax 100
    
-   –outSAMprimaryFlag AllBestScore
    
-   –outSAMattributes NH HI AS nM NM MD jM jI XS
    
-   –outFilterMultimapNmax 10
    
-   –outFilterMatchNmin 16
    
-   –outFilterMatchNminOverLread 0.66
    
-   –outFilterMismatchNmax 2
    
-   –outFilterMismatchNoverReadLmax 0.05
    
-   –outFilterIntronMotifs RemoveNoncanonicalUnannotated
    
-   –twopassMode None
    

We extracted 24-nt reads, calculated read coverage for each position of the genome using genomeCoverageBed (bedtools v.2.27.1), normalized it by the total number of uniquely mapped reads in each sample, and calculated 24-nt sRNA coverage for each locus of interest using bedtools map -mean function.

### DNA methylation analysis

To estimate DNA methylation levels, we used published BS-seq data for 12 accessions[53](https://www.nature.com/articles/s41588-025-02293-0#ref-CR53 "Kawakatsu, T. et al. Epigenomic diversity in a global collection of Arabidopsis thaliana accessions. Cell 166, 492–505 (2016)."). After trimming with TrimGalore ([https://github.com/FelixKrueger/TrimGalore](https://github.com/FelixKrueger/TrimGalore)) with –clip\_r1 10 –clip\_r2 15 –three\_prime\_clip\_r1 10 –three\_prime\_clip\_r2 10, reads for each accession were mapped to its corresponding genome with Bismark[109](https://www.nature.com/articles/s41588-025-02293-0#ref-CR109 "Krueger, F. & Andrews, S. R. Bismark: a flexible aligner and methylation caller for bisulfite-seq applications. Bioinformatics 27, 1571–1572 (2011).") with –score\_min L,0,-0.5 for a relaxed mismatch threshold and the –un –ambiguous parameters to obtain additional unmapped and multiply-mapping reads. Methylation was called as described[110](https://www.nature.com/articles/s41588-025-02293-0#ref-CR110 "Pisupati, R., Nizhynska, V., Mollá Morales, A. & Nordborg, M. On the causes of gene-body methylation variation in Arabidopsis thaliana. PLoS Genet. 19, e1010728 (2023)."). CG, CHG and CHH methylation levels for genes and SVs in each accession were then calculated for each gene by focusing on all Cs in the specific context within the gene and calculating the ratio between the total number of methylated and unmethylated reads across all sites.

#### Mapping to TAIR10 versus own genome

To estimate reference bias, we mapped BS-seq data for all accessions to the TAIR10 genome and performed CG, CHG and CHH methylation level estimation in the same way as for own genomes. We then focused on annotation groups with a one-to-one correspondence with an Araport11 gene (the current annotation of the TAIR10 genome). We calculated Pearson’s correlation coefficient between the methylation level estimates obtained from TAIR10 mapping and accession-genome mapping. We also estimated the number of genes that were correctly or wrongly estimated using TAIR10 mapping. For each methylation context, we called a gene ‘wrongly estimated’ if the methylation level in TAIR10 and the own genome differed by more than 50% (methlevel\_min/methlevel\_max ≤ 0.5). For a more refined analysis of reference bias, see Supplementary Note [8](https://www.nature.com/articles/s41588-025-02293-0#MOESM1).

### Reporting summary

Further information on research design is available in the [Nature Portfolio Reporting Summary](https://www.nature.com/articles/s41588-025-02293-0#MOESM2) linked to this article.

Data availability
-----------------

Raw sequencing data (PacBio CLR and Illumina PCR-free short reads) and genome assemblies have been deposited in the European Nucleotide Archive (ENA) under project accession [PRJEB73474](https://www.ebi.ac.uk/ena/data/view/PRJEB73474) (ERP158243). Illumina PCR-free short reads for 61 additional accessions used to investigate the contribution of satellite repeats can be accessed under project accession [PRJEB73476](https://www.ebi.ac.uk/ena/data/view/PRJEB73476) (ERP158245). BS-seq data from mature leaves of 14-leaf rosettes are from the 1001 Genomes Project[53](https://www.nature.com/articles/s41588-025-02293-0#ref-CR53 "Kawakatsu, T. et al. Epigenomic diversity in a global collection of Arabidopsis thaliana accessions. Cell 166, 492–505 (2016).") and are available under GEO accession [GSE43857](http://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE43857). ChIP-, RNA-seq and sRNA-seq data were likewise previously published[54](https://www.nature.com/articles/s41588-025-02293-0#ref-CR54 "Kornienko, A. E., Nizhynska, V., Molla Morales, A., Pisupati, R. & Nordborg, M. Population-level annotation of lncRNAs in Arabidopsis reveals extensive expression variation associated with transposable element-like silencing. Plant Cell 36, 85–111 (2023)."): ChIP–seq data from 14-leaf rosettes are available under GEO accession [GSE226682](http://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE226682); RNA-seq data from seedlings, 9-leaf rosettes, flowers and pollen are available under GEO accession [GSE226691](http://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE226691); and sRNA-seq data from flowers are available under the GEO accession [GSE224571](http://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE224571). Several widely used public databases were used in the analyses: NCBI Protein Blast, UniProtKB (version 2024\_06), and the TAIR10 genome annotation. Maps were generated using public domain data from the Natural Earth project via the R package rnaturalearth. See also [https://1001genomes.org/](https://1001genomes.org/), where a collection of accession-based JBrowse2 genome viewers and a pan-genome JBrowse2 browser are available, along with other relevant information.

Code availability
-----------------

All scripts, including methods for analyzing the pangenome graph, can be found in an ad hoc GitHub repository ([https://github.com/Gregor-Mendel-Institute/1001Gplus\_paper](https://github.com/Gregor-Mendel-Institute/1001Gplus_paper); archived at [https://doi.org/10.5281/zenodo.15790915](https://doi.org/10.5281/zenodo.15790915))[111](https://www.nature.com/articles/s41588-025-02293-0#ref-CR111 "Igolkina, A. et al. Gregor-Mendel-Institute/1001Gplus_paper: v1.0.0. Zenodo 
https://doi.org/10.5281/zenodo.15790915
(2025)."). The Pannagram toolkit[46](https://www.nature.com/articles/s41588-025-02293-0#ref-CR46 "Igolkina, A. A., Bezlepsky, A. D. & Nordborg, M. Pannagram: unbiased pangenome alignment and the mobilome calling. Preprint at bioRxiv 
https://doi.org/10.1101/2025.02.07.637071
(2025).") can be found in a separate repository ([https://github.com/iganna/pannagram](https://github.com/iganna/pannagram); v1.1 archived at [https://doi.org/10.5281/zenodo.15791785](https://doi.org/10.5281/zenodo.15791785))[112](https://www.nature.com/articles/s41588-025-02293-0#ref-CR112 "Igolkina, A. iganna/pannagram: version for the 27-genomes paper (v1.1). Zenodo 
https://doi.org/10.5281/zenodo.15791785
(2025)."), and the same is true for the automated PacBio long-read genome assembly pipeline ([https://github.com/weigelworld/auto-asm](https://github.com/weigelworld/auto-asm); archived at [https://doi.org/10.5281/zenodo.15775624](https://doi.org/10.5281/zenodo.15775624))[113](https://www.nature.com/articles/s41588-025-02293-0#ref-CR113 "Wrightsman, T., Kubica, C. & Ashkenazy, H. Automated assembly pipeline for PacBio long read datasets. Zenodo 
https://doi.org/10.5281/zenodo.15775624
(2025).").

References
----------

1.  Gallone, B. et al. Domestication and divergence of _Saccharomyces cerevisiae_ beer yeasts. _Cell_ **166**, 1397–1410 (2016).
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Domestication%20and%20divergence%20of%20Saccharomyces%20cerevisiae%20beer%20yeasts&journal=Cell&volume=166&publication_year=2016&author=Gallone%2CB) 
    
2.  Istace, B. et al. De novo assembly and population genomic survey of natural yeast isolates with the Oxford Nanopore MinION sequencer. _GigaScience_ **6**, 1–13 (2017).
    
    [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=28369459)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC5466710)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=De%20novo%20assembly%20and%20population%20genomic%20survey%20of%20natural%20yeast%20isolates%20with%20the%20Oxford%20Nanopore%20MinION%20sequencer&journal=GigaScience&volume=6&pages=1-13&publication_year=2017&author=Istace%2CB) 
    
3.  Peter, J. et al. Genome evolution across 1,011 _Saccharomyces cerevisiae_ isolates. _Nature_ **556**, 339–344 (2018).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BC1cXosVCgt70%3D)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=29643504)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC6784862)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Genome%20evolution%20across%201%2C011%20Saccharomyces%20cerevisiae%20isolates&journal=Nature&volume=556&pages=339-344&publication_year=2018&author=Peter%2CJ) 
    
4.  Walkowiak, S. et al. Multiple wheat genomes reveal global variation in modern breeding. _Nature_ **588**, 277–283 (2020).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BB3cXisVeqtr3P)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=33239791)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC7759465)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Multiple%20wheat%20genomes%20reveal%20global%20variation%20in%20modern%20breeding&journal=Nature&volume=588&pages=277-283&publication_year=2020&author=Walkowiak%2CS) 
    
5.  Alonge, M. et al. Major impacts of widespread structural variation on gene expression and crop improvement in tomato. _Cell_ **182**, 145–161 (2020).
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Major%20impacts%20of%20widespread%20structural%20variation%20on%20gene%20expression%20and%20crop%20improvement%20in%20tomato&journal=Cell&volume=182&publication_year=2020&author=Alonge%2CM) 
    
6.  Jayakodi, M. et al. The barley pan-genome reveals the hidden legacy of mutation breeding. _Nature_ **588**, 284–289 (2020).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BB3cXisVeqtr3K)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=33239781)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC7759462)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=The%20barley%20pan-genome%20reveals%20the%20hidden%20legacy%20of%20mutation%20breeding&journal=Nature&volume=588&pages=284-289&publication_year=2020&author=Jayakodi%2CM) 
    
7.  Hufford, M. B. et al. De novo assembly, annotation, and comparative analysis of 26 diverse maize genomes. _Science_ **373**, 655–662 (2021).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BB3MXhslOisLnM)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=34353948)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC8733867)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=De%20novo%20assembly%2C%20annotation%2C%20and%20comparative%20analysis%20of%2026%20diverse%20maize%20genomes&journal=Science&volume=373&pages=655-662&publication_year=2021&author=Hufford%2CMB) 
    
8.  Liu, Y. et al. Pan-Genome of wild and cultivated soybeans. _Cell_ **182**, 162–176 (2020).
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Pan-Genome%20of%20wild%20and%20cultivated%20soybeans&journal=Cell&volume=182&publication_year=2020&author=Liu%2CY) 
    
9.  Qin, P. et al. Pan-genome analysis of 33 genetically diverse rice accessions reveals hidden genomic variations. _Cell_ **184**, 3542–3558 (2021).
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Pan-genome%20analysis%20of%2033%20genetically%20diverse%20rice%20accessions%20reveals%20hidden%20genomic%20variations&journal=Cell&volume=184&publication_year=2021&author=Qin%2CP) 
    
10.  Ebert, P. et al. Haplotype-resolved diverse human genomes and integrated analysis of structural variation. _Science_ **372**, eabf7117 (2021).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BB3MXotFGluro%3D)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=33632895)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC8026704)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Haplotype-resolved%20diverse%20human%20genomes%20and%20integrated%20analysis%20of%20structural%20variation&journal=Science&volume=372&publication_year=2021&author=Ebert%2CP) 
    
11.  Rech, G. E. et al. Population-scale long-read sequencing uncovers transposable elements associated with gene expression variation and adaptive signatures in Drosophila. _Nat. Commun._ **13**, 1948 (2022).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BB38Xps1Ojtrc%3D)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=35413957)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC9005704)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Population-scale%20long-read%20sequencing%20uncovers%20transposable%20elements%20associated%20with%20gene%20expression%20variation%20and%20adaptive%20signatures%20in%20Drosophila&journal=Nat.%20Commun.&volume=13&publication_year=2022&author=Rech%2CGE) 
    
12.  Zhou, Y. et al. Graph pangenome captures missing heritability and empowers tomato breeding. _Nature_ **606**, 527–534 (2022).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BB38XhsFWhu7bO)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=35676474)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC9200638)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Graph%20pangenome%20captures%20missing%20heritability%20and%20empowers%20tomato%20breeding&journal=Nature&volume=606&pages=527-534&publication_year=2022&author=Zhou%2CY) 
    
13.  Li, R. et al. A sheep pangenome reveals the spectrum of structural variations and their effects on tail phenotypes. _Genome Res._ **33**, 463–477 (2023).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BB2cXitFyqu7%2FO)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=37310928)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC10078295)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=A%20sheep%20pangenome%20reveals%20the%20spectrum%20of%20structural%20variations%20and%20their%20effects%20on%20tail%20phenotypes&journal=Genome%20Res.&volume=33&pages=463-477&publication_year=2023&author=Li%2CR) 
    
14.  Ferguson, S. et al. Plant genome evolution in the genus Eucalyptus is driven by structural rearrangements that promote sequence divergence. _Genome Res._ **34**, 606–619 (2024).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BB2cXitF2ks7rO)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=38589251)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC11146599)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Plant%20genome%20evolution%20in%20the%20genus%20Eucalyptus%20is%20driven%20by%20structural%20rearrangements%20that%20promote%20sequence%20divergence&journal=Genome%20Res.&volume=34&pages=606-619&publication_year=2024&author=Ferguson%2CS) 
    
15.  Liao, W.-W. et al. A draft human pangenome reference. _Nature_ **617**, 312–324 (2023).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BB3sXpvVansLk%3D)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=37165242)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC10172123)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=A%20draft%20human%20pangenome%20reference&journal=Nature&volume=617&pages=312-324&publication_year=2023&author=Liao%2CW-W) 
    
16.  Wlodzimierz, P. et al. Cycles of satellite and transposon evolution in Arabidopsis centromeres. _Nature_ **618**, 557–565 (2023).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BB3sXhtVejsbzI)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=37198485)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Cycles%20of%20satellite%20and%20transposon%20evolution%20in%20Arabidopsis%20centromeres&journal=Nature&volume=618&pages=557-565&publication_year=2023&author=Wlodzimierz%2CP) 
    
17.  He, Q. et al. A graph-based genome and pan-genome variation of the model plant Setaria. _Nat. Genet._ **55**, 1232–1242 (2023).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BB3sXhtF2itbrK)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=37291196)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC10335933)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=A%20graph-based%20genome%20and%20pan-genome%20variation%20of%20the%20model%20plant%20Setaria&journal=Nat.%20Genet.&volume=55&pages=1232-1242&publication_year=2023&author=He%2CQ) 
    
18.  Shi, T. et al. The super-pangenome of Populus unveils genomic facets for its adaptation and diversification in widespread forest trees. _Mol. Plant_ **17**, 725–746 (2024).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BB2cXnslahu7k%3D)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=38486452)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=The%20super-pangenome%20of%20Populus%20unveils%20genomic%20facets%20for%20its%20adaptation%20and%20diversification%20in%20widespread%20forest%20trees&journal=Mol.%20Plant&volume=17&pages=725-746&publication_year=2024&author=Shi%2CT) 
    
19.  Kang, M. et al. The pan-genome and local adaptation of _Arabidopsis thaliana_. _Nat. Commun._ **14**, 6259 (2023).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BB3sXitFamtLnK)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=37802986)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC10558531)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=The%20pan-genome%20and%20local%20adaptation%20of%20Arabidopsis%20thaliana&journal=Nat.%20Commun.&volume=14&publication_year=2023&author=Kang%2CM) 
    
20.  Cochetel, N. et al. A super-pangenome of the North American wild grape species. _Genome Biol._ **24**, 290 (2023).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BB3sXis1CnsrzM)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=38111050)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC10729490)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=A%20super-pangenome%20of%20the%20North%20American%20wild%20grape%20species&journal=Genome%20Biol.&volume=24&publication_year=2023&author=Cochetel%2CN) 
    
21.  Beaulieu, C. et al. The Marchantia polymorpha pangenome reveals ancient mechanisms of plant adaptation to the environment. _Nat. Genet._ **57**, 729–740 (2025).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BB2MXktVWmsbo%3D)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=39962240)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC11906373)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=The%20Marchantia%20polymorpha%20pangenome%20reveals%20ancient%20mechanisms%20of%20plant%20adaptation%20to%20the%20environment&journal=Nat.%20Genet.&volume=57&pages=729-740&publication_year=2025&author=Beaulieu%2CC) 
    
22.  Li, X. et al. Large-scale gene expression alterations introduced by structural variation drive morphotype diversification in _Brassica oleracea_. _Nat. Genet._ **56**, 517–529 (2024).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BB2cXjs1Slt7c%3D)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=38351383)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC10937405)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Large-scale%20gene%20expression%20alterations%20introduced%20by%20structural%20variation%20drive%20morphotype%20diversification%20in%20Brassica%20oleracea&journal=Nat.%20Genet.&volume=56&pages=517-529&publication_year=2024&author=Li%2CX) 
    
23.  Lian, Q. et al. A pan-genome of 69 _Arabidopsis thaliana_ accessions reveals a conserved genome structure throughout the global species range. _Nat. Genet._ **56**, 982–991 (2024).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BB2cXot1Gqurc%3D)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=38605175)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC11096106)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=A%20pan-genome%20of%2069%20Arabidopsis%20thaliana%20accessions%20reveals%20a%20conserved%20genome%20structure%20throughout%20the%20global%20species%20range&journal=Nat.%20Genet.&volume=56&pages=982-991&publication_year=2024&author=Lian%2CQ) 
    
24.  Kileeg, Z., Wang, P. & Mott, G. A. Chromosome-scale assembly and annotation of eight _Arabidopsis thaliana_ ecotypes. _Genome Biol. Evol._ **16**, evae169 (2024).
    
    [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=39101619)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC11327923)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Chromosome-scale%20assembly%20and%20annotation%20of%20eight%20Arabidopsis%20thaliana%20ecotypes&journal=Genome%20Biol.%20Evol.&volume=16&publication_year=2024&author=Kileeg%2CZ&author=Wang%2CP&author=Mott%2CGA) 
    
25.  Quah, F. X. et al. Lake Malawi cichlid pangenome graph reveals extensive structural variation driven by transposable elements. _Genome Res._ **35**, 1094–1107 (2025).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BB2MXhvFamtbjL)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=40210437)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC12047535)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Lake%20Malawi%20cichlid%20pangenome%20graph%20reveals%20extensive%20structural%20variation%20driven%20by%20transposable%20elements&journal=Genome%20Res.&volume=35&pages=1094-1107&publication_year=2025&author=Quah%2CFX) 
    
26.  Schloissnig, S. et al. Long-read sequencing and structural variant characterization in 1,019 samples from the 1000 Genomes Project. Preprint at _bioRxiv_ [https://doi.org/10.1101/2024.04.18.590093](https://doi.org/10.1101/2024.04.18.590093) (2024).
    
27.  Jiao, C. et al. Pan-genome bridges wheat structural variations with habitat and breeding. _Nature_ **637**, 384–393 (2025).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BB2cXis1amu7%2FI)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=39604736)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Pan-genome%20bridges%20wheat%20structural%20variations%20with%20habitat%20and%20breeding&journal=Nature&volume=637&pages=384-393&publication_year=2025&author=Jiao%2CC) 
    
28.  Eizenga, J. M. et al. Pangenome graphs. _Annu. Rev. Genomics Hum. Genet._ **21**, 139–162 (2020).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BB3cXhtVWhsrfM)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=32453966)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC8006571)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Pangenome%20graphs&journal=Annu.%20Rev.%20Genomics%20Hum.%20Genet.&volume=21&pages=139-162&publication_year=2020&author=Eizenga%2CJM) 
    
29.  Garrison, E. et al. Building pangenome graphs. _Nat. Methods_ **21**, 2008–2012 (2024).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BB2cXitlant77L)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=39433878)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Building%20pangenome%20graphs&journal=Nat.%20Methods&volume=21&pages=2008-2012&publication_year=2024&author=Garrison%2CE) 
    
30.  Nordborg, M. et al. The pattern of polymorphism in _Arabidopsis thaliana_. _PLoS Biol._ **3**, e196 (2005).
    
    [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=15907155)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC1135296)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=The%20pattern%20of%20polymorphism%20in%20Arabidopsis%20thaliana&journal=PLoS%20Biol.&volume=3&publication_year=2005&author=Nordborg%2CM) 
    
31.  Clark, R. M. et al. Common sequence polymorphisms shaping genetic diversity in _Arabidopsis thaliana_. _Science_ **317**, 338–342 (2007).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BD2sXnslGrs7k%3D)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=17641193)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Common%20sequence%20polymorphisms%20shaping%20genetic%20diversity%20in%20Arabidopsis%20thaliana&journal=Science&volume=317&pages=338-342&publication_year=2007&author=Clark%2CRM) 
    
32.  Atwell, S. et al. Genome-wide association study of 107 phenotypes in _Arabidopsis thaliana_ inbred lines. _Nature_ **465**, 627–631 (2010).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BC3cXjvVShur8%3D)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=20336072)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC3023908)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Genome-wide%20association%20study%20of%20107%20phenotypes%20in%20Arabidopsis%20thaliana%20inbred%20lines&journal=Nature&volume=465&pages=627-631&publication_year=2010&author=Atwell%2CS) 
    
33.  Horton, M. W. et al. Genome-wide patterns of genetic variation in worldwide _Arabidopsis thaliana_ accessions from the RegMap panel. _Nat. Genet._ **44**, 212–216 (2012).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BC38XlsF2jsw%3D%3D)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=22231484)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC3267885)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Genome-wide%20patterns%20of%20genetic%20variation%20in%20worldwide%20Arabidopsis%20thaliana%20accessions%20from%20the%20RegMap%20panel&journal=Nat.%20Genet.&volume=44&pages=212-216&publication_year=2012&author=Horton%2CMW) 
    
34.  1001 Genomes Consortium. 1,135 genomes reveal the global pattern of polymorphism in _Arabidopsis thaliana_. _Cell_ **166**, 481–491 (2016).
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=1%2C135%20genomes%20reveal%20the%20global%20pattern%20of%20polymorphism%20in%20Arabidopsis%20thaliana&journal=Cell&volume=166&pages=481-491&publication_year=2016) 
    
35.  Zou, Y.-P. et al. Adaptation of _Arabidopsis thaliana_ to the Yangtze River basin. _Genome Biol._ **18**, 239 (2017).
    
    [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=29284515)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC5745794)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Adaptation%20of%20Arabidopsis%20thaliana%20to%20the%20Yangtze%20River%20basin&journal=Genome%20Biol.&volume=18&publication_year=2017&author=Zou%2CY-P) 
    
36.  Durvasula, A. et al. African genomes illuminate the early history and transition to selfing in _Arabidopsis thaliana_. _Proc. Natl Acad. Sci. USA_ **114**, 5213–5218 (2017).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BC2sXntVOrsr8%3D)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=28473417)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC5441814)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=African%20genomes%20illuminate%20the%20early%20history%20and%20transition%20to%20selfing%20in%20Arabidopsis%20thaliana&journal=Proc.%20Natl%20Acad.%20Sci.%20USA&volume=114&pages=5213-5218&publication_year=2017&author=Durvasula%2CA) 
    
37.  Fulgione, A., Koornneef, M., Roux, F., Hermisson, J. & Hancock, A. M. Madeiran _Arabidopsis thaliana_ reveals ancient long-range colonization and clarifies demography in Eurasia. _Mol. Biol. Evol._ **35**, 564–574 (2017).
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC5850838)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Madeiran%20Arabidopsis%20thaliana%20reveals%20ancient%20long-range%20colonization%20and%20clarifies%20demography%20in%20Eurasia&journal=Mol.%20Biol.%20Evol.&volume=35&pages=564-574&publication_year=2017&author=Fulgione%2CA&author=Koornneef%2CM&author=Roux%2CF&author=Hermisson%2CJ&author=Hancock%2CAM) 
    
38.  Quadrana, l. The _Arabidopsis thaliana_ mobilome and its impact at the species level. _eLife_ **5**, e15716 (2016).
    
    [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=27258693)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC4917339)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=The%20Arabidopsis%20thaliana%20mobilome%20and%20its%20impact%20at%20the%20species%20level&journal=eLife&volume=5&publication_year=2016&author=Quadrana%2Cl) 
    
39.  Fultz, D., McKinlay, A., Enganti, R. & Pikaard, C. S. Sequence and epigenetic landscapes of active and silent nucleolus organizer regions in _Arabidopsis_. _Sci. Adv._ **9**, eadj4509 (2023).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BB3sXitlamtrjN)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=37910609)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC10619934)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Sequence%20and%20epigenetic%20landscapes%20of%20active%20and%20silent%20nucleolus%20organizer%20regions%20in%20Arabidopsis&journal=Sci.%20Adv.&volume=9&publication_year=2023&author=Fultz%2CD&author=McKinlay%2CA&author=Enganti%2CR&author=Pikaard%2CCS) 
    
40.  Schmuths, H., Meister, A., Horres, R. & Bachmann, K. Genome size variation among accessions of _Arabidopsis thaliana_. _Ann. Bot._ **93**, 317–321 (2004).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BD2cXjtVCksrs%3D)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=14724121)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC4242198)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Genome%20size%20variation%20among%20accessions%20of%20Arabidopsis%20thaliana&journal=Ann.%20Bot.&volume=93&pages=317-321&publication_year=2004&author=Schmuths%2CH&author=Meister%2CA&author=Horres%2CR&author=Bachmann%2CK) 
    
41.  Long, Q. et al. Massive genomic variation and strong selection in _Arabidopsis thaliana_ lines from Sweden. _Nat. Genet._ **45**, 884–890 (2013).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BC3sXpvVymsrw%3D)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=23793030)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC3755268)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Massive%20genomic%20variation%20and%20strong%20selection%20in%20Arabidopsis%20thaliana%20lines%20from%20Sweden&journal=Nat.%20Genet.&volume=45&pages=884-890&publication_year=2013&author=Long%2CQ) 
    
42.  Kidwell, M. G. Transposable elements and the evolution of genome size in eukaryotes. _Genetica_ **115**, 49–63 (2002).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BD38XkvVaisLY%3D)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=12188048)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Transposable%20elements%20and%20the%20evolution%20of%20genome%20size%20in%20eukaryotes&journal=Genetica&volume=115&pages=49-63&publication_year=2002&author=Kidwell%2CMG) 
    
43.  Bista, I. et al. Genomics of cold adaptations in the Antarctic notothenioid fish radiation. _Nat. Commun._ **14**, 3412 (2023).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BB3sXht1amu7bO)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=37296119)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC10256766)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Genomics%20of%20cold%20adaptations%20in%20the%20Antarctic%20notothenioid%20fish%20radiation&journal=Nat.%20Commun.&volume=14&publication_year=2023&author=Bista%2CI) 
    
44.  Zapata, L. et al. Chromosome-level assembly of _Arabidopsis thaliana_ Ler reveals the extent of translocation and inversion polymorphisms. _Proc. Natl Acad. Sci. USA_ **113**, E4052–60 (2016).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BC28XhtFentrnF)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=27354520)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC4948326)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Chromosome-level%20assembly%20of%20Arabidopsis%20thaliana%20Ler%20reveals%20the%20extent%20of%20translocation%20and%20inversion%20polymorphisms&journal=Proc.%20Natl%20Acad.%20Sci.%20USA&volume=113&pages=E4052-60&publication_year=2016&author=Zapata%2CL) 
    
45.  Fransz, P. et al. Molecular, genetic and evolutionary analysis of a paracentric inversion in _Arabidopsis thaliana_. _Plant J._ **88**, 159–178 (2016).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BC28XhsFSjt7jI)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=27436134)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC5113708)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Molecular%2C%20genetic%20and%20evolutionary%20analysis%20of%20a%20paracentric%20inversion%20in%20Arabidopsis%20thaliana&journal=Plant%20J.&volume=88&pages=159-178&publication_year=2016&author=Fransz%2CP) 
    
46.  Igolkina, A. A., Bezlepsky, A. D. & Nordborg, M. Pannagram: unbiased pangenome alignment and the mobilome calling. Preprint at _bioRxiv_ [https://doi.org/10.1101/2025.02.07.637071](https://doi.org/10.1101/2025.02.07.637071) (2025).
    
47.  Puchta, H. The repair of double-strand breaks in plants: mechanisms and consequences for genome evolution. _J. Exp. Bot._ **56**, 1–14 (2005).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BD2MXkt1Wlsg%3D%3D)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=15557293)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=The%20repair%20of%20double-strand%20breaks%20in%20plants%3A%20mechanisms%20and%20consequences%20for%20genome%20evolution&journal=J.%20Exp.%20Bot.&volume=56&pages=1-14&publication_year=2005&author=Puchta%2CH) 
    
48.  Jaegle, B. et al. Extensive sequence duplication in Arabidopsis revealed by pseudo-heterozygosity. _Genome Biol._ **24**, 44 (2023).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BB3sXlsFSlsLY%3D)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=36895055)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC9999624)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Extensive%20sequence%20duplication%20in%20Arabidopsis%20revealed%20by%20pseudo-heterozygosity&journal=Genome%20Biol.&volume=24&publication_year=2023&author=Jaegle%2CB) 
    
49.  Borredá, C., Leduque, B., Colot, V. & Quadrana, L. Transposable element products, functions, and regulatory networks in _Arabidopsis_. Preprint at _bioRxiv_ [https://doi.org/10.1101/2024.04.02.587720](https://doi.org/10.1101/2024.04.02.587720) (2024).
    
50.  Sierra, P. & Durbin, R. Identification of transposable element families from pangenome polymorphisms. _Mob. DNA_ **15**, 13 (2024).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BB2cXhsFSiu77F)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=38926873)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC11202377)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Identification%20of%20transposable%20element%20families%20from%20pangenome%20polymorphisms&journal=Mob.%20DNA&volume=15&publication_year=2024&author=Sierra%2CP&author=Durbin%2CR) 
    
51.  Saidi, S., Blaison, M., del Pilar Rodríguez-Ordóñez, M., Confais, J. & Quesneville, H. panREPET: a reference-free pipeline for detecting shared Transposable Elements from pan-genomes to retrace their dynamics in a species. Preprint at _bioRxiv_ [https://doi.org/10.1101/2024.06.17.598857](https://doi.org/10.1101/2024.06.17.598857) (2025).
    
52.  Groza, C., Chen, X., Wheeler, T. J., Bourque, G. & Goubert, C. A unified framework to analyze transposable element insertion polymorphisms using graph genomes. _Nat. Commun._ **15**, 8915 (2024).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BB2cXit1OrtLbO)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=39414821)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC11484939)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=A%20unified%20framework%20to%20analyze%20transposable%20element%20insertion%20polymorphisms%20using%20graph%20genomes&journal=Nat.%20Commun.&volume=15&publication_year=2024&author=Groza%2CC&author=Chen%2CX&author=Wheeler%2CTJ&author=Bourque%2CG&author=Goubert%2CC) 
    
53.  Kawakatsu, T. et al. Epigenomic diversity in a global collection of _Arabidopsis thaliana_ accessions. _Cell_ **166**, 492–505 (2016).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BC28XhtFynu7bO)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=27419873)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC5172462)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Epigenomic%20diversity%20in%20a%20global%20collection%20of%20Arabidopsis%20thaliana%20accessions&journal=Cell&volume=166&pages=492-505&publication_year=2016&author=Kawakatsu%2CT) 
    
54.  Kornienko, A. E., Nizhynska, V., Molla Morales, A., Pisupati, R. & Nordborg, M. Population-level annotation of lncRNAs in _Arabidopsis_ reveals extensive expression variation associated with transposable element-like silencing. _Plant Cell_ **36**, 85–111 (2023).
    
    [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=37683092)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC10734619)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Population-level%20annotation%20of%20lncRNAs%20in%20Arabidopsis%20reveals%20extensive%20expression%20variation%20associated%20with%20transposable%20element-like%20silencing&journal=Plant%20Cell&volume=36&pages=85-111&publication_year=2023&author=Kornienko%2CAE&author=Nizhynska%2CV&author=Molla%20Morales%2CA&author=Pisupati%2CR&author=Nordborg%2CM) 
    
55.  Pachamuthu, K. & Borges, F. Epigenetic control of transposons during plant reproduction: from meiosis to hybrid seeds. _Curr. Opin. Plant Biol._ **75**, 102419 (2023).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BB3sXhsFWgsL3K)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=37480640)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Epigenetic%20control%20of%20transposons%20during%20plant%20reproduction%3A%20from%20meiosis%20to%20hybrid%20seeds&journal=Curr.%20Opin.%20Plant%20Biol.&volume=75&publication_year=2023&author=Pachamuthu%2CK&author=Borges%2CF) 
    
56.  Tettelin, H. et al. Genome analysis of multiple pathogenic isolates of _Streptococcus agalactiae_: implications for the microbial ‘pan-genome’. _Proc. Natl Acad. Sci. USA_ **102**, 13950–13955 (2005).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BD2MXhtVOqsbjL)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=16172379)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC1216834)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Genome%20analysis%20of%20multiple%20pathogenic%20isolates%20of%20Streptococcus%20agalactiae%3A%20implications%20for%20the%20microbial%20%E2%80%98pan-genome%E2%80%99&journal=Proc.%20Natl%20Acad.%20Sci.%20USA&volume=102&pages=13950-13955&publication_year=2005&author=Tettelin%2CH) 
    
57.  Balding, D., Moltke, I. & Marioni, J. (eds.) _Handbook of Statistical Genomics_, Vol. 1, 145–175 (Wiley, 2019).
    
58.  Schreiber, M., Jayakodi, M., Stein, N. & Mascher, M. Plant pangenomes for crop improvement, biodiversity and evolution. _Nat. Rev. Genet._ **25**, 563–577 (2024).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BB2cXktVyjsLo%3D)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=38378816)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC7616794)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Plant%20pangenomes%20for%20crop%20improvement%2C%20biodiversity%20and%20evolution&journal=Nat.%20Rev.%20Genet.&volume=25&pages=563-577&publication_year=2024&author=Schreiber%2CM&author=Jayakodi%2CM&author=Stein%2CN&author=Mascher%2CM) 
    
59.  Cork, J. M. & Purugganan, M. D. High-diversity genes in the _Arabidopsis_ genome. _Genetics_ **170**, 1897–1911 (2005).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BD2MXhtFeis7%2FP)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=15911589)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC1449776)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=High-diversity%20genes%20in%20the%20Arabidopsis%20genome&journal=Genetics&volume=170&pages=1897-1911&publication_year=2005&author=Cork%2CJM&author=Purugganan%2CMD) 
    
60.  Morgante, M. et al. Gene duplication and exon shuffling by helitron-like transposons generate intraspecies diversity in maize. _Nat. Genet._ **37**, 997–1002 (2005).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BD2MXpsFWisLo%3D)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=16056225)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Gene%20duplication%20and%20exon%20shuffling%20by%20helitron-like%20transposons%20generate%20intraspecies%20diversity%20in%20maize&journal=Nat.%20Genet.&volume=37&pages=997-1002&publication_year=2005&author=Morgante%2CM) 
    
61.  Marques-Bonet, T., Ryder, O. A. & Eichler, E. E. Sequencing primate genomes: what have we learned? _Annu. Rev. Genomics Hum. Genet._ **10**, 355–386 (2009).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BD1MXht12qsrjO)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=19630567)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC6662594)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Sequencing%20primate%20genomes%3A%20what%20have%20we%20learned%3F&journal=Annu.%20Rev.%20Genomics%20Hum.%20Genet.&volume=10&pages=355-386&publication_year=2009&author=Marques-Bonet%2CT&author=Ryder%2COA&author=Eichler%2CEE) 
    
62.  Stuart, T. et al. Population scale mapping of transposable element diversity reveals links to gene regulation and epigenomic variation. _eLife_ **5**, e20777 (2016).
    
    [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=27911260)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC5167521)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Population%20scale%20mapping%20of%20transposable%20element%20diversity%20reveals%20links%20to%20gene%20regulation%20and%20epigenomic%20variation&journal=eLife&volume=5&publication_year=2016&author=Stuart%2CT) 
    
63.  McInerney, J. O., McNally, A. & O’Connell, M. J. Why prokaryotes have pangenomes. _Nat. Microbiol._ **2**, 17040 (2017).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BC2sXlsVCiurw%3D)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=28350002)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Why%20prokaryotes%20have%20pangenomes&journal=Nat.%20Microbiol.&volume=2&publication_year=2017&author=McInerney%2CJO&author=McNally%2CA&author=O%E2%80%99Connell%2CMJ) 
    
64.  Ranade, K. et al. High-throughput genotyping with single nucleotide polymorphisms. _Genome Res._ **11**, 1262–1268 (2001).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BD3MXltFaitbs%3D)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=11435409)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC311112)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=High-throughput%20genotyping%20with%20single%20nucleotide%20polymorphisms&journal=Genome%20Res.&volume=11&pages=1262-1268&publication_year=2001&author=Ranade%2CK) 
    
65.  Osmond, M. M. & Coop, G. Estimating dispersal rates and locating genetic ancestors with genome-wide genealogies. _eLife_ **13**, e72177 (2024).
    
    [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=39589398)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC11658769)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Estimating%20dispersal%20rates%20and%20locating%20genetic%20ancestors%20with%20genome-wide%20genealogies&journal=eLife&volume=13&publication_year=2024&author=Osmond%2CMM&author=Coop%2CG) 
    
66.  Chakravarti, A. Population genetics—making sense out of sequence. _Nat. Genet._ **21**, 56–60 (1999).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DyaK1MXltlWhuw%3D%3D)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=9915503)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Population%20genetics%E2%80%94making%20sense%20out%20of%20sequence&journal=Nat.%20Genet.&volume=21&pages=56-60&publication_year=1999&author=Chakravarti%2CA) 
    
67.  Lewanski, A. L., Grundler, M. C. & Bradburd, G. S. The era of the ARG: an introduction to ancestral recombination graphs and their significance in empirical evolutionary genomics. _PLoS Genet._ **20**, e1011110 (2024).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BB2cXitVWgsLY%3D)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=38236805)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC10796009)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=The%20era%20of%20the%20ARG%3A%20an%20introduction%20to%20ancestral%20recombination%20graphs%20and%20their%20significance%20in%20empirical%20evolutionary%20genomics&journal=PLoS%20Genet.&volume=20&publication_year=2024&author=Lewanski%2CAL&author=Grundler%2CMC&author=Bradburd%2CGS) 
    
68.  Nielsen, R., Vaughn, A. H. & Deng, Y. Inference and applications of ancestral recombination graphs. _Nat. Rev. Genet._ **26**, 47–58 (2024).
    
    [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=39349760)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Inference%20and%20applications%20of%20ancestral%20recombination%20graphs&journal=Nat.%20Rev.%20Genet.&volume=26&pages=47-58&publication_year=2024&author=Nielsen%2CR&author=Vaughn%2CAH&author=Deng%2CY) 
    
69.  Novák, A., Miklós, I., Lyngsø, R. & Hein, J. StatAlign: an extendable software package for joint Bayesian estimation of alignments and evolutionary trees. _Bioinformatics_ **24**, 2403–2404 (2008).
    
    [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=18753153)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=StatAlign%3A%20an%20extendable%20software%20package%20for%20joint%20Bayesian%20estimation%20of%20alignments%20and%20evolutionary%20trees&journal=Bioinformatics&volume=24&pages=2403-2404&publication_year=2008&author=Nov%C3%A1k%2CA&author=Mikl%C3%B3s%2CI&author=Lyngs%C3%B8%2CR&author=Hein%2CJ) 
    
70.  Chatzou, M. et al. Multiple sequence alignment modeling: methods and applications. _Brief. Bioinform._ **17**, 1009–1023 (2016).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BC1cXlsVSqsLY%3D)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=26615024)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Multiple%20sequence%20alignment%20modeling%3A%20methods%20and%20applications&journal=Brief.%20Bioinform.&volume=17&pages=1009-1023&publication_year=2016&author=Chatzou%2CM) 
    
71.  Katoh, K. (ed.) in _Multiple Sequence Alignment: Methods and Protocols_ 17–37 (Springer, 2021).
    
72.  Redelings, B. D. BAli-Phy version 3: model-based co-estimation of alignment and phylogeny. _Bioinformatics_ **37**, 3032–3034 (2021).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BB38Xit1Cru7w%3D)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=33677478)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=BAli-Phy%20version%203%3A%20model-based%20co-estimation%20of%20alignment%20and%20phylogeny&journal=Bioinformatics&volume=37&pages=3032-3034&publication_year=2021&author=Redelings%2CBD) 
    
73.  Kille, B., Balaji, A., Sedlazeck, F. J., Nute, M. & Treangen, T. J. Multiple genome alignment in the telomere-to-telomere assembly era. _Genome Biol._ **23**, 182 (2022).
    
    [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=36038949)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC9421119)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Multiple%20genome%20alignment%20in%20the%20telomere-to-telomere%20assembly%20era&journal=Genome%20Biol.&volume=23&publication_year=2022&author=Kille%2CB&author=Balaji%2CA&author=Sedlazeck%2CFJ&author=Nute%2CM&author=Treangen%2CTJ) 
    
74.  Song, B., Buckler, E. S. & Stitzer, M. C. New whole-genome alignment tools are needed for tapping into plant diversity. _Trends Plant. Sci._ **29**, 355–369 (2023).
    
    [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=37749022)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=New%20whole-genome%20alignment%20tools%20are%20needed%20for%20tapping%20into%20plant%20diversity&journal=Trends%20Plant.%20Sci.&volume=29&pages=355-369&publication_year=2023&author=Song%2CB&author=Buckler%2CES&author=Stitzer%2CMC) 
    
75.  Rabanal, F. A. et al. Pushing the limits of HiFi assemblies reveals centromere diversity between two _Arabidopsis thaliana_ genomes. _Nucleic Acids Res._ **50**, 12309–12327 (2022).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BB3sXptlKjtro%3D)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=36453992)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC9757041)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Pushing%20the%20limits%20of%20HiFi%20assemblies%20reveals%20centromere%20diversity%20between%20two%20Arabidopsis%20thaliana%20genomes&journal=Nucleic%20Acids%20Res.&volume=50&pages=12309-12327&publication_year=2022&author=Rabanal%2CFA) 
    
76.  Ou, S. et al. Effect of sequence depth and length in long-read assembly of the maize inbred NC358. _Nat. Commun._ **11**, 2288 (2020).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BB3cXptVertLY%3D)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=32385271)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC7211024)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Effect%20of%20sequence%20depth%20and%20length%20in%20long-read%20assembly%20of%20the%20maize%20inbred%20NC358&journal=Nat.%20Commun.&volume=11&publication_year=2020&author=Ou%2CS) 
    
77.  Koren, S. et al. Canu: scalable and accurate long-read assembly via adaptive _k_\-mer weighting and repeat separation. _Genome Res._ **27**, 722–736 (2017).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BC2sXhtFyjsrvI)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=28298431)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC5411767)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Canu%3A%20scalable%20and%20accurate%20long-read%20assembly%20via%20adaptive%20k-mer%20weighting%20and%20repeat%20separation&journal=Genome%20Res.&volume=27&pages=722-736&publication_year=2017&author=Koren%2CS) 
    
78.  Walker, B. J. et al. Pilon: an integrated tool for comprehensive microbial variant detection and genome assembly improvement. _PLoS ONE_ **9**, e112963 (2014).
    
    [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=25409509)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC4237348)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Pilon%3A%20an%20integrated%20tool%20for%20comprehensive%20microbial%20variant%20detection%20and%20genome%20assembly%20improvement&journal=PLoS%20ONE&volume=9&publication_year=2014&author=Walker%2CBJ) 
    
79.  Alonge, M. et al. Automated assembly scaffolding using RagTag elevates a new tomato system for high-throughput genome editing. _Genome Biol._ **23**, 258 (2022).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BB38XjtF2kt7rM)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=36522651)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC9753292)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Automated%20assembly%20scaffolding%20using%20RagTag%20elevates%20a%20new%20tomato%20system%20for%20high-throughput%20genome%20editing&journal=Genome%20Biol.&volume=23&publication_year=2022&author=Alonge%2CM) 
    
80.  Vollger, M. R. et al. Long-read sequence and assembly of segmental duplications. _Nat. Methods_ **16**, 88–94 (2019).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BC1cXisFCitLvK)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=30559433)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Long-read%20sequence%20and%20assembly%20of%20segmental%20duplications&journal=Nat.%20Methods&volume=16&pages=88-94&publication_year=2019&author=Vollger%2CMR) 
    
81.  Maheshwari, S., Ishii, T., Brown, C. T., Houben, A. & Comai, L. Centromere location in _Arabidopsis_ is unaltered by extreme divergence in CENH3 protein sequence. _Genome Res._ **27**, 471–478 (2017).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BC2sXhtVahsrfJ)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=28223399)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC5340974)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Centromere%20location%20in%20Arabidopsis%20is%20unaltered%20by%20extreme%20divergence%20in%20CENH3%20protein%20sequence&journal=Genome%20Res.&volume=27&pages=471-478&publication_year=2017&author=Maheshwari%2CS&author=Ishii%2CT&author=Brown%2CCT&author=Houben%2CA&author=Comai%2CL) 
    
82.  Simon, L. et al. Genetic and epigenetic variation in 5S ribosomal RNA genes reveals genome dynamics in _Arabidopsis thaliana_. _Nucleic Acids Res._ **46**, 3019–3033 (2018).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BC1cXitlGjurjJ)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=29518237)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC5887818)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Genetic%20and%20epigenetic%20variation%20in%205S%20ribosomal%20RNA%20genes%20reveals%20genome%20dynamics%20in%20Arabidopsis%20thaliana&journal=Nucleic%20Acids%20Res.&volume=46&pages=3019-3033&publication_year=2018&author=Simon%2CL) 
    
83.  Rabanal, F. A. et al. Unstable inheritance of 45S rRNA genes in _Arabidopsis thaliana_. _G3_ **7**, 1201–1209 (2017).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BC1cXhsFGku7rF)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=28188182)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC5386868)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Unstable%20inheritance%20of%2045S%20rRNA%20genes%20in%20Arabidopsis%20thaliana&journal=G3&volume=7&pages=1201-1209&publication_year=2017&author=Rabanal%2CFA) 
    
84.  Chan, P. P. & Lowe, T. M. tRNAscan-SE: searching for tRNA genes in genomic sequences. _Methods Mol. Biol._ **1962**, 1–14 (2019).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BB3cXhtFGrt78%3D)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=31020551)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC6768409)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=tRNAscan-SE%3A%20searching%20for%20tRNA%20genes%20in%20genomic%20sequences&journal=Methods%20Mol.%20Biol.&volume=1962&pages=1-14&publication_year=2019&author=Chan%2CPP&author=Lowe%2CTM) 
    
85.  Ou, S. et al. Benchmarking transposable element annotation methods for creation of a streamlined, comprehensive pipeline. _Genome Biol._ **20**, 275 (2019).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BC1MXisVSntb3O)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=31843001)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC6913007)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Benchmarking%20transposable%20element%20annotation%20methods%20for%20creation%20of%20a%20streamlined%2C%20comprehensive%20pipeline&journal=Genome%20Biol.&volume=20&publication_year=2019&author=Ou%2CS) 
    
86.  Ellinghaus, D., Kurtz, S. & Willhoeft, U. LTRharvest, an efficient and flexible software for de novo detection of LTR retrotransposons. _BMC Bioinformatics_ **9**, 18 (2008).
    
    [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=18194517)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC2253517)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=LTRharvest%2C%20an%20efficient%20and%20flexible%20software%20for%20de%20novo%20detection%20of%20LTR%20retrotransposons&journal=BMC%20Bioinformatics&volume=9&publication_year=2008&author=Ellinghaus%2CD&author=Kurtz%2CS&author=Willhoeft%2CU) 
    
87.  Ou, S. & Jiang, N. LTR\_retriever: a highly accurate and sensitive program for identification of long terminal repeat retrotransposons. _Plant Physiol._ **176**, 1410–1422 (2018).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BC1cXhs1CjtbzO)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=29233850)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=LTR_retriever%3A%20a%20highly%20accurate%20and%20sensitive%20program%20for%20identification%20of%20long%20terminal%20repeat%20retrotransposons&journal=Plant%20Physiol.&volume=176&pages=1410-1422&publication_year=2018&author=Ou%2CS&author=Jiang%2CN) 
    
88.  Xu, Z. & Wang, H. LTR\_FINDER: an efficient tool for the prediction of full-length LTR retrotransposons. _Nucleic Acids Res._ **35**, W265–W268 (2007).
    
    [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=17485477)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC1933203)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=LTR_FINDER%3A%20an%20efficient%20tool%20for%20the%20prediction%20of%20full-length%20LTR%20retrotransposons&journal=Nucleic%20Acids%20Res.&volume=35&pages=W265-W268&publication_year=2007&author=Xu%2CZ&author=Wang%2CH) 
    
89.  Ou, S. & Jiang, N. LTR\_FINDER\_parallel: parallelization of LTR\_FINDER enabling rapid identification of long terminal repeat retrotransposons. _Mob. DNA_ **10**, 48 (2019).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BC1MXisVykurjE)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=31857828)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC6909508)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=LTR_FINDER_parallel%3A%20parallelization%20of%20LTR_FINDER%20enabling%20rapid%20identification%20of%20long%20terminal%20repeat%20retrotransposons&journal=Mob.%20DNA&volume=10&publication_year=2019&author=Ou%2CS&author=Jiang%2CN) 
    
90.  Su, W., Gu, X. & Peterson, T. TIR-Learner, a new ensemble method for TIR transposable element annotation, provides evidence for abundant new transposable elements in the maize genome. _Mol. Plant_ **12**, 447–460 (2019).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BC1MXjs1GgsLo%3D)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=30802553)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=TIR-Learner%2C%20a%20new%20ensemble%20method%20for%20TIR%20transposable%20element%20annotation%2C%20provides%20evidence%20for%20abundant%20new%20transposable%20elements%20in%20the%20maize%20genome&journal=Mol.%20Plant&volume=12&pages=447-460&publication_year=2019&author=Su%2CW&author=Gu%2CX&author=Peterson%2CT) 
    
91.  Shi, J. & Liang, C. Generic repeat finder: a high-sensitivity tool for genome-wide de novo repeat detection. _Plant Physiol._ **180**, 1803–1815 (2019).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BC1MXitVCisbnF)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=31152127)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC6670090)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Generic%20repeat%20finder%3A%20a%20high-sensitivity%20tool%20for%20genome-wide%20de%20novo%20repeat%20detection&journal=Plant%20Physiol.&volume=180&pages=1803-1815&publication_year=2019&author=Shi%2CJ&author=Liang%2CC) 
    
92.  Xiong, W., He, L., Lai, J., Dooner, H. K. & Du, C. HelitronScanner uncovers a large overlooked cache of helitron transposons in many plant genomes. _Proc. Natl Acad. Sci. USA_ **111**, 10263–10268 (2014).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BC2cXhtVOitL7L)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=24982153)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC4104883)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=HelitronScanner%20uncovers%20a%20large%20overlooked%20cache%20of%20helitron%20transposons%20in%20many%20plant%20genomes&journal=Proc.%20Natl%20Acad.%20Sci.%20USA&volume=111&pages=10263-10268&publication_year=2014&author=Xiong%2CW&author=He%2CL&author=Lai%2CJ&author=Dooner%2CHK&author=Du%2CC) 
    
93.  Zhang, R.-G. et al. TEsorter: an accurate and fast method to classify LTR-retrotransposons in plant genomes. _Hortic. Res._ **9**, uhac017 (2022).
    
    [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=35184178)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC9002660)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=TEsorter%3A%20an%20accurate%20and%20fast%20method%20to%20classify%20LTR-retrotransposons%20in%20plant%20genomes&journal=Hortic.%20Res.&volume=9&publication_year=2022&author=Zhang%2CR-G) 
    
94.  Katoh, K., Misawa, K., Kuma, K.-I. & Miyata, T. MAFFT: a novel method for rapid multiple sequence alignment based on fast Fourier transform. _Nucleic Acids Res._ **30**, 3059–3066 (2002).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BD38XlslOqu7s%3D)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=12136088)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC135756)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=MAFFT%3A%20a%20novel%20method%20for%20rapid%20multiple%20sequence%20alignment%20based%20on%20fast%20Fourier%20transform&journal=Nucleic%20Acids%20Res.&volume=30&pages=3059-3066&publication_year=2002&author=Katoh%2CK&author=Misawa%2CK&author=Kuma%2CK-I&author=Miyata%2CT) 
    
95.  Garrison, E. et al. Variation graph toolkit improves read mapping by representing genetic variation in the reference. _Nat. Biotechnol._ **36**, 875–879 (2018).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BC1cXhsFChurbJ)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=30125266)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC6126949)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Variation%20graph%20toolkit%20improves%20read%20mapping%20by%20representing%20genetic%20variation%20in%20the%20reference&journal=Nat.%20Biotechnol.&volume=36&pages=875-879&publication_year=2018&author=Garrison%2CE) 
    
96.  Stanke, M., Diekhans, M., Baertsch, R. & Haussler, D. Using native and syntenically mapped cDNA alignments to improve de novo gene finding. _Bioinformatics_ **24**, 637–644 (2008).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BD1cXislKlt7o%3D)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=18218656)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Using%20native%20and%20syntenically%20mapped%20cDNA%20alignments%20to%20improve%20de%20novo%20gene%20finding&journal=Bioinformatics&volume=24&pages=637-644&publication_year=2008&author=Stanke%2CM&author=Diekhans%2CM&author=Baertsch%2CR&author=Haussler%2CD) 
    
97.  Seppey, M., Manni, M. & Zdobnov, E. M. BUSCO: assessing genome assembly and annotation completeness. _Methods Mol. Biol._ **1962**, 227–245 (2019).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BB3cXpvVCnsA%3D%3D)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=31020564)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=BUSCO%3A%20assessing%20genome%20assembly%20and%20annotation%20completeness&journal=Methods%20Mol.%20Biol.&volume=1962&pages=227-245&publication_year=2019&author=Seppey%2CM&author=Manni%2CM&author=Zdobnov%2CEM) 
    
98.  Shumate, A. & Salzberg, S. L. Liftoff: accurate mapping of gene annotations. _Bioinformatics_ **37**, 1639–1643 (2021).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BB3MXitlGgt7bE)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=33320174)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC8289374)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Liftoff%3A%20accurate%20mapping%20of%20gene%20annotations&journal=Bioinformatics&volume=37&pages=1639-1643&publication_year=2021&author=Shumate%2CA&author=Salzberg%2CSL) 
    
99.  Haas, B. J. et al. Automated eukaryotic gene structure annotation using EVidenceModeler and the program to assemble spliced alignments. _Genome Biol._ **9**, R7 (2008).
    
    [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=18190707)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC2395244)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Automated%20eukaryotic%20gene%20structure%20annotation%20using%20EVidenceModeler%20and%20the%20program%20to%20assemble%20spliced%20alignments&journal=Genome%20Biol.&volume=9&publication_year=2008&author=Haas%2CBJ) 
    
100.  Campbell, M. S. et al. MAKER-P: a tool kit for the rapid creation, management, and quality control of plant genome annotations. _Plant Physiol._ **164**, 513–524 (2014).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BC2cXks1SmsL8%3D)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=24306534)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=MAKER-P%3A%20a%20tool%20kit%20for%20the%20rapid%20creation%2C%20management%2C%20and%20quality%20control%20of%20plant%20genome%20annotations&journal=Plant%20Physiol.&volume=164&pages=513-524&publication_year=2014&author=Campbell%2CMS) 
    
101.  Trapnell, C. et al. Differential gene and transcript expression analysis of RNA-seq experiments with TopHat and Cufflinks. _Nat. Protoc._ **7**, 562–578 (2012).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BC38Xjt1Cjsrc%3D)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=22383036)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC3334321)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Differential%20gene%20and%20transcript%20expression%20analysis%20of%20RNA-seq%20experiments%20with%20TopHat%20and%20Cufflinks&journal=Nat.%20Protoc.&volume=7&pages=562-578&publication_year=2012&author=Trapnell%2CC) 
    
102.  Pertea, G. & Pertea, M. GFF utilities: GffRead and GffCompare. _F1000Res._ **9**, ISCB Comm J-304 (2020).
    
    [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=32489650)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC7222033)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=GFF%20utilities%3A%20GffRead%20and%20GffCompare&journal=F1000Res.&volume=9&publication_year=2020&author=Pertea%2CG&author=Pertea%2CM) 
    
103.  Buchfink, B., Reuter, K. & Drost, H.-G. Sensitive protein alignments at tree-of-life scale using DIAMOND. _Nat. Methods_ **18**, 366–368 (2021).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BB3MXosVCltrw%3D)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=33828273)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC8026399)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Sensitive%20protein%20alignments%20at%20tree-of-life%20scale%20using%20DIAMOND&journal=Nat.%20Methods&volume=18&pages=366-368&publication_year=2021&author=Buchfink%2CB&author=Reuter%2CK&author=Drost%2CH-G) 
    
104.  Dobin, A. et al. STAR: ultrafast universal RNA-seq aligner. _Bioinformatics_ **29**, 15–21 (2013).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BC38XhvV2gsbnF)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=23104886)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=STAR%3A%20ultrafast%20universal%20RNA-seq%20aligner&journal=Bioinformatics&volume=29&pages=15-21&publication_year=2013&author=Dobin%2CA) 
    
105.  Liao, Y., Smyth, G. K. & Shi, W. featureCounts: an efficient general purpose program for assigning sequence reads to genomic features. _Bioinformatics_ **30**, 923–930 (2014).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BC2cXltFGqu7c%3D)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=24227677)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=featureCounts%3A%20an%20efficient%20general%20purpose%20program%20for%20assigning%20sequence%20reads%20to%20genomic%20features&journal=Bioinformatics&volume=30&pages=923-930&publication_year=2014&author=Liao%2CY&author=Smyth%2CGK&author=Shi%2CW) 
    
106.  Ramírez, F. et al. deepTools2: a next generation web server for deep-sequencing data analysis. _Nucleic Acids Res._ **44**, W160–W165 (2016).
    
    [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=27079975)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC4987876)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=deepTools2%3A%20a%20next%20generation%20web%20server%20for%20deep-sequencing%20data%20analysis&journal=Nucleic%20Acids%20Res.&volume=44&pages=W160-W165&publication_year=2016&author=Ram%C3%ADrez%2CF) 
    
107.  Quinlan, A. R. & Hall, I. M. BEDTools: a flexible suite of utilities for comparing genomic features. _Bioinformatics_ **26**, 841–842 (2010).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BC3cXivFGkurc%3D)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=20110278)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC2832824)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=BEDTools%3A%20a%20flexible%20suite%20of%20utilities%20for%20comparing%20genomic%20features&journal=Bioinformatics&volume=26&pages=841-842&publication_year=2010&author=Quinlan%2CAR&author=Hall%2CIM) 
    
108.  Martin, M. Cutadapt removes adapter sequences from high-throughput sequencing reads. _EMBnet J._ **17**, 10–12 (2011).
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Cutadapt%20removes%20adapter%20sequences%20from%20high-throughput%20sequencing%20reads&journal=EMBnet%20J.&volume=17&pages=10-12&publication_year=2011&author=Martin%2CM) 
    
109.  Krueger, F. & Andrews, S. R. Bismark: a flexible aligner and methylation caller for bisulfite-seq applications. _Bioinformatics_ **27**, 1571–1572 (2011).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BC3MXmvVWqurw%3D)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=21493656)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC3102221)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Bismark%3A%20a%20flexible%20aligner%20and%20methylation%20caller%20for%20bisulfite-seq%20applications&journal=Bioinformatics&volume=27&pages=1571-1572&publication_year=2011&author=Krueger%2CF&author=Andrews%2CSR) 
    
110.  Pisupati, R., Nizhynska, V., Mollá Morales, A. & Nordborg, M. On the causes of gene-body methylation variation in _Arabidopsis thaliana_. _PLoS Genet._ **19**, e1010728 (2023).
    
    [CAS](https://www.nature.com/articles/cas-redirect/1:CAS:528:DC%2BB3sXhtVait7zI)  [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=Retrieve&db=PubMed&dopt=Abstract&list_uids=37141384)  [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC10187938)  [Google Scholar](http://scholar.google.com/scholar_lookup?&title=On%20the%20causes%20of%20gene-body%20methylation%20variation%20in%20Arabidopsis%20thaliana&journal=PLoS%20Genet.&volume=19&publication_year=2023&author=Pisupati%2CR&author=Nizhynska%2CV&author=Moll%C3%A1%20Morales%2CA&author=Nordborg%2CM) 
    
111.  Igolkina, A. et al. Gregor-Mendel-Institute/1001Gplus\_paper: v1.0.0. _Zenodo_ [https://doi.org/10.5281/zenodo.15790915](https://doi.org/10.5281/zenodo.15790915) (2025).
    
112.  Igolkina, A. iganna/pannagram: version for the 27-genomes paper (v1.1). _Zenodo_ [https://doi.org/10.5281/zenodo.15791785](https://doi.org/10.5281/zenodo.15791785) (2025).
    
113.  Wrightsman, T., Kubica, C. & Ashkenazy, H. Automated assembly pipeline for PacBio long read datasets. _Zenodo_ [https://doi.org/10.5281/zenodo.15775624](https://doi.org/10.5281/zenodo.15775624) (2025).
    

[Download references](https://citation-needed.springer.com/v2/references/10.1038/s41588-025-02293-0?format=refman&flavour=references)

Acknowledgements
----------------

We thank Z. Bao, A. Duque and G. Ofir for discussion and comments on the paper. E. Grigoreva supplied the polymorphism data for Fig. [2c](https://www.nature.com/articles/s41588-025-02293-0#Fig2). M.N. wrote much of this paper while on a sabbatical in M. Przeworski’s lab at Columbia University and thanks all members of her lab, as well as the labs of G. Sella and P. Andolfatto, for their hospitality and feedback. This work was funded by the Deutsche Forschungsgemeinschaft (DFG), the Austrian Science Fund (FWF) and the Biotechnology and Biological Sciences Research Council (BBSRC) through ERA-CAPS Project 1001GenomesPlus (BBSRC BB/S004661/1 to P.K., D.W. and M.N.), the Austrian Academy of Sciences (to M.N.), the Max Planck Society (to D.W.) and the European Union’s Framework Programme for Research and Innovation Horizon 2020 (2014–2020) under the Marie Curie Skłodowska Grant Agreement 847548 (to H.-J.L.), as well as ERC Advanced Grant EPICLINES (to M.N.).

Funding
-------

Open access funding provided by Max Planck Society.

Author information
------------------

Author notes

1.  These authors contributed equally: Anna A. Igolkina, Sebastian Vorbrugg, Fernando A. Rabanal, Hai-Jun Liu, Haim Ashkenazy, Aleksandra E. Kornienko.
    

### Authors and Affiliations

1.  Gregor Mendel Institute, Austrian Academy of Sciences, Vienna, Austria
    
    Anna A. Igolkina, Hai-Jun Liu, Aleksandra E. Kornienko, Almudena Mollá Morales, Benjamin Jaegle, Viktoria Nizhynska, Ilka Reichardt & Magnus Nordborg
    
2.  Max Planck Institute for Biology Tübingen, Tübingen, Germany
    
    Sebastian Vorbrugg, Fernando A. Rabanal, Haim Ashkenazy, Joffrey Fitz, Max Collenberg, Christian Kubica, Travis Wrightsman, Ilja Bezrukov, Christa Lanz, Felix Bemm & Detlef Weigel
    
3.  Royal Botanic Gardens Kew, London, UK
    
    Vitaly Voloshin & Paul Kersey
    
4.  All-Russian Research Institute of Agricultural Microbiology, Saint Petersburg, Russia
    
    Alexander D. Bezlepsky
    
5.  Corteva Agriscience, Johnston, IA, USA
    
    Victor Llaca
    
6.  Max Planck Institute for Plant Breeding Research, Cologne, Germany
    
    Pádraic J. Flood & Angela Hancock
    
7.  Addis Ababa University, Addis Ababa, Ethiopia
    
    Sileshi Nemomissa
    
8.  Institute of Botany, Chinese Academy of Sciences, Beijing, China
    
    Ya-Long Guo
    
9.  Institute for Bioinformatics and Medical Informatics, University of Tübingen, Tübingen, Germany
    
    Detlef Weigel
    

Authors

1.  Anna A. Igolkina
    
    [View author publications](https://www.nature.com/search?author=Anna%20A.%20Igolkina)
    
    Search author on:[PubMed](https://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=search&term=Anna%20A.%20Igolkina) [Google Scholar](https://scholar.google.co.uk/scholar?as_q=&num=10&btnG=Search+Scholar&as_epq=&as_oq=&as_eq=&as_occt=any&as_sauthors=%22Anna%20A.%20Igolkina%22&as_publication=&as_ylo=&as_yhi=&as_allsubj=all&hl=en)
    
2.  Sebastian Vorbrugg
    
    [View author publications](https://www.nature.com/search?author=Sebastian%20Vorbrugg)
    
    Search author on:[PubMed](https://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=search&term=Sebastian%20Vorbrugg) [Google Scholar](https://scholar.google.co.uk/scholar?as_q=&num=10&btnG=Search+Scholar&as_epq=&as_oq=&as_eq=&as_occt=any&as_sauthors=%22Sebastian%20Vorbrugg%22&as_publication=&as_ylo=&as_yhi=&as_allsubj=all&hl=en)
    
3.  Fernando A. Rabanal
    
    [View author publications](https://www.nature.com/search?author=Fernando%20A.%20Rabanal)
    
    Search author on:[PubMed](https://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=search&term=Fernando%20A.%20Rabanal) [Google Scholar](https://scholar.google.co.uk/scholar?as_q=&num=10&btnG=Search+Scholar&as_epq=&as_oq=&as_eq=&as_occt=any&as_sauthors=%22Fernando%20A.%20Rabanal%22&as_publication=&as_ylo=&as_yhi=&as_allsubj=all&hl=en)
    
4.  Hai-Jun Liu
    
    [View author publications](https://www.nature.com/search?author=Hai-Jun%20Liu)
    
    Search author on:[PubMed](https://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=search&term=Hai-Jun%20Liu) [Google Scholar](https://scholar.google.co.uk/scholar?as_q=&num=10&btnG=Search+Scholar&as_epq=&as_oq=&as_eq=&as_occt=any&as_sauthors=%22Hai-Jun%20Liu%22&as_publication=&as_ylo=&as_yhi=&as_allsubj=all&hl=en)
    
5.  Haim Ashkenazy
    
    [View author publications](https://www.nature.com/search?author=Haim%20Ashkenazy)
    
    Search author on:[PubMed](https://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=search&term=Haim%20Ashkenazy) [Google Scholar](https://scholar.google.co.uk/scholar?as_q=&num=10&btnG=Search+Scholar&as_epq=&as_oq=&as_eq=&as_occt=any&as_sauthors=%22Haim%20Ashkenazy%22&as_publication=&as_ylo=&as_yhi=&as_allsubj=all&hl=en)
    
6.  Aleksandra E. Kornienko
    
    [View author publications](https://www.nature.com/search?author=Aleksandra%20E.%20Kornienko)
    
    Search author on:[PubMed](https://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=search&term=Aleksandra%20E.%20Kornienko) [Google Scholar](https://scholar.google.co.uk/scholar?as_q=&num=10&btnG=Search+Scholar&as_epq=&as_oq=&as_eq=&as_occt=any&as_sauthors=%22Aleksandra%20E.%20Kornienko%22&as_publication=&as_ylo=&as_yhi=&as_allsubj=all&hl=en)
    
7.  Joffrey Fitz
    
    [View author publications](https://www.nature.com/search?author=Joffrey%20Fitz)
    
    Search author on:[PubMed](https://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=search&term=Joffrey%20Fitz) [Google Scholar](https://scholar.google.co.uk/scholar?as_q=&num=10&btnG=Search+Scholar&as_epq=&as_oq=&as_eq=&as_occt=any&as_sauthors=%22Joffrey%20Fitz%22&as_publication=&as_ylo=&as_yhi=&as_allsubj=all&hl=en)
    
8.  Max Collenberg
    
    [View author publications](https://www.nature.com/search?author=Max%20Collenberg)
    
    Search author on:[PubMed](https://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=search&term=Max%20Collenberg) [Google Scholar](https://scholar.google.co.uk/scholar?as_q=&num=10&btnG=Search+Scholar&as_epq=&as_oq=&as_eq=&as_occt=any&as_sauthors=%22Max%20Collenberg%22&as_publication=&as_ylo=&as_yhi=&as_allsubj=all&hl=en)
    
9.  Christian Kubica
    
    [View author publications](https://www.nature.com/search?author=Christian%20Kubica)
    
    Search author on:[PubMed](https://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=search&term=Christian%20Kubica) [Google Scholar](https://scholar.google.co.uk/scholar?as_q=&num=10&btnG=Search+Scholar&as_epq=&as_oq=&as_eq=&as_occt=any&as_sauthors=%22Christian%20Kubica%22&as_publication=&as_ylo=&as_yhi=&as_allsubj=all&hl=en)
    
10.  Almudena Mollá Morales
    
    [View author publications](https://www.nature.com/search?author=Almudena%20Moll%C3%A1%20Morales)
    
    Search author on:[PubMed](https://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=search&term=Almudena%20Moll%C3%A1%20Morales) [Google Scholar](https://scholar.google.co.uk/scholar?as_q=&num=10&btnG=Search+Scholar&as_epq=&as_oq=&as_eq=&as_occt=any&as_sauthors=%22Almudena%20Moll%C3%A1%20Morales%22&as_publication=&as_ylo=&as_yhi=&as_allsubj=all&hl=en)
    
11.  Benjamin Jaegle
    
    [View author publications](https://www.nature.com/search?author=Benjamin%20Jaegle)
    
    Search author on:[PubMed](https://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=search&term=Benjamin%20Jaegle) [Google Scholar](https://scholar.google.co.uk/scholar?as_q=&num=10&btnG=Search+Scholar&as_epq=&as_oq=&as_eq=&as_occt=any&as_sauthors=%22Benjamin%20Jaegle%22&as_publication=&as_ylo=&as_yhi=&as_allsubj=all&hl=en)
    
12.  Travis Wrightsman
    
    [View author publications](https://www.nature.com/search?author=Travis%20Wrightsman)
    
    Search author on:[PubMed](https://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=search&term=Travis%20Wrightsman) [Google Scholar](https://scholar.google.co.uk/scholar?as_q=&num=10&btnG=Search+Scholar&as_epq=&as_oq=&as_eq=&as_occt=any&as_sauthors=%22Travis%20Wrightsman%22&as_publication=&as_ylo=&as_yhi=&as_allsubj=all&hl=en)
    
13.  Vitaly Voloshin
    
    [View author publications](https://www.nature.com/search?author=Vitaly%20Voloshin)
    
    Search author on:[PubMed](https://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=search&term=Vitaly%20Voloshin) [Google Scholar](https://scholar.google.co.uk/scholar?as_q=&num=10&btnG=Search+Scholar&as_epq=&as_oq=&as_eq=&as_occt=any&as_sauthors=%22Vitaly%20Voloshin%22&as_publication=&as_ylo=&as_yhi=&as_allsubj=all&hl=en)
    
14.  Alexander D. Bezlepsky
    
    [View author publications](https://www.nature.com/search?author=Alexander%20D.%20Bezlepsky)
    
    Search author on:[PubMed](https://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=search&term=Alexander%20D.%20Bezlepsky) [Google Scholar](https://scholar.google.co.uk/scholar?as_q=&num=10&btnG=Search+Scholar&as_epq=&as_oq=&as_eq=&as_occt=any&as_sauthors=%22Alexander%20D.%20Bezlepsky%22&as_publication=&as_ylo=&as_yhi=&as_allsubj=all&hl=en)
    
15.  Victor Llaca
    
    [View author publications](https://www.nature.com/search?author=Victor%20Llaca)
    
    Search author on:[PubMed](https://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=search&term=Victor%20Llaca) [Google Scholar](https://scholar.google.co.uk/scholar?as_q=&num=10&btnG=Search+Scholar&as_epq=&as_oq=&as_eq=&as_occt=any&as_sauthors=%22Victor%20Llaca%22&as_publication=&as_ylo=&as_yhi=&as_allsubj=all&hl=en)
    
16.  Viktoria Nizhynska
    
    [View author publications](https://www.nature.com/search?author=Viktoria%20Nizhynska)
    
    Search author on:[PubMed](https://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=search&term=Viktoria%20Nizhynska) [Google Scholar](https://scholar.google.co.uk/scholar?as_q=&num=10&btnG=Search+Scholar&as_epq=&as_oq=&as_eq=&as_occt=any&as_sauthors=%22Viktoria%20Nizhynska%22&as_publication=&as_ylo=&as_yhi=&as_allsubj=all&hl=en)
    
17.  Ilka Reichardt
    
    [View author publications](https://www.nature.com/search?author=Ilka%20Reichardt)
    
    Search author on:[PubMed](https://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=search&term=Ilka%20Reichardt) [Google Scholar](https://scholar.google.co.uk/scholar?as_q=&num=10&btnG=Search+Scholar&as_epq=&as_oq=&as_eq=&as_occt=any&as_sauthors=%22Ilka%20Reichardt%22&as_publication=&as_ylo=&as_yhi=&as_allsubj=all&hl=en)
    
18.  Ilja Bezrukov
    
    [View author publications](https://www.nature.com/search?author=Ilja%20Bezrukov)
    
    Search author on:[PubMed](https://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=search&term=Ilja%20Bezrukov) [Google Scholar](https://scholar.google.co.uk/scholar?as_q=&num=10&btnG=Search+Scholar&as_epq=&as_oq=&as_eq=&as_occt=any&as_sauthors=%22Ilja%20Bezrukov%22&as_publication=&as_ylo=&as_yhi=&as_allsubj=all&hl=en)
    
19.  Christa Lanz
    
    [View author publications](https://www.nature.com/search?author=Christa%20Lanz)
    
    Search author on:[PubMed](https://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=search&term=Christa%20Lanz) [Google Scholar](https://scholar.google.co.uk/scholar?as_q=&num=10&btnG=Search+Scholar&as_epq=&as_oq=&as_eq=&as_occt=any&as_sauthors=%22Christa%20Lanz%22&as_publication=&as_ylo=&as_yhi=&as_allsubj=all&hl=en)
    
20.  Felix Bemm
    
    [View author publications](https://www.nature.com/search?author=Felix%20Bemm)
    
    Search author on:[PubMed](https://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=search&term=Felix%20Bemm) [Google Scholar](https://scholar.google.co.uk/scholar?as_q=&num=10&btnG=Search+Scholar&as_epq=&as_oq=&as_eq=&as_occt=any&as_sauthors=%22Felix%20Bemm%22&as_publication=&as_ylo=&as_yhi=&as_allsubj=all&hl=en)
    
21.  Pádraic J. Flood
    
    [View author publications](https://www.nature.com/search?author=P%C3%A1draic%20J.%20Flood)
    
    Search author on:[PubMed](https://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=search&term=P%C3%A1draic%20J.%20Flood) [Google Scholar](https://scholar.google.co.uk/scholar?as_q=&num=10&btnG=Search+Scholar&as_epq=&as_oq=&as_eq=&as_occt=any&as_sauthors=%22P%C3%A1draic%20J.%20Flood%22&as_publication=&as_ylo=&as_yhi=&as_allsubj=all&hl=en)
    
22.  Sileshi Nemomissa
    
    [View author publications](https://www.nature.com/search?author=Sileshi%20Nemomissa)
    
    Search author on:[PubMed](https://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=search&term=Sileshi%20Nemomissa) [Google Scholar](https://scholar.google.co.uk/scholar?as_q=&num=10&btnG=Search+Scholar&as_epq=&as_oq=&as_eq=&as_occt=any&as_sauthors=%22Sileshi%20Nemomissa%22&as_publication=&as_ylo=&as_yhi=&as_allsubj=all&hl=en)
    
23.  Angela Hancock
    
    [View author publications](https://www.nature.com/search?author=Angela%20Hancock)
    
    Search author on:[PubMed](https://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=search&term=Angela%20Hancock) [Google Scholar](https://scholar.google.co.uk/scholar?as_q=&num=10&btnG=Search+Scholar&as_epq=&as_oq=&as_eq=&as_occt=any&as_sauthors=%22Angela%20Hancock%22&as_publication=&as_ylo=&as_yhi=&as_allsubj=all&hl=en)
    
24.  Ya-Long Guo
    
    [View author publications](https://www.nature.com/search?author=Ya-Long%20Guo)
    
    Search author on:[PubMed](https://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=search&term=Ya-Long%20Guo) [Google Scholar](https://scholar.google.co.uk/scholar?as_q=&num=10&btnG=Search+Scholar&as_epq=&as_oq=&as_eq=&as_occt=any&as_sauthors=%22Ya-Long%20Guo%22&as_publication=&as_ylo=&as_yhi=&as_allsubj=all&hl=en)
    
25.  Paul Kersey
    
    [View author publications](https://www.nature.com/search?author=Paul%20Kersey)
    
    Search author on:[PubMed](https://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=search&term=Paul%20Kersey) [Google Scholar](https://scholar.google.co.uk/scholar?as_q=&num=10&btnG=Search+Scholar&as_epq=&as_oq=&as_eq=&as_occt=any&as_sauthors=%22Paul%20Kersey%22&as_publication=&as_ylo=&as_yhi=&as_allsubj=all&hl=en)
    
26.  Detlef Weigel
    
    [View author publications](https://www.nature.com/search?author=Detlef%20Weigel)
    
    Search author on:[PubMed](https://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=search&term=Detlef%20Weigel) [Google Scholar](https://scholar.google.co.uk/scholar?as_q=&num=10&btnG=Search+Scholar&as_epq=&as_oq=&as_eq=&as_occt=any&as_sauthors=%22Detlef%20Weigel%22&as_publication=&as_ylo=&as_yhi=&as_allsubj=all&hl=en)
    
27.  Magnus Nordborg
    
    [View author publications](https://www.nature.com/search?author=Magnus%20Nordborg)
    
    Search author on:[PubMed](https://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=search&term=Magnus%20Nordborg) [Google Scholar](https://scholar.google.co.uk/scholar?as_q=&num=10&btnG=Search+Scholar&as_epq=&as_oq=&as_eq=&as_occt=any&as_sauthors=%22Magnus%20Nordborg%22&as_publication=&as_ylo=&as_yhi=&as_allsubj=all&hl=en)
    

### Contributions

P.K., D.W. and M.N. conceived and supervised the project. P.J.F., S.N., A.H. and Y.-L.G. contributed materials. F.A.R., A.E.K., M.C., A.M.M., V.L., V.N., I.R., C.L. and F.B. generated data. F.A.R., H.A., B.J. and T.W. assembled the genomes. A.A.I., H.A., M.C. and C.K. annotated the genomes. H.-J.L. and A.E.K. analyzed expression, epigenetics and short-read mapping bias. A.A.I. and S.V. performed the SV analysis. A.A.I. analyzed the mobile-ome. A.A.I. and A.D.B. analyzed the pangenome alignment. A.A.I., H.A., A.E.K. and V.V. analyzed the gene-ome. J.F. developed the genome browser. I.B. provided computational support. A.A.I., S.V., F.A.R., H.-J.L., H.A., A.E.K., D.W. and M.N. wrote the paper.

### Corresponding authors

Correspondence to [Detlef Weigel](mailto:weigel@tue.mpg.de) or [Magnus Nordborg](mailto:magnus.nordborg@gmi.oeaw.ac.at).

Ethics declarations
-------------------

### Competing interests

D.W. holds equity in Computomics, which advises plant breeders. D.W. also consults for KWS SE, a plant breeder and seed producer with activities throughout the world. J.F. is an employee of Tropic TI, Lda. The other authors declare no competing interests.

Peer review
-----------

### Peer review information

_Nature Genetics_ thanks Marie Mirouze and the other, anonymous, reviewer(s) for their contribution to the peer review of this work. [Peer reviewer reports](https://www.nature.com/articles/s41588-025-02293-0#MOESM3) are available.

Additional information
----------------------

**Publisher’s note** Springer Nature remains neutral with regard to jurisdictional claims in published maps and institutional affiliations.

Extended data
-------------

### [Extended Data Fig. 1 The pattern of polymorphism on chromosomes 2–5.](https://www.nature.com/articles/s41588-025-02293-0/figures/9)

**a**–**d**, Whole-genome alignments. **e**–**h**, Density of PGGB graph bubbles. **i**–**l**, Nucleotide diversity. For chromosome 1 and further explanation, see Fig. [2a–c](https://www.nature.com/articles/s41588-025-02293-0#Fig2).

### [Extended Data Fig. 2 SV type and gene-relative location.](https://www.nature.com/articles/s41588-025-02293-0/figures/10)

**a**, Cartoons illustrating our classification of length variants into sSVs and cSVs in the whole-genome alignment and graph representations. **b**, The distribution of sSVs and cSVs across chromosomes—cSVs are more common in pericentromeric regions. **c**, Fraction of sSVs and cSVs by length. The prevalence of short sSVs is at least partly explained by the low probability of the multiple events required for cSVs to occur in short DNA segments. **d**, The number of putative insertions (presence allele in 1–3 accessions) and deletions (absence allele in 1–3 accessions) of varying lengths in genes and intergenic regions. **e**, Same for exons and introns.

### [Extended Data Fig. 3 Size distribution of graph nodes by TE-content.](https://www.nature.com/articles/s41588-025-02293-0/figures/11)

Large nodes are found not only for presence alleles that correspond to complete annotated TE but also for other categories, demonstrating that these are also part of the mobile-ome.

### [Extended Data Fig. 4 The graph of the nestedness of existing _A. thaliana_ TE annotations.](https://www.nature.com/articles/s41588-025-02293-0/figures/12)

Each node is a cluster of similar sequences (with length and identity thresholds of 0.85), where the size of the node indicates its relative abundance. The graph can be decomposed into one dominant connected component and several smaller ones, as shown on the right.

### [Extended Data Fig. 5 Details of gene-ome analysis.](https://www.nature.com/articles/s41588-025-02293-0/figures/13)

**a**, TE genes were defined as the union of two sets of genes: (1) those with >50% annotated TE sequence in at least one accession, and (2) those with ORFs similar to proteins known to be involved in TE function. **b**, Comparison of gene presence variation in this study to a recent analysis in 69 _A. thaliana_ accessions 23. For both PC genes and TE genes, our presence–absence variability is higher for gene models compared to gene loci, probably because our gene annotation pipeline misses lowly expressed genes in the four tissues we used. The PC gene model variability in the study from the Mercier lab 23 is substantially higher than in our data. This likely reflects the fact that while we used pan-genome coordinates to match genes between accessions, they used an orthogroup search approach. Consider this case: a gene is both present and has a gene model in every accession, but in three accessions, a shorter gene model was annotated. The orthogroup approach would identify this case as two gene families residing in the locus and call both gene models dispensable, while our approach would treat this locus as one and identify both gene and gene model as core. **c**, Gene presence frequency distribution for TE genes. **d**, _A. lyrata_ synteny and sequence similarity analysis for TE genes (TAIR10 and new) with the same 80% sequence-similarity stringency as in Fig. [6](https://www.nature.com/articles/s41588-025-02293-0#Fig6). TE genes are plotted by their gene IDs along the chromosomes. The small number of data points compared to PC genes is because most TE genes were not found in the _A. lyrata_ genome. **e**, Functional domains (‘NA’ indicates genes with no match) for genes grouped by new vs. old and PC vs. TE. **f**, The same for PC genes grouped by frequency of presence. **g**, The same PC and TE genes grouped by ancestral status. **h**, The distribution of PC and TE genes along all five chromosomes grouped by frequency of presence. **i**, The same grouped by ancestral status.

### [Extended Data Fig. 6 Gene silencing and expression by gene presence frequency and ancestral status.](https://www.nature.com/articles/s41588-025-02293-0/figures/14)

**a**, Median expression vs. frequency for all accessions. **b**, H3K9me2 and H3K27me3 54 genes vs. their frequency. Values plotted are medians of quantile- and input-normalized ChIP-seq signals. **c**, 24-nt sRNAs coverage of genes of different frequencies. Left: distribution in flowers of accession 6024. Right: median coverage. **d**, Locus-wide CHG, CG and CHH methylation levels in leaves 53 for genes of different frequency. Left: distribution in accession 6024. Right: median levels. **e**, Expression (median TPM) vs. ancestral status for all accessions. **f**, H3K9me2 and H3K27me3 54 vs. ancestral status. Values plotted are medians of quantile- and input-normalized ChIP-seq signals. **g**, 24-nt sRNAs locus-wide coverage in accession 6024, flowers, for genes of different ancestral status. **h**, Methylation levels in leaves 53 for genes of different ancestral status. Left: accession 6024. Right: median methylation levels. All heatmaps were created using the pheatmap package in _R_, and all, except for expression, are scaled by row to facilitate within- and between-accession comparison. Box plots show the median and the 25th and 75th percentiles (box bounds), and the smallest and largest values within 1.5× the interquartile range (whiskers); outliers are not plotted. Significance of median differences was assessed using two-tailed Wilcoxon tests. Sample sizes are shown above the top boxplot in Fig. [6i–j](https://www.nature.com/articles/s41588-025-02293-0#Fig6).

### [Extended Data Fig. 7 Extended pan-genome analysis.](https://www.nature.com/articles/s41588-025-02293-0/figures/15)

**a**, Saturation curves for sSVs for different lengths. Each curve is drawn through points that are the averaged values from 20 repetitions. The curves were normalized to start and end at the same points. Larger sSVs saturate more quickly. **b**, Normalized saturation curves for different genome components: the dependence on sample size for the union (‘pan’) and intersection (‘core’) sequence length, separately for the full genome, the mobile-ome and the gene-ome. Within the ‘pan’ curves, the mobile-ome saturates the fastest, the gene-ome the slowest and the entire genome at an intermediate rate. Gene-ome and whole genome ‘core’ curves show similar trends. **c**–**f**, Pan-genome vs. reference genome coordinates for chromosomes 2–5. The pericentromeric region (light blue) shows a higher ‘dilution’ of the spatial coordinates due to the increased number of SVs in this region. The centromeric region is dark blue.

Supplementary information
-------------------------

### [Supplementary Information](https://static-content.springer.com/esm/art%3A10.1038%2Fs41588-025-02293-0/MediaObjects/41588_2025_2293_MOESM1_ESM.pdf)

Supplementary Notes 1–8 and Figs. 1–33.

### [Reporting Summary](https://static-content.springer.com/esm/art%3A10.1038%2Fs41588-025-02293-0/MediaObjects/41588_2025_2293_MOESM2_ESM.pdf)

### [Peer Review file](https://static-content.springer.com/esm/art%3A10.1038%2Fs41588-025-02293-0/MediaObjects/41588_2025_2293_MOESM3_ESM.pdf)

### [Supplementary Table 1](https://static-content.springer.com/esm/art%3A10.1038%2Fs41588-025-02293-0/MediaObjects/41588_2025_2293_MOESM4_ESM.xlsx)

Origin and sequencing data for the 27 accessions.

### [Supplementary Table 2](https://static-content.springer.com/esm/art%3A10.1038%2Fs41588-025-02293-0/MediaObjects/41588_2025_2293_MOESM5_ESM.xlsx)

Large inversions.

### [Supplementary Table 3](https://static-content.springer.com/esm/art%3A10.1038%2Fs41588-025-02293-0/MediaObjects/41588_2025_2293_MOESM6_ESM.txt)

Organellar inserts.

### [Supplementary Table 4](https://static-content.springer.com/esm/art%3A10.1038%2Fs41588-025-02293-0/MediaObjects/41588_2025_2293_MOESM7_ESM.txt)

RNA-seq read-map data.

Rights and permissions
----------------------

**Open Access** This article is licensed under a Creative Commons Attribution 4.0 International License, which permits use, sharing, adaptation, distribution and reproduction in any medium or format, as long as you give appropriate credit to the original author(s) and the source, provide a link to the Creative Commons licence, and indicate if changes were made. The images or other third party material in this article are included in the article’s Creative Commons licence, unless indicated otherwise in a credit line to the material. If material is not included in the article’s Creative Commons licence and your intended use is not permitted by statutory regulation or exceeds the permitted use, you will need to obtain permission directly from the copyright holder. To view a copy of this licence, visit [http://creativecommons.org/licenses/by/4.0/](http://creativecommons.org/licenses/by/4.0/).

[Reprints and permissions](https://s100.copyright.com/AppDispatchServlet?title=A%20comparison%20of%2027%20Arabidopsis%20thaliana%20genomes%20and%20the%20path%20toward%20an%20unbiased%20characterization%20of%20genetic%20polymorphism&author=Anna%20A.%20Igolkina%20et%20al&contentID=10.1038%2Fs41588-025-02293-0&copyright=The%20Author%28s%29&publication=1061-4036&publicationDate=2025-08-19&publisherName=SpringerNature&orderBeanReset=true&oa=CC%20BY)

About this article
------------------

[![Check for updates. Verify currency and authenticity via CrossMark](data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjgxIiB3aWR0aD0iNTciIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+PGcgZmlsbD0ibm9uZSIgZmlsbC1ydWxlPSJldmVub2RkIj48cGF0aCBkPSJtMTcuMzUgMzUuNDUgMjEuMy0xNC4ydi0xNy4wM2gtMjEuMyIgZmlsbD0iIzk4OTg5OCIvPjxwYXRoIGQ9Im0zOC42NSAzNS40NS0yMS4zLTE0LjJ2LTE3LjAzaDIxLjMiIGZpbGw9IiM3NDc0NzQiLz48cGF0aCBkPSJtMjggLjVjLTEyLjk4IDAtMjMuNSAxMC41Mi0yMy41IDIzLjVzMTAuNTIgMjMuNSAyMy41IDIzLjUgMjMuNS0xMC41MiAyMy41LTIzLjVjMC02LjIzLTIuNDgtMTIuMjEtNi44OC0xNi42Mi00LjQxLTQuNC0xMC4zOS02Ljg4LTE2LjYyLTYuODh6bTAgNDEuMjVjLTkuOCAwLTE3Ljc1LTcuOTUtMTcuNzUtMTcuNzVzNy45NS0xNy43NSAxNy43NS0xNy43NSAxNy43NSA3Ljk1IDE3Ljc1IDE3Ljc1YzAgNC43MS0xLjg3IDkuMjItNS4yIDEyLjU1cy03Ljg0IDUuMi0xMi41NSA1LjJ6IiBmaWxsPSIjNTM1MzUzIi8+PHBhdGggZD0ibTQxIDM2Yy01LjgxIDYuMjMtMTUuMjMgNy40NS0yMi40MyAyLjktNy4yMS00LjU1LTEwLjE2LTEzLjU3LTcuMDMtMjEuNWwtNC45Mi0zLjExYy00Ljk1IDEwLjctMS4xOSAyMy40MiA4Ljc4IDI5LjcxIDkuOTcgNi4zIDIzLjA3IDQuMjIgMzAuNi00Ljg2eiIgZmlsbD0iIzljOWM5YyIvPjxwYXRoIGQ9Im0uMiA1OC40NWMwLS43NS4xMS0xLjQyLjMzLTIuMDFzLjUyLTEuMDkuOTEtMS41Yy4zOC0uNDEuODMtLjczIDEuMzQtLjk0LjUxLS4yMiAxLjA2LS4zMiAxLjY1LS4zMi41NiAwIDEuMDYuMTEgMS41MS4zNS40NC4yMy44MS41IDEuMS44MWwtLjkxIDEuMDFjLS4yNC0uMjQtLjQ5LS40Mi0uNzUtLjU2LS4yNy0uMTMtLjU4LS4yLS45My0uMi0uMzkgMC0uNzMuMDgtMS4wNS4yMy0uMzEuMTYtLjU4LjM3LS44MS42Ni0uMjMuMjgtLjQxLjYzLS41MyAxLjA0LS4xMy40MS0uMTkuODgtLjE5IDEuMzkgMCAxLjA0LjIzIDEuODYuNjggMi40Ni40NS41OSAxLjA2Ljg4IDEuODQuODguNDEgMCAuNzctLjA3IDEuMDctLjIzcy41OS0uMzkuODUtLjY4bC45MSAxYy0uMzguNDMtLjguNzYtMS4yOC45OS0uNDcuMjItMSAuMzQtMS41OC4zNC0uNTkgMC0xLjEzLS4xLTEuNjQtLjMxLS41LS4yLS45NC0uNTEtMS4zMS0uOTEtLjM4LS40LS42Ny0uOS0uODgtMS40OC0uMjItLjU5LS4zMy0xLjI2LS4zMy0yLjAyem04LjQtNS4zM2gxLjYxdjIuNTRsLS4wNSAxLjMzYy4yOS0uMjcuNjEtLjUxLjk2LS43MnMuNzYtLjMxIDEuMjQtLjMxYy43MyAwIDEuMjcuMjMgMS42MS43MS4zMy40Ny41IDEuMTQuNSAyLjAydjQuMzFoLTEuNjF2LTQuMWMwLS41Ny0uMDgtLjk3LS4yNS0xLjIxLS4xNy0uMjMtLjQ1LS4zNS0uODMtLjM1LS4zIDAtLjU2LjA4LS43OS4yMi0uMjMuMTUtLjQ5LjM2LS43OC42NHY0LjhoLTEuNjF6bTcuMzcgNi40NWMwLS41Ni4wOS0xLjA2LjI2LTEuNTEuMTgtLjQ1LjQyLS44My43MS0xLjE0LjI5LS4zLjYzLS41NCAxLjAxLS43MS4zOS0uMTcuNzgtLjI1IDEuMTgtLjI1LjQ3IDAgLjg4LjA4IDEuMjMuMjQuMzYuMTYuNjUuMzguODkuNjdzLjQyLjYzLjU0IDEuMDNjLjEyLjQxLjE4Ljg0LjE4IDEuMzIgMCAuMzItLjAyLjU3LS4wNy43NmgtNC4zNmMuMDcuNjIuMjkgMS4xLjY1IDEuNDQuMzYuMzMuODIuNSAxLjM4LjUuMjkgMCAuNTctLjA0LjgzLS4xM3MuNTEtLjIxLjc2LS4zN2wuNTUgMS4wMWMtLjMzLjIxLS42OS4zOS0xLjA5LjUzLS40MS4xNC0uODMuMjEtMS4yNi4yMS0uNDggMC0uOTItLjA4LTEuMzQtLjI1LS40MS0uMTYtLjc2LS40LTEuMDctLjctLjMxLS4zMS0uNTUtLjY5LS43Mi0xLjEzLS4xOC0uNDQtLjI2LS45NS0uMjYtMS41MnptNC42LS42MmMwLS41NS0uMTEtLjk4LS4zNC0xLjI4LS4yMy0uMzEtLjU4LS40Ny0xLjA2LS40Ny0uNDEgMC0uNzcuMTUtMS4wNy40NS0uMzEuMjktLjUuNzMtLjU4IDEuM3ptMi41LjYyYzAtLjU3LjA5LTEuMDguMjgtMS41My4xOC0uNDQuNDMtLjgyLjc1LTEuMTNzLjY5LS41NCAxLjEtLjcxYy40Mi0uMTYuODUtLjI0IDEuMzEtLjI0LjQ1IDAgLjg0LjA4IDEuMTcuMjNzLjYxLjM0Ljg1LjU3bC0uNzcgMS4wMmMtLjE5LS4xNi0uMzgtLjI4LS41Ni0uMzctLjE5LS4wOS0uMzktLjE0LS42MS0uMTQtLjU2IDAtMS4wMS4yMS0xLjM1LjYzLS4zNS40MS0uNTIuOTctLjUyIDEuNjcgMCAuNjkuMTcgMS4yNC41MSAxLjY2LjM0LjQxLjc4LjYyIDEuMzIuNjIuMjggMCAuNTQtLjA2Ljc4LS4xNy4yNC0uMTIuNDUtLjI2LjY0LS40MmwuNjcgMS4wM2MtLjMzLjI5LS42OS41MS0xLjA4LjY1LS4zOS4xNS0uNzguMjMtMS4xOC4yMy0uNDYgMC0uOS0uMDgtMS4zMS0uMjQtLjQtLjE2LS43NS0uMzktMS4wNS0uN3MtLjUzLS42OS0uNy0xLjEzYy0uMTctLjQ1LS4yNS0uOTYtLjI1LTEuNTN6bTYuOTEtNi40NWgxLjU4djYuMTdoLjA1bDIuNTQtMy4xNmgxLjc3bC0yLjM1IDIuOCAyLjU5IDQuMDdoLTEuNzVsLTEuNzctMi45OC0xLjA4IDEuMjN2MS43NWgtMS41OHptMTMuNjkgMS4yN2MtLjI1LS4xMS0uNS0uMTctLjc1LS4xNy0uNTggMC0uODcuMzktLjg3IDEuMTZ2Ljc1aDEuMzR2MS4yN2gtMS4zNHY1LjZoLTEuNjF2LTUuNmgtLjkydi0xLjJsLjkyLS4wN3YtLjcyYzAtLjM1LjA0LS42OC4xMy0uOTguMDgtLjMxLjIxLS41Ny40LS43OXMuNDItLjM5LjcxLS41MWMuMjgtLjEyLjYzLS4xOCAxLjA0LS4xOC4yNCAwIC40OC4wMi42OS4wNy4yMi4wNS40MS4xLjU3LjE3em0uNDggNS4xOGMwLS41Ny4wOS0xLjA4LjI3LTEuNTMuMTctLjQ0LjQxLS44Mi43Mi0xLjEzLjMtLjMxLjY1LS41NCAxLjA0LS43MS4zOS0uMTYuOC0uMjQgMS4yMy0uMjRzLjg0LjA4IDEuMjQuMjRjLjQuMTcuNzQuNCAxLjA0Ljcxcy41NC42OS43MiAxLjEzYy4xOS40NS4yOC45Ni4yOCAxLjUzcy0uMDkgMS4wOC0uMjggMS41M2MtLjE4LjQ0LS40Mi44Mi0uNzIgMS4xM3MtLjY0LjU0LTEuMDQuNy0uODEuMjQtMS4yNC4yNC0uODQtLjA4LTEuMjMtLjI0LS43NC0uMzktMS4wNC0uN2MtLjMxLS4zMS0uNTUtLjY5LS43Mi0xLjEzLS4xOC0uNDUtLjI3LS45Ni0uMjctMS41M3ptMS42NSAwYzAgLjY5LjE0IDEuMjQuNDMgMS42Ni4yOC40MS42OC42MiAxLjE4LjYyLjUxIDAgLjktLjIxIDEuMTktLjYyLjI5LS40Mi40NC0uOTcuNDQtMS42NiAwLS43LS4xNS0xLjI2LS40NC0xLjY3LS4yOS0uNDItLjY4LS42My0xLjE5LS42My0uNSAwLS45LjIxLTEuMTguNjMtLjI5LjQxLS40My45Ny0uNDMgMS42N3ptNi40OC0zLjQ0aDEuMzNsLjEyIDEuMjFoLjA1Yy4yNC0uNDQuNTQtLjc5Ljg4LTEuMDIuMzUtLjI0LjctLjM2IDEuMDctLjM2LjMyIDAgLjU5LjA1Ljc4LjE0bC0uMjggMS40LS4zMy0uMDljLS4xMS0uMDEtLjIzLS4wMi0uMzgtLjAyLS4yNyAwLS41Ni4xLS44Ni4zMXMtLjU1LjU4LS43NyAxLjF2NC4yaC0xLjYxem0tNDcuODcgMTVoMS42MXY0LjFjMCAuNTcuMDguOTcuMjUgMS4yLjE3LjI0LjQ0LjM1LjgxLjM1LjMgMCAuNTctLjA3LjgtLjIyLjIyLS4xNS40Ny0uMzkuNzMtLjczdi00LjdoMS42MXY2Ljg3aC0xLjMybC0uMTItMS4wMWgtLjA0Yy0uMy4zNi0uNjMuNjQtLjk4Ljg2LS4zNS4yMS0uNzYuMzItMS4yNC4zMi0uNzMgMC0xLjI3LS4yNC0xLjYxLS43MS0uMzMtLjQ3LS41LTEuMTQtLjUtMi4wMnptOS40NiA3LjQzdjIuMTZoLTEuNjF2LTkuNTloMS4zM2wuMTIuNzJoLjA1Yy4yOS0uMjQuNjEtLjQ1Ljk3LS42My4zNS0uMTcuNzItLjI2IDEuMS0uMjYuNDMgMCAuODEuMDggMS4xNS4yNC4zMy4xNy42MS40Ljg0LjcxLjI0LjMxLjQxLjY4LjUzIDEuMTEuMTMuNDIuMTkuOTEuMTkgMS40NCAwIC41OS0uMDkgMS4xMS0uMjUgMS41Ny0uMTYuNDctLjM4Ljg1LS42NSAxLjE2LS4yNy4zMi0uNTguNTYtLjk0LjczLS4zNS4xNi0uNzIuMjUtMS4xLjI1LS4zIDAtLjYtLjA3LS45LS4ycy0uNTktLjMxLS44Ny0uNTZ6bTAtMi4zYy4yNi4yMi41LjM3LjczLjQ1LjI0LjA5LjQ2LjEzLjY2LjEzLjQ2IDAgLjg0LS4yIDEuMTUtLjYuMzEtLjM5LjQ2LS45OC40Ni0xLjc3IDAtLjY5LS4xMi0xLjIyLS4zNS0xLjYxLS4yMy0uMzgtLjYxLS41Ny0xLjEzLS41Ny0uNDkgMC0uOTkuMjYtMS41Mi43N3ptNS44Ny0xLjY5YzAtLjU2LjA4LTEuMDYuMjUtMS41MS4xNi0uNDUuMzctLjgzLjY1LTEuMTQuMjctLjMuNTgtLjU0LjkzLS43MXMuNzEtLjI1IDEuMDgtLjI1Yy4zOSAwIC43My4wNyAxIC4yLjI3LjE0LjU0LjMyLjgxLjU1bC0uMDYtMS4xdi0yLjQ5aDEuNjF2OS44OGgtMS4zM2wtLjExLS43NGgtLjA2Yy0uMjUuMjUtLjU0LjQ2LS44OC42NC0uMzMuMTgtLjY5LjI3LTEuMDYuMjctLjg3IDAtMS41Ni0uMzItMi4wNy0uOTVzLS43Ni0xLjUxLS43Ni0yLjY1em0xLjY3LS4wMWMwIC43NC4xMyAxLjMxLjQgMS43LjI2LjM4LjY1LjU4IDEuMTUuNTguNTEgMCAuOTktLjI2IDEuNDQtLjc3di0zLjIxYy0uMjQtLjIxLS40OC0uMzYtLjctLjQ1LS4yMy0uMDgtLjQ2LS4xMi0uNy0uMTItLjQ1IDAtLjgyLjE5LTEuMTMuNTktLjMxLjM5LS40Ni45NS0uNDYgMS42OHptNi4zNSAxLjU5YzAtLjczLjMyLTEuMy45Ny0xLjcxLjY0LS40IDEuNjctLjY4IDMuMDgtLjg0IDAtLjE3LS4wMi0uMzQtLjA3LS41MS0uMDUtLjE2LS4xMi0uMy0uMjItLjQzcy0uMjItLjIyLS4zOC0uM2MtLjE1LS4wNi0uMzQtLjEtLjU4LS4xLS4zNCAwLS42OC4wNy0xIC4ycy0uNjMuMjktLjkzLjQ3bC0uNTktMS4wOGMuMzktLjI0LjgxLS40NSAxLjI4LS42My40Ny0uMTcuOTktLjI2IDEuNTQtLjI2Ljg2IDAgMS41MS4yNSAxLjkzLjc2cy42MyAxLjI1LjYzIDIuMjF2NC4wN2gtMS4zMmwtLjEyLS43NmgtLjA1Yy0uMy4yNy0uNjMuNDgtLjk4LjY2cy0uNzMuMjctMS4xNC4yN2MtLjYxIDAtMS4xLS4xOS0xLjQ4LS41Ni0uMzgtLjM2LS41Ny0uODUtLjU3LTEuNDZ6bTEuNTctLjEyYzAgLjMuMDkuNTMuMjcuNjcuMTkuMTQuNDIuMjEuNzEuMjEuMjggMCAuNTQtLjA3Ljc3LS4ycy40OC0uMzEuNzMtLjU2di0xLjU0Yy0uNDcuMDYtLjg2LjEzLTEuMTguMjMtLjMxLjA5LS41Ny4xOS0uNzYuMzFzLS4zMy4yNS0uNDEuNGMtLjA5LjE1LS4xMy4zMS0uMTMuNDh6bTYuMjktMy42M2gtLjk4di0xLjJsMS4wNi0uMDcuMi0xLjg4aDEuMzR2MS44OGgxLjc1djEuMjdoLTEuNzV2My4yOGMwIC44LjMyIDEuMi45NyAxLjIuMTIgMCAuMjQtLjAxLjM3LS4wNC4xMi0uMDMuMjQtLjA3LjM0LS4xMWwuMjggMS4xOWMtLjE5LjA2LS40LjEyLS42NC4xNy0uMjMuMDUtLjQ5LjA4LS43Ni4wOC0uNCAwLS43NC0uMDYtMS4wMi0uMTgtLjI3LS4xMy0uNDktLjMtLjY3LS41Mi0uMTctLjIxLS4zLS40OC0uMzctLjc4LS4wOC0uMy0uMTItLjY0LS4xMi0xLjAxem00LjM2IDIuMTdjMC0uNTYuMDktMS4wNi4yNy0xLjUxcy40MS0uODMuNzEtMS4xNGMuMjktLjMuNjMtLjU0IDEuMDEtLjcxLjM5LS4xNy43OC0uMjUgMS4xOC0uMjUuNDcgMCAuODguMDggMS4yMy4yNC4zNi4xNi42NS4zOC44OS42N3MuNDIuNjMuNTQgMS4wM2MuMTIuNDEuMTguODQuMTggMS4zMiAwIC4zMi0uMDIuNTctLjA3Ljc2aC00LjM3Yy4wOC42Mi4yOSAxLjEuNjUgMS40NC4zNi4zMy44Mi41IDEuMzguNS4zIDAgLjU4LS4wNC44NC0uMTMuMjUtLjA5LjUxLS4yMS43Ni0uMzdsLjU0IDEuMDFjLS4zMi4yMS0uNjkuMzktMS4wOS41M3MtLjgyLjIxLTEuMjYuMjFjLS40NyAwLS45Mi0uMDgtMS4zMy0uMjUtLjQxLS4xNi0uNzctLjQtMS4wOC0uNy0uMy0uMzEtLjU0LS42OS0uNzItMS4xMy0uMTctLjQ0LS4yNi0uOTUtLjI2LTEuNTJ6bTQuNjEtLjYyYzAtLjU1LS4xMS0uOTgtLjM0LTEuMjgtLjIzLS4zMS0uNTgtLjQ3LTEuMDYtLjQ3LS40MSAwLS43Ny4xNS0xLjA4LjQ1LS4zMS4yOS0uNS43My0uNTcgMS4zem0zLjAxIDIuMjNjLjMxLjI0LjYxLjQzLjkyLjU3LjMuMTMuNjMuMi45OC4yLjM4IDAgLjY1LS4wOC44My0uMjNzLjI3LS4zNS4yNy0uNmMwLS4xNC0uMDUtLjI2LS4xMy0uMzctLjA4LS4xLS4yLS4yLS4zNC0uMjgtLjE0LS4wOS0uMjktLjE2LS40Ny0uMjNsLS41My0uMjJjLS4yMy0uMDktLjQ2LS4xOC0uNjktLjMtLjIzLS4xMS0uNDQtLjI0LS42Mi0uNHMtLjMzLS4zNS0uNDUtLjU1Yy0uMTItLjIxLS4xOC0uNDYtLjE4LS43NSAwLS42MS4yMy0xLjEuNjgtMS40OS40NC0uMzggMS4wNi0uNTcgMS44My0uNTcuNDggMCAuOTEuMDggMS4yOS4yNXMuNzEuMzYuOTkuNTdsLS43NC45OGMtLjI0LS4xNy0uNDktLjMyLS43My0uNDItLjI1LS4xMS0uNTEtLjE2LS43OC0uMTYtLjM1IDAtLjYuMDctLjc2LjIxLS4xNy4xNS0uMjUuMzMtLjI1LjU0IDAgLjE0LjA0LjI2LjEyLjM2cy4xOC4xOC4zMS4yNmMuMTQuMDcuMjkuMTQuNDYuMjFsLjU0LjE5Yy4yMy4wOS40Ny4xOC43LjI5cy40NC4yNC42NC40Yy4xOS4xNi4zNC4zNS40Ni41OC4xMS4yMy4xNy41LjE3LjgyIDAgLjMtLjA2LjU4LS4xNy44My0uMTIuMjYtLjI5LjQ4LS41MS42OC0uMjMuMTktLjUxLjM0LS44NC40NS0uMzQuMTEtLjcyLjE3LTEuMTUuMTctLjQ4IDAtLjk1LS4wOS0xLjQxLS4yNy0uNDYtLjE5LS44Ni0uNDEtMS4yLS42OHoiIGZpbGw9IiM1MzUzNTMiLz48L2c+PC9zdmc+)](https://crossmark.crossref.org/dialog/?doi=10.1038/s41588-025-02293-0)

### Cite this article

Igolkina, A.A., Vorbrugg, S., Rabanal, F.A. _et al._ A comparison of 27 _Arabidopsis thaliana_ genomes and the path toward an unbiased characterization of genetic polymorphism. _Nat Genet_ (2025). https://doi.org/10.1038/s41588-025-02293-0

[Download citation](https://citation-needed.springer.com/v2/references/10.1038/s41588-025-02293-0?format=refman&flavour=citation)

-   Received: 31 May 2024
    
-   Accepted: 10 July 2025
    
-   Published: 19 August 2025
    
-   DOI: https://doi.org/10.1038/s41588-025-02293-0
    

### Share this article

Anyone you share the following link with will be able to read this content:

Get shareable link

Sorry, a shareable link is not currently available for this article.

Copy to clipboard

Provided by the Springer Nature SharedIt content-sharing initiative

[Download PDF](https://www.nature.com/articles/s41588-025-02293-0.pdf)
