# Sample Size Calculation to reach a predefined power for a future three-arm study with a new treatment, based on the existing network

R Shiny app: https://nmass.shinyapps.io/nma3arms/

1. sampledat.csv

   a sample dataset for investigators to refer; when using the shiny app to calculate the sample size, please upload your dataset using the same format as sampledat.csv
   
   This dataset contains 5 columns that are:
   - studlab: study id
   - treat1: name of treatment 1
   - treat2: name of treatment 2
   - TE: treatment effect size (log odds ratio) between treat1 and treat2
   - seTE: standard error of the estimated TE

   Note that for trials with more than two arms, all pairwise comparisons are required in the dataset. For example, a three-arm trial should have 3 rows of comparisons, a four-arm trial shold have 6 rows, etc.


2. app.R


   Main function for R shiny app. To run it successfully, SolveSampleSize.R is needed.
 
3. SampleSize.R


   Contains functions used for solve the optimization problems. 
