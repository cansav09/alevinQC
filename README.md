## alevinQC

[![Travis CI build status](https://travis-ci.com/csoneson/alevinQC.svg?branch=master)](https://travis-ci.com/csoneson/alevinQC)
[![Codecov.io coverage status](https://codecov.io/github/csoneson/alevinQC/coverage.svg?branch=master)](https://codecov.io/github/csoneson/alevinQC)

The `alevinQC` R package provides functionality for generating QC reports
summarizing the output of [alevin](https://salmon.readthedocs.io/en/latest/alevin.html)
([Srivastava et al., bioRxiv doi:10.1101/335000,
2018](https://www.biorxiv.org/content/early/2018/10/24/335000)). The reports can
be generated in html or pdf format, or as R/Shiny applications.

### Installation:

```
BiocManager::install("csoneson/alevinQC")
```

### Example usage:

```
alevinQCReport(baseDir = system.file("extdata/alevin_example", package = "alevinQC"),
               sampleId = "testSample", 
               outputFile = "alevinReport.html", 
               outputFormat = "html_document",
               outputDir = tempdir(), forceOverwrite = TRUE)
```

For more information, we refer to the package vignette.

![](inst/extdata/alevinQC_screenshot1.png)
![](inst/extdata/alevinQC_screenshot2.png)
