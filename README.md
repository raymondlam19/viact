# viact testing (CV, multi-label classification)

Dependencies
-----------------------------------------------------------
numpy, pandas, matplotlib, seaborn, cv2, time, keras, tensorflow(1.14)

Data Preprocessing
-----------------------------------------------------------
1) Convert xml intro pd.DataFrame
2) Check the images
3) Convert column helmet, mask into binary (y_train)
4) Load images (x_train)
5) Normalize x_train
6) Split training and valdiation set

Modelling using Keras
-----------------------------------------------------------
* Using f1 as metric because of imbalance classes in 'helmet'
* Using mobilenet because it's much faster & return low loss!

Model Evaluation
-----------------------------------------------------------
1) Plot loss and accuracy (train, val)
  * Underfitting because not enough of data(images)
2) Plot confusion matrix (val)
3) f1_score (val)
4) Show errors

Conclusions:
-----------------------------------------------------------
* Prediction can be improved by adding more data(images)
