The code in this repository is based on that created for my master's thesis at Utah State University, "Using Natural Language Processing to Quantify the Efficacy of Language Simplification as a Communication Strategy."  The goal of the project was to see if people both with and without Parkinson's Disease could intentionally simplify their language, as measured by several lexial richness metrics, to be able to communicate more clearly.  The results indicated that both groups were overall successful at the task and, as judged by soft cosine similarity, were able to overall tell similar stories to the original.  This indicates that simplification could be a useful strategy for people with communication disorders to be more easily understood by others and warrants further research.

The code contained in this repository will allow anyone to repeat the analyses described above, either with synthetic simplifications of the comparison story, or with other texts that fit their own project.  The four folders within contain different types of files.  In the Data folder there is raw data (stories) in the Group 1, Group 2 and Original subfolders.  The Functions folder contains two functions which had to be written/adapted to suit my purposes, one to calculated an Advanced Guiraud score based on American English words and the other to calculate a Cohen's d effect size statistic.  The Plots folder contains example plots one can use to compare with their own plots generated from working through the example with their own data.  Lastly, the Scripts folder contains the code examples to work through in the format of Juypter Notebooks.

# Instructions

## 1 
To run through this code yourself, you'll need to download each folder and have access to either a local Jupyter Notebook implementation or online via [Google Colab](https://colab.research.google.com/) or similar.  Local versions of JupyterLab or a traditional Juypter Notebook can be downloaded from [Project Jupyter](https://jupyter.org/) or are included in the basic [Anaconda](https://www.anaconda.com/) installation.  

## 2 
If using a local version of Jupyter, you can either download the files to your working directory or simply change the specified save and load paths to your own file path.  If using Colab, they have information on how to directly link to this repository [here](https://colab.research.google.com/github/googlecolab/colabtools/blob/main/notebooks/colab-github-demo.ipynb).

## 3 
To start working through the provided example, you will need to first complete the "Test Original," "Test Group 1" and "Test Group 2" scripts, in any order.  The result of this step will be three data frames, one each for the original text, group 1 and group 2.

## 4 
Then move to either the "Test Lexical Richness Plots" or "Test Statistical Testing" scripts.  The plots script will create box plots with overlaid data points (like this one ![box plot with points](https://github.com/bcnalley/lexical-simplification-nlp/blob/main/Plots/MSTTR_boxplot_points.png?raw=true)).  After running the testing script, you will have results to tests which check normality and homogeneity of variance assumptions for 1 and 2 sample t-tests.

## 5 
Finish with "Test Soft Cosine Similarity."  This script will leave you with a box plot () and soft cosine similarity scores for each story and group of stories.


I hope someone out there finds my example helpful in completing your own research or solving a problem!
