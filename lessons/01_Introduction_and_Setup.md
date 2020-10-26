## Introduction

The workflow will be performed in Galaxy.
Log in to https://galaxy.cluster.tufts.edu with your Tufts credentials.

Information on Tufts Galaxy can be found [here](https://it.tufts.edu/research-technology/bioinformatics/tufts-galaxy).

Workflow Overview:

<img src="../img/workflow.png" width="200">

Our dataset is from the publication:

Chang et al. **Next-Generation Sequencing Reveals HIV-1-Mediated Suppression of T Cell Activation and RNA Processing and Regulation of Noncoding RNA Expression in a CD4+T Cell Line.** mBio 2011doi: 10.1128/mBio.00134-11

The raw reads have been downsampled to 1 million reads per file in order to speed up computation.The full dataset is available from NCBI under accession [SRP013224](https://www.ncbi.nlm.nih.gov/sra?term=SRP013224).

The following steps will walk you through how to run the tools. In each step certain parameters are set. If a parameter option appears on the screen but there is no mention of how to set it, leave it at the default. There are questions throughout, which serve to guide you through the results and check your understanding.

## Create a new history
- Click the **+** at the top of the history panel
- Name the history **rnaseq day 1**

<img src="../img/new_history.png" width="200">

## Import the raw data from a shared data library on our server
- Click **Shared Data** on the top menu bar and select **Data Libraries**
- Select **chang_2011**
- Click **Export to History** next to the Search bar and select **As a Collection**
- Click **Continue** to add all files as a list to our current history 
- Name the collection **chang_2011**
- Click **Create list**

You’ll see the collection in your history, you can optionally choose to hide the original files


<img src="../img/chang_2011.png" width="200">

## View Fastq files
- Click on the list **chang_2011** to expand, you’ll see 11 sequencing files with extension **fastq.qz**
- Click on the **eye icon** on the first sequence file **HIV_12hr_rep1** and look at the fastq reads

<details>
<summary> <b>Question 1: The table below shows a line of different symbols that can be used in quality scores from different quality score encodings (black line). The lines of different colors show the range of symbols used in a specific quality encoding. Based on the symbols you see in the quality score line from the fastq read in our dataset, which Illumina quality score encoding appears to be used in our dataset?</b> </summary>
<br>
Answer: Illumina 1.8+ </details> 

<img src="../img/base_qual.png" width="500">

[Next: Process Raw Reads](03_Process_raw_reads.md)

[Previous: Repository Home](./README.md)
