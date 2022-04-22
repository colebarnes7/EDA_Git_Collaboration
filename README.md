# Project-1
This project is taking a look at Bank Loan Modeling and what criteria in a client leads to personal loan offers being accepted. The data source included below was cleaned and outputted to a CSV file so that each member could read into their respective notebooks. The team worked to study the effects of the following criteria on the acceptance of personal loans:
* Income Level
* Age
* Education Level
* Family Size
* Mortgage Status
* Zip Codes

## Contributors
* Cole Barnes
* Debolina Bhaumik
* Ryan Cheng
* Kanu Madhok

## Data Source
https://www.kaggle.com/datasets/itsmesunil/bank-loan-modelling

## Technologies
* Python
* Pandas
* Matplotlib
* Jupyter Notebook
* NumPy
* SciPy
* Excel
* Requests
* Gmaps
* Json

## Installation
Code was tested using Python 3.8. The environment was setup as follows:
```
conda create -n PythonData38 python=3.8 anaconda
source activate PythonData38
jupyter notebook
```
If environment does not include some of the technologies from above install using the following in terminal:
```
conda install pandas
conda install matplotlib
conda install numpy
pip install scipy
```

## Featured Notebooks
| Document Title | Purpose |
| ------------- | ------------- |
| cleaning_data.ipynb | Cleaned raw data and outputted to CSV |
| cole_retrieval.ipynb | Analyzed relationships between income and personal loans  |
| debolina_notebook.ipynb | Working on data distribution, correlation and impact of education and family size on Personal loan |
| City_Retrieval.ipynb | Working to gather and assign cities to different zip codes using Google Geocode api |
| Zip_Code_Analysis.ipynb | Identifying relationships between zip code, personal loan, and other attributes of the dataset |
| Mortgage_Analysis.ipynb | Working to analyze how likely a loan is going to be accepted based off of previous debt/value of mortgage |

## Visualization and Analysis
Income vs Personal Loan Plots and Analysis<br/>
![Bar plot of mean incomes](/Graphs/income_plots/income_loans_bar.png)
* Clients with a personal loan have a much higher annual income on average ($144,745.83) than clients who do not have a personal loan ($66,237,39)<br/>
![Bin1 Pie](/Graphs/income_plots/income_bin1_loans_pie.png)
![Bin2 Pie](/Graphs/income_plots/income_bin2_loans_pie.png)
![Bin3 Pie](/Graphs/income_plots/income_bin3_loans_pie.png)
![Bin4 Pie](/Graphs/income_plots/income_bin4_loans_pie.png)
* No client with an annual income less than $25,000 had a personal loan taken out
* Only 0.3% of clients with an annual income between $25,000-75,000 had a personal loan
* 15.9% of clients with an annual income between $75,000-$150,000 had a personal loan
* 49.3% of clients with an annual income over $150,000 had a personal loan
* As the annual income of a client increases, it becomes exceedingly more likely for them to want to take out a personal loan with the bank. This is likely due to these clients having more capital in order to start paying off the loans they take out.<br/>  
Age, Education Level and Family Size vs Personal Loan Plots and Analysis<br/>
* Age of the customers in the dataset is normally distributed generally falling between 30 and 60 years of age. The mean and median age are almost equal
* Work experience is normally distributed, while income is positively skewed.
![Income Histogram](/data/cleaned_data/income_histogram.png)
![Age/Experience Scatter](/data/cleaned_data/scatter_age_experience_boxplot.png)
![Loan/Income Boxplot](/data/cleaned_data/loan_income_boxplot.png)
* Since income is positively skewed, the mean is higher than the median as a large portion of the dataset resides between $45k-55k income
![Education Bar](/data/cleaned_data/distribution_PL_among_Education.png)
![Education Pie](/data/cleaned_data/Proportion_edu_levels_Personal_Loan.png)
![Family Size](/data/cleaned_data/Proportion_family_size_among_PL.png)
* Of the customers who have a personal loan, 42.7% and 37.9% had an advanced and graduate level of education respectively.
* Customers with a higher level of education should be targeted with personal loan offers.
* Of customers with a personal loan, 27.9% and 27.7% of them had a family size of 4 and 3 respectively.<br/>