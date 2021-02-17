This is a Capstone 1 Project, where the focus was to get a basic understanding of the macro factors affecting agricultural production.
Here we aimed to predict crop production, given the year, location and external factors, using data science techniques. The project followed the following steps;
- Data Wrangling: Collected Data from various sources USDA, BLS and NOAA websites for related information. In some cases build a web scrapper to extract data that was labor intensive.
- Exploratory Analysis: Answer few initial general questions about the data and the agricultural practice/results. To gain better understanding of the data and the subject.
- Machine Learning: To predict the production values for crops at county-level. Applying preprocessing like feature selection, Category encoding and normalization.

For further details please refer to the code in the Scripts folder, that Jupyter Notebook for easy viewing. All the related documentation is available on Google docs, with the links to each of them in the documents folder. All of the data used is also uploaded here.

### Installation
A brew installation of `GDAL` is required before installating `geopandas` dependency.
```bash
brew install gdal
``` 
For MacOS `big-sur` if you come accross below error while install `GDAL` or `geopandas`,
`clang: error: invalid version number in 'MACOSX_DEPLOYMENT_TARGET=11.0'`
follow the below steps mentioned, reference [here](https://stackoverflow.com/questions/63972113/big-sur-clang-invalid-version-error-due-to-macosx-deployment-target)
1. Run the below command to if any software update fixes it.
    ```bash
    >>> softwareupdate --all --install --force
    Software Update Tool

    Finding available software
    No updates are available.
    ```
2. If the above doesn't fix it, try uninstalling and re-installing `xcode-select` as,
    ```bash
    sudo rm -rf /Library/Developer/CommandLineTools
    sudo xcode-select --install
    ```