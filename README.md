# Retinal_AI_ML
A machine learning model that predicts disease status using retinal image datasets.

## Dataset
Total Images: 501
Normal: 300 images
Cataract: 100 images
Glaucoma: 101 images

## Preprocessing:
Oversampling performed using ADASYN to balance the dataset.
Images were preprocessed and resized for compatibility with the ResNet50 model.

## Model Architecture
Base Model: ResNet50 (pretrained on ImageNet)
### Fine-Tuning:
Dropout layers added to reduce overfitting.
Learning rate scheduler implemented for optimization.
Categorical Crossentropy used as the loss function.

## Training Process
Framework: Python with TensorFlow/Keras
Augmentation: Only slight: rotation, height and width shift and brightness changes.
Evaluation Metrics: Accuracy, precision, recall, F1-score.

## Results & Considerations
Fine-tuning significantly improved performance.
Overfitting concerns were addressed using dropout and learning rate scheduling.
