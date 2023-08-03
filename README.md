# Alzheimer's Detection using Deep Learning

In this project, I conducted a comparative study of three deep learning models on a dataset of MRI images containing 6000 images divided into four classes. 

## Models and Results:
1. **ResNet50 Model**: Achieved an accuracy of 64%.
2. **VGG16 Model**: Achieved an accuracy of 82%.
3. **Custom CNN Model**: Developed a custom CNN model with the following key components:
   - Rescaling layer to normalize pixel values to a scale of 0-1, improving convergence.
   - Three convolutional layers with filter sizes of 16, 32, and 64, using ReLU activation.
   - MaxPooling2D layers for spatial dimension reduction and model robustness.
   - Dropout layer for preventing overfitting and improving generalization.
   - Flatten layer to prepare data for fully connected layers.
   - Two dense layers with 128 and 4 neurons, both using ReLU activation.
   - Final output layer with 'softmax' activation for multi-class classification.
   - Achieved an impressive accuracy of 95%.

## Model Training and Evaluation:
- The model was trained with batch size, number of epochs, and validation split defined.
- The model was compiled with categorical cross-entropy loss function and the Adam optimizer.
- Model training was performed using the 'fit' method, and evaluation on test data using the 'evaluate' method.

This project demonstrates the successful implementation of deep learning models for Alzheimer's detection and highlights the efficiency of the custom CNN model in achieving high accuracy.
