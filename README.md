# Supervised_Learning

Supervised learning is a category of machine learning that trains using labeled data in order to make new predicitions given a set of feature instances. In the supervised.ipynb notebook, we will first use supervised learning in order to predict a 6-dimensional space of planet parameters (T,ln(H2O),ln(CO2),ln(CH4),ln(CO),ln(NH3)) from a 52-dimensional space of spectra values (one dimension for each wavelength bin). We will explore supervised learning methods including support vector regressors, decision tree regressors, random forest regressors, k-nearest neighbor regressors, along with ensemble learning methods, such as voting, stacking, and bagging regressors. Other models in the notebook include boosting methods, such as adaptive boosting (ADA), gradient boosting (GBM), and extreme gradient boosting (XGBoost). 

Then, we will use the spectra values to predict an 18-dimensional space consisting of the 16th, 50th, and 84th percentiles (Light track) of the same planet parameter values we saw above. The regular track was to predict the full distribution of the planet parameters, and while I did not include this hdf5 file here, it can be reproduced from the Ariel baseline solution notebook. The Ariel Baseline solution was included in this notebook, along with their helper functions in order to see how to compute the spec_matrix. I added their Light Track solution, which is the Ariel submission csv file.

Data Files from NeurIPS 2022 Ariel Data Challenge: 

Ariel Website (includes data): [https://www.ariel-datachallenge.space]()

Zenodo (includes data): [https://zenodo.org/record/6770103#.Y1r51-zMLPb]()

1. **Features 1:** AuxiliaryTable: Star and Planet Parameters (91392,10)
2. **Features 2:** spec_matrix: Wavelength bin [0], spectra (transit depth) [1], noise in the transit [2], error in wavelength bin [3] for 52 wavelength bins (91392,52,4)

The entire 91392 values for the spectra data for the challenge were given, however, the file was too large to be uploaded here.

3. **Targets:** FM_Parameter_Table: Consists of Planet Temperature, and log traces concentrations for H2O, CH4, CO2, CO, NH3 (91392,6)

The test versions of these files consist of 500 instances rather than 91392, and only the test auxilliary data, spectra, and noise are provided here.
