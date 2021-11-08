# Illegal Conversion Risk Analytics

This is a project I managed with the Building Census project located in the office of the Chief Enforcement Officer at the NYC Department of Buildings and the Columbia University sociology department. The goal was to identify buildings in New York City that are at high risk of an illegal conversion. An illegal conversion occurs when an existing residential or commercial building is altered or modified to create an additional room, space, or unit without first getting approval from the DOB. Illegal conversions therefore often do not complying with Building and Fire Code. Many fire deaths are caused by illegal conversions because the illegally converted room or unit is often located in a cellar or attic that lack a second egress to escape a fire.

### Data
1. HPD, DOB and DOF data from NYC Open Data.  
2. HPD provides the list of 317,000 buildings in its jurisdiction, fields include BIN, classification, year built, etc.  
3. HPD data also includes buildings not currently registered with the housing authority (DOB Enforcement suspects these buildings as high risk due to high proportion of accidents and fires relative to other buildings with the same building classification).
4. DOB illegal conversion complaints  
5. Illegal conversion complaints routed to the DOB via 311  
6. DOF building classifications  

### Methods: Regression and Network Analysis
a. Use regression analysis to determine what factors are correlated with illegal conversions  
b. Summary of regression results:  
- 1-2 family unregistered buildings are more likely to be illegal conversions  
- Bad Actor Factor: A building in the network of an owner whose other buildings have received complaints is more likely to be an illegal conversion  

### Risk Analytics
- 110 of the owners were determined to be “bad actors”:  
    - Have a high percentage of violations and no access as final illegal conversion dispositions in their portfolio  
    - Own a high number of 1-2 family and non-registered buildings  
- The 110 bad actors own 14,459 out of the 317,539  HPD buildings (4.6% of the HPD buildings)  
- 12,986 of these buildings have had no illegal conversion complaints in the past three years  
- Highest risk buildings:  
    - 1759 1-2 family, unregistered buildings unknown to the DOB (no previous illegal conversion complaints)
 
 ### Spatial Analysis
 Map of 1759 High Risk Buildings  
 Highest density of illegal conversions are located in Queens and Brooklyn  
 
 ![HIGH RISK BUILDINGS MAP](https://user-images.githubusercontent.com/11237613/104370860-78775180-54ed-11eb-81b9-54599f394e26.png)

