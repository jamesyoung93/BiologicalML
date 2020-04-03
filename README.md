# BiologicalML
Biological Machine Learning  

There are 3 biological machine learning projects in this directory. 

# 1. Drug Repurposing Success Prediciton 
Using xgboost and available data from a previous study https://www.nature.com/articles/s41598-019-42806-6#data-availability, I beat the original reports AUC using XGBoost. This means my model had better predictive ability for picking drugs that would be succesfully repurposed.
- Beat the author's AUC of 0.922 by implementing XGBoost instead of Random Forest

# 2. Predicting Gestational Age Using RNAseq Data (DREAM challenge) 
This was part of a "DREAM" challenge hosted by Synapse. I worked on this group with fellow grad students in the biology department over the summer. The group write up can be viewed here https://github.com/jamesyoung93/Preterm-Dream-Challenge. I have also included my personal contributions in the files above. These contribution include 
- Feature selection on ~ 900,000 features which were RNA probes (I used xgboost importance to retain only top features)
- Modeling with XGBoost down to an RMSE of about ~4 in both train and test where response variable was the week of gestation (pregnancy)
- This work was done in python so these are the ipynb files


# 3. Protein Translational Efficiency 
Using xgboost I made a predictive model for translational efficiency of eventual proteins based on their nucleotide and amino acid sequences as well as the physical characteristics of those molecules such as hydrophobicity, molecular weight, rareness of codons, RNA folding energy, and charge. The proteins were given a score (protein expression level) based on experimental work found in this article https://www.nature.com/articles/s41467-019-13810-1#Sec23. I tried to predict that score (protein level) using my previously described input variables.
- Attained RMSE of 0.6 when predicting a range of protein expression scored 1 through 5.

