# Final Project - BA 505

### Team Members
* Disha Desai
* Diandre Clarke
* Hillary Fitts


### Objective
Perform exploratory data analysis and predictive analytics for the selected data source by utilizing Python, NumPy, Pandas, Matplolib, Jupyter, and GitHub. We have taken a data of New York City Housing Sale. This includes sale records of more than 80000 transactions that occured in the 2017-2018 period. Each of this record is classified into 21 different attributes. Through the analysis of this we aim to understand the relationship between different factors guiding the Housing Sale in New York City. This shall help us explore trends, identify areas with high and low sale in the past year etc. Further, we intend to find the significant factors driving the prices of housing sale and develop a model to predict the future prices.


### Data Source
The data for this project is sourced from [New York City Department of Finance](https://www1.nyc.gov/site/finance/taxes/property-rolling-sales-data.page) We have used the Department of Finance's Rolling Sales files that lists properties sold from November 2017 to October 2018. The files primarily include information about the neighbourhood, building type, square footage, tax class and other details related to the property sold. Below is a Glossary of the data we have included as columns in our project from this:  
1. Borough:  
The name of the borough in which the property is located.  
2. Neighborhood:  
Department of Finance assessors determine the neighborhood name in the course of valuing properties. The common name of the neighborhood is generally the same as the name Finance designates. However, there may be slight differences in neighborhood boundary lines and some sub-neighborhoods may not be included.  
3. Building Class Category:  
This is a field that we are including so that users of the Rolling Sales Files can easily identify similar roperties by broad usage (e.g. One Family Homes) without looking up individual Building Classes. Files are sorted by Borough, Neighborhood, Building Class Category, Block and Lot.  
* Tax Class at Present:  
Every property in the city is assigned to one of four tax classes (Classes 1, 2, 3, and 4), based on the use of the property.    
 * Class 1: Includes most residential property of up to three units (such as one-, two-, and three-family homes and small stores or offices with one or two attached apartments), vacant land that is zoned for residential use, and most condominiums that are not more than three stories.
 * Class 2: Includes all other property that is primarily residential, such as cooperatives and condominiums.
 * Class 3: Includes property with equipment owned by a gas, telephone or electric company.
 * Class 4: Includes all other properties not included in class 1,2, and 3, such as offices, factories, warehouses, garage buildings, etc. 
* Block:  
A Tax Block is a sub-division of the borough on which real properties are located. The Department of Finance uses a Borough-Block-Lot classification to label all real property in the City. “Whereas” addresses describe the street location of a property, the block and lot distinguishes one unit of real property from another, such as the different condominiums in a single building. Also, block and lots are not subject to name changes based on which side of the parcel the building puts its entrance on.
* Lot:  
A Tax Lot is a subdivision of a Tax Block and represents the property unique location.
* Easement:  
An easement is a right, such as a right of way, which allows an entity to make limited use of another’s real property. For example: MTA railroad tracks that run across a portion of another property.
* Building Class at Present:  
The Building Classification is used to describe a property’s constructive use. The first position of the Building Class is a letter that is used to describe a general class of properties (for example “A” signifies one-family homes, “O” signifies office buildings. “R” signifies condominiums). The second position, a number, adds more specific information about the property’s use or construction style (using our previous examples “A0” is a Cape Cod style one family home, “O4” is a tower type office building and “R5” is a commercial condominium unit). The term Building Class used by the Department of Finance is interchangeable with the term Building Code used by the department of Buildings. 
* Address:  
The street address of the property as listed on the Sales File. Coop sales include the apartment number in the address field.
* Zip Code: The property’s postal code
* Residential Units:  
The number of residential units at the listed property.
* Commercial Units:  
The number of commercial units at the listed property.
* Total Units:  
The total number of units at the listed property.
* Land Square Feet:
The land area of the property listed in square feet.
* Gross Square Feet:  
The total area of all the floors of a building as measured from the exterior surfaces of the outside walls of the building, including the land area and space within any building or structure on the property.    
* Year Built:  
Year the structure on the property was built.
* Building Class at Time of Sale:
The Building Classification is used to describe a property’s constructive use. The first
position of the Building Class is a letter that is used to describe a general class of
properties (for example “A” signifies one-family homes, “O” signifies office buildings. “R”
signifies condominiums). The second position, a number, adds more specific information
about the property’s use or construction style (using our previous examples “A0” is a Cape
Cod style one family home, “O4” is a tower type office building and “R5” is a commercial
condominium unit). The term Building Class as used by the Department of Finance is
interchangeable with the term Building Code as used by the Department of Buildings.
* Sales Price:  
Price paid for the property.
  - Sales Price of 0:  
  A sale price of 0 indicates that there was a transfer of ownership without a cash consideration. There can be a number of reasons for a $0 sale including transfers of ownership from parents to children.
* Sale Date:  
Date the property sold.  

### Features
This project can be helpful for exploring the Housing market of New York City. There are many attributes like boroughs that differentiate New York City Housing market from others. Also, the project can be extremely useful for estimating the future prices of properties in New York City.

### Code Example:
Below code was used to plot the number of NYC Housing Sale in 2017-18 classified by Boroughs.
> df['Borough'].value_counts()[:].plot(kind='bar')  
plt.ylabel('No.of Housing Sale')  
plt.title("NYC 2018 Housing Sale")  
plt.xlabel('NYC Boroughs')  
tick_val = [0, 1, 2, 3, 4]  
tick_lab = ['Queens', 'Brooklyn', 'Manhattan', 'Staten Island', 'Bronx']  
plt.xticks(tick_val, tick_lab)  
plt.show()

### Contribute:
Our project takes into account the various factors of the housing market that govern the prices of properties in NYC. It offers a scope to use macro indicators for more precise predictions. It can be explored how macro factors like Housing Price Index, Total Unemployment, S&P 500, GDP etc influence the property prices in New York City.


    