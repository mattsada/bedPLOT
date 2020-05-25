# invPLOT
Set of custom R scripts for visualizing (using ggplot2) genomic inversions.

## Description
Set of custom R scripts that takes a tab-delimited bed-file (including header) with the following fields specified: `chr---start---end---size`
and outputs a set number of figures that visualizes genomic inversions annotated in bed file. Package was developed to standardize inversion plotting, but scripts will execute on any type of structural variation (SV) pressent ininput bed-file. 

## Examples
All example figures were generated by implementing designed funtions on test-data (included) drawn from 49 Strand-seq libraries (reference sample HG0002).

### 01 - Size distribution density 
Script `SV.size.dens.R` takes the total number of SVs pressent in the input bed file and plots the size distribution. Using a kernel density estimate to show the probability density function of the variable. 

![SV.size.dens.R](https://github.com/mattsada/invPLOT/blob/master/example_figures/SV.size.dens.R.png)

### 02 - Size distribution box plot
Script `SV.size.box.R` plots the size distributions of SVs pressent in input bed file. Outliers, first and fourth quantile as well as mean inversion size are visualized in the same plot.

![SV.dens.box.R](https://github.com/mattsada/invPLOT/blob/master/example_figures/SV.size.box.R.png)

### 03 - Size distribution violine plot
Script `SV.size.violine.R` plots SV size distribution as a un-trimmed violine plot, annotating quantiles as well as SV size density.

![SV.size.violine.R](https://github.com/mattsada/invPLOT/blob/master/example_figures/SV.size.violin.R.png)


