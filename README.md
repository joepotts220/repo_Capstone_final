## Data Analysis Capstone Project:  Joe Potts, March 2025

#### Overview
This project was designed to show what characteristics of an office building have the greatest influence on the amount of electricity or natural gas used.  The climate zone that the building  located in was also considered. A series of correlation techniques was used to show the relationships between a given building characteristic, climate zone and energy used. 
#### Data
The primary data source is the 2018 Energy Information Administration (EIA) Commercial Buildings Energy Consumption Survey (CBECS) microdata file.  https://www.eia.gov/consumption/commercial/data/2018/index.php?view=microdata



The secondary data source was a dataframe built by me showing the low and high limits of cooling degree days and heating degree days in each of the three climate zones used in the study.  The source of the data is:  "An Assessment of Actual and Potential Building Climate Zone Change and Variability From the Last 30 Years Through 2100 Using NASA’s MERRA and CMIP5 Simulations".  See pages 4 and 5. https://www.wemcouncil.org/wp/wp-content/uploads/2015/07/1450_PaulStackhouseJr.pdf


#### Project Structure
- Create two dataframs for each data source
- Join the two data sources into one dataframe
- Create two calculated columns using data from each data source
- Summary data analysis and data cleaning
- Correlation analysis using matrices and unstacking techniques
- Plotting individual relationships
#### Features
- Used a virtual environment
- Used two data souces that were joined
- Summarized cleaned data
- Created four matplotlib plots
- Created four functions
- Created two calculated columns
- Notated code with # comments and markdown cells in a Jupyter notebook
- Created a data dictionary

#### AI Use 
I did use Google Gemini to troublshoot the fuctions that created the calculated columns.  I did Google research on how to create the columns and made a framework of the function, but found it impossible to make the function work without further help. 

#### Getting Started
- To view the project:
   1.  Clone the project repo to local: git clone https://github.com/joepotts220/repo_Capstone_final.git
    2.  Install requirements.txt:  pip install -r requirements.txt
    3.  View Jupyter notebook:  capstone_final.ipynb
#### Dependencies
- matplotlib
- pandas
- numpy

#### Virtual Environment Instructions
1. After you have cloned the repo to your machine, navigate to the project 
folder in GitBash/Terminal.
1. Create a virtual environment in the project folder. 
1. Activate the virtual environment.
1. Install the required packages. 
1. When you are done working on your repo, deactivate the virtual environment.

 Command | Linux/Mac | GitBash |
|---------|-----------|---------|
| Create | `python3 -m venv venv` | `python -m venv venv` |
| Activate | `source venv/bin/activate` | `source venv/Scripts/activate` |
| Install | `pip install -r requirements.txt` | `pip install -r requirements.txt` |
| Deactivate | `deactivate` | `deactivate` |

#### Conclusions
The only conclusion I can draw from the project data is the building square footage has a strong relationship to the energy used.  This supports the reasonable assumption that the bigger a building is, the more or less energy it will need to heat or cool, and power the needed equipment.
The climate zone was not related to energy use.

#### Exceptions
The reason for the limited conclusion I was able to draw from the data is that all of the pertinent data in the CBECS survey is catagorical data with the exception of annual electicity use, annual natrual gas used and the square foot measure. I tried a method of changing catagorical data by using dummy values, but it made little difference in the correlation results-and it created more columns. So, if there was a variable with five catagories to choose from and each identified with the numbers 1 to 5, the dummy value method would create five new columns.  I discussed this issue with my mentor, and we decided to use the data as presented in the source. 

#### Recommended improvements
- Further research on catagorical data analysis


