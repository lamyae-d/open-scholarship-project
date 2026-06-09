# French Artistic Heritage in the Metropolitan Museum Collection

## Project Overview

This project investigates the representation of French artistic heritage within the Metropolitan Museum of Art Open Access collection. Using museum metadata and digital humanities methods, the project explores how French cultural heritage is documented, classified, collected, and represented across different museum departments, object categories, artist nationalities, and acquisition periods.

The project was developed as part of the course *Open Scholarship in History and the Humanities: Resources, Tools, and Methods for Research Implementation* and follows principles of open, transparent, and reproducible research using Python, Jupyter Notebook, and GitHub.

---

## Research Question

### Main Research Question

What aspects of French artistic heritage are most prominently represented in the Metropolitan Museum of Art collection?

### Sub-Questions

- Which museum departments contain the largest number of French heritage objects?
- Which object classifications are most frequently associated with French heritage?
- How is French heritage represented through culture and artist nationality?
- During which periods were French heritage objects most actively acquired?
- What patterns of representation can be identified through museum metadata?

---

## Key Findings

The analysis demonstrates that French artistic heritage occupies a significant position within the Metropolitan Museum collection.

The largest concentrations of French heritage objects are found in the Drawings and Prints department, followed by European Sculpture and Decorative Arts and Photographs. This indicates a strong institutional representation of French visual and graphic arts.

The classification analysis reveals that prints, drawings, and photographs are the most common object categories associated with French heritage. These categories account for a substantial proportion of French-related records in the collection.

The comparison between Culture and Artist Nationality shows that French heritage is represented both through cultural classification and through artists identified as French. Artist nationality appears more frequently than cultural classification, suggesting that artists play a central role in documenting French heritage within the museum.

The accession year analysis reveals distinct acquisition waves rather than a continuous collecting pattern. Several periods show notable increases in acquisitions, indicating moments when French heritage entered the collection at particularly high rates.

---

## Dataset

### Source

Metropolitan Museum of Art Open Access Dataset (MetObjects)

Dataset Repository:

https://github.com/metmuseum/openaccess

### Dataset Description

The Metropolitan Museum of Art Open Access dataset provides publicly available metadata for hundreds of thousands of museum objects. The dataset contains information about artworks, artists, cultures, departments, classifications, historical periods, and acquisition records.

The dataset was downloaded as a CSV file and analyzed using Python and Jupyter Notebook.

### Data File

- MetObjects.csv

---

## Why This Dataset

This dataset was selected because it provides extensive metadata suitable for cultural heritage research and digital humanities analysis.

The collection allows researchers to investigate museum objects through multiple dimensions, including cultural affiliation, artist information, object classification, departmental organization, historical period, and acquisition history.

The dataset is particularly valuable because it combines cultural, historical, and institutional information in a structured and machine-readable format that supports computational analysis.

---

## Analytical Approach

This project uses museum metadata as a source for investigating patterns of cultural representation.

The analysis focuses on how French artistic heritage is represented through metadata fields that describe:

- Cultural identity
- Artist identity
- Institutional categorization
- Object classification
- Acquisition history

The project combines exploratory data analysis, descriptive statistics, and visualization techniques to identify patterns within the collection.

---

## Metadata Used

The following metadata variables were selected for analysis:

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

These variables provide insights into cultural, historical, and institutional dimensions of French heritage representation.

---

## Workflow

### 1. Data Access

- Downloaded the Metropolitan Museum Open Access Dataset.
- Stored the dataset locally.
- Imported the dataset into Jupyter Notebook using Pandas.
- Conducted an initial inspection of dataset structure and available metadata.

### 2. Data Inspection

- Examined dataset dimensions.
- Reviewed metadata fields.
- Displayed sample records.
- Identified variables relevant to the research question.

### 3. Data Selection

- Focused on records associated with French heritage.
- Selected metadata fields relevant to cultural heritage analysis.
- Reduced the dataset to a research-specific subset.

### 4. Data Cleaning

- Checked for missing values.
- Evaluated metadata completeness.
- Inspected metadata consistency.
- Prepared selected variables for analysis.

### 5. Exploratory Analysis

The following analyses were conducted:

#### Culture Distribution

Examined the frequency of cultural classifications within the dataset and identified the representation of French culture.

#### Department Distribution

Investigated which museum departments contain the largest numbers of French heritage objects.

#### Classification Distribution

Analyzed the most common object classifications associated with French heritage.

#### Artist Nationality Analysis

Explored the role of French artists in the collection and compared nationality-based representation with culture-based representation.

#### Accession Year Analysis

Investigated temporal acquisition patterns and identified periods of intensified collecting activity.

### 6. Visualisation

Visualizations were created to support interpretation and communication of findings.

These include:

- Frequency distributions
- Bar charts
- Comparative visualizations
- Temporal trend visualizations

### 7. Interpretation

The results were interpreted within the context of cultural heritage representation and museum collecting practices.

Patterns identified through metadata were used to answer the research question and evaluate the representation of French heritage within the collection.

### 8. Documentation

All stages of the research process were documented within the Jupyter Notebook and GitHub repository.

### 9. Reproducibility

The workflow was designed to be reproducible and transparent.

The notebook contains all code, analysis steps, visualizations, and interpretations necessary to reproduce the results.


## Analysis Summary

### Culture Analysis

The culture analysis identified French culture as one of the most frequently represented cultural categories within the collection.

### Department Analysis

French heritage objects are concentrated in a relatively small number of departments, particularly:

- Drawings and Prints
- European Sculpture and Decorative Arts
- Photographs
- Costume Institute

This suggests that French heritage is especially represented through visual, decorative, and graphic arts.

### Classification Analysis

The classification analysis revealed that the most common object categories include:

- Prints
- Drawings
- Photographs
- Textiles
- Decorative arts

These categories dominate the museum's representation of French artistic heritage.

### Culture and Artist Nationality Comparison

The comparison between Culture and Artist Nationality showed that French heritage is represented through both cultural classification and artist identity.

The larger number of records associated with French artists suggests that artist nationality is a particularly important dimension of French heritage representation within the collection.

### Accession Year Analysis

The accession year analysis revealed several acquisition peaks across the twentieth and early twenty-first centuries.

These peaks indicate periods during which French heritage objects entered the collection at increased rates, reflecting changing museum collecting priorities and acquisition opportunities.


## Limitations

Several limitations should be considered when interpreting the results:

- Museum metadata may contain missing values.
- Artist nationality information is not always complete.
- Cultural classifications depend on institutional cataloguing decisions.
- Metadata cannot fully capture the complexity of cultural identity.
- Results are limited to objects available within the Metropolitan Museum Open Access collection.
- The analysis relies on metadata rather than direct examination of objects.


## Potential Metadata Enhancement

Future work could improve the dataset through metadata enrichment.

Possible enhancements include:

- Linking artist records with Wikidata.
- Connecting objects to external cultural heritage repositories.
- Integrating geographical information.
- Adding information about artistic movements.
- Incorporating historical and biographical data.

Such enrichment would support more advanced cultural heritage analysis and provide broader historical context.


## Repository Structure

project/

├── Data/

│   └── MetObjects.csv

│

├── heritage_data_analysis.ipynb

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

All data processing, analysis, visualization, and interpretation steps are documented within the Jupyter Notebook. The workflow can be reproduced by loading the dataset and executing the notebook from beginning to end.

Version control was maintained through GitHub and GitHub Desktop to ensure transparency and traceability of project development.


## Future Work

Future extensions of this project may include:

- Advanced statistical analysis.
- Metadata enrichment using linked open data.
- Network analysis of artists and institutions.
- Geographic visualizations.
- Comparative studies of multiple cultural groups.
- Interactive visualizations for public exploration.


## Conclusion

This project demonstrates how museum metadata can be used to investigate cultural heritage through computational and digital humanities methods.

By focusing on French artistic heritage within the Metropolitan Museum of Art collection, the analysis identifies patterns of representation across cultural classifications, artist nationalities, museum departments, object classifications, and acquisition periods.

The results show that French heritage occupies a prominent position within the collection and that metadata analysis provides valuable insights into museum collecting practices and cultural representation. The project also highlights the importance of open data, reproducible workflows, and transparent research methods for cultural heritage studies.
