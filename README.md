# Code and data associated with the manuscript ``Quantifying inclination shallowing and representing flattening uncertainty in sedimentary paleomagnetic poles''

## code

This folder contains Jupyter notebooks developed using a Python 3 kernel that generates the figures and conducts the data analysis associated with the study. 

#### Cutface_bedding.ipynb

This notebook compiles bedding measurements for the Cutface Creek Sandstone that were used to determine the tilt correction for the paleomagnetic data.

#### Cutface_common_mean_tests.ipynb

This notebook implements common mean tests between the detrital remanent magnetization (DRM) 'ht' component of the Cutface Creek Sandstone and directions for pigmentary hematite 'mt' and the North Shore volcanic group for progressively applied f factors to the DRM directions.

#### Cutface_pmag.ipynb

This notebook conducts data analysis and visualizations associated with the Cut Face Creek paleomagnetic data. The following is accomplished in the notebook:
- plots are developed for the specimen level data from the Cut Face Creek Sandstone using the fits developed in Pmag_GUI
- data from the North Shore Volcanic Group are imported and compared to the Cut Face data including a common mean test with the 'mt' Cut Face directions
- a schematic figure illustrating the effects on directions of inclination shallowing is developed
- the E/I method is applied to the Cut Face DRM directions with the results being analyzed including plots of the resulting f factor and implied paleolatitude distributions
- the E/I relationship for the CRM and corrected DRM directions is calculated and plotted
- the f values estimated for the empirical comparisons in the ```Cutface_common_mean_tests.ipynb``` notebook are plotted with that determined from the E/I method

#### Cutface_Kent.ipynb

This notebook develops the method that is now implemented in ```ipmag.find_ei_kent``` and described in the text in order to incorporate inclination flattening uncertainty in paleomagnetic poles. This approach takes the f factors that are output from E/I bootstraps to estimate the elliptical shape of the Kent distribution that can summarize the uncertainty associated with inclination shallowing. The notebook also implements a compilation based approach that develops this Kent distribution uncertainty estimate from resampling the f factors within the compilation developed in this study. This method is implemented in the ```ipmag.find_compilation_kent``` function.

#### Inc_shallowing_compilation.ipynb

This notebook compiles published estimated f factors from the literature. These data are then visualized with histograms and summarized in a table that is exported into the format within the Supporting Information.

## data

This folder contains structural measuments from the Cut Face Creek sandstone, paleomagentic data developed from the Cut Face Sandstone and compiled paleomagnetic data from the North Shore Volcanics. 



