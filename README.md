# King County Housing Analysis
![15 Best Tips for Selling Your Home](https://github.com/Muthonikahuko/Phase-2-project/assets/54804370/6df46da7-1286-461f-bf19-e363b34f0afd)

Authors: 1. Ian Vaati 
         2. Bernadette Nganga
         3. Muthoni Kahuko

# Business understanding and problem overview
In this project, I will provide information using regression modeling analysis of house sales data in King County, for real estate agencies to advise homeowners on how renovations and improvements can affect the estimated values of their homes.

# Data understanding
From the ks_house_data.csv the data included records of 21597 houses sold in King County. We noticed that we have 21 columns:
id', 'date', 'price', 'bedrooms', 'bathrooms', 'sqft_living',
'sqft_lot', 'floors', 'waterfront', 'view', 'condition', 'grade',
'sqft_above', 'sqft_basement', 'yr_built', 'yr_renovated', 'zipcode',
'lat', 'long', 'sqft_living15', 'sqft_lot1'
We have the id which did not appear relevant at this stage. We also have the price which was our target variable. 
Thirdly we have quality of bedrooms, bathrooms, and floors with a grading system for the properties which contains the condition and grade. We have several dimensions in square feet such as the living area, lot area, above, and the basement. 
We also have the location data by zipcode, latitude, longitude, and distance to the nearest 15 neighbors
Lastly, we have year-built, year renovated, views, and waterfront

This was our data:

![data preview](https://github.com/Muthonikahuko/Phase-2-project/assets/54804370/25a196e3-c8fb-45b6-8b63-20e2f9f034c3)

Through this, we were able to see the data types we were working with. we realised we needed to investigate and clean the data as well.

![Data prev](https://github.com/Muthonikahuko/Phase-2-project/assets/54804370/b0f29169-f565-4434-a2b1-e055c25e230e)

# Data Cleaning
- We started Checking which columns have missing values and by what percentage. We noticed that yr_renovated, waterfront, and view had missing values. Which we fixed.
- We fixed the data types
- Looked for outliers and removed them from our data frame

![analysi](https://github.com/Muthonikahuko/Phase-2-project/assets/54804370/58f97ade-b05d-46fc-8cad-0f942e9be336)

Through the heatmap, we realized that the square footage of the living space had an effect on the pricing of the building more than any other feature of the house.

# Modelling the data
# Model 1
The data was ready for a baseline model giving us an R-squared value of 0.428 
![Model 1 results](https://github.com/Muthonikahuko/Phase-2-project/assets/54804370/2272bf3e-7938-4fcf-ac94-5b034c029a34)

![regression model 1](https://github.com/Muthonikahuko/Phase-2-project/assets/54804370/f5fb0ca9-e346-4e47-9d60-996423270768)

# Model 2
The data gave us an R-squared value of 0.538

![Model 2 results](https://github.com/Muthonikahuko/Phase-2-project/assets/54804370/5912c508-22d8-4a32-b22e-93cb4f9fb0e8)

![Model 2 regression](https://github.com/Muthonikahuko/Phase-2-project/assets/54804370/d23d7d43-1f65-40bb-971c-f9d6a6f5a16f)

# Model 3
The data gave us an R-squared value of 0.542
![Model 3 results](https://github.com/Muthonikahuko/Phase-2-project/assets/54804370/19777744-b769-4e2a-871e-f2dece8e93f8)

# Summary
The final model that we chose is Model 3. This is the reason:
- Baseline Model R-squared: 0.428
- Final Model R-squared: 0.542

The R-squared value in the final model (0.542) is higher than in the baseline model (0.428) and the model 2 (0.538). This indicates that the final model explains a larger proportion of the variance in the dependent variable (log-transformed price) compared to the baseline model. In practical terms, the final model provides a better fit to the data, capturing more of the variation in property prices.

# Recommendations
- Real estate agencies can benefit from utilizing the regression model for pricing guidance to provide homeowners with accurate insights into how renovations or improvements can affect the estimated value of their homes
- Agencies can also use the coefficients of the model to identify key renovation opportunities that have the most significant impact on home values.
- It's important for agencies to tailor their recommendations to individual homeowners based on their property's current condition, size, and location
- Keeping homeowners informed about current real estate market conditions is crucial, and agencies should educate their clients on how these conditions may affect the return on investment for renovations.






































