Ames Iowa Housing Predictive Linear Model

This project was based on the Kaggle competition, it challenged us to create a predictive model to determine housing prices within Ames Iowa given historical data.

Kaggle Competition Link - https://www.kaggle.com/c/house-prices-advanced-regression-techniques

I chose to approach this challenge by building out a Linear Regression, which was the easiest and most interpertable model.  Given the size of this data another valid model could have been a Fully Connected Neural Net. 

Scoring for this project was R^2 score which is the amount of variance in price that the model was able to account for.  My best submission had a 0.86 R2 score.

Model Used: Regularized Linear Regression - I heavily used Lasso Regularization to both eliminate features and supress features that were less relevent.  If I were to revisit this project I would spend more time feature engineering and possibly create some geo-spatial relationships between different neighborhoods in addition.  Fortunately, there were tons of relevent features that were including in the base data that had extremely low p-values and were highly correlated.  

The link provided is to my google-slides presentation for this project . ___________________________

Project Directory:
CSVs - 
    train.csv - Kaggle Provided CSV with target (price) to train models on.
    validation.csv - Kaggle Provided CSV without target (price) to create predictions and Kaggle
                     submissions with.
    train_cleaned.csv - The cleaned and scaled version of Kaggles CSV that I used for model fitting
                        including newly engineered features, and eliminates some features.
    validation_cleaned.csv - Validation data that has been scaled / imputed the same way that my train 
                             data was.
                             
                             
Kaggle Submissions - 
        Submission1.csv
        Submission2.csv
        
        
Python Files-
    Ames_Iowa_Housing_Predictive_Model.ipynb - Train set cleaning and aggregation, feature imputation, and model building.
    validation_cleaning.ipynb - Kaggle validation set cleaning /regularization.
    
    
Train CSV Data Dictionary: 

SalePrice - the property's sale price in dollars. This is the target variable that you're trying to predict.
MSSubClass: The building class
MSZoning: The general zoning classification
LotFrontage: Linear feet of street connected to property
LotArea: Lot size in square feet
Street: Type of road access
Alley: Type of alley access
LotShape: General shape of property
LandContour: Flatness of the property
Utilities: Type of utilities available
LotConfig: Lot configuration
LandSlope: Slope of property
Neighborhood: Physical locations within Ames city limits
Condition1: Proximity to main road or railroad
Condition2: Proximity to main road or railroad (if a second is present)
BldgType: Type of dwelling
HouseStyle: Style of dwelling
OverallQual: Overall material and finish quality
OverallCond: Overall condition rating
YearBuilt: Original construction date
YearRemodAdd: Remodel date
RoofStyle: Type of roof
RoofMatl: Roof material
Exterior1st: Exterior covering on house
Exterior2nd: Exterior covering on house (if more than one material)
MasVnrType: Masonry veneer type
MasVnrArea: Masonry veneer area in square feet
ExterQual: Exterior material quality
ExterCond: Present condition of the material on the exterior
Foundation: Type of foundation
BsmtQual: Height of the basement
BsmtCond: General condition of the basement
BsmtExposure: Walkout or garden level basement walls
BsmtFinType1: Quality of basement finished area
BsmtFinSF1: Type 1 finished square feet
BsmtFinType2: Quality of second finished area (if present)
BsmtFinSF2: Type 2 finished square feet
BsmtUnfSF: Unfinished square feet of basement area
TotalBsmtSF: Total square feet of basement area
Heating: Type of heating
HeatingQC: Heating quality and condition
CentralAir: Central air conditioning
Electrical: Electrical system
1stFlrSF: First Floor square feet
2ndFlrSF: Second floor square feet
LowQualFinSF: Low quality finished square feet (all floors)
GrLivArea: Above grade (ground) living area square feet
BsmtFullBath: Basement full bathrooms
BsmtHalfBath: Basement half bathrooms
FullBath: Full bathrooms above grade
HalfBath: Half baths above grade
Bedroom: Number of bedrooms above basement level
Kitchen: Number of kitchens
KitchenQual: Kitchen quality
TotRmsAbvGrd: Total rooms above grade (does not include bathrooms)
Functional: Home functionality rating
Fireplaces: Number of fireplaces
FireplaceQu: Fireplace quality
GarageType: Garage location
GarageYrBlt: Year garage was built
GarageFinish: Interior finish of the garage
GarageCars: Size of garage in car capacity
GarageArea: Size of garage in square feet
GarageQual: Garage quality
GarageCond: Garage condition
PavedDrive: Paved driveway
WoodDeckSF: Wood deck area in square feet
OpenPorchSF: Open porch area in square feet
EnclosedPorch: Enclosed porch area in square feet
3SsnPorch: Three season porch area in square feet
ScreenPorch: Screen porch area in square feet
PoolArea: Pool area in square feet
PoolQC: Pool quality
Fence: Fence quality
MiscFeature: Miscellaneous feature not covered in other categories
MiscVal: $Value of miscellaneous feature
MoSold: Month Sold
YrSold: Year Sold
SaleType: Type of sale
SaleCondition: Condition of sale

Thanks for reading, feel free to reach out anytime at gibert.medeiros8046@gmail.com for questions or comments, I would love any feedback as im constantly trying to expand my knowledge.