
# Renewable Energy Consumption Analysis (USA)

## Project Overview

This analysis examines renewable energy consumption patterns in the United States from 1973 to 2024, providing insights into the growth, composition, and sectoral distribution of renewable energy sources. The interactive Power BI dashboard visualizes key metrics including total renewable energy consumption, source breakdowns, and sectoral utilization patterns. This analysis serves as a valuable resource for energy policymakers, sustainability analysts, and industry stakeholders seeking to understand the evolution and current state of renewable energy adoption in the U.S.

[📊 Power BI Dashboard Link](https://app.powerbi.com/view?r=eyJrIjoiYmE3ODliMjYtOTI2MC00ZmY0LWFiZDUtOWI3Mjc0ZDk2MWExIiwidCI6IjM0YzAxYWRhLTc5MDItNGQ2My04MjgyLThkYzRiZjhmNTUxZCJ9)

The analysis focuses on four critical dimensions of renewable energy consumption:

1. **Historical Consumption Trends** - Long-term patterns in renewable energy adoption
2. **Energy Source Composition** - Breakdown of different renewable energy types
3. **Sectoral Consumption** - Distribution across industrial, residential, commercial, and transportation sectors
4. **Source-Sector Relationships** - How different energy sources serve various consumption sectors

## Dataset Description

The data model follows a streamlined structure optimized for time-series analysis of renewable energy consumption:

### Tables

* **Dataset**: The primary fact table containing detailed consumption records with the following key fields:
  - `Energy Source`: Type of renewable energy (e.g., Biomass, Solar, Wind)
  - `FactDate`: Date of consumption record
  - `Month`: Numeric month identifier
  - `Month name`: Textual month name
  - `Sector`: Consumption sector (Industrial, Residential, Commercial, Transportation)
  - `Value(TBTU)`: Consumption volume in trillion British thermal units
  - `Year`: Year of consumption

* **DateTable**: A comprehensive date dimension table enabling temporal analysis with:
  - `Date`: Full date field
  - `Month`: Numeric month
  - `Month Number`: Sequential month identifier
  - `Month Year`: Month and year combination
  - `Quarter`: Calendar quarter

* **Measures **: A dedicated table containing calculated metrics including:
  - `baseline`: Reference consumption values for comparative analysis

### Data Model Relationships

The model establishes a star schema with the dataset as the central fact table connected to the DateTable through the FactDate field, enabling efficient time-based analysis and visualization.
![image](https://app.powerbi.com/view?r=eyJrIjoiYmE3ODliMjYtOTI2MC00ZmY0LWFiZDUtOWI3Mjc0ZDk2MWExIiwidCI6IjM0YzAxYWRhLTc5MDItNGQ2My04MjgyLThkYzRiZjhmNTUxZCJ9)

## Executive Summary

### Overview of Findings

The analysis reveals significant growth and evolving patterns in U.S. renewable energy consumption over the past five decades:

* Total renewable energy consumption reached **384,036.57 TBTU** in the most recent data
* **Biomass Energy** emerged as the dominant renewable source, accounting for the largest share of consumption
* The industrial sector represents the primary consumer of renewable energy, followed by residential usage
* Consumption patterns show distinct seasonal variations and long-term growth trends

### Key Metrics

| Metric | Value |
|--------|--------|
| Total Renewable Energy Consumption | 384,036.57 TBTU |
| Top Renewable Source | Biomass Energy |
| Leading Consumption Sector | Industrial |
| Historical Growth Pattern | Steady increase with acceleration in recent decades |

## Insights Deep Dive

### Category 1: Historical Consumption Trends

The time-series analysis reveals several important patterns:

* Renewable energy consumption has grown substantially since 1970, with particularly rapid expansion beginning in the early 2000s
* The growth trajectory shows periodic fluctuations likely tied to economic cycles, policy changes, and technological advancements
* Recent years demonstrate accelerated adoption, suggesting increasing market penetration and policy support for renewable energy sources

### Category 2: Energy Source Composition

The renewable energy mix shows significant diversity with varying contributions:

* **Biomass Energy** dominates the renewable portfolio with 141,866.49 TBTU consumed
* **Wood Energy** represents the second largest source at 112,315.11 TBTU
* Conventional hydroelectric power contributes 42,333 TBTU
* Emerging sources like solar and wind energy show smaller but growing consumption volumes
* The portfolio includes niche sources like waste energy and geothermal, indicating a diversified renewable strategy

### Category 3: Sectoral Consumption Patterns

Renewable energy serves different sectors with varying intensity:

* The **industrial sector** consumes the majority share at 50.82% of total renewable energy
* **Residential consumption** accounts for 25.04% of the total
* **Commercial sector** utilization represents 13.07%
* **Transportation** has the smallest share at 2.61%
* This distribution suggests renewable energy is primarily supporting industrial processes and residential needs

### Category 4: Source-Sector Relationships

The analysis reveals how different renewable sources serve various sectors:

* Biomass energy appears heavily utilized across multiple sectors, particularly industrial applications
* Wood energy shows significant residential consumption patterns
* Emerging sources like solar and wind demonstrate growing adoption in commercial and residential sectors
* The industrial sector's dominance suggests opportunities for expanding renewable applications in manufacturing and processing industries

## Recommendations

Based on these insights, several strategic recommendations emerge:

1. **Industrial Sector Focus**: Develop targeted programs to expand renewable energy adoption in industrial applications, building on the sector's existing leadership position.

2. **Residential Growth Opportunities**: Create incentives and awareness campaigns to increase residential renewable energy consumption, particularly for emerging sources like solar.

3. **Transportation Sector Development**: Implement policies and infrastructure investments to grow renewable energy utilization in transportation, addressing the current under-representation.

4. **Biomass Optimization**: Continue supporting biomass energy development while ensuring sustainable sourcing practices to maintain its leading position.

5. **Emerging Source Acceleration**: Provide research funding and market incentives for solar, wind, and other emerging renewable sources to diversify the energy portfolio.

6. **Seasonal Planning**: Develop strategies to optimize renewable energy production and consumption during peak seasonal periods identified in the historical trends.

## Assumptions

* The dataset provides complete and accurate consumption records for all renewable energy sources
* Sector classifications are consistent across all years of the analysis
* Consumption values are reported using standardized measurement methodologies
* The analysis covers all major renewable energy sources in the U.S. market


- Sector selection capabilities
- Detailed consumption breakdowns by source and sector
- Historical trend visualization with consumption metrics

This comprehensive analysis serves as a foundation for understanding renewable energy adoption patterns and identifying opportunities for continued growth in sustainable energy consumption.
