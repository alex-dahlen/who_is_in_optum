# who_is_in_optum
Python code to accompany the paper "Selection bias in large healthcare claims databases". 

This is a zip-code level analaysis of the selection bias inherent in a particular healthcare claims database known as Optum's de-indentified 
Clinformatics Data Mart (CDM).  These styles of datasets are increasingly being used to generate real-world evidence for medical research, but
they also contain significant bias toward an older, Whiter, richer population.  

In this analysis, we use zip code-level census data to quantify this selection bias.  

This code goes through several steps:

    Read in census data at the census tract level
    Roll it up to the zip code level, and joining it to Optum population data.
    Exploratory analysis of how census data and Optum sampling are related
    Onverse variance weighted regression model (Primary outcome for our analysis)
    Sensitivity analyses.
    Making chloropleth maps of the distribution of Optum's sampling.

Optum data is private so it cannot be shared. I am sharing the code for transparency and for other researchers who want to do reserach 
that combines census data with claims data at the aggregated level. 
