**Dataset Info**
<u> Fatty Liver Dataset: <u>
https://figshare.com/articles/dataset/BEHSOF_Advanced_Non-alcoholic_fatty_liver_dataset_with_clinical_metadata_and_ultrasound_images_for_Deep_learning_Models/26389069
<u> Hepatitis C Dataset: <u>
https://archive.ics.uci.edu/dataset/571/hcv+data  
OR
directly import in python
Install the ucimlrepo package
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
OR
Import from Kaggle
```python
import kagglehub

# Download latest version
path = kagglehub.dataset_download("fedesoriano/hepatitis-c-dataset")

print("Path to dataset files:", path)
```
                     

