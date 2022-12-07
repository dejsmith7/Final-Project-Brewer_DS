# Final-Project-Brewer_DS
This is the final project submission by Dejah Smith for the Practical Computing course.

My project is an extension of an ongoing initiative that is measuring the affects of human activities related to land use on nutrient cycles across a low-nutrient coastal plain wetland. The structure of the experiment involves 8 plots that undergo either a mowed treatment (M) or a mowed fertilized treatment (MF). The results of this ecological experiement were the foundation to my research. Sanger sequencing was conducted on 10 soil bacterial isolate pairs from the different plot treatments. I conducted whole genome sequencing to identify metabolic and physiological differences between the pairs.

For my submission, I chose to highlight two bacterial isolate species: Arthrobacter ramosus and Pseudomonas koreensis 
I used a pangenomic workflow to analyze the pairs and the presence/absence of genes from mowed (M) and mowed fertilized (MF) plots.
Pangeomic analyses allow you to view a full set of genes and determine their homology as well as the functions they share. This is important to know for my research because I am analyzing not only the genes present across the two treatments but how they may overlap between microbial species and the influence these genes have on plant-microbe interactions.

Arthrobacter species are known to be oligotrophs, meaning they can live in environments with low nutrients. Pseudomonas species are known to be copiotrophs, meaning they live in environments with high levels of nutrients, thriving off of Carbon availability.

## The set of isolates corresponding with A. ramosus are: WRC_263 (mowed treatment) and WRC_267 (mowed fertilized treatment)
Arthrobacter ramosus has a very slow growth rate which can be seen below:


<img width="305" alt="ARAMOSUS" src="https://user-images.githubusercontent.com/112521409/206233696-55c652d5-2655-4a57-82a1-0024b2516b3c.png">
(Image credit: Aied Garcia)

Based on this growth rate, I predicted that the functional genes present across the two treatments would be fairly low.


## The set of isolates corresponding with P. koreensis are: WRC_271 (mowed treatment) and WRC_315 (mowed fertilized treatment)
Pseudomonas koreensis has a very slow growth rate which can be seen below:


<img width="305" alt="PKOR" src="https://user-images.githubusercontent.com/112521409/206234779-bd62b0d5-4ce9-40e3-8e4c-cf2354a8cf33.png">
(Image credit: Aied Garcia)

Based on this growth rate, I predicted that there would be a large amount of functional genes present across the two treatments.

# Predictions are great... but what actually happened?
After runninng a pangenomic analysis on both isolate groups the following was the result:

The phylogram for A. ramosus shows a clear presence/absence comparison between the two treatments

<img width="917" alt="ARAMOSUS-PAN" src="https://user-images.githubusercontent.com/112521409/206236551-101ffdc2-1daa-4d89-ab47-2a5554486f5d.png">

COGs are defined as Clusters of Orthologous Genes
These gene clusters can be present across various genomes and are categorized by their function.
The COG20 pathway relates to a set of genes that function to drive processes related to nutrient uptake, metabolism and protein synthesis. As this project is related to affect of human acitivty on plant-microbe relationships and nutrient accessibility, this pathway was the most fitting to annotate against.

The phylogram for P. koreensis also shows a clear presence/absence of genes between the two treatments

<img width="882" alt="PKOR-PAN" src="https://user-images.githubusercontent.com/112521409/206238789-8c4e48c1-61f7-49bc-a31e-253e9e36a840.png">

The enriched functions derived from each pangenomic analyses only had four orthologous functional genes present across both isolate species and their respective treatments:


<img width="935" alt="PKOR_ARAMOSUS_tableF" src="https://user-images.githubusercontent.com/112521409/206259455-bd85d20b-62d0-4a6e-aa5f-37e55937dc03.png">

Here is the legend for the table presented:
COG20_FUNCTION: this is the functional pathway and set of genes that the enrichment was calculated against
enrichment_score: this is a measure developed by statistician, Amy Willis to quantify how much the function shown is unique to genomes within a group against your genomes
unadjusted_p_value: this is the p-value for the enrichment test
adjusted_q_alue: this is the q-value used to control the false discovery rate of multiple tests
associated_groups: the groups that are assoociated with the function
function_accessionn: accession number
gene_clusters_ids: gene clusters associated with the function listed
p_M, p_MF: groups based on treatment either mowed (M) or mowed fertilized (MF)
N_M, N_MF: the total number of genomes within the group specified


# So what does this tell us?

The functional genes found within our genomes and across the COG20 functional pathway all are related to nutrient uptake, regulation and protein synthesis.

The first row function corresponds with the gene pstA which functions to allow transport of inorganic phosphates for the production of ATP and synthesis of proteins.

The second row function corresponds with the gene yidH which functions to respond to oxidative stress in the membrane.

The third row function corresponds with a general gene category, Metal-dependent hydrolase which functions to break down nutrients into smaller units.

The fourth row function corresponds with the gene PiuB or PepSY, which functions to regulate peptidase activity, specifically those that inhibit chaperones. This gene also plays a role in protecting the cell from lysis. 

# With this, I am confident that with further analysis of these isolates as well as the others, I will be able to answer the following questions...

Why are the only orthologus genes seen in the mowed fertilized treatment?

Where are these genes located within the genome and what can this location tell us?

How do we mitigate environmental stress to preserve these plant-microbe relationships to maintain biodiversity in these areas?

## All of the above are future topics that I am interested in finding the answers to and look forward to discovering in the future!


References:
Anvi'o - https://anvio.org/ , https://anvio.org/learn/pangenomics/
NCBI COG Database - https://www.ncbi.nlm.nih.gov/research/cog/
Peralta Lab (growth rate graphs)
