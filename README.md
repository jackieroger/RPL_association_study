# RPL_association_study

This repository contains the code associated with our paper:

Leveraging electronic health records to identify risk factors for recurrent pregnancy loss across two medical centers

Jacquelyn Roger, Feng Xie, Jean Costello, Alice Tang, Jay Liu, Tomiko Oskotsky, Sarah Woldemariam, Idit Kosti, Brian Le, Michael P. Snyder, Linda C. Giudice, Gary M. Shaw, David K. Stevenson, Aleksandar Rajkovic, M. Maria Glymour, Dara Torgerson, Nima Aghaeepour, Hakan Cakmak, Ruth B. Lathi, Marina Sirota

Our study utilized electronic health record (EHR) data that was standardized to the Observational Medical Outcomes Partnership (OMOP) common data model. To replicate this study using another OMOP EHR database, follow the query instructions below and then use the code in these R markdown scripts to filter your patients, aggregate diagnoses, implement analyses, analyze results, and create figures.

Query instructions:
1. Query your OMOP database to identify patients that meet the initial inclusion criteria for the RPL group. The initial RPL criteria is: any record of pregnancy loss (as defined in the pregnancy loss, recurrent pregnancy loss, and history of pregnancy loss sections of Supplementary File 1).
2. Query your OMOP database to identify patients that meet the initial inclusion criteria for the Control group. The initial Control criteria is: any record of live-birth (as defined in the live-birth section of Supplementary File 1).
3. Query the included RPL and Control patients' subsets of the following OMOP tables: person, condition_occurrence, observation, procedure_occurrence, and visit_occurrence.
4. The inputs for Rmd 01 are: the table subsets from #3, the OMOP concept table, and the concept lists in Supplementary File 1.

System requirements: This code was developed and tested using R version 4.0.2 on the macOS Monterey version 12.6.3. Diagnosis aggregation used Phecodes version 1.2, and the mapping files can be downloaded from their website: https://phewascatalog.org/phecodes

Installation guide: To run the code, clone this repository. Cloning typically takes a minute or less.

The data used for our project (UCSF and Stanford EHR) is not publically available. UCSF-affiliated individuals can request access to UCSF EHR data by contacting UCSF Information Commons (Info.Commons@ucsf.edu). Stanford’s EHR data is managed through the Stanford Research Repository (https://med.stanford.edu/starr-tools.html). Individuals not affiliated with UCSF may request to set up an official collaboration with a UCSF-affiliated investigator by contacting the principal investigator, Marina Sirota (marina.sirota@ucsf.edu). Requests should be processed within a couple of weeks.

License:

    Our RPL association study code analyzes EHR data from RPL and control patients, and identifies diagnoses associated with RPL.
    Copyright (C) 2023 Jacquelyn Roger

    This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this program.  If not, see <http://www.gnu.org/licenses/>.

    Contact: jacquelyn.roger@ucsf.edu
    Located at Bakar Institute at UCSF
