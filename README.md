# Getting start
+ **dp_getdata.ipynb**: Prepare training data for the following steps
+ **dp_model.ipynb**: construct and train multi-scale model, provide metrics in patches level
+ **dp_predict.ipynb**: detect cancerous cell through sliding window, draw heatmap and privide metrics in pixel level

# Dependency
Tensorflow 2.0, Scikit-learn, openslide

# Procedure 

# Model

# Experiment and Result
![experiment sample](https://github.com/Steven13737/Detecting-Cancerous-Cell-in-Gigapixel-Images/blob/master/results/110/tumor.png)
![experiment sample](https://github.com/Steven13737/Detecting-Cancerous-Cell-in-Gigapixel-Images/blob/master/results/101/tumor.png)
![](https://github.com/Steven13737/Detecting-Cancerous-Cell-in-Gigapixel-Images/blob/master/results/091/tumor.png)

# Evulation
In pixel level, we use IOU, accuracy and recall to evulate our model

| Image    | IOU     | Accuracy| Recall |
| ---------| :-----: | :-----: | :-----:|
| 110      | 0.70    | 0.89    |  0.93  | 
| 101      | 0.55    | 0.98    |  0.70  |
| 091      | 0.42    | 0.82    |  0.98  |

In patches, we use ROC and AUC to evulate our result

![](https://github.com/Steven13737/Detecting-Cancerous-Cell-in-Gigapixel-Images/blob/master/results/110/ROC.png)
![](https://github.com/Steven13737/Detecting-Cancerous-Cell-in-Gigapixel-Images/blob/master/results/101/ROC.png)
![](https://github.com/Steven13737/Detecting-Cancerous-Cell-in-Gigapixel-Images/blob/master/results/091/ROC.png)
