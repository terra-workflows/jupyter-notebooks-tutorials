# Welcome to The GATK BroadE Day 4 BigQuery Tutorial Workspace

This workspace introduces BigQuery functionality with notebooks that demonstrate how to manipulate cohorts and two ways of querying BigQuery data (via SQL and R). 

It also includes a teaser notebook on Hail, an open-source, scalable framework for exploring and analyzing  large scale data sets. The notebooks runs through a demo of how to use Hail in a notebook to analysize public-access 1,000 genomes data.

## BigQuery Resources
* For more instructions on using BigQuery in a notebook, see this [Google Cloud Platform intro](https://cloud.google.com/blog/products/gcp/google-cloud-platform-for-data-scientists-using-jupyter-notebooks-with-apache-spark-on-google-cloud). 
* Intro to controlling BigQuery costs: [https://cloud.google.com/bigquery/docs/controlling-costs](https://cloud.google.com/bigquery/docs/controlling-costs)
* BigQuery best practices: [https://cloud.google.com/bigquery/docs/best-practices-costs](https://cloud.google.com/bigquery/docs/best-practices-costs)
* BigQuery cost calculator: [https://cloud.google.com/products/calculator/](https://cloud.google.com/products/calculator/)

## Variant Calling and BigQuery Resources  
There are a lot of built-in genomics tools already in BigQuery (including GATK). 
* BigQuery genomics: [https://cloud.google.com/genomics/](https://cloud.google.com/genomics/) 
* Analyzing variants: [https://cloud.google.com/genomics/docs/how-tos/analyze-variants](https://cloud.google.com/genomics/docs/how-tos/analyze-variants)
* On Github: [https://github.com/googlegenomics/](https://github.com/googlegenomics/)


## Hail Resources

The Hail Team at Broad gives regular workshops through Broad-E. Please defer to their coursework material.

* **Contact the Hail team** at hail@broadinstitute.org
* **Follow Hail on Twitter** @hailgenetics
* **Citing Hail** If you use Hail for published work, please cite the software:  Hail, https://github.com/hail-is/hail

Thank you to Tim Majarian from the Leonardo Team for providing the demo dataset and notebook, which was adjusted to work on Terra for this workshop.

-----
## Workspace Data  
The BigQuery notebooks in this workspace uses only notebooks (that pull data from BigQuery) and have no associated data of their own.

The Hail demo notebook features data in a Hail MatrixTable, which has been organized in a data model table and can be seen in the **Data** tab. The data is phase 3 genotypes from the 1,000 genomes with some mock phenotype measures for Type 2 Diabetes

## Workspace Tools
Likewise, there are no tools in this notebooks-based tutorial workspace. 

If you are interested in WDL based workflows you can use for  analyses, check out the [Showcase](https://app.terra.bio/#library/showcase) area in Terra, which features many of our popular GATK workflows in workspaces ready to run your data.

## Notebooks
Users can run code cells manually and view intermediate outputs. Markdown cells explain the function of the code cells. This is a great way to understand each step in the notebook and give you the chance to manipulate the parameters to see what happens with output.


**1_R_environment_setup**    
Run this notebook to set up the workspace for the rest of the BigQuery tutorial notebooks.

| Runtime Environments | Value |
| --- | --- |
| CPU Minimum| 2|
| Disksize Minimum | 100 GB |
| Memory Minimum | 13 GB |



**2_R_How_to_retrieve_a_cohort_using_BigQuery**     
This notebook provides examples of how to manipulate cohorts using standard SQL (via the R library bigrquery) to access BigQuery. 

| Runtime Environments | Value |
| --- | --- |
| CPU Minimum| 2|
| Disksize Minimum | 100 GB |
| Memory Minimum | 13 GB |



**3_R_How_to_read_data_from_BigQuery**     
This notebook shows how to retrieve a subset of data from the 1,000 genomes project public data in two different ways: standard SQL and R coding. 

| Runtime Environments | Value |
| --- | --- |
| CPU Minimum| 2|
| Disksize Minimum | 100 GB |
| Memory Minimum | 13 GB |


**4_Python_environment_setup**    
Run this notebook to set up the workspace before the Hail tutorial notebook.

| Runtime Environments | Value |
| --- | --- |
| CPU Minimum| 2|
| Disksize Minimum | 100 GB |
| Memory Minimum | 13 GB |


**5_Hail_Short_Demo_Mock_Data**     
This small demonstration of Hail code utilizes a mock data set where a diagnosis of Type 2 Diabetes has been randomly assigned to a set of samples from the 1000 genomes data set. The corresponding bmi values of the Type 2 Diabetes cohort have been altered to show the power of Hail tools for comparing phenotypes.  **Avoid storage costs:** Because this notebook outputs tsv, text, ipynb and html files into the general workspace bucket, you will incur additional storage costs if you don't remove these (or delete the workspace) after using the notebook.

| Runtime Environments | Value |
| --- | --- |
| CPU Minimum| 2|
| Disksize Minimum | 100 GB |
| Memory Minimum | 13 GB |
 
-----

## Time and cost 
This workspace focuses on the use of notebooks, thus the time and cost of completing the tutorial depends on the runtime environment of your notebook and the length of time you spend actively working in the notebook. With the runtime environments above, users can expect the cost to be much less than a dollar an hour for each notebook. The specific cost will be displayed on the top right corner of your screen, next to the notebook machine options. 

In addition to the cost of running a notebook, you will incur BigQuery costs when you query data. Querying the first TB of data every month is free. You can find [Google's cost calculator here](https://cloud.google.com/products/calculator/). 

-----

## Appendix

### GATK @ BroadE 2019 in the Terra Support Center

Get yourself oriented with the entire workshop in the [Terra Support Center](https://broadinstitute.zendesk.com/hc/en-us/community/topics). (more on Terra Support below).

### Terra documentation and support

Documents and helpful guides to support your journey through Terra are available in the Terra Support Center. Navigate there by following the “Learn About Terra” link in the left-side menu. At the time of this workshop, we are still actively writing and publishing documents but we’ve got a good set of docs in the Quick Start Guide to get you going.

Please post any questions or concerns to our forum site : [Terra Forum](https://broadinstitute.zendesk.com/hc/en-us/community/topics/360000500432-General-Discussion).
