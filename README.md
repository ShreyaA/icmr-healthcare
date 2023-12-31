<h1 >Problem Statement </h1>

ICMR wants to analyze different types of cancers, such as breast cancer, renal cancer, colon cancer, lung cancer, and prostate cancer becoming a cause of worry in recent years. They would like to identify the probable cause of these cancers in terms of genes responsible for each cancer type. This would lead us to early identification of each type of cancer reducing the fatality rate.
Dataset Details:
The input dataset contains 802 samples for the corresponding 802 people who have been detected with different types of cancer. Each sample contains expression values of more than 20K genes. Samples have one of the types of tumors: BRCA, KIRC, COAD, LUAD, and PRAD.

<h2> Project Task: Week 1 </h2>
<ul>
  <li> Exploratory Data Analysis: Merge both the datasets. Plot the merged dataset as a hierarchically-clustered heatmap.</li>
  <li> Perform Null-hypothesis testing. </li>
  <li> Dimensionality Reduction:
Each sample has expression values for around 20K genes. However, it may not be necessary to include all 20K genes expression values to analyze each cancer type. Therefore, we will identify a smaller set of attributes which will then be used to fit multiclass classification models. </li>
</ul>
So, the first task targets the dimensionality reduction using various techniques such as, PCA, LDA, and t-SNE. 
  Input: Complete dataset including all genes (20531)
Output: Selected Genes from each dimensionality reduction method

<h2> Project Task: Week 2 </h2>
Clustering Genes and Samples:
Our next goal is to identify groups of genes that behave similarly across samples and identify the distribution of samples corresponding to each cancer type. Therefore, this task focuses on applying various clustering techniques, e.g., k-means, hierarchical and mean shift clustering, on genes and samples.
First, apply the given clustering technique on all genes to identify:
<ul>
  <li>Genes whose expression values are similar across all samples</li>
  <li>Genes whose expression values are similar across samples of each cancer type</li>
</ul>
Next, apply the given clustering technique on all samples to identify:
<ul>
  <li>Samples of the same class (cancer type) which also correspond to the same cluster</li>
  <li>Samples identified to be belonging to another cluster but also to the same class (cancer type)</li>
</ul>

Building Classification Model(s) with Feature Selection:
Our final task is to build a robust classification model(s) for identifying each type of cancer. It also aims at the to do feature selection in order to identify the genes that help in classifying each cancer type.

<h2> Sub-tasks: </h2>
<ul>
  <li>Build a classification model(s) using multiclass SVM, Random Forest, and Deep Neural Network to classify the input data into five cancer types </li>
  <li>Apply the feature selection algorithms, forward selection and backward elimination to refine selected attributes (selected in Task-2) using the classification model from the previous step </li>
  <li>Validate the genes selected from the last step using statistical significance testing (t-test for one vs. all and F-test) </li>
</ul>

Download the Data sets from https://www.dropbox.com/sh/8q39v4rvo9hq7hy/AAAfAs9J12eevM_9_jPySJ1xa?dl=0.
