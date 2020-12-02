# AstronomyML
Final project S for CS189/289 Fall 2020.  
Group: CKK (Chenhui Hao, Kaijing Ding, Ke Liu, Zishan Cheng)

## Description 

Requirements to run different models are specified in each notebook file. 

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
We used the method described in [Astronomy Dataset for ML](https://github.com/haochenhui97/AstronomyDatasetForML). Since all the observed astronomy parameters are different among observation sites, we use Beijing as the case study. We download 10-year dataranging from 2009-1-1 0:0 UT to 2019-1-1 0:0 UT with step size of one hour at Beijing. The result of data preprocessing (preliminary_analysis.ipynb) is saved as [processed_moon_10yrs.csv](https://github.com/haochenhui97/AstronomyML/blob/main/Data/processed_moon_10yrs.csv).

## Training Models
We ran some data analysis and drew several plots in []() to help us better understand the law of sun's and moon's motions.  
We used [Fourier Transform](https://github.com/haochenhui97/AstronomyML/blob/main/Scripts/position_prediction.ipynb) to calculate moon's RA, DEC, position and sun's RA, DEC, position.  
We used [Random Forest](https://github.com/haochenhui97/AstronomyML/blob/main/Scripts/Theoretical%20models%20on%20moon%20phase.ipynb) and [Neural Network](https://github.com/haochenhui97/AstronomyML/blob/main/Scripts/Neural_network/neural_network.ipynb) to predict moon phases.  
