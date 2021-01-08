# Vehicles-Emissions-Prediction

## Objective

This project aiming to create supervised model that can predict the CO2 Emissions for new light-duty vehicles for retail sale in Canada and accomplish high evaluation accuracy.

## Data 

#### `FuelConsumption.csv`:

We have downloaded a fuel consumption dataset, **`FuelConsumption.csv`**, which contains model-specific fuel consumption ratings and estimated carbon dioxide emissions for new light-duty vehicles for retail sale in Canada. [Dataset source](http://open.canada.ca/data/en/dataset/98f1a129-f628-4ce4-b24d-6f16bf24dd64?cm_mmc=Email_Newsletter-_-Developer_Ed%2BTech-_-WW_WW-_-SkillsNetwork-Courses-IBMDeveloperSkillsNetwork-ML0101EN-SkillsNetwork-20718538&cm_mmca1=000026UJ&cm_mmca2=10006555&cm_mmca3=M12345678&cvosrc=email.Newsletter.M12345678&cvo_campaign=000026UJ&cm_mmc=Email_Newsletter-_-Developer_Ed%2BTech-_-WW_WW-_-SkillsNetwork-Courses-IBMDeveloperSkillsNetwork-ML0101EN-SkillsNetwork-20718538&cm_mmca1=000026UJ&cm_mmca2=10006555&cm_mmca3=M12345678&cvosrc=email.Newsletter.M12345678&cvo_campaign=000026UJ&cm_mmc=Email_Newsletter-_-Developer_Ed%2BTech-_-WW_WW-_-SkillsNetwork-Courses-IBMDeveloperSkillsNetwork-ML0101EN-SkillsNetwork-20718538&cm_mmca1=000026UJ&cm_mmca2=10006555&cm_mmca3=M12345678&cvosrc=email.Newsletter.M12345678&cvo_campaign=000026UJ&cm_mmc=Email_Newsletter-_-Developer_Ed%2BTech-_-WW_WW-_-SkillsNetwork-Courses-IBMDeveloperSkillsNetwork-ML0101EN-SkillsNetwork-20718538&cm_mmca1=000026UJ&cm_mmca2=10006555&cm_mmca3=M12345678&cvosrc=email.Newsletter.M12345678&cvo_campaign=000026UJ)

-   **MODELYEAR** e.g. 2014
-   **MAKE** e.g. Acura
-   **MODEL** e.g. ILX
-   **VEHICLE CLASS** e.g. SUV
-   **ENGINE SIZE** e.g. 4.7
-   **CYLINDERS** e.g 6
-   **TRANSMISSION** e.g. A6
-   **FUELTYPE** e.g. z
-   **FUEL CONSUMPTION in CITY(L/100 km)** e.g. 9.9
-   **FUEL CONSUMPTION in HWY (L/100 km)** e.g. 8.9
-   **FUEL CONSUMPTION COMB (L/100 km)** e.g. 9.2
-   **CO2 EMISSIONS (g/km)** e.g. 182   --> low --> 0

## Methodolgies

- Exploratory Data Analysis (EDA).
- Data Visualization.
- Supervised Machine Learning. 
- Multiple Linear Regression (MLR).
- Polynomial Regression.
- Model Evaluation.

## Technologies

- Python.
- Jupyter.
- Pandas.
- Numpy.
- Matplotlib.
- scikit-learn.

## Results
Considering the following **Evaluation Metrics**, we can see that **Polynomial Regression** is more suitable to build our model.


<table align="left" style="width: 40%">
  <tr align="left">
    <th>Model</th>
    <th>MAE</th> 
    <th>MSE</th>
    <th>R2</th>
  </tr>
  <tr>
    <td>MLR</td>
    <td>11.65</td>
    <td>330.18</td>
    <td>0.91</td>
  </tr>
  <tr>
    <td>Polynomial Reg.</td>
    <td>7.59</td>
    <td>173.06</td>
    <td>0.95</td>
  </tr>
</table>
<br>
<br>
<br>
<br>
<br>


#### Evaluation Metrics:

- **Mean Absolute Error MAE:** It is the mean of the absolute value of the errors. it's non negative and values close to zero are better.<br>
    **𝑀𝐴𝐸=1𝑛∑𝑖=1𝑛|𝑦𝑖−𝑦𝑖^|**

- **Mean Squared Error MSE:** The average squared difference between the estimated values and true value. it's non negative and values close to zero are better.<br>
    **𝑀𝑆𝐸=1𝑛∑𝑖=1𝑛(𝑦𝑖−𝑦𝑖^)2**

- **R-squared score** is not error, but is a popular metric for accuracy of your model. It represents how close the data are to the fitted regression line. The higher the R-squared, the better the model fits your data. Best possible score is 1.0 and it can be negative (because the model can be arbitrarily worse).<br>
**𝑅2=1−𝑆𝑆𝑟𝑒𝑠𝑆𝑆𝑡𝑜𝑡**<br>
Where; $SS_{res}$ is the sum of squares of the residual errors. And $SS_{tot}$ is the total sum of the errors.
