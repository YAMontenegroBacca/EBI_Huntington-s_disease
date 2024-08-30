### English Version 
# Data Management
In order to ensure the integrity and quality of the data obtained and manipulated, as well as the transparency and reproducibility of the analyses performed, the following protocol has been developed for data management:

## Types of Data:
- **Primary Data:** Refers to the genetic sequences obtained from public databases.
- **Secondary Data:** Refers to the results of the analysis and processing of the obtained sequences using tools from EBI (European Bioinformatics Institute).
- **Metadata:** Each data (primary or secondary) must contain contextual information about the downloaded sequences.
    - **Primary:** source, download date, search parameters, filters used
    - **Analysis Data (Secondary):** tools and versions used, analysis parameters.
- **Documentation:** This refers to a specific folder describing the project, including the data management protocol, README file, and other relevant documents.
Storage:
The data managed in the project will be stored and shared in the GitHub repository: repository link Below is an example of the organization of the repository according to the already created folders and files:

- Documentation
    - README.md
    - Data_management_Es.md
    - Data_management_En.md
- Primary_Data
    - Programmatic_access
        - first_search.py
- Secondary_Data

**Note:** Each folder will store the corresponding information based on the tools used. Each generated data file contains its respective file with the corresponding metadata.

## Data Processing and Analysis
For this project, tools provided by the European Molecular Biology Laboratory - European Bioinformatics Institute (EMBL-EBI) will be used. These tools include:

- Programmatic access tools
- Databases: Europe PMC, ENA, EVA, and PDBe
- ENSEMBL
- Expression Atlas
- Uniprot
- AlphaFold
- Interpro
- Reactome
- IntAct

## FAIR Principles
### Findable
GitHub data has been organized using easily understandable names, and each folder in GitHub has been created to make it clear what information it contains. Additionally, each file contains a brief description of its purpose and details about input, output, and required parameters for execution. Secondary data, i.e., data generated after using analysis tools, should contain a unique identifier so that it can be identified and accessed easily and without confusion. Finally, both primary and secondary data must include their respective metadata with the information described in the Types of Data to Handle section.

### Accessible
All project information will be constantly updated in the GitHub repository. This is a public repository, so the information can be accessed freely without any restrictions. The tools and results generated in the project will be openly accessible to avoid limitations in their use or review.

### Interoperable
The obtained and generated data will have standard formats that can be accessed by different systems, platforms, and tools. The commonly used formats will be FASTA, CSV or TSV, JSON, or XML. Each type of generated data will describe the input and output formats to limit data usage issues. Additionally, clear language will be used, ontologies will be employed, and general descriptions will be generated in both Spanish and English for easy understanding.

### Reusable
Data will be generated ensuring that it contains the necessary information to understand both its acquisition and generation, ensuring that it can be used later by different individuals. In some cases, documents will include screenshots indicating the results that have been generated, as platforms used may change over time, and an image of the version being used can help better understand the process undertaken.

