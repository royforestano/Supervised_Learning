# Supervised_Learning

Supervised learning is a category of machine learning that trains using labeled data in order to make new predicitions given a set of feature instances. In the supervised.ipynb notebook, we will explore supervised learning methods including support vector regressors, decision tree regressors, random forest regressors, k-nearest neighbor regressors, along with ensemble learning methods, such as voting, stacking, and bagging regressors. Other models in the notebook include boosting methods, such as adaptive boosting (ADA), gradient boosting (GBM), and extreme gradient boosting (XGBoost).

Data Files from NeurIPS 2022 Ariel Data Challenge: 

Ariel Website (includes data): [https://www.ariel-datachallenge.space]()
Zenodo (includes data): [https://zenodo.org/record/6770103#.Y1r51-zMLPb]()

1. **Features 1:** AuxiliaryTable: Star and Planet Parameters (91392,10)
2. **Features 2:** spec_matrix: Wavelength bin [0], spectra (transit depth) [1], noise in the transit [2], error in wavelength bin [3] for 52 wavelength bins (91392,52,4)

The entire 91392 values for the spectra data for the challenge were given, however, the file was too large to be uploaded here.

3. **Targets:** FM_Parameter_Table: Consists of Planet Temperature, and log traces concentrations for H2O, CH4, CO2, CO, NH3 (91392,6)

The test versions of these files consist of 500 instances rather than 91392, and only the test auxilliary data, spectra, and noise are provided here.
