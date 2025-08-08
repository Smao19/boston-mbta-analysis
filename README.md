# MBTA Transit Analysis Project

## Additional Resources
- [Project Presentation and Detailed Report](https://drive.google.com/drive/folders/1-2L4KaZrSI45flOVaamYcYVe1CUu12xS?usp=sharing)

## Overview
This project analyzes transit accessibility and service distribution across Boston's MBTA subway system, identifying underserved areas and potential expansion opportunities. By combining MBTA transit data with US Census population data, we evaluate transit accessibility and develop recommendations for system improvements.

## Research Questions
- Which areas of Boston are most underserved by the MBTA?
- What areas are the best candidates for system expansion?

## Key Findings
- Chelsea, Everett, South Boston, and Dorchester were identified as significantly underserved areas
- Machine learning models helped identify patterns in transit accessibility across census blocks

## Methodology
### Data Sources
- MBTA API: Station locations and service data
- US Census API: Population data for Suffolk, Middlesex, and Norfolk counties
- MassGIS: Geographic shapefiles for census block mapping

### Analysis Techniques
1. **Transit Demand Scoring**
   - Developed a custom demand score formula: (population_density²) * (distance/800)
   - Incorporated distance thresholds: 800m minimum (well-served areas) and 10km maximum (beyond rapid transit range)

2. **Machine Learning Models**
   - Linear Regression: Predicting transit demand scores
   - K-means Clustering: Grouping census blocks by accessibility levels

## Tools & Technologies
- Python
- Pandas & NumPy for data manipulation
- Scikit-learn for machine learning models
- Folium for Mapping
- GeoPandas for geospatial analysis
- Matplotlib & Seaborn for visualization

## Setup & Installation
1. Clone the repository
2. Install required packages(there's a few):
3. Set up API keys for MBTA and Census APIs
4. Run the Jupyter notebook(mainNotebook) to replicate.

## Team Members
- Sebastian Arteaga (arteaga.s@northeastern.edu)
- Darwin Alarcon (alarcon.dar@northeastern.edu)
- Suraj Swamy (swamy.sur@northeastern.edu)
- Jason Lam (lam.jason@northeastern.edu)

## Acknowledgments
- Northeastern University DS3000: Foundations of Data Science
- Dr. Mohit Singhal (m.singhal@northeastern.edu)
- MBTA for providing access to their API
- US Census Bureau for population data
- MassGIS for geospatial data
