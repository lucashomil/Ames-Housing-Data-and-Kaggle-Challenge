
# Executive Summary

## Problem Statement

The main purpose of this data science project is to predict the home prices in Ames, Iowa by using regression models. By doing this data analysis, we can find the theoretical relationship have in mind. Probably, there is specific interest in the magnitudes and signs of the coefficients. Throughout the iterative modeling and feature selection processes manually and automatedly, we can gain a deeper insight into 80 variables which were directly related to property sales and understand better the mechanism behind various models.


## Data Description
In this data science project, I'll explore the Ames, Iowa Housing Dataset, prepared by Dean De Cock, and described in the paper [Ames, Iowa: Alternative to the Boston Housing Data as an End of Semester Regression Project](http://jse.amstat.org/v19n3/decock.pdf)

| feature | dype |Description
| --- | --- | --- |
| MS SubClass | int64 |
| MS Zoning | object |Identifies the general zoning classification of the sale.
| Lot Frontage | float64 |Linear feet of street connected to property
| Lot Area | int64 |Lot size in square feet
| Street | object |Type of road access to property
| Lot Shape | object |General shape of property
| Land Contour | object |Flatness of the property
| Neighborhood | object |Physical locations within Ames city limits
| Condition 1 | object |Proximity to main road or railroad
| Condition 2 | object |Proximity to main road or railroad (if a second is present)
| Bldg Type | object |Type of dwelling
| House Style | object |Style of dwelling
| Overall Qual | int64 |Overall material and finish quality
| Overall Cond | int64 |Overall condition rating
10 Very Excellent
| Year Built | int64 |Original construction date
| Year Remod/Add | int64 |Remodel date (same as construction date if no remodeling or additions)
| Roof Style | object |Type of roof
Flat Flat
| Roof Matl | object |Roof material
| Exterior 1st | object |Exterior covering on house
| Exterior 2nd | object |Exterior covering on house (if more than one material)
| Mas Vnr Type | object |Masonry veneer type
| Mas Vnr Area | float64 |Masonry veneer area in square feet
| Exter Qual | object |Exterior material quality
| Exter Cond | object |Present condition of the material on the exterior
| Foundation | object |Type of foundation
| Bsmt Qual | object |Height of the basement
| Bsmt Cond | object |General condition of the basement
| Bsmt Exposure | object |Walkout or garden level basement walls
| BsmtFin Type 1 | object | Quality of basement finished area
| BsmtFin Type 2 | object |Quality of second finished area (if present)
| Total Bsmt SF | float64 |Total square feet of basement area
| Heating | object |Type of heating
| Heating QC | object |Heating quality and condition
| Central Air | object |Central air conditioning
| Electrical | object |Electrical system
| Gr Liv Area | int64 |Above grade (ground) living area square feet
| Bsmt Full Bath | float64 |Basement full bathrooms
| Bsmt Half Bath | float64 |Basement half bathrooms
| Full Bath | int64 |Full bathrooms above grade
| Half Bath | int64 |Half baths above grade
| Bedroom AbvGr | int64 |Number of bedrooms above basement level
| Kitchen AbvGr | int64 |Number of kitchens
| Kitchen Qual | object |Kitchen quality
| TotRms AbvGrd | int64 |Total rooms above grade (does not include bathrooms)
| Functional | object |Home functionality rating
| Fireplaces | int64 |Number of fireplaces
| Fireplace Qu | object |Fireplace quality
| Garage Type | object |Garage location
| Garage Yr Blt | float64 |Year garage was built
| Garage Finish | object |Interior finish of the garage Fin Finished
| Garage Cars | float64 |Size of garage in car capacity
| Garage Area | float64 |Size of garage in square feet
| Garage Qual | object |Garage quality
| Garage Cond | object |Garage condition
| Paved Drive | object |Paved driveway
| Wood Deck SF | int64 |Wood deck area in square feet
| Open Porch SF | int64 |Open porch area in square feet
| Enclosed Porch | int64 |Enclosed porch area in square feet
| 3Ssn Porch | int64 |Three season porch area in square feet
| Screen Porch | int64 |Screen porch area in square feet
| Pool Area | int64 |Pool area in square feet
| Mo Sold | int64 |Month Sold
| Yr Sold | int64 |Year Sold
| Sale Type | object |Type of sale
| SalePrice | int64 | the property's sale price in dollars

# Conclusion

My Lasso model is done with a cross validated score of 89.5% on my train set which indicated that the model works good.

However, in regression with multiple independent variables, the coefficient tell us how much the dependent variable is expected to increase when that independent variable increases by one, holding all the other independent variables constant. However, if the variables are entered in the multiple regression and those variables are correlated with each other to high degree and correlated to our target variable, then the beta weights for these correlated independent variables are arbitrarily allocated predictive credit among the correlated independent variables.
