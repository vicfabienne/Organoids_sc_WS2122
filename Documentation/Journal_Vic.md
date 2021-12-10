# Organoid Single Cell Seminar

## 10/12/2021
### Plan:
In order to be able to process all the datasets we need in short time I'm thinking about using PiGx scRNA-seq
to do the preprocessing and QC reporting and only using the results for further downstream processing. The pipeline will
output `SingleCellExperiment` objects that are made for Bioconductor. They can be converted to the Python `AnnData` object
by using the [zellkonverter](https://bioconductor.org/packages/devel/bioc/vignettes/zellkonverter/inst/doc/zellkonverter.html)
package.

all the single-cell datasets that we need:
    1. organoid - cntrl 1
    2. organoid - cntrl 2
    3. atlas - day9
    4. atlas - day27 - donor 1
    5. atlas - day27 - donor 2

1. finish ScanPy tutorial to know about the basics
2. install PiGx scRNA and run the test
3. set up a scalable environment for the single cell data sets - start with one: organoid - cntrl 1
4. run PiGx for it
5. try to make sense from the output
6. try to convert the output
7. do some scanpy downstream analysis