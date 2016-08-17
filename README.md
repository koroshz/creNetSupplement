# creNetScripts
Example runs and command line scripts for facilitating creNET runs.

##USAGE##

```{R}
./runCreNet.R -n creNet -m test -e entities.txt -r relations.txt -d train_data.txt -t test_data.txt
```


It is assumed that train_data.txt and test_data.txt (if applicable) are tab delimited text files with the following column structure:

1. The first column is the response vector and the column name should be 'y'
2. Other columns are normalized (as in limma for microarray or edgeR for RNA-seq) gene expression data. The column names are assumed to be the entrez id's of the genes. Please note that the data should not be standardaized, only background corrected and normalized. Standardization will be done internally.
