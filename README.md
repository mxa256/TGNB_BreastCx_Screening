# Transgender and Non-Binary (TGNB) Breast Cancer Screening Rates at Single Insitution

##My contributions
I performed a single institution analysis of breast cancer screening rates in transgender and non-binary patients. This work was published in the Annals of Surgical Oncology. [The link to the abstract and publication is here.](https://pubmed.ncbi.nlm.nih.gov/34704183/)
I participated in patient cohort construction and data collection, performed all of the data analysis, wrote the manuscript, and edited the manuscript per peer review feedback.

##Key findings
The key takeaways from this study are as follows:  <br>
1. TGNB patients designated female at birth had low breast cancer screening rates (ranging from 2.0% - 50.0%). This is lower than institutional breast cancer screening rates and nationally reported breast cancer screening rates  <br>
2. TGNB patients designated male at birth had low breast cancer screening rates (ranging from 7.1 - 47.6%).  <br>
3. There were no significant predictors of breast cancer screening on multivariate regression analysis.

##Data source and patient cohort
TGNB patients within our medical institution (Northwestern Memorial Hospital) were comprehensively identified. Encounters between March 2019 and February 2021 were flagged for review (N = 84,236); records flagged included those with (1) an International Classification of Diseases 10th Revision (ICD-10) diagnosis code for gender dysphoria; (2) any gender identity or designated sex at birth electronic medical record field (including cisgender patients); or (3) a clinical note containing a TGNB-related keyword. Keywords for text mining included ‘transwoman’, ‘transman’, ‘trans woman’, ‘trans man’, ‘non-binary’, ‘nonbinary’, ‘gender fluid’, ‘gender dysphoria’, ‘genderqueer’, ‘MTF’, ‘FTM’, ‘transgender’, and ‘transsexual’. Text mining hits were reported with 100-character snips for screening. Structured demographic sexual orientation and gender identity (SOGI) data fields were also queried.  <br> 

The final correctly identified TGNB population consisted of 1684 patients.  <br> 

Patients over the age of 40 years were included, and patients with a history of breast cancer were also excluded as these patients would not undergo screening mammography.  <br>

The final cohort for analysis included 253 patients.

##Data Analysis
All data analysis was performed using RStudio. Here, I am providing an abbreviated version of my data analysis. The original Rmd file is long and redundant. I removed the coding analysis for the assigned male at birth group, because it is the same as the assigned female at birth group. I wanted to keep the uploaded file short so it could be easier to read through and follow.
Key steps in data analysis included:  <br>
1. Data loading and clean up - inspecting variables, factoring, labeling, editing mistakes, excluding certain patients
2. Exploratory data analysis
3. Creating subgroups for analysis (assigned female versus male at birth)
4. Running regression analyses
5. Calculating screening rates
6. Calculating lifetime mammograms
7. Calculating mammogram person-years
8. Comparing to institutional rates and national rates for screening in cisgender patients

##Results
Here are the key results and visualizations from the paper. 

