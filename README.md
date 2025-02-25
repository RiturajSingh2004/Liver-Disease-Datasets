####**Dataset Info** <br>
##<ins> Fatty Liver Dataset: </ins><br>
https://figshare.com/articles/dataset/BEHSOF_Advanced_Non-alcoholic_fatty_liver_dataset_with_clinical_metadata_and_ultrasound_images_for_Deep_learning_Models/26389069 <br>
##<ins> Hepatitis C Dataset: </ins><br>
https://archive.ics.uci.edu/dataset/571/hcv+data <br>  
OR <br>
directly import in python <br>
Install the ucimlrepo package <br>
```python 
pip install ucimlrepo
```
Import the dataset into your code
```python 
from ucimlrepo import fetch_ucirepo 
  
# fetch dataset 
hcv_data = fetch_ucirepo(id=571) 
  
# data (as pandas dataframes) 
X = hcv_data.data.features 
y = hcv_data.data.targets 
  
# metadata 
print(hcv_data.metadata) 
  
# variable information 
print(hcv_data.variables) 
```
OR <br>
Import from Kaggle <br>
```python
import kagglehub

# Download latest version
path = kagglehub.dataset_download("fedesoriano/hepatitis-c-dataset")

print("Path to dataset files:", path)
```
                     

