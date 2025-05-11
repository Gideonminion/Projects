# Traffic Sign Recognition

This project uses deep learning to recognize four types of traffic signs:

* Priority Road
* Give Way
* Stop
* No Entry

## How it Works

1. **Dataset:** The project uses the GTSRB dataset, a collection of over 50,000 traffic sign images. We select images of the four target signs for training and testing.
2. **Model:** We use a pre-trained ResNet34 model. ResNet34 is a powerful deep learning model commonly used for image classification.  We fine-tune it to recognize our specific traffic signs.
3. **Training:**  We train the model on the selected traffic sign images, teaching it to distinguish between the four types.
4. **Evaluation:**  We test the model's accuracy on a separate set of images it hasn't seen before. 

## Results

The trained model achieves high accuracy in recognizing the four traffic signs, typically exceeding 90% accuracy on our test set. Actual accuracy may vary depending on the specific training run and dataset split.

## Key Features

* **ResNet34:**  Utilizes a powerful pre-trained model for accurate image classification.
* **GTSRB Dataset:** Leverages a large and diverse dataset for training.
* **High Accuracy:** The model performs well in identifying the target traffic signs.
