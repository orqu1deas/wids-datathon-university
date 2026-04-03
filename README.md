<p align="center">
  <img src="https://www.widsworldwide.org/wp-content/uploads/2023/05/WiDS_logo_nav.png" alt="WiDS Logo" width="250"/>
</p>

<h1 align="center">WiDS Datathon 2026</h1>

## Hybrid RAG + Enhanced Vulnerability Index for Wildfire Economic Resilience

### Track Selection

This project was developed under **Track 2: Designing for Economic Resilience**, which focuses on understanding and mitigating the economic consequences of wildfires. In particular, the objective is to support decision-making processes that contribute to preserving workdays, protecting wages, and improving the targeting of economic safety nets for vulnerable communities.

<p align="center">
  <img src="assets/GIF.gif" alt="SOLARA Demo" width="900"/>
</p>

---

## Project Title & Team Info

**Project Title**: _Hybrid RAG + Enhanced Vulnerability Index for Wildfire Economic Resilience_  
**Team Name**: _SOLARA_  
**University**: _Instituto Tecnológico de Estudios Superiores de Monterrey (ITESM)_  
**Course**: _Data Science & Mathematics_  
**Term**: _6th Semester_

**Team Members**:

- Kira Darian Gómez Pantoja
- Juan Pablo Guerrero Escudero
- Romina Nájera Fuentes
- María José Ocharte Álvarez
- Sergio Rock Arredondo
- María José Zamora Gómez

---

## Project Overview

Wildfires have evolved into a multidimensional challenge that extends beyond environmental damage and into significant economic disruption. Communities affected by wildfires often experience loss of income, reduced employment opportunities, and long-term financial instability. Despite the availability of extensive datasets, existing tools remain fragmented and insufficient for identifying which populations are most economically vulnerable.

SOLARA addresses this gap by integrating heterogeneous data sources into a unified analytical framework. The system combines wildfire activity data, sociodemographic indicators, economic metrics, and climate variables to construct a comprehensive view of vulnerability. In addition, it incorporates a Hybrid Retrieval-Augmented Generation (Hybrid RAG) system that enables the integration of structured data with unstructured information such as policies and reports.

---

## Dataset Overview

The foundation of this project is built upon the Watch Duty wildfire dataset, which provides detailed geospatial and temporal information on wildfire activity across the United States. This dataset includes approximately 62,000 geo-referenced wildfire events and over 1,200 fire perimeters, offering a comprehensive representation of fire occurrence, progression, and spatial extent. :contentReference[oaicite:0]{index=0}

However, wildfire location alone does not fully capture the economic impact experienced by affected communities. To address this limitation, the dataset was enriched with additional data sources spanning four key domains: sociodemographic, economic, climatic, and document-based information.

Sociodemographic data were obtained from the U.S. Census Bureau, including variables such as population density, income per capita, education levels, disability prevalence, and insurance coverage. These variables provide insight into structural vulnerability and the capacity of communities to respond to and recover from wildfire events.

Economic data were collected from the U.S. Census Bureau, the Bureau of Labor Statistics, and the USDA, incorporating indicators such as poverty rates, household income, employment conditions, and rural-urban classification. These variables are critical for understanding the economic fragility of different regions and their resilience to disruption.

Climate data were integrated from sources such as NASA POWER and Open-Meteo, including temperature, precipitation, relative humidity, wind conditions, and drought indices. These variables capture environmental conditions that influence wildfire intensity and spread.

Additionally, a corpus of legally scraped documents was constructed, including wildfire-related policies, insurance frameworks, community reports, and news articles. This unstructured data component supports the Hybrid RAG system, enabling the retrieval of contextual and policy-relevant information.

All datasets were harmonized at the county level, which serves as the primary spatial unit of analysis. Temporal alignment was also performed to reconcile differences in data frequency, including yearly, monthly, and weekly observations. This harmonization process ensures consistency across sources and enables the integration of heterogeneous data into a unified analytical framework.

The resulting dataset is multi-source, multi-dimensional, and designed to support both quantitative modeling and qualitative information retrieval. As highlighted in the technical pitch, this integrated data landscape allows the system to move beyond isolated analyses and instead provide a cohesive understanding of wildfire exposure, economic vulnerability, and recovery capacity.

---

## Approach

The project follows a structured pipeline that combines data engineering, unsupervised learning, and AI-based retrieval systems.

First, raw datasets were cleaned, processed, and aligned across spatial and temporal dimensions. Feature engineering was applied to construct meaningful indicators of vulnerability and exposure.

Second, clustering techniques were used to identify latent patterns across climate, sociodemographic, and economic dimensions. These clusters support the development of an enhanced vulnerability index, which captures structural differences across regions.

Finally, a Hybrid RAG system was implemented to bridge structured and unstructured data. This system integrates document-based retrieval, and a knowledge graph, enabling the generation of context-aware and interpretable responses.

---

## Results

The resulting system enables a multidimensional understanding of wildfire impact. Rather than focusing exclusively on hazard prediction, it provides insights into which communities are most economically vulnerable and why.

Through clustering and index development, the system identifies distinct vulnerability profiles across counties. The integration of the Hybrid RAG component allows users to query both data-driven insights and policy-relevant information in a unified interface.

This approach supports a shift from reactive wildfire response toward proactive, data-informed economic resilience strategies.

---

## Team Contributions

| Name                         | Contributions                                                                 |
| ---------------------------- | ----------------------------------------------------------------------------- |
| Juan Pablo Guerrero Escudero | Knowledge Graph design, GraphRAG implementation, backend architecture         |
| Romina Nájera Fuentes        | Data ingestion, clustering, vulnerability index (WRVI) development, frontend  |
| María José Ocharte Álvarez   | EDA, clustering, WRVI development, frontend, poster design                    |
| Sergio Rock Arredondo        | Legal document scraping, Document RAG pipeline, backend development, planning |
| María José Zamora Gómez      | Feature engineering, preprocessing, clustering, RAG support, presentation     |
| Kira Darian Gómez Pantoja    | EDA, data cleaning and preprocessing, frontend                                |
