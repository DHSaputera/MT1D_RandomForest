# MT1D_RandomForest



1D Magnetotelluric inversion using Random Forest.

In geophysical exploration, earth's subsurface can be imaged by measuring electromagnetic fields in the surface.
Magnetotelluric (MT) is one of the passive electromagnetic method, typically the electromagnetic source is coming from the sun, radio waves, lightning.

For 1D problem, the earth's subsurface is characterized by electrical impedance, which is the ratio between electric and magnetic fields measured at the surface.
The magnitude of the electrical impedance is proportional to the layer's resistivities, which is calculated as the apparent resistivity.
The phase, the ratio of imaginary and real component, of the electrical impedance characterize the change in the subsurface.

Inversion goal is to find the best earth subsurface model with the response that fit the measured data. There exist many algorithm to do this process.
In this code, I implemented random forest regressor for predicting the best earth model that fit a given data. 

I provide the jupyter notebook for generating data and build random forest model for three layer case. I also provide the pre-made data and pre-trained model that can be loaded in the notebook.
MT1D_RandomData : generating random 1D MT data with log-uniform distributed parameters. [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/DHSaputera/MT1D_RandomForest/blob/main/MT1D_RandomData.ipynb)
mt1d_inversion_randomforest: building random forest model for inversion. [![Open In Colab](https://colab.research.google.com/github/DHSaputera/MT1D_RandomForest/blob/main/mt1d_inversion_randomforest.ipynb)

For machine learning model in more complex case, there should be many work that can be searched in google scholar.

The code for calculating 1D MT response can be found in https://www.digitalearthlab.com/tutorial/tutorial-1d-mt-forward/
