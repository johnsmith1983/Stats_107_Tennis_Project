# Stats_107_Tennis_Project
Stats 107 project on analyzing tennis statistics using R

## How to Reproduce the Results

Follow these steps to reproduce the data cleaning, processing, and preliminary visualizations:

1. **Download or clone the GitHub repository.** Open the `Stats_107_Tennis_Project` folder in RStudio by opening the `Tennis Project.Rproj` file.

2. **Check the requirements.** Open and run `00_requirements.R`. This project currently uses Base R functions and does not require additional packages.

3. **Load the project functions.** The file `00_functions.R` contains the function `calculate_ace_difference()`, which calculates the difference between the winner's and loser's ace counts.

4. **Clean the raw data.** Open and knit `11_TennisDataCleaning.Rmd`. This file imports `Data/atp_matches_2023.csv`, removes matches with missing ace statistics, selects the variables needed for the analysis, and separates the matches by court surface. It saves the cleaned CSV files and the `12_DataSaving.RData` file in the `Data` folder.

5. **Process the cleaned data.** Open and knit `21_TennisDataProcessing.Rmd`. This file loads the cleaned datasets, calculates the ace difference between winners and losers, and generates summary statistics. It saves the processed datasets in `22_DataSaving.RData`.

6. **Create the preliminary visualizations.** Open and knit `31_TennisDataVisualization.Rmd`. This file loads the processed datasets and creates boxplots, histograms, summary tables, and interpretations comparing ace counts across grass, clay, and hard court surfaces.

7. **View the results.** The knitted HTML files contain the output from each R Markdown document, including the data processing results, graphs, summary tables, and interpretations.

## Files in the repository:

| Data

| | - - 12_DataSaving.RData

| | - - 22_DataSaving.RData

| | - - atp_matches_2023.csv

| | - - tennis_clay.csv

| | - - tennis_clean.csv

| | - - tennis_grass.csv

| | - - tennis_hard.csv

| .gitignore

| 00_functions.R

| 00_requirements.R

| 11_TennisDataCleaning.Rmd

| 11_TennisDataCleaning.html

| 11_TennisDataCleaning.pdf

| 21_TennisDataProcessing.Rmd

| 21_TennisDataProcessing.html

| 31_TennisDataVisualization.Rmd

| 31_TennisDataVisualization.html

| FINALREPORT.Rmd

| FINALREPORT.pdf

| README.md

| README.txt

| Tennis Project.Rproj


-------------------------------------------------------------------------------

12_DataSaving.RData             - Stores the cleaned tennis datasets, including the complete dataset and separate datasets for grass, clay, and hard courts

22_DataSaving.RData             - Stores the processed tennis datasets, including the calculated ace differences between match winners and losers

atp_matches_2023.csv            - Full data list of the atp_matches_2023 download from a github repository

tennis_clay.csv                 - List of all matches played on Clay surface

tennis_clean.csv                - List of all the matches with the data we need to answer our question (9 categories), which was reduced to 2815 data points

tennis_grass.csv                - List of all matches played on Grass surface

tennis_hard.csv                 - List of all matches played on Hard surface

.gitignore                      - Tells GitHub not to send over all of the little R files that form every time you open your own project

00_functions.R                  - An R script file to hold all of the functions we will be using in the project

00_requirements.R               - An R script file holding all the library downloads that we need for the project

11_TennisDataCleaning.Rmd       - Has the procedure and code for how we cleaned the data into a new .csv file

11_TennisDataCleaning.html      - Same but knitted as an HTML

11_TennisDataCleaning.pdf       - Same but knitted as a PDF

21_TennisDataProcessing.Rmd     - Has the processing of the data by adding Ace Differences

21_TennisDataProcessing.html    - Same but knitted as an HTML

31_TennisDataVisualization.Rmd  - Creates the first visualization of data and comments on the data

31_TennisDataVisualization.html - Same but knitted as an HTML

FINALREPORT.Rmd                 - The Final report for the halfway evaluation

FINALREPORT.pdf                 - PDF version

README.md                       - Explains every file and what it has, as well as its location in the folder

README.txt                      - Same as the other README but in text file format as per instructions

Tennis Project.Rproj            - R project file that has all of the files to access on the bottom-right Files tab

-------------------------------------------------------------------------------

Source of the data:
https://github.com/Aneeshers/tennis-sackmann-archive/tree/main/atp
