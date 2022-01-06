# About

In order to accelerate research on pediatric sleep and its connection to health, [Nationwide Children's Hospital (NCH)](https://www.nationwidechildrens.org/) and [Carnegie Mellon University (CMU)](https://www.ece.cmu.edu/) introduce the NCH Sleep DataBank. This dataset has 3,984 pediatric sleep studies on 3,673 unique patients conducted at NCH in Columbus, Ohio, USA between 2017 and 2019, along with the patients' longitudinal clinical data. The published polysomnography (PSG) contains the patient's physiological signals as well as the technician’s assessment of the sleep stages and descriptions of additional irregularities.

The novelties of this dataset include:

1. **Size:** Its large size is suitable for discovering new scientific insights via data mining.
2. **Patient population:** It explicitly focuses on pediatric patients.
3. **Clinical setting:** The sleep studies were gathered in the real-world clinical setting at NCH as opposed to, for example, a controlled clinical trial.
4. **Rich set of clinical data:** The accompanying 5.6 million records of clinical data are extracted from the EHR, and are separated into encounters, medications, measurements (e.g. body mass index), diagnoses, and procedures.

The NCH Sleep DataBank is a valuable resource for advancing automatic sleep scoring and real-time sleep disorder prediction, among many other potential scientific discoveries. Accompanying code in Python to assist users in interacting with the dataset is [published on GitHub](https://github.com/liboyue/sleep_study).

The National Sleep Research Resource is grateful to the [Nationwide Children's Hospital (NCH)](https://www.nationwidechildrens.org/) and [Carnegie Mellon University (CMU)](https://www.ece.cmu.edu/) team for sharing these data.

## Data preamble and access restrictions

The NCH Sleep DataBank is only available for non-commercial use.

## Citation and acknowledgement

When using this dataset, please cite the following:

> [Zhang GQ, Cui L, Mueller R, Tao S, Kim M, Rueschman M, Mariani S, Mobley D, Redline S. The National Sleep Research Resource: towards a sleep data commons. J Am Med Inform Assoc. 2018 Oct 1;25(10):1351-1358. doi: 10.1093/jamia/ocy064. PMID: 29860441; PMCID: PMC6188513.](https://pubmed.ncbi.nlm.nih.gov/29860441/)
>
> [Lee H, Li B, DeForte S, Splaingard M, Huang Y, Chi Y, & Lin S. NCH Sleep DataBank: A Large Collection of Real-world Pediatric Sleep Studies. Preprint at https://arxiv.org/abs/2102.13284 (2021)](https://arxiv.org/abs/2102.13284)

Please include the following text in the Acknowledgements:

> NCH Sleep DataBank was supported by the National Institute of Biomedical Imaging and Bioengineering of the National Institutes of Health under Award Number R01EB025018. The National Sleep Research Resource was supported by the U.S. National Institutes of Health, National Heart Lung and Blood Institute (R24 HL114473, 75N92019R002).

## Data overview

**[/datasets](:files_path:/datasets)** <br/> Covariate datasets derived from the original [health_data files](:files_path:/health_data). The NSRR team recommends using `nchsdb-dataset-harmonized`, which contains variables (e.g., :nsrr_age:, :nsrr_bmi:) that overlap with other NSRR harmonized datasets.

**[/health_data](:files_path:/health_data)** <br/> Data (CSV) from the NCH clinical data warehouse. [Click here for an overview of the file formats and contents](:files_path:/health_data/Sleep_Study_Data_File_Format.pdf).

**[/sleep_data](:files_path:/sleep_data)** <br/> Raw physiological data (EDF) and annotations (TSV) from overnight polysomnography.

## Change log

*January 2022*
- Add [covariate datasets](:files_path:/datasets) derived from CSV files in [/health_data folder](:files_path:/health_data)

*October 2021*
- Unpaused approval of data requests. Replaced **DIAGNOSIS.csv** in **health_data** folder. Note from the contributor: *We replaced columns ('DX_CODE', 'DX_NAME', 'DX_ALT_CODE', 'CLASS_OF_PROBLEM', ‘CHRONIC_YN') corresponding a rare diagnosis with "redacted" to prevent potential privacy issues. A rare diagnosis is defined as a diagnosis that has less than 10 unique patients from all NCH records from 01/01/2000 to 12/31/2020.*

*September 2021*
- Pause approval of data requests

*February 2021*

- Make NCHSDB dataset available for data requests
