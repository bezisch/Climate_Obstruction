# Climate_Obstruction

This repository contains the code and data for building and running a 
Named Entity Recognition (NER) pipeline on a corpus of corporate documents, see here: 
https://www.budget.senate.gov/imo/media/doc/fossil_fuel_report1.pdf

## Overview

The pipeline proceeds in three steps: preparing entities from LexisNexis 
sources as additional source, creating a structured NER codebook, and running the codebook against 
the document corpus. The resulting codebook and entity tables form the basis 
of the dataset publication.

## Files

Creation_NER_Codebook.ipynb constructs the NER codebook from raw entity 
inputs. It outputs NER_Codebook_1559.xlsx, which lists all 1559 named entities 
with their categories.

Preparation_LexisNexis_Entities.ipynb prepares and cleans the entity data 
extracted from LexisNexis sources.

Run_NER_Codebook.ipynb runs the finalized codebook against the full document 
corpus and produces entity match outputs.

We add the .html files for readability without a Jupyter environment.

## Data

NER_Codebook_1559.xlsx is the main codebook output with 1559 entities.
df_a_airtable.xlsx and df_b_airtable.xlsx are the Airtables for both datasets (their difference is explained in the manuscript).


## Related

This repository is part of the broader Corporate Obstructionism research 
project. The NER codebook feeds into the dataset publication as well as the 
analysis of corporate climate obstruction strategies.
