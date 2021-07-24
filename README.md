# Data-Cleaning
We have the data here for an RNA-Seq experiment of a cancer tumor tissue sequenced at different time points.
To reduce experimental errors, the cells of the tissue were replicated into three pools for the tissue and each pool of cells was sequenced at the beginning(0hrs), 4hrs, 5hrs, 6hrs...12hrs. As a result, we have measurements of each gene in 30 samples.

gene_data_anomaly.csv - contains the normalized counts after RNA sequencing for every gene for samples S1, S2,..., S30.

Due to an anomaly in the system, the data has missing values (NaNs) at certain data points. This is a bottleneck for further processing of data and we need to deal with this missing data.
