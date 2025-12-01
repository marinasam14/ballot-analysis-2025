# Analysis of 2025 Ballot Results 

This repository contains data, analytic code, and findings based on scraped results from the 2025 New York City elections

## Data

This analysis uses TK spreadsheets from the following sources

*`ballot_results_github/data/full_results_2025_copy.csv`: unofficial results from the NYC Board of Elections using the boe_scraper from [THE CITY](https://github.com/thecityny/boe-scraper)
* `ballot_results_github/data/nyed_25c_git`: NYC election district shapefiles, clipped to shoreline. You can find the most current version [here](https://www.nyc.gov/content/planning/pages/resources/datasets/election-districts)
*`ballot_results_github/data/nyed_25c_neighborhood_name_reproj4326_git.geojson`: 2025 ed shapefile with cleaned NTA names

## Methodology

The notebook `ballot-results-2025-github.ipynb` cleans the full mayoral results and prepares the data for ballot donut visualizations that show each ballot proposal's vote share
performs the following analysis

The notebook `ballot-map-2025` also cleans the full mayoral results and creates a column for an ed match. It calculate vote share percentages per election district and categorizes it into guintiles for a Datawrapper chloropeth map. It then prepares the results for spatial joining using two shapefiles and exports six datasets for maps.

## Outputs

The notebooks output this spreadsheet which contains:

*`ballot_results_2025_only.csv`
*`proposal_1_results_2025.csv`
*`proposal_2_results_2025.csv`
*`proposal_3_results_2025.csv`
*`proposal_4_results_2025.csv`
*`proposal_5_results_2025.csv`
*`proposal_6_results_2025.csv`

## Running the Analysis Yourself

You can run the analysis yourself. To do so you'll need the following installed on your computer:

* Python 3
* The Python libraries specified in `requirements.txt`.

## Licensing

All code in this repository is available under the MIT License. 