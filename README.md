# Disease data integration

Background: This repo is for the data integration of the HLCA v2 datasets. 

The notebooks included are:

### Data preprocessing and integration
This includes quality control and data integration pipeline

### Outlier dataset analysis
For datasets that did not integrate well, I conducted analysis:
1. technical aspects: PCR analysis and checked transferred labels
3. biological aspects: DE across datasets, COPD-specific gene expression comparison across studies
#### Conclusions
- batch effects strong from:
    - low seq depth
    - fragment end
    - few genes with strongly different expression patterns
- Next steps
    - improve feature selection: Remove outlier genes!
    - low Quality → don’t use
    - Don’t use sample ID for HVG selection
    - Try healthy/normal integration first
        - take all the normal datasets
    - Try adding another 5’ dataset
### Data evaluation: purity score

### Data evaluation: based on COPD-specific marker genes
Test the score for:
COPD-associated gene signatures (take max score per cluster only)
