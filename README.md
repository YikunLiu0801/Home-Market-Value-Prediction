# [Regression] Home Market Value Prediction

Construct a market value prediction model to predict a home's current market value and score a test data set with this model.

Both training and test data are home sale transactions from 2015 in King County, WA. The prediction result is a CSV file of ZPIDs and home price predictions in a column named “SaleDollarCnt” for all homes in the test set.

Two metrics to meature the accuracy:

- AAPE: 𝑚𝑒𝑎𝑛(𝑎𝑏𝑠(𝑝𝑟𝑒𝑑𝑖𝑐𝑡𝑒𝑑−𝑎𝑐𝑡𝑢𝑎𝑙)/𝑎𝑐𝑡𝑢𝑎𝑙)
- MAPE: 𝑚𝑒𝑑𝑖𝑎𝑛(𝑎𝑏𝑠(𝑝𝑟𝑒𝑑𝑖𝑐𝑡𝑒𝑑−𝑎𝑐𝑡𝑢𝑎𝑙)/𝑎𝑐𝑡𝑢𝑎𝑙)

Description of fields contained in the training and test data sets
- PropertyID: Unique ID for home
- TransDate: Date of current sale
- SaleDollarCnt: Price of current sale
- BathroomCnt: Number of bathrooms in home
- BedroomCnt: Number of bedrooms in home
- BuiltYear: Year home was constructed
- FinishedSquarefeet: Finished square footage of the home
- GarageSquareFeet: Size of protected garage space if any
- LotsizeSquarefeet: Lot size of property in square feet
- StoryCnt: Number of stories for the home
- latitude: Latitude of the home * 1,000,000
- longitude: Longitude of the home * 1,000,000
- Usecode: Type of home (all homes in both training and test are single-family homes)
- ZoneCodeCounty: The intensity of use or density the lot is legally allowed to be built-up to
- viewtypeid: Nominal variable indicating the type of view from the home (blank or NULL
value indicates no view)
- censusblockgroup: The FIPS code for the census block group this property is located in.
You can derive the census tract FIPS by truncating the rightmost digit.
- BGMedHomeValue: The median home value in the block group
- BGMedRent: The median rent value in the block group
- BGMedYearBuilt: The median year structures in the block group were built
- BGPctOwn: Percentage of homes that are owner-occupied in the block group
- BGPctVacant: Percentage of housing that is vacant in the block group
- BGMedIncome: Median income of households residing in the block group
- BGPctKids: Percentage of households with children under 18 years present at home
- BGMedAge: Median age of residents of the block group
