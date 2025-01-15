Military Equipment Recognition in Images using ResNet50

Background  
In modern military conflicts, recognizing military equipment in images is crucial for monitoring and decision-making. This project aims to use machine learning, specifically deep neural networks, to accurately classify images of military and civilian vehicles. By utilizing open-source datasets and modern AI technologies, the project supports effective tracking of military equipment in conflict zones, bypassing government censorship and providing valuable real-time data for both military and civilian purposes.

Dataset  
The dataset used in this project is the "Normal_vs_Military_Vehicles" dataset from Kaggle. It contains images of two classes:
- Military vehicles
- Civilian vehicles

The dataset is divided into three categories: train, validation, and test, with a total of 20,500 images.

Main Analysis Procedures  
1. Getting Data to the Cluster: The dataset was uploaded to a Hadoop cluster using the scp client, following the necessary VPN setup for external access to the university's network.  
2. CNN Model Selection: The model used is ResNet50, a deep learning architecture pre-trained on ImageNet. Transfer learning was applied to adapt ResNet50 for this task, allowing the model to classify images of military and civilian vehicles.  
3. Comparison of Model Versions: Four versions of the model were tested, each with different settings for data augmentation, optimizers (SGD, Adam), and training techniques. These versions were evaluated based on accuracy, training time, and loss reduction.

Model Performance  
- Version 1 (basic model): Achieved the best accuracy of 97.03%.

Conclusions  
The ResNet50 model demonstrated high efficiency for classifying military and civilian vehicles, with Version 1 providing the highest accuracy. The project also highlighted the benefits of transfer learning and data augmentation. The results are applicable to various military monitoring systems and can be adapted for broader object recognition tasks.
