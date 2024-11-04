# Belly Button Challenge

## Table of Contents
- [Introduction](#Introduction)
- [Features](#Features)
- [Before You Begin](#Before-you-begin)
- [Usage](#Usage)
- [Code Details](#Code-details)
- [Contributors](#Contributors)
- [Reference](#Reference)

## Introduction
The Belly Button Biodiversity Dashboard is an interactive web application that allows users to explore the biodiversity of bacteria found in human belly buttons. This project visualizes sample data on various bacterial species, helping users gain insights into microbiomes by viewing charts and metadata based on individual test subjects.

This dashboard features:
- A Metadata Panel displaying demographic information.
- An interactive Bubble Chart and Bar Chart illustrating bacterial cultures for selected samples.
- The data and code are ideal for educational purposes, emphasizing the use of D3.js, Plotly, and JavaScript to create data-driven, interactive dashboards.

## Features
- Metadata Panel: Displays demographic information for the selected sample, such as age, ethnicity, location, and wash frequency.
- Bubble Chart: Visualizes the number of bacterial cultures per sample, with each bubble representing an OTU (Operational Taxonomic Unit).
- Bar Chart: Shows the top 10 bacterial cultures in the selected sample.
- Dropdown: Allows users to select different test samples to update charts and metadata in real-time.

## Before You Begin 
1. Create a New GitHub Repository:
   - Name the new repository belly-button-challenge.
   - Ensure it’s a public repository.
2. Clone the Repository to Your Local Machine:
```bash
git clone git@github.com:jananaum7/belly-button-challenge.git
```
3. Copy Starter Files:
   - Inside the belly-button-challenge repository on your local machine, copy the contents of the StarterCode folder provided in the Module 14 Challenge into the repository.
       - index.html
       - samples.json
       - the static folder 
4. Push changes to GitHub
   - Stage and commit the files:
```bash
git add .
```
```bash
git commit -m "Add starter code for belly button biodiversity dashboard"
```
```bash
git push origin main
```
5. Deploy to GitHub Pages:
   - Go to your GitHub repository belly-button-challenge on GitHub.
   - In the repository, go to Settings > Pages.
   - Under Source, select the main branch, and then select the root (/) directory.
   - Click Save.
   - GitHub Pages will now deploy the project, and a link to the live site will be generated.

## Usage
   - Load the Dashboard: Open index.html in any web browser.
   - Use the dropdown menu to select a test subject by their ID.
   - Explore the Data:
       - The Metadata Panel updates to show demographic details of the selected subject.
       - The Bar Chart shows the top 10 bacterial cultures found in that sample.
       - The Bubble Chart displays bacterial cultures for that sample, with bubble size indicating quantity.

## Code Details
- app.js Functions
  - buildMetadata(sample): Fetches demographic data for the selected sample and displays it in the metadata panel. The panel is updated each time a new sample is selected.
  - buildCharts(sample): Fetches sample data, then creates two charts:
    - A Bubble Chart showing all bacterial cultures for the sample.
    - A Bar Chart showing the top 10 bacterial cultures, with bacteria count on the x-axis.
  - init(): Initializes the dashboard by loading the dropdown with available sample IDs, then loading the first sample's data to populate charts and metadata.
  - optionChanged(newSample): Updates the dashboard based on the new sample ID selected.

## Contributers
J. Naum 

## Reference
Portions of the code and README structure were developed with the assistance of *ChatGPT*.
