# Data Analysis of  ecommerce sites data

### Requirements 
Ensure you have `Python 3` and the package manager `pip` installed.\
Run the following command to in your jupyter notebook
```
!pip install pyunpack
!pip install rarfile
!pip install patool
!pip install gdown
!pip install numpy
!pip install pandas
!pip install matplotlib
!pip install seaborn
!pip install pyspark
!pip install findspark
```
### Data Set
The CSV file used has the following details about products from various ecommerce sites.
* UUID (Primary Key)
* Price (String)
* Price_unfiltered (String)
* Product Type
* Category
* Level 1 -> This is just a classification of a product.

The dataset has `13790000` observations\
The zipped dataset was downloaded from  `google drive` using `gdown` and extracted using `rarfile ` and `pyunpack`.

### Data Visualization
 `pandas`was used to load a chunksize of `100000` from the data for easy processing while `matplotlib` and `seaborn` was used for the visualization.

### Running the code
* The code are all in a jupyter-notebook : restart the kernel and run all cells from google colab or jupyter notebook locally to view outputs

### Results Obtained
Due to the size of the data, `Pyspark` was use since it would not load data into the RAM unless a computation is required.\
The following results were generated from the data .
1. Products without prices
2. Count of products without prices and with prices in each Product Type, Category, Level 1
3. Correct Product Prices in the correct format (eg: $56) wherever possible and separate them into currency and value columns.
4. List out the categories with average price of product.

