# DeepAMR (Repository in progress)
## Abstract
Complete methodology based on deep learning (DL) and transfer learning for the direct analysis of raw
MS data for the identification of antibiotic resistance in three different bacterial species, Escherichia coli, Klebsiella pneumoniae and Staphylococcus aureus.

here we made available the models resulting from the study "DeepAMR: Antimicrobial resistance prediction based on deep neural networks and transfer learning".

for more details about the model and the corresponding research see the article at: (link to article)
## Data : (binning.py)
For this work we have used data from <a href="https://doi.org/10.5061/dryad.bzkh1899q" rel="nofollow">DOI: 10.5061/dryad.bzkh1899q</a>, we constructed our own datasets following the author's recommendations related to bin size and treatment of samples with inconclusive resistance profiles. 
## DeepAMR model
The models were trained using keras version 2.4.3 and tensorflow version 2.3.0 and saved in .h5 format.
![esquema paper](https://user-images.githubusercontent.com/43461313/201794393-78c50952-ff42-425b-b5ee-c275481e835d.png)

```python
from keras.models import load_model

model = load_model('path_of_the_model.h5')
model.summary()
```

## Examples
In the examples folder you will find two Google Colab notebooks, the first one is DeepAMR.ipynb, an interactive implementation of the model applied in this research. It is possible to load the data directly from this repository, but, we recommend downloading them to use them locally in order to reduce execution times.  

DeepAMR_transfer_learning.ipynb contains an example of using one of the pre-trained models to evaluate it in the external databases present in <a href="https://doi.org/10.5061/dryad.bzkh1899q" rel="nofollow">DOI: 10.5061/dryad.bzkh1899q</a>.





