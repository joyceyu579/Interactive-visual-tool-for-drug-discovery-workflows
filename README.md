## Repository overview 
This repository contains an interactive data visualization tool built using Python and HTML. Its purpose is to visualize a common workflow used in pharmaceutical companies for drug research and development. The interactive visualization tool is capable of summarizing ~6 months worth of lab data into one flow diagram and captures more than 5 different types of data (passage of time, genetic strains of animals, sequencing information of top drug candidates, screening results, drug characterization data, and more.) 

Most importantly, the interactive visualization tool can be used to track the origins of the company's products and serves as a deliverable to clients. 

This visualization tool was made specifically for employees and customers of Curia Global's Antibody Discovery team starting in August 2023. During this intitative of introducing new tools into the workplace, I worked wih the research team and Curia's IT/cybersecurity department to ensure compliancy with all company and client data; and taught bash/python basics to advance the skills of older colleagues/scientists.  

#### Inspirations and historical context:
The most famous use case of this flowmap dates back to 1812 in a picture created by Joseph Minard called [Minard's Map](https://en.wikipedia.org/wiki/Charles_Joseph_Minard) . This map contains 6 different types of data stored in 2 dimensions to summarize Napoleon's Russian Campaign of 1812 (a war in Russia).

Inspired by Joseph Minard and his map, [Captain Matthew Henry Phineas Riall Sankey](https://en.wikipedia.org/wiki/Matthew_Henry_Phineas_Riall_Sankey) created what is now known as the Sankey diagram. Overtime and to this day, it has been used to capture the life-cycle assessments of products in scientific fields like physics, chemistry, and engineering. An interactive version of the sankey diagram is what's created using the contents in this repository.

## Repository contents
This repository contains...
- 1 jupyter notebook containing the script to build the interactive visual (05082024_AntibodyDiscovery_Interactive_Viz_tool.ipynb)
- 2 .csv files containing data used by the notebook (05082024_ExampleDataSet.csv, AntibodyRecoveryHits.csv)
- 1 .xlsx file containing a template for the lab scientist to add their data as it is retrieved in the lab. (05082024_TemplateDataSet.xlsx)

## How to generate your interactive diagram: 
To use the contents in this repository, it is assumed that the user (i.e. team members and clients of Curia's Antibody department) is familiar with an in-vivo/in-vitro antibody discovery workflow.
It is also assumed that the user does not have much experience with programming nor using python notebooks, but has access to the software and has working knowledge of excel.
1) In the .xslx file, upload the data that corresponds with whats highlighted in yellow.
2) Save the .xslx file as a .csv file named 05082024_ExampleDataSet.csv .
3) In the AntibodyRecoveryHits.csv file, replace all your top hits from each screen with what was obtained in the wet-lab. Save your progress.
4) Open the folder up in File explorer (if you are on Windows) or Finder (if you are on Mac).
5) Click the file path bar and type in `terminal`. Hit enter. Your terminal or command prompt will pop up.
6) Type in jupyter lab. Hit enter. Web browser will appear. 
7) Double click .ipynb file.
8) Run the notebook. It will take a minute to build the diagram.
9) When the notebook is done running, you will get a pop up in a new web browser with your interactive image. A file (.html) will also be automatically saved in your computer's downloads folder. 
10) Double click .html file, and your interactive image will appear. Play around with it as you please! Hovering over different nodes and links reveals more information. 
11) Send .html file to the respective client or team members. 

## Languages, Libraries, and environment used:
- Languages: Python, CSS/HTML, Bash 
- Libraries: plotly, req, datascience, pandas, numpy, webcolors, matploptlib
- Environment: Jupyter notebook
- Other tools: Command line, Microsoft excel