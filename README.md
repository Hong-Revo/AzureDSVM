# AzureDSVM

The AzureDSVM (Azure Data Science Virtual Machine) is an R Package for Data Scientists
working with the Azure compute platform as a complement to the
underlying AzureSMR for controlling [Azure Data Science Virtual Machines](https://docs.microsoft.com/en-us/azure/machine-learning/machine-learning-data-science-provision-vm).

Azure Data Science Virtual Machine (DSVM) is a powerful data science development environment with pre-installed tools and packages that empower data scientists for convenient data wrangling, model building, and service deployment. 

The R package of `AzureDSVM` aims at offering functions that can be conveniently used by R data scientists for operating and using Azure Data Science Virtual Machine (DSVM) elastically and economically within local R session. 

To install the package from github:

    devtools::install_github("Azure/AzureDSVM")

Help pages are also provided for all functions within the
package. With RStudio for example type AzureDSVM into search when the
package is loaded to see a list of functions/help pages or else

    library(help=AzureDSVM)

Note: The package will work with any open source R Session or with
Microsoft R extensions.

# Features

* Elasiticity

    * Deployment of a DSVM with customized information such as machine name, machine size (with compute/memory optimized general-purpose CPU, Nvidia K80/M60 GPU, etc.), operating system (Windows Server 2016, Ubunbut 16.04, and CentOS), authentication method (public key based or password based), etc.
    * Enjoy all benefits of a Windows/Linux DSVM. E.g., all tools for data science work such as R/Python/Julia programming languages, SQL Server, Visual Studio with RTVS, etc., remote working environment via RStudio Server or Jupyter Notebook interface, and machine learning & artificial intelligence packages such as Microsoft CNTK, MXNet, and XGBoost.
    * Execution of R analytics on DSVM(s) with various Microsoft R Server computing contexts such as "local parallel" and "cluster parallel".
    * Seamless interaction with remote R Server session with `mrsdeploy` functions.
    * Post-deployment installation of extension for customizing system environment, reinstalling/uninstalling software, etc.

* Scalability 

    * Deployment of a collection of heterogeneous DSVMs for a group of data scientists.
    * Scale up DSVM and form them into a cluster for parallel/distributed computation with Microsoft R Server backend. 
    
* Usability

    * Deploy, start, stop, and delete DSVM(s) on demand.
    * Monitor data consumption and estimate expense of using DSVM(s) with hourly aggregation granularity.

# Tutorials

To get started with this package, see the Vignettes:

* [Get started](https://github.com/Azure/AzureDSVM/blob/master/vignettes/00Introduction.Rmd)
* [Deployment of a single DSVM](https://github.com/Azure/AzureDSVM/blob/master/vignettes/10Deploy.Rmd)
* [Deployment of multiple DSVMs](https://github.com/Azure/AzureDSVM/blob/master/vignettes/20Multi.Rmd)
* [Do computation on a single DSVM or a cluster of DSVMs](https://github.com/Azure/AzureDSVM/blob/master/vignettes/30Compute.Rmd)
* [Monitor data consumption and expense spent on using DSVM(s)](https://github.com/Azure/AzureDSVM/blob/master/vignettes/40Cost.Rmd)
* Putting all together
    * [Use case - k-means clustering](https://github.com/Azure/AzureDSVM/blob/master/vignettes/60Kmeans.Rmd)
    * [Use case - Hot spots analysis](https://github.com/Azure/AzureDSVM/blob/master/vignettes/70Hotspot.Rmd)
    * [Use case - Binary classification](https://github.com/Azure/AzureDSVM/blob/master/vignettes/80ModelSelect.Rmd)

# Code of Conduct

This project has adopted the [Microsoft Open Source Code of
Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct
FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com)
with any additional questions or comments.
