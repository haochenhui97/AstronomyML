# AstronomyML
Late project S for CS189/289 Fall 2020.  
Group: CKK (Chenhui Hao, Kaijing Ding, Ke Liu, Zishan Cheng)

## Description 

Requirements to run different models are specified in each notebook file. 

## Repository Navigation 
- Data
  - data.csv
- Scripts  
  - data_preprocess.ipynb
  - random_forest  
  - neural_network.ipynb  
  - position_prediction  
- Final_report.pdf  
- README  

## Generating Data
We used the method described in [Astronomy Dataset for ML](). Since all the observed astronomy parameters are different among observation sites, we use Beijing as the case study. We download 10-year dataranging from 2009-1-1 0:0 UT to 2019-1-1 0:0 UT with step size of one hour at Beijing. The result of data preprocessing (data_preprocssing.ipynb) is saved as [data.csv]().

## Training Models
We ran some data analysis and drew several plots in []() to help us better understand the law of sun's and moon's motions.  
We used [Fourier Transform]() to calculate moon's RA, DEC, position and sun's RA, DEC, position.  
We used [Random Forest]() and [Neural Network]() to predict moon phases.  
