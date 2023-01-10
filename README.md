# DeepAMR
Complete methodology based on deep learning (DL) and transfer learning for the direct analysis of raw
MS data for the identification of antibiotic resistance in three different bacterial species, Escherichia coli, Klebsiella pneumoniae and Staphylococcus aureus.

here we made available the models resulting from the study "DeepAMR: Antimicrobial resistance prediction based on deep neural networks and transfer learning".

for more details about the model and the corresponding research see the article at: (link to article)
## Data :(binning.py)
descripcion de la creacion de datos utilizados
Para este trabajo hemos utilizados los datos de <a href="https://doi.org/10.5061/dryad.bzkh1899q" rel="nofollow">DOI: 10.5061/dryad.bzkh1899q</a>, contruimos nuestros propios datasets siguiendo las recomendaciones del autor relacionadas al tamaño del bin y tratamiento de las muestras con perfiles de resistencia no concluyente.
## DeepAMR model
The models were trained using keras version 2.4.3 and tensorflow version 2.3.0 and saved in .h5 format.
![esquema paper](https://user-images.githubusercontent.com/43461313/201794393-78c50952-ff42-425b-b5ee-c275481e835d.png)

```python
from keras.models import load_model

model = load_model('path_of_the_model.h5')
model.summary()
```

Data source: <a href="https://doi.org/10.5061/dryad.bzkh1899q" rel="nofollow">DOI: 10.5061/dryad.bzkh1899q</a>

