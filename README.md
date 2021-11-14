# SA-Petrol-Price-Prediction-v2
## version 2.0.0 of the south african petrol price prediction.

This version focuses on the breakdown of petrol price and the how domestic and international influences have on the total price of petrol.
This project is divided into 4 parts maily:
### 1. The Prepare Process 
This is the phase to prepare data by collecting and storing it. The data to be collected will be collected as per the question os the project inhand. 4 sets of data will be collected for the project to be sufficient and these are: (a) Total Petrol price since Jan 2011 till Nov 2021 (b) Petrol price breakdown from Jan 2011 to Nov 2021 (c) Weekly  & monthly brent crude oil in USD for the same period and , (d) The weekly and monthly exchange rates between Rand and USD for the same period.
#### How will the data be collected
The data will be collected by using three different methods:
* Web scrapping using Python beautifulsoup library 
* Using Excel import data from web option - This was used for data which was found in html pdf form which was almost impossible to web scrap using python
* Web scarpping apps like ParseHub and Octaparse 8 which are free and also offers paid premium subscription 

#### Data sources
Data was collected/scrapped from three very reliable sources all from the goverment agencies. Fuel prices and breakdown were collected from sapia and the energy dept website while the crude oil prices were collected from eia website. below is the links to all the data sources:
* https://www.sapia.org.za/Overview/Old-fuel-prices
* http://www.energy.gov.za/files/esources/petroleum/petroleum_arch.html
* https://www.eia.gov/dnav/pet/hist/LeafHandler.ashx?n=pet&s=rbrte&f=w
This data will be stored both in CVS and Excel spreadsheet which will be shared 

#### Data type and format
The only petrol price we are interested in is the 95 ULP inland/Gauteng. This is the most popular and widely used petrol in south africa as such other petrol kind were removed/negleted for this research. Only two types of data types will be used in this research which are 
* Datetime - for the date (time period)
*  float - for the numeric numbers since all the data excluding the date will be in number currency 

### 2. Data Processing
This is the phase of cleaning checking all the right information about our data. The data from the collected steps will need to be cleaned, transformed into usable format, and therafter be combined into one usuable dataset for further analysis.

#### Data Cleaning
Data from web scrapping, spreadsheets, and web scrapping software will be cleaned as follows:
* Remove duplicates, extra spaces and blanks where neccessary (python and spreadsheet tools)
* Fix misspellings and renaming some header or replacing headers where they are missing 
* Remove all formats and convert to datetime and float (number or currency in spreadsheet)
* in spreadsheets the find and replace method was used for further cleaning our data 
* A total of 4 spreadsheets and dataframes were worked on which are (i) Crude oil Prices, (ii) ZAR-USD exchange rate (iii) Total Petrol Price and (iv) Petrol Price breakdown which will followed the processes above of cleaning.
* These datasets were all merged to one clean, formatted and ready to use dataset called dataframe_v..
