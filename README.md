# Prediction-of-Heart-Failure-Patients
An exploratory analysis on clinical dataset of heart failure patients and prediction with neural network.

## Project Summary
With the successful integration of machine learning technique for medical diagnosis, heart physicians and medical practitioners are able to forecast the possibility whether a heart failure patient can survive or not by prioritising serum creatinine and ejection fraction for consideration. As such further research into the incorporation of computational algorithm should be encouraged. 

This research aims to confirm the machine learning classifier modelling and exploratory analysis to obtain the most important risk factors in the clinical dataset carried out by Davide Chicco and Giuseppe Jurman (2020) and further improve the research analysis by performing Descriptive statistical analysis, Principal component analysis and Factor analysis as well as Binary classification modelling with Neural Network of different hidden layers, draw conclusion on clinical features of patients with heart failure disease.

## Data Description
The heart clinical dataset consists of 299 heart failure patients collected between April–December 2015 at the Faisalabad Institute of Cardiology and at the Allied Hospital in Faisalabad (Punjab, Pakistan). The patients comprising of 194 men and 105 women diagnosed with left ventricular systolic dysfunction with heart failure history. The dataset consists of 13 clinical features describing the patient’s health condition, state of their body and lifestyle as shown in the table below detailing the patient’s age, anaemia level, whether or not the patients have hypertension or not, level of the creatinine phosphokinase (CPK) in the body, if the patient is diabetic or not and so on as well as their data types, unit measurement and type of variable.

![image](https://user-images.githubusercontent.com/76513466/137559169-97306ec8-1fb1-446c-93f6-0c901d2a2ac8.png)

As this dataset arranged into 299 rows and 13 columns, is a multivariate comprising of binary and continuous variable types, the tables above highlight the binary variables in regard to the clinical features with the deceased patient amounting for 67.89% of the total sample population in contrast to the 32.11% of the patient alive after the follow-up period.

## Data Mining Techniques and Applications
Statistical analysis can be descriptive or predictive depending on the aim of the analysis. Descriptive statistics involves the measure of dispersion, distribution, summary, and central tendency of data. The main purpose of statistical analysis is to draw statistical inference and make generalisation of each sample group and population. Predictive analysis uses data, statistical algorithms, and machine learning techniques to determine the likelihood of future results based on historical data through various predictive modelling techniques such as Linear regression (or least square method), Logistic regression, Time series analysis, ANN and so on.

![image](https://user-images.githubusercontent.com/76513466/137569302-17a2ad04-8306-4689-b0ee-e49713c6d9fb.png)

![image](https://user-images.githubusercontent.com/76513466/137569453-65c8796f-3964-4c21-b7f5-2b4b5c8ce641.png)

![image](https://user-images.githubusercontent.com/76513466/137569493-cd644076-6773-4684-91aa-c4ae40e332a4.png)

![image](https://user-images.githubusercontent.com/76513466/137569767-a968c673-7ac0-464a-af71-5e32cc21d387.png)

## Principal Component Analysis (PCA)
Principal Component Analysis (PCA) is a dimensionality-reduction method used to reduce the parameters of a dataset by presenting each data point only on the first major components while obtaining data of lower parameters by preserving as many different variations of data as possible. It is used to identify and replace a group of highly correlated variables that may be redundant with a few principal correlated variables and still retain the key features of the dataset.

Similar to PCA, the new variables obtained after undergoing factor analysis are orthogonal and can also be classified as a pre-processing step in data mining although it is incorporated in structured dataset containing both qualitative and quantitative variables. . Factor analysis acts as PCA for quantitative variable types and Multiple Correspondence Analysis for qualitative variables when the goal of pre-processing is to obtain variable factors.

![image](https://user-images.githubusercontent.com/76513466/137569606-5b4c87b0-abe6-4e3b-8789-e60dc217b0a0.png)

![image](https://user-images.githubusercontent.com/76513466/137569631-6309df3a-e406-425e-a96a-2db2fcc6281f.png)

![image](https://user-images.githubusercontent.com/76513466/137569667-56d88cfd-1c53-4b43-871d-7a6f93235c7b.png)

![image](https://user-images.githubusercontent.com/76513466/137569676-06fbbfce-e5f9-4efd-8764-5af66ef0d6fd.png)

![image](https://user-images.githubusercontent.com/76513466/137569693-da005888-ecea-4048-aed4-a94f0fc9e840.png)

![image](https://user-images.githubusercontent.com/76513466/137569703-7244b7f7-abaa-449b-b880-9895575192a3.png)

![image](https://user-images.githubusercontent.com/76513466/137569723-8fe3d20b-c697-40a1-810c-650be2cabd4a.png)

## Artificial Neural Network
A group of logistic regression analysis with inputs, hidden layers, and predicted probability with neurons each with bias and activation function constitute the concept of neural networks. A neural network is a series of algorithms that endeavors to recognize underlying relationships in a set of data through a process that mimics the way the human brain operates. Neural networks are multi-layer networks of neurons (the blue and magenta nodes in the chart below) that we use to classify things, make predictions, etc.

![image](https://user-images.githubusercontent.com/76513466/137569184-928d896c-6f12-4c60-8203-63cedf831d86.png)

### Steps and Results from Artificial Neural Network
Neural network is built by splitting and training dataset to understand the relationship between the clinical data and the classifier prediction model.
- To build the neural network for this dataset, the continuous variable types are normalised to balance the variance range and simplify the data features so that all the variables are within the range of 0 and 1.
- The data features normalised include Age, Creatinine Phosphokinase, Ejection Fraction, Platelets, Serum Creatinine, Serum Sodium and Time.
- The Death Event is converted into 2 levels factor variable of 0 and 1 with the as.factor() R function set to death or alive outcome and the Time variable and Sex feature are excluded from the dataset.
- The model response returned a TRUE and FALSE output with a result matrix of 1 column and several rows of information.
- The caret library helps streamline the process of creating a prediction model with two column outputs and the cbind is to plot the prediction model against the predicted death 
event.
- The result show conclusion of 56 dead outcome and 34 Alive outcome after which the model is evaluated using test$DEATH_EVENT.
- A confusion matrix is constructed below of a cross tabulation between the observed and predicted variable outcome. The p-value indicates a high accuracy level to accept the 
prediction model.

![image](https://user-images.githubusercontent.com/76513466/137569367-67d6f0d2-6af6-4f2b-86fd-bf4e951c47bd.png)

## Conclusion
Upon the successful completion of this research analysis, it can be drawn that this clinical dataset can be accurately reduced with the application of principal components methods such as Principal Components Analysis and Factor Analysis as well as Machine Learning Algorithm, neural networks. This research can be further expanded by experimenting with the parameters of the neural network to improve the prediction model accuracy.


