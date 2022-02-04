# codecademy_projects
Portfolio Project for Codecademy's Deep Learning.
This model works on this dataset : https://www.kaggle.com/c/forest-cover-type-prediction/data
The dataset is labelled onto seven differet forest types : [Spruce/Fir,Lodgepole Pine,Ponderosa Pine,Cottonwood/Willow,Aspen,Douglas-fir,Krummholz]
more details about the data can be found the link above.

Model: "sequential_19"
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
dense_69 (Dense)             (None, 256)               2560      
_________________________________________________________________
dense_70 (Dense)             (None, 128)               32896     
_________________________________________________________________
dense_71 (Dense)             (None, 64)                8256      
_________________________________________________________________
dense_72 (Dense)             (None, 32)                2080      
_________________________________________________________________
dense_73 (Dense)             (None, 16)                528       
_________________________________________________________________
dense_74 (Dense)             (None, 8)                 136       
_________________________________________________________________
dense_75 (Dense)             (None, 7)                 63        
=================================================================
Total params: 46,519
Trainable params: 46,519
Non-trainable params: 0

Given above is a summary of the model which trained with a batch size of 512 and 300 epochs(although early stopping callback was triggered just before the target epoch)
Given below is the model evaluation on the test split of the dataset
   
   precision    recall  f1-score   support

           0       0.85      0.87      0.86     42506
           1       0.89      0.87      0.88     56705
           2       0.86      0.81      0.83      6915
           3       0.74      0.77      0.76       526
           4       0.72      0.64      0.68      1884
           5       0.70      0.76      0.72      3491
           6       0.85      0.89      0.87      4176

    accuracy                           0.86    116203
   macro avg       0.80      0.80      0.80    116203
weighted avg       0.86      0.86      0.86    116203

find more visualisations in the notebook.
cheerio.
