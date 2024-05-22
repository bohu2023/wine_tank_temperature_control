# wine_tank_temperature_control

Solution File is located [here](solution.ipynb)

## Introduction

Temperature control plays a crucial role in the process of wine making, whether during the formentation or for storage. The Wine Tank Temperature Control and Mangement System aims to optimize the temperature control within wine tanks by evaluating Artificial Intelligence techniques, therefore to improve the quanlity and efficiency of wine production. The system offers several advantages:  
Consistency: Maintain consistent temperatures for uniform wine quality.  
Energy Efficiency: Optimize energy usage by minimizing unnecessary heating or cooling.  
Cost Savings: Efficient valve operations lead to cost savings over time.  
Quality Assurance: Reduce the risk of spoilage or off-flavors.  

## Data Description

tank_id: unique identifier of the wine tank  
t_is: current temperature when the data is collected  
h_valve: the status of the heater valve, 1 is open, 0 is closed  
t_valve: the status of the cooler valve, 1 is open, 0 is closed  
t_set: the target temperature set for control  
t_min: the minimum temperature set for control  
t_max: the maximum temperature set for control  
time_index: the time when the data is collected  
month: month name  

Dataset is located at [here](data/all_c.csv)

## Conclusion

The purpose of the Wine Tank Temperature Control and Management Analysis is to recommand the best model can be used to control the wine tank temperature during formentation and storage process. The following steps are carried during our analysis:  
1, Data collection: data is collected from the company's cloud production database  
2, Data clean: the original raw data is cleanned and reconstructed to fit the problem definition  
3, Data analysis: source data is visulized and interpretated  
4, Model hyperparameter tunning and selection: multiple classfication models are studied with hyperparameter tunning   to achieve the best score. Recommandation is given as a result of model cross validation  
5, keras classification is also run for cost effective analysis  
The recommanded model is decision tree with tunned hyperparameters.  
  
## Next Steps

1) data collection - we need to collect more data with different management temperature    
2) add previous temperature and valve status to fit the models, check if this will improve the score   
3) try with more models, such as time series analysis  
