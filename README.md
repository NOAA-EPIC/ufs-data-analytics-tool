# ufs-data-analytics-tool

__Purpose:__ 

The purpose of the tool is to extract additional information regarding the input and baseline datasets residing within the RDHPCS -- in an effort to assist NOAA in the cleaning & restructuring of the current UFS data structure. In this demontration, the tool will be applied against the UFS input and baseline datasets residing within the RDHPC platform, Orion.

__Capabilities:__ 

The tool will be able to perform the following actions:

- Apply feature engineering to obtain additional information regarding the data files. 
  
- Extract all data filenames mapping them to their corresponding relative directory path, 
  root folder, filename, filesize, file format, compiler (if applicable), CNTL folder (if applicable),
  "input" or "restart" file type, resolution (km) category, resolution (C resolution) category. 
  
- Analyze & plot the current storage size of each UFS data file per timestamp per dataset type (input, baseline). 
  Note: At the time at which the tool is being executed, it will extract the data information from the RDHPC
  platform at that time. Thus, the data information of the datasets residing within the RDHPC will be dynamic 
  as the datasets are being cleaned.
  
- Extract number of nodes ("folders") per file to assist in categorization of the folders -- currently, node levels vary.
- Confirm no input data files are being duplicated per UFS Component's root folder and per CNTL folder.
- Categorize, sort by feature, & write restructuring data table to csv file.

__Future Capabilities:__  
- This tool can be used as a skeleton framework for acquiring additional information regarding the data analytics of future datasets of interest (e.g. SRW data, MRW data, etc).
- Construct the hierarchical trees for each unique dataset residing within a RDHPC platform.

__Prerequisite:__

- On Orion, user must sym link from their home directory to the main directory containing the datasets of interest.

__Reference(s):__
- Latest UFS Weather Model Guide:
    - https://ufs-weather-model.readthedocs.io/en/latest/InputsOutputs.html
