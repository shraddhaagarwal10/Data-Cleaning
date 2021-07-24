# Data-Cleaning
### Info About File:
We have the data here for an RNA-Seq experiment of a cancer tumor tissue sequenced at different time points.
To reduce experimental errors, the cells of the tissue were replicated into three pools for the tissue and each pool of cells was sequenced at the beginning(0hrs), 4hrs, 5hrs, 6hrs...12hrs. As a result, we have measurements of each gene in 30 samples.

gene_data_anomaly.csv - contains the normalized counts after RNA sequencing for every gene for samples S1, S2,..., S30.

Due to an anomaly in the system, the data has missing values (NaNs) at certain data points. This is a bottleneck for further processing of data and we need to deal with this missing data.
### Task:
Locate the genes which have missing values for certain samples.

Case 1: 
If a gene has a missing value for all three replicates of any time point in the dataset, remove the gene completely from the dataset.

Case 2:
If a gene has a missing value for one of the three replicates of any time point, fill it with the mean of the values for the other two replicates.

Case 3:
If a gene has a missing value for two of the three replicates of any time point, fill both the missing values with the value of the third non-missing replicate at that time point.

After cleaning the data, save the resolved gene anomaly file.
