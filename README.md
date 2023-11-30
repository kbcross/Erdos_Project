# Erdos_Project_Predict_Crop_Yield
We used supervised machine learning to predict soybean crop yield in Nebraska and Oklahoma based on soil nutrients and microbiome data. All of the data was used from this paper: https://link.springer.com/article/10.1007/s12275-022-2363-x


Description of Files

"Paper.pdf" This is the journal article that collected the soil and crop yeild data. All soil nutrient data can be found in supplemental material and the OTUs can be found using the accession numner found in their paper.

"Combined_soil_otu_data.xlsx" This includes the soil nutrient data and otu data (collapsed at the order level) and is the input for some of the ML models tested

"filtered_otu_table.csv" This table is the otu table with mitochondria, chloroplasts, and any OTUs with fewer than 10 reads in fewer than 10 samples removed.

"soil_nutrient_data.xlsx" This is all the soil nutrient data.

"Soybean_otu_taxonomy.xlsx" This is the otus table. This will open up unformatted in excel, but if you upload into python as a csv then you will be able to view and use the file. 



"1_data_clean_up_(done).py" This python script includes everything that the group did to generate "filtered_otu_table.csv".

"2_data_exploratory_analysis.py" This python script includes various exploratory analysis such as a relative abundance plot, NMDS plot, and correlation matrix.

"3_supervise_ml.py" This python script includes all the supervised machine learning that the group completed, including K nearest neighbor regression, linear regression, random forest regression, support vector regression, and feature importance using feature importance. We also repeated this analysis with and without the microbiome data. 
