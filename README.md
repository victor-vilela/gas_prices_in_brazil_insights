# Gas Prices in Brazil Insights

#### This project was made by Victor Vilela.

# 1. The Company.

The National Agency of Petroleum, Natural Gas and Bio fuels (ANP in Portuguese) releases weekly reports of gas, diesel and other fuels prices used in transportation across the country. These datasets bring the mean value per liter, number of gas stations analyzed and other information grouped by regions and states across the country.

# 2. Objective

Create insights into how different regions in Brazil saw their fuel prices changes

# 3. Solution Strategy

My strategy to solve this challenge was inspired by CRIPS-DS <!-- medium -->:

## 3.1. Tools
- Pandas
- Numpy
- Matplotlib
- Seaborn

## 3.2. Process

**Step 01. Data Description:**
- Rename Columns
- Data Dimensions
- Data Types (RAW)
- Change Data Types
- Data Types (Changed)

**Step 02. Descriptive Statistical:**

| attributes                    |          mean |   median |           std |        min |      max |     skew |   kurtosis |
|:------------------------------|--------------:|---------:|--------------:|-----------:|---------:|---------:|-----------:|
| numero_de_postos_pesquisados  |   221.066     |  99      |   387.94      |      1     | 4167     |  4.55525 |   27.5701  |
| preco_medio_revenda           |    11.4734    |   2.899  |    19.1618    |      0.766 |  107.5   |  2.10695 |    3.51105 |
| desvio_padrao_revenda         |     0.684132  |   0.121  |     1.40332   |      0     |   10.748 |  2.84447 |    8.45871 |
| preco_minimo_revenda          |     9.97782   |   2.69   |    16.4338    |      0.59  |  100     |  2.17068 |    3.99278 |
| preco_maximo_revenda          |    13.2339    |   3.2    |    22.4514    |      0.999 |  120     |  2.13819 |    3.64197 |
| margem_media_revenda          | -4697.38      |   0.381  | 21163.5       | -99999     |   36.847 | -4.28112 |   16.3283  |
| coef_de_variacao_revenda      |     0.0452982 |   0.041  |     0.0247629 |      0     |    0.395 |  1.00484 |    2.50332 |
| preco_medio_distribuicao      | -4682.19      |   2.359  | 21145.8       | -99999     |   83.137 | -4.28582 |   16.3686  |
| desvio_padrao_distribuicao    | -4690.13      |   0.076  | 21144         | -99999     |   18.385 | -4.28583 |   16.3686  |
| preco_minimo_distribuicao     | -4683.31      |   2.238  | 21145.6       | -99999     |   83     | -4.28582 |   16.3686  |
| preco_maximo_distribuicao     | -4680.97      |   2.5376 | 21146.1       | -99999     |   94.5   | -4.28582 |   16.3686  |
| coef_de_variacao_distribuicao | -4690.64      |   0.029  | 21143.9       | -99999     |    0.78  | -4.28583 |   16.3686  |

**Step 03. Preparation EDA:**
- Hypotheses Creation
- Feature Engineering
- Data Filtering

**Step 04. Exploratory Data Analysis:**
- Answering Hypotheses

# 4. Top 3 Data Insights

**Hypothesis 01: Percentage change over 2020, the year of the COVID-19 pandemic**
- Fuel prices dropped across the country after the start of the pandemic.

**Hypothesis 02:States with the highest values per Product - Annually**
- States far from the Brazilian coast, are the ones with the highest fuel prices.

**Hypothesis 03:How have different regions of Brazil seen their gas prices change?**
- GLP prices have increased year by year since 2004, so that some regions had more than 150% increase.

# 5. Business Results

- Historically, fuel prices in Brazil have increased considerably so that some products had more than 100% increase over the 15 years analyzed.
- Some states far from the Brazilian coast, such as Acre, are the ones with the highest fuel prices, probably because access is more difficult and consequently the cost of logistics will be more expensive as well.

# 6. Lessons Learned

- Manipulate OOP visualization toos (Matplotlib and Seaborn)
- Best Practices to filtering and manipulate data using pandas and numpy

# 7. Next Steps to Improve

- Create a dashboard with Streamlit to best analysis

