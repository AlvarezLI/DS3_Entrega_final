# Animal Image Classification Project

## Project Description
This project focuses on building and evaluating machine learning models for classifying images of animals (cats, dogs, and snakes). The goal is to develop a model that can accurately predict the animal class from images, using both a simple Convolutional Neural Network (CNN) and an improved model leveraging MobileNetV2.

## Dataset Summary
The dataset contains 3,000 images split into three classes:
- **cats/**: 1,000 images of cats, showcasing different breeds and environments.
- **dogs/**: 1,000 images of dogs, capturing various breeds and activities.
- **snakes/**: 1,000 images of snakes, representing different species and habitats.

Image Details:
- **Resolution**: 256x256 pixels
- **File Format**: JPG
- **Color Space**: RGB

This dataset is ideal for building models for multi-class animal recognition and has applications in areas like pet technology, wildlife identification, and biodiversity conservation.

## Model Overview
Two models were developed and evaluated:
1. **Simple CNN Model**: A basic convolutional neural network trained from scratch.
2. **Improved CNN Model with MobileNetV2**: A model using transfer learning from MobileNetV2, a pre-trained model based on ImageNet.

### Performance of the Simple CNN Model:
- **Training Accuracy**: Reached **89%** by the 6th epoch.
- **Validation Accuracy**: The best validation accuracy reached **45%** by the 10th epoch.
- **Training Loss**: Reduced gradually.
- **Validation Loss**: Remained high, fluctuating and indicating overfitting.

#### Epoch Breakdown for Simple CNN Model:
- **Epoch 1**: Training Accuracy: 89% | Validation Accuracy: 45% | Training Loss: 0.2514 | Validation Loss: 2.5142
- **Epoch 10**: Training Accuracy: 89% | Validation Accuracy: 45% | Training Loss: 0.2886 | Validation Loss: 3.8860

### Performance of the Improved CNN Model with MobileNetV2:
- **Training Accuracy**: Reached **95.3%** by the 9th epoch and **96.1%** by the 15th epoch.
- **Validation Accuracy**: Reached **96%** at the end of training.
- **Training Loss**: Decreased steadily.
- **Validation Loss**: Consistently low, confirming the model’s ability to generalize well on unseen data.

#### Epoch Breakdown for Improved CNN Model with MobileNetV2:
- **Epoch 9**: Training Accuracy: **95.31%** | Validation Accuracy: **95.5%** | Training Loss: 0.1223 | Validation Loss: 0.1137
- **Epoch 15**: Training Accuracy: **96.11%** | Validation Accuracy: **96%** | Training Loss: 0.0920 | Validation Loss: 0.09

## Conclusion
- The **simple CNN model** struggled with overfitting, failing to generalize well on the validation set.
- The **MobileNetV2-based model** outperformed the simple CNN, with a significant improvement in both training and validation accuracy, demonstrating the benefits of transfer learning and model complexity.

## License
This project is under the MIT License. The dataset is available for academic and non-commercial usage under the source's terms.

## Dataset Source
The dataset used for this project is available on Hugging Face:
[Animal Image Classification Dataset](https://huggingface.co/datasets/AlvaroVasquezAI/Animal_Image_Classification_Dataset)
