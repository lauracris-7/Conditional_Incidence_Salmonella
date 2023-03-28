# Conditional_Incidence_Salmonella
Scripts used in the methodology developed for the EnvDis thesis
by Laura C. Gonzalez Villeta

Ojective of the analysis: 
The code does look at how the risk of salmonellosis in humans depends on weather variables

## Content and order for running the scripts:
1. Conditional_Probability_Analysis_and_plots_complete_Detrend: "master" file to import the data and apply all the functions. 
2. Function_Input_files: reads salmonellosis incidence, weather and residents data
3. Function_Wavelet_analysis: Wavelet analysis for  to check for periodicity in the data
4. Function_Detrend_analysis: Remove temporal trend from the time-series of salmonellosis
5. Function_Conditional_Incidence_Uniform: stratification of disease and categorized weather data
6. Function_Reconstruction: application of the conditional probability calculated in England and Wales. Valitation of the weather factors chosen
7. Function_Plot_Reconstruction: visualization of the comparison of empirical and modelled cases
8. Function_Conditional_Incidence_Quantile: stratification of disease and weather data with a quantile distribution (i.e. each weather bin contains the same number of observations).
9. Function_Plot_Conditional_Incidence_Quantile: visualization of the conditional incidence of 3 simultaneous weather factors.
 
## Adaptations required to use the code:
- Select weather variables of interest (File 1., lines 39-41)
- Match the dataframe structure for readint the data in a wide format
- Adapt the reporting delays if working with an infectious agent other than Salmonella  (File 1., line 28, variable "width")
- Size of weather bins customizable (File 1., line 101)
