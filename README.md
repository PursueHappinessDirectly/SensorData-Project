# SensorData-Project
The sequence of file is:     
1. sensor_dataRead.ipynb      
   Input: sensorswww_data.txt, Output: sensor_raw_data.csv     
2. sensor_EDA.ipynb          
   Input: sensor_raw_data.csv, Output: sensor_data_remove_missing.csv      
3. sensor_featureEngineer.ipynb       
   Input: sensor_data_remove_missing.csv, Output: sensor_data_engineered.csv      
4. sensor_modelBuilding.ipynb      

Summary of data analysis:    
Part one: sensor_dataRead.ipynb       
■ The original data is in the format of website log file. Each record is formatted in JSON style. Here I transfered the original data into Pandas data frame.       

Part two: sensor_EDA.ipynb        
Explored questions below.     
■ Is 9419 a coincidence？    
■ How active are the user weekly?     
■ How to define conversion rate in this case?          
■ Will the reference source have influence on conversion?  
■ Performed funnel analysis for the signup flow and found the cell-phone verification step to be the bottleneck due to unclear format requirements.        
■ 

Part three: sensor_featureEngineer.ipynb      
■ Created and engineered features for conversion predictions.     

Part four: sensor_modelBuilding.ipynb         
■ Build machine learning models (GBDT and Logistic Regression) to predict user signup behaviors.      
■ Tuned hyper parameters through grid search.       
■ Evaluated model performance through AUC score and achieved 98.5% accuracy.        
■ Correlated user retention with persona analysis service and correlated user churn with poor quality of introduction video.       
