# Machine Learning algorithm that predicts heart diseases based on log-spectograms.


## Step 1: Data Importing
Import the data and setting the base path for easier access. Import the dataset based on patients as subgroups and connecting the patients with the features from another file.


## Step 2: Data Wrangling
1. Remove the trivial features from the feature set.
2. Transform feature data types into useable data types(age -> numeric values, data -> datetime) and dealing with missing data by subbing in n/a.
3. Create patient-diagnosis association.


## Step 3: Splitting the dataset into train/validation/test datasets
We use stratified sampling due to the low numbers of rare cases to keep the realistic distribution and avoid accidentally leaving a diagnosis out of the training set.


## Step 4: Cross-validation
K-fold cross validation is performed on the data to distribute the patients with rare diseases uniformly.


## Step 5: Dummy Baselines
Create a dummy baseling to evaluate the perforamce of the complex model later to determine the performance od each disease prediction.


## Step 6: Model on spectogram 
