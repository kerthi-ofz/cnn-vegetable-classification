# cnn-vegetable-classification

Steps Performed:
**Import Libraries**
Uses NumPy, Matplotlib, and TensorFlow/Keras for data handling, visualization, and deep learning.
**Load Dataset**
Loads training, validation, and test images from separate directories using image_dataset_from_directory().
Resizes all images to 180 × 180 pixels.
Creates batches of 32 images for efficient training.
**Visualize Data**
Displays sample images along with their class labels to verify the dataset.
**Build CNN Model**
**Rescaling Layer:** Normalizes pixel values from 0–255 to 0–1.
**Convolution Layers:** Extract image features such as edges, textures, and shapes.
**MaxPooling Layers**: Reduce image dimensions while retaining important features.
**Flatten Layer:** Converts feature maps into a 1D vector.
**Dropout** (0.2): Acts as regularization to reduce overfitting.
**Dense Layers**: Perform final classification into fruit/vegetable categories.
Compile the Model**
**Uses the Adam optimizer.
Uses Sparse Categorical Crossentropy loss for multiclass classification.
Tracks accuracy during training.
Train the Model
Trains the CNN for 25 epochs using training data.
Evaluates performance on the validation dataset after each epoch.
Plot Performance
**Displays graphs for:**
Training vs Validation Accuracy
Training vs Validation Loss
