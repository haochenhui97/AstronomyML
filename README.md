# AstronomyML
Final project S for CS189/289 Fall 2020.  
Group: CKK (Chenhui Hao, Kaijing Ding, Ke Liu, Zishan Cheng)

## Description 

This project is inspired by ancient Chinese astronomer Liu Hong's method of predicting positions of heavenly objects and moon phases. We reviewed and improved his works by building parametric models to acquire more accuracy in prediction of positions and lunar illumination. We also applied Neural Network and Random Forests models to discover patterns of lunar movements and make predictions on lunar illumination without any Astronomy knowledge beforehand, and found inspiring results in prediction accuracy compared with theory-based OLS model. 

## Repository Navigation 
- Data
  - raw_sun_10yrs.txt
  - raw_moon_10yrs.txt
  - horizons_results_sun_1yr.txt
  - horizons_results_moon_1yr.txt
  - processed_moon_10yrs.csv
- Scripts  
  - preliminary_analysis.ipynb
  - position_prediction  
  - Theoretical models on moon phase.ipynb 
  - Neural_network
    - neural_network.ipynb  
    - my_logs
    - checkpoint
    - my_keras_model.h5
    - my_keras_weights.ckpt.data-00000-of-00001
    - my_keras_weights.ckpt.index
- Final_report.pdf  
- README.md  

## Generating Data
We used the method described in our early project [Astronomy Dataset for ML](https://github.com/haochenhui97/AstronomyDatasetForML) to generate data with the following changes:
- added one more feature of percentage of illumination on moon surface;
- chose Beijing as the only observing site;
- downloaded 10-year data from 2009-1-1 00:00 UT to 2019-1-1 00:00 UT;
- changed step size to be one hour to increase prediction accuracy; 
- downloaded the same format of solar ephemerides in addition to lunar ephemerides from the same [NASA HORIZONS Web-Interface](https://ssd.jpl.nasa.gov/horizons.cgi#top) since moon phase is influenced by not only its own position but also the solar position.

The results of [data preprocessing] (https://github.com/haochenhui97/AstronomyML/blob/main/Scripts/preliminary_analysis.ipynb) are saved as [processed_moon_10yrs.csv](https://github.com/haochenhui97/AstronomyML/blob/main/Data/processed_moon_10yrs.csv) and [processed_sun_10yrs.csv](https://github.com/haochenhui97/AstronomyML/blob/main/Data/processed_sun_10yrs.csv).

## Training Models
We ran some data analysis and drew several plots in []() to help us better understand the law of solar and lunar motions.  
We used [Fourier Transform](https://github.com/haochenhui97/AstronomyML/blob/main/Scripts/position_prediction.ipynb) to calculate moon's RA, DEC, position and sun's RA, DEC, position.  
We used [Random Forest](https://github.com/haochenhui97/AstronomyML/blob/main/Scripts/Theoretical%20models%20on%20moon%20phase.ipynb) and [Neural Network](https://github.com/haochenhui97/AstronomyML/blob/main/Scripts/Neural_network/neural_network.ipynb) to predict moon phases.  
