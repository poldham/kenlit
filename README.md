# Kenlit

This repository compiles open access data on scientific publications from Kenya. 

The data is drawn from two sources:

1. Microsoft Academic Graph (January 2019 Release) which is provided under an [Open Data Commons Attribution Licence (ODC-By) v. 1.0](https://opendatacommons.org/licenses/by/1.0/). Visit [Microsoft Academic Graph](https://www.microsoft.com/en-us/research/project/microsoft-academic-graph/) to learn more and view the [documentation](https://docs.microsoft.com/en-us/academic-services/graph/).

2. The Lens. The Lens is an open access database for scientific and patent literature. The Lens has recently expanded coverage of the scientific literature to include Crossref, PubMed, Microsoft Academic Graph, and CORE (for open access full text articles).

Data from MAG is used to identify research outputs from organisations in Kenya. 

Data from the Lens (which aggregates from a range of sources) is mainly used to identify other scientific publications about Kenya. 

At present `Kenlit` consists of: 

- 28,462 publications directly linked to organisations in Kenya.
- 160,654 publications that make reference to Kenya in the title, abstract or author keywords but are not directly linked to Kenyan research organisations. 

### Data processing

Data processing is carried out using a Databricks Apache Spark cluster using the `sparklyr` package to work with Microsoft Academic Graph. 

Data cleaning is carried out in R using tidyverse packages. Additional data cleaning is performed using VantagePoint from Search Technology Inc.


Kenlit is a work in progress and suggestions or corrections are welcome. 