# RPL_association_study

This repository contains the code associated with our paper: Risk factors for recurrent pregnancy loss from electronic health record data in two medical centers: a case-control study.

To replicate this study on another OMOP EHR database, follow the query instructions below and then use the code in Rmds 01-13 to filter your patients, aggregate diagnoses, implement analyses, analyze results, and make figures.

Query instructions:
1. Query your OMOP EHR database to identify patients that meet the initial inclusion criteria for the RPL group. The initial RPL criteria is: any record of pregnancy loss (as defined in the pregnancy loss, recurrent pregnancy loss, and history of pregnancy loss sections of Supplementary File 1).
2. Query your OMOP EHR database to identify patients that meet the initial inclusion criteria for the Control group. The initial Control criteria is: any record of live-birth (as defined in the live-birth section of Supplementary File 1).
3. Query the included RPL and Control patients' subsets of the following OMOP tables: person, condition_occurrence, observation, procedure_occurrence, and visit_occurrence.
4. The inputs for Rmd 01 are: the table subsets from #3, the OMOP concept table, and the concept lists in Supplementary File 1.
