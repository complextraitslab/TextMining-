# TextMining-

#google folder link with documents 
#https://drive.google.com/drive/u/0/folders/1Aj-T8jUyBMgcNk72M1KrBUtRsTKsAmQq




# Text-Mining-Review
using pipeline from https://github.com/maiziezhoulab/Autism_genepheno/blob/master/bin/Autism_genepheno_PMC_scraper.py


location 


Directory: /harddrive_10tb_storage/Text_mining
Env: conda activate /home/gomest/miniconda3/envs/text_mine
Run: python3 ALS_scraper.py --pmc_id_list pmc_result_ALS_AND_Gene.txt --out XML_ALS_datasets_5years





Step 0:
python3 ALS_scraper.py --pmc_id_list pmc_result_ALS_AND_Gene.txt --out XML_ALS_datasets_5years

Step 1:

python Autism_genepheno_step1_parallel.py --ASDPTO_dir ./ALSONTOLOGY_New.csv --UMLS_dir ./UMLS.txt --allGene_dir ./ALSoD_gene_associations.tsv --papers_dir ./XML_ALS_datasets_5years/ --HPOtreeview_dir ./HPO_treeview.txt --out_dir ./ALS_genepheno_results/

# The ASDPTO part phenotype list
ASDPTO_dir = 'ALSONTOLOGY_New.csv'

# The UMLS part phenotype list
UMLS_dir = 'UMLS.txt'              

# The autism-associated gene list from VariCarta database
allGene_dir = 'ALSoD_gene_associations.tsv'  ****
