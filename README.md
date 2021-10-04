# Face-Mask-Detection-using-Machine-learning-algorithms
This repository shows the work done in my master thesis using machine learning algorithms which became essential in our daily life and how it can be used to make life easier. The data for Face mask detection model was collected and pre-processed to be ready to be used then, a model was created and tested on several pre-trained neural networks like ResNet, VGG, DenseNet and YOLO and every one of them have achieved different results after several tuning and testing for each neural network. Observing the loss and accuracy with comparing accuracy and validation accuracy for every neural network to know which one performed well also, another test was made using webcam to test the model with different type of masks with different faces to test the model.
As YOLO is one of the most powerful networks in object detection, it was used to detect masks with high accuracy. The neural networks and filters of the model are changed according to the number of classes; thus, calculation of max batches, steps and filters are needed as the model has two classes the calculations would be:
 Max_batches= classes*2000= 2*2000=4000
 Steps= 0.8*max_batches, 0.9*max_batches= 0.8*4000, 0.9*4000=3200,3600
 Width = 416, Height= 416
 Classes = 2
 Filters = (classes+5) *3= (2+5) *3= 21
The results are shown in below figure:
Fig- 61- Results
66
Table-6- YOLO Results
Mean average precision
Accuracy for Masked faces
Accuracy for unmasked faces
Precision
Recall
F1-score
90.3%
88.89%
92.97%
0.86
0.88
0.87
Fig-62 -Test 1
67
Fig-63 -Test 2
Fig-64- Test 3
68
The results form YOLO were high and stable, and the model was able to detect masked and unmasked faces with high accuracy.
