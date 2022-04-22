# Project-1
This project is taking a look at Bank Loan Modeling and what criteria in a client leads to personal loan offers being accepted. The data source included below was cleaned and outputted to a CSV file so that each member could read into their respective notebooks. The team worked to study the effects of the following criteria on the acceptance of personal loans:
* Income Level
* Age
* Education Level
* Family Size
* Mortgage Status
* Living Conditions (rural vs urban)

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

## Visualization and Analysis
Income vs Personal Loan Plots and Analysis

![Bar plot of mean incomes](/data_retrieval/plots/income_loans_bar.png)
* Clients with a personal loan have a much higher annual income on average ($144,745.83) than clients who do not have a personal loan ($66,237,39)

![Bin1 Pie](/data_retrieval/plots/income_bin1_loans_pie.png)
![Bin2 Pie](/data_retrieval/plots/income_bin2_loans_pie.png)
![Bin3 Pie](/data_retrieval/plots/income_bin3_loans_pie.png)
![Bin4 Pie](/data_retrieval/plots/income_bin4_loans_pie.png)
* No client with an annual income less than $25,000 had a personal loan taken out
* Only 0.3% of clients with an annual income between $25,000-75,000 had a personal loan
* 15.9% of clients with an annual income between $75,000-$150,000 had a personal loan
* 49.3% of clients with an annual income over $150,000 had a personal loan
* As the annual income of a client increases, it becomes exceedingly more likely for them to want to take out a personal loan with the bank. This is likely due to these clients having more capital in order to start paying off the loans they take out.  

