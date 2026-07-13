# French Artistic Heritage in the Metropolitan Museum Collection

## Project Overview

This project investigates how French artistic heritage is represented within the Metropolitan Museum of Art Open Access collection. It uses museum metadata and digital humanities methods to examine patterns across cultural classifications, artist nationalities, museum departments, object classifications, and accession years.

## Research Question

**What aspects of French artistic heritage are most prominently represented in the Metropolitan Museum of Art collection?**

## Dataset Source and Licensing

The original data comes from the [Metropolitan Museum of Art Open Access repository](https://github.com/metmuseum/openaccess). The Met makes its Open Access data available under the Creative Commons Zero (CC0) public-domain dedication, supporting reuse, analysis, and redistribution.

The original `MetObjects.csv` file is not included in this repository because it exceeds GitHub’s file-size limit. The filtered data used for this project is available here:

- [Filtered French heritage dataset](https://github.com/lamyae-d/open-scholarship-project/blob/main/Data/french_heritage_objects.csv)
- [Jupyter Notebook](https://github.com/lamyae-d/open-scholarship-project/blob/main/notebooks/heritage_data_analysis.ipynb)

## Tools Used

| Tool | Purpose |
|---|---|
| Python | Data processing and analysis |
| pandas | Loading, filtering, and analysing metadata |
| Matplotlib | Creating visualisations |
| Jupyter Notebook | Combining code, results, and documentation |
| GitHub and GitHub Desktop | Repository management and version control |
| Microsoft Excel | Initial data inspection |

## Key Findings

### How French Heritage Objects Were Identified

Step 6 above (filtering) selects any record where either the Culture field equals "French" or the Artist Nationality field equals "French":

french_df = df[(df["Culture"] == "French") | (df["Artist Nationality"] == "French")]

This OR condition is why both metadata fields are used together — an object only needs to match one of the two to be included.
## Workflow

The project follows a reproducible workflow:

1. Data collection from the [Metropolitan Museum Open Access repository](https://github.com/metmuseum/openaccess).
2. Loading the dataset into Jupyter Notebook using pandas.
3. Initial inspection of dataset structure and metadata using `df.shape` and `df.head()`. The dataset contains 484,956 rows and 54 columns.
4. Missing value analysis using `df.isnull().sum()` to identify columns with incomplete data.
5. Selection of relevant metadata variables.
6. Filtering records related to French artistic heritage, producing the [filtered dataset](https://github.com/lamyae-d/open-scholarship-project/blob/main/Data/french_heritage_objects.csv).
7. Exploratory data analysis using the [notebook](https://github.com/lamyae-d/open-scholarship-project/blob/main/notebooks/heritage_data_analysis.ipynb).
8. Creation of visualisations, see [Department Distribution](https://github.com/lamyae-d/open-scholarship-project/blob/main/notebooks/department_distribution.png), [Classification Distribution](https://github.com/lamyae-d/open-scholarship-project/blob/main/notebooks/classification_distribution.png), [Culture and Artist Comparison](https://github.com/lamyae-d/open-scholarship-project/blob/main/notebooks/culture_artist_comparison.png), and [Accession Year Analysis](https://github.com/lamyae-d/open-scholarship-project/blob/main/notebooks/accession_year_analysis.png).
9. Interpretation of results.
10. Documentation and publication through GitHub.
### Key Functions Used

The analysis primarily relies on pandas functions such as read_csv(), value_counts(), filtering operations, and missing value inspection to explore and prepare the dataset. Matplotlib was used to create visualisations of department distributions, classification distributions, metadata comparisons, and accession year patterns. These functions enabled the identification and interpretation of trends within the museum metadata.

### Department Analysis

French heritage objects are strongly concentrated in the following departments:

- Drawings and Prints
- European Sculpture and Decorative Arts
- Costume Institute
- Photographs

This suggests that French artistic heritage is particularly represented through graphic arts, decorative arts, fashion, and photography.

### Classification Analysis

The most common object classifications include:

- Prints
- Drawings
- Photographs
- Textiles
- Paintings

These classifications dominate the museum's representation of French artistic heritage.

### Culture and Artist Nationality Comparison

French heritage is represented through both cultural classification and artist nationality. Artist nationality appears more frequently than cultural classification, indicating that French artists play an important role in the museum's documentation of French heritage.

### Accession Year Analysis

The accession year analysis reveals several acquisition peaks rather than a continuous collecting pattern. This indicates periods during which French heritage objects entered the collection at particularly high rates.

## FAIR Principles

This project follows the FAIR principles for research data:

**Findable** – The dataset is publicly available through the Metropolitan Museum Open Access repository.

**Accessible** – The dataset can be freely downloaded and accessed by researchers.

**Interoperable** – Metadata is provided in a structured CSV format that can be used across different software environments.

**Reusable** – Open licensing and detailed workflow documentation support future reuse.

## Peer Review and Testing

The repository and Jupyter Notebook were reviewed from the perspective of a new user to evaluate the clarity of documentation, workflow transparency, and reproducibility. Particular attention was given to whether the research question, data source, analytical workflow, and visualisations could be understood without additional explanation.

The review confirmed that the workflow can be followed through the README and notebook documentation. The repository structure, code organisation, and visualisations support the reproducibility of the analysis.

## Reproducibility

All stages of the research process are documented within the Jupyter Notebook. The notebook contains the complete workflow, code, visualisations, interpretations, and conclusions necessary to reproduce the analysis.

Version control was maintained through GitHub and GitHub Desktop to ensure transparency and traceability of project development.

## Repository Structure

open-scholarship-project/
│
├── Data/
│   └── french_heritage_objects.csv
│
├── notebooks/
│   ├── heritage_data_analysis.ipynb
│   ├── department_distribution.png
│   ├── classification_distribution.png
│   ├── culture_artist_comparison.png
│   ├── french_heritage_identification.png
│   └── accession_year_analysis.png
│
└── README.md

## Documentation Decisions

Several documentation decisions were made during the project to improve transparency and reproducibility. The workflow, analytical steps, interpretations, and visualisations were documented directly within the Jupyter Notebook. Repository organisation and version control were maintained through GitHub and GitHub Desktop to support traceability and future reuse of the project.

## AI-Assisted Development

ChatGPT was used as a supplementary learning and troubleshooting tool during the development of this project, particularly for Python programming, GitHub workflow, and documentation support.

## Limitations

Several limitations should be considered when interpreting the results:

- Missing values exist in Culture and Artist Nationality.
- Metadata cannot fully represent the complexity of cultural identity.
- Cultural classifications depend on institutional cataloguing practices.
- The analysis is limited to objects contained within the Metropolitan Museum collection.
- Results rely on metadata rather than direct examination of museum objects.
- Re-running the notebook with a freshly downloaded MetObjects.csv from the Metropolitan Museum Open Access repository may produce slightly different results than documented here (for example, different Department Analysis numbers), since the museum periodically updates its dataset. For exact reproducibility of the results reported in this README, use the already-committed `Data/french_heritage_objects.csv` rather than re-downloading and re-filtering the source data.

## Future Work

Potential extensions of this project include:

- Metadata enrichment through Wikidata.
- Geographic visualisations of object origins.
- Analysis of artistic movements and historical periods.
- Comparative studies of multiple cultural groups.
- Interactive visualisations for public exploration.

## Conclusion

This project demonstrates how museum metadata can be used to investigate cultural heritage through computational and digital humanities methods.

By focusing on French artistic heritage within the Metropolitan Museum of Art collection, the analysis identifies patterns of representation across cultural classifications, artist nationalities, museum departments, object classifications, and acquisition history.

The results show that French heritage occupies a significant position within the collection and that open data enables transparent, reproducible, and accessible cultural heritage research.
