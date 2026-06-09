# French Artistic Heritage in the Metropolitan Museum Collection

## Project Overview

This project explores the representation of French artistic heritage within the Metropolitan Museum of Art Open Access collection. Using museum metadata and digital humanities methods, the project investigates how French cultural heritage is documented, classified, and represented across different museum departments, object categories, and acquisition periods.

The project was developed as part of the course *Open Scholarship in History and the Humanities: Resources, Tools, and Methods for Research Implementation* and follows the principles of reproducible research using GitHub, Jupyter Notebook, and Python.


## Research Question

What aspects of French artistic heritage are most prominently represented in the Metropolitan Museum of Art collection?

Sub-questions:

- Which departments contain the largest number of French heritage objects?
- Which object classifications are most common?
- How is French artistic heritage distributed across acquisition years?
- How does artist nationality contribute to the representation of French heritage?
- What patterns can be identified through museum metadata?


## Dataset

### Source

Metropolitan Museum of Art Open Access Dataset (MetObjects)

Source:
https://github.com/metmuseum/openaccess

### Dataset Description

The Metropolitan Museum of Art provides an openly accessible dataset containing information about hundreds of thousands of museum objects. The dataset includes extensive metadata describing artworks, artists, cultures, departments, classifications, accession information, and historical context.

The dataset was downloaded as a CSV file and analyzed using Python and Jupyter Notebook.

File used:

- MetObjects.csv


## Why This Dataset

This dataset was selected because it provides rich and well-structured metadata suitable for cultural heritage research.

The collection allows researchers to explore museum objects through multiple dimensions, including:

- Culture
- Artist nationality
- Department
- Classification
- Historical period
- Accession information

The dataset is particularly valuable for Digital Humanities research because it combines cultural, historical, and institutional information in a machine-readable format suitable for computational analysis.


## Analytical Approach

The project uses museum metadata as a source for investigating patterns of cultural representation.

The analysis focuses on the following metadata dimensions:

- Culture
- Artist Nationality
- Department
- Classification
- Object Name
- Accession Year

These variables were selected because they provide insights into how French heritage is represented within the museum collection and how institutional collecting practices have evolved over time.


## Metadata Used

The following metadata fields were selected for analysis:

- Culture
- Artist Nationality
- Department
- Classification
- Object Name
- Title
- AccessionYear
- Period
- Dynasty
- Artist Role

These metadata fields support the identification of cultural, historical, and institutional patterns within the collection.


## Workflow

### 1. Data Access

- Downloaded the Metropolitan Museum Open Access Dataset.
- Stored the dataset locally.
- Loaded the dataset into Jupyter Notebook using Pandas.
- Conducted an initial inspection of dataset structure and metadata fields.

### 2. Data Inspection

- Examined dataset dimensions.
- Reviewed column names and metadata availability.
- Explored sample records.
- Identified relevant variables for research purposes.

### 3. Selection and Sampling

- Focused on records associated with French heritage.
- Selected metadata variables relevant to the research question.
- Reduced the dataset to a manageable subset while preserving important contextual information.

### 4. Data Cleaning

- Checked for missing values.
- Inspected metadata consistency.
- Removed unnecessary fields.
- Standardized selected metadata where appropriate.

### 5. Analysis

The analysis explored:

#### Culture Analysis

- Frequency of French cultural representation.

#### Department Analysis

- Distribution of French heritage objects across museum departments.

#### Classification Analysis

- Distribution of object types and classifications.

#### Artist Nationality Analysis

- Representation of French artists within the collection.

#### Accession Year Analysis

- Temporal distribution of acquisitions.
- Identification of acquisition peaks and collecting trends.

### 6. Visualisation

Visualisations were created to support interpretation of the results.

These include:

- Bar charts
- Frequency distributions
- Comparative visualisations
- Temporal trend analysis

### 7. Documentation

The research process was documented throughout the project using:

- Markdown cells in Jupyter Notebook
- GitHub repository documentation
- Version control through GitHub Desktop

### 8. Reproducibility

The workflow was designed to be reproducible.

All major steps are documented and can be re-executed using the provided notebook and dataset.


## Main Findings

### Department Representation

The analysis revealed that French heritage objects are concentrated in a limited number of museum departments.

Departments such as:

- Drawings and Prints
- European Sculpture and Decorative Arts
- Photographs

contain a substantial proportion of French-related objects.

This indicates a strong institutional emphasis on specific forms of French artistic production.

### Classification Representation

Several classifications appear more frequently than others.

Common categories include:

- Prints
- Drawings
- Photographs
- Textiles
- Decorative Arts

These categories dominate the representation of French heritage within the collection.

### Artist Nationality

The analysis suggests that artist nationality provides an important indicator of French artistic heritage.

French artists are represented across multiple departments and classifications, demonstrating the broad influence of French artistic production.

### Accession Year Patterns

The accession year analysis shows that museum acquisitions occurred in distinct waves rather than at a constant rate.

Several acquisition peaks can be observed throughout the twentieth and early twenty-first centuries, suggesting periods of intensified collecting activity.



## Limitations

Several limitations should be considered when interpreting the results:

- Museum metadata may contain missing values.
- Nationality information is not always complete.
- Cultural classifications depend on museum cataloguing practices.
- Metadata representation may not fully capture the complexity of cultural heritage.
- Results are limited to objects included in the Metropolitan Museum Open Access collection.


## Potential Metadata Enrichment

Future work could expand the project through metadata enrichment.

Possible enhancements include:

- Linking artist records with Wikidata.
- Connecting objects to external cultural heritage repositories.
- Integrating geographical information.
- Incorporating historical event data.
- Exploring relationships between artists, movements, and institutions.

Such enrichment would allow more complex analyses of cultural heritage networks and historical contexts.



## Repository Structure

project/

├── data/

│   └── MetObjects.csv

│

├── notebooks/

│   └── heritage_data_analysis.ipynb

│

└── README.md



## Tools Used

- Python
- Pandas
- Matplotlib
- Jupyter Notebook
- GitHub
- GitHub Desktop
- Microsoft Excel



## Reproducibility Statement

This project follows the principles of open and reproducible research.

All data processing, analysis, and visualisation steps are documented within the Jupyter Notebook. The workflow can be reproduced by loading the dataset and executing the notebook from beginning to end.

Version control was maintained through GitHub to ensure transparency and traceability of changes throughout the project.


## Future Work

Future development of this project could include:

- More advanced statistical analysis.
- Metadata enrichment through linked open data.
- Network analysis of artists and institutions.
- Geographic visualisations.
- Comparative studies of multiple cultural groups.
- Interactive visualisations for public exploration.


## Conclusion

This project demonstrates how museum metadata can be used to investigate cultural heritage through computational methods.

By focusing on French artistic heritage within the Metropolitan Museum of Art collection, the analysis reveals patterns of cultural representation across departments, object classifications, artist nationalities, and acquisition periods. The project also highlights the value of open museum data, reproducible workflows, and digital humanities methodologies for cultural heritage research.
