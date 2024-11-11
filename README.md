# GB Road Condition Detection Using YOLOv5
### Author: Ehtijad Ali Shah
### Email: Ehtyalee1919@gmail.com


### 1. Introduction
This project focuses on developing an object detection model to identify road conditions and directions on the challenging roads of Gilgit. Using YOLOv5, the model aims to detect turns (left, right) and straight roads, as well as unexpected obstacles, to improve safety and inform autonomous navigation systems. Such real-time detection of road conditions can support applications in autonomous driving, driver assistance systems, and road monitoring.

### 2. Objective
The main objective of this project is to build an accurate and efficient object detection model for identifying different road types and conditions in images. This involves:
●	Preprocessing the image data.
●	Implementing YOLOv5 for object detection.
●	Training and fine-tuning the model on labeled road data.
●	Evaluating the model's performance and visualizing the results.

### 3. Dataset
The dataset for this project was sourced from Roboflow and consists of labeled images from Gilgit roads, classified into four categories: straight, left turn, right turn, and unexpected.
●	Data Division:
○	Training Set: 70% of images.
○	Validation Set: 15% of images.
○	Test Set: 15% of images.
●	Image Preprocessing: Images were resized and normalized for optimal input to YOLOv5.

### 4. Model Architecture
YOLOv5 was chosen for its real-time object detection capabilities. The model architecture is as follows:
1.	Backbone: CSPDarknet53 for feature extraction.
2.	Neck: PANet layers for feature fusion.
3.	Head: Outputs bounding boxes and class probabilities.
### Hyperparameters:
●	Input Size: 416x416 pixels.
●	Batch Size: 16.
●	Epochs: 50.
●	Learning Rate: Experimented with values from 0.001 to 0.01.
________________________________________
### 5. Results
The model was trained for 25 epochs, and both training and validation accuracy were tracked. Key performance metrics are as follows:
●	Validation Accuracy: Approximately 85%.
●	Training Loss: Converged after 25 epochs.
 

### 6. Conclusion
This project successfully implemented YOLOv5 for road condition and turn detection in images from Gilgit roads, achieving promising results in real-time detection of road conditions and turns.
### 6.1 Key Achievements
1.	Model Accuracy: Achieved around 85% accuracy on validation, demonstrating reliable performance.
2.	Data Augmentation: Augmentation techniques, such as rotation and scaling, helped improve generalization.
3.	Visualization: Result visualizations were effective in assessing detection quality.
### 6.2 Future Work
1.	Increasing Dataset Diversity: Adding more samples with varied lighting and weather conditions.
2.	Enhanced Model Architecture: Experimenting with YOLOv8 or hybrid architectures for further accuracy.
3.	Real-time Application: Deploying the model for real-time inference in autonomous navigation or driver assistance systems.


