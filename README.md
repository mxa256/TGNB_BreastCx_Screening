# Transgender and Non-Binary (TGNB) Breast Cancer Screening Rates at Single Insitution

##My contributions  <br>
I performed a single institution analysis of breast cancer screening rates in transgender and non-binary patients. This work was published in the Annals of Surgical Oncology. [The link to the abstract and publication is here.](https://pubmed.ncbi.nlm.nih.gov/34704183/)
I participated in patient cohort construction and data collection, performed all of the data analysis, wrote the manuscript, and edited the manuscript per peer review feedback.

##Key findings  <br>
The key takeaways from this study are as follows:  <br>
1. TGNB patients designated female at birth had low breast cancer screening rates (ranging from 2.0% - 50.0%). This is lower than institutional breast cancer screening rates and nationally reported breast cancer screening rates  <br>
2. TGNB patients designated male at birth had low breast cancer screening rates (ranging from 7.1 - 47.6%).  <br>
3. There were no significant predictors of breast cancer screening on multivariate regression analysis.

##Data source and patient cohort  <br>
TGNB patients within our medical institution (Northwestern Memorial Hospital) were comprehensively identified. Encounters between March 2019 and February 2021 were flagged for review (N = 84,236); records flagged included those with (1) an International Classification of Diseases 10th Revision (ICD-10) diagnosis code for gender dysphoria; (2) any gender identity or designated sex at birth electronic medical record field (including cisgender patients); or (3) a clinical note containing a TGNB-related keyword. Keywords for text mining included ‘transwoman’, ‘transman’, ‘trans woman’, ‘trans man’, ‘non-binary’, ‘nonbinary’, ‘gender fluid’, ‘gender dysphoria’, ‘genderqueer’, ‘MTF’, ‘FTM’, ‘transgender’, and ‘transsexual’. Text mining hits were reported with 100-character snips for screening. Structured demographic sexual orientation and gender identity (SOGI) data fields were also queried.  <br> 

The final correctly identified TGNB population consisted of 1684 patients.  <br> 

Patients over the age of 40 years were included, and patients with a history of breast cancer were also excluded as these patients would not undergo screening mammography.  <br>

The final cohort for analysis included 253 patients.

##Data Analysis  <br>
All data analysis was performed using RStudio. Here, I am providing an abbreviated version of my data analysis. The original Rmd file is long and redundant. I removed the coding analysis for the assigned male at birth group, because it is the same as the assigned female at birth group. I wanted to keep the uploaded file short so it could be easier to read through and follow.
Key steps in data analysis included:  <br>
1. Data loading and clean up - inspecting variables, factoring, labeling, editing mistakes, excluding certain patients
2. Exploratory data analysis
3. Creating subgroups for analysis (assigned female versus male at birth)
4. Running regression analyses
5. Calculating screening rates
6. Calculating lifetime mammograms
7. Calculating mammogram person-years
8. Comparing our findings to institutional rates and national rates for screening in cisgender patients

##Results  <br>
Here are the key results and visualizations from the paper. <br>

<img width="1277" alt="image" src="https://github.com/mxa256/TGNB_BreastCx_Screening/assets/19754522/32779189-790a-40d9-91dd-e3542dc205fd">

This table outlines the screening mammography rates among TGNB DFAB patients according to NCCN and USPSTF guidelines. The numerator represents the number of patients who underwent on-time screening and total lifetime screening, while the denominator represents the number of patients with breasts (i.e., did not have top surgery) who were eligible for screening at age 40 or 50 years, respectively. For the on-time screening numerators, a 2-year grace period was given for patients to obtain screening on time.  <br>

<img width="1281" alt="image" src="https://github.com/mxa256/TGNB_BreastCx_Screening/assets/19754522/72d40489-e266-4f5d-8bf5-794aed95573f">

Table 5 outlines mammography screening rates among TGNB DMAB patients. The UCSF Center for Transgender Health and Fenway Health guidelines (screening mammogram at age 50 years and ≥5 years of hormone therapy) were applied to TGNB DMAB patients. The denominator represents patients ≥50 years of age on at least 5 years of hormone therapy, while the numerator represents the number of patients who underwent on-time screening and total lifetime screening.  <br>


![image](https://github.com/mxa256/TGNB_BreastCx_Screening/assets/19754522/81c33dec-3c47-48f8-9a6e-f42f76128687)

This plot (made with ggplot) shows the number of lifetime mammograms versus eligible screening years per patient. The black line indicates the recommended screening rate, with one mammogram occurring every 2 years. Only TGNB DMAB patients over the age of 50 years who received at least 5 years of hormone therapy were included. Eleven TGNB designated female at birth (DFAB) patients were excluded due to receiving mastectomy prior to screening eligibility. TGNB DMAB = transgender women and non-binary persons designated male at birth, TGNB DFAB = transgender men and non-binary persons designated female at birth.  <br>
You can see that most patients fall below the black line of optimal screening rate, indicating that they are not receiving on time.

