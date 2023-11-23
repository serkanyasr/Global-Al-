# UrbanSound8K Sound Classification

This project was written to build a sound classification model on the UrbanSound8K dataset. The dataset contains a total of 8732 audio samples in 10 different audio classes recorded from different environments.

## Requirements

To run this project you need to have the following requirements:

- Python 3.8+
- TensorFlow 2.7+
- NumPy
- Pandas
- Matplotlib

## Dataset

The UrbanSound8K dataset can be downloaded from the [UrbanSound8K website](https://urbansounddataset.weebly.com/). This dataset has the following characteristics:

- **Total Number of Sound Samples:** 8732
- **Sound Classes:** 10 (for example, air_conditioner, car_horn, children_playing, dog_bark, drilling, engine_idling, gun_shot, jackhammer, siren, street_music)
- Duration of each Sound Sample:** Variable (average duration approximately 4-5 seconds)
- Sampling Frequency:** 44.1 kHz

## Code

The script consists of the following sections:

- **Data loading and preprocessing**
- **Model creation**
- **Model training**
- **Model rating**

## Data Loading and Preprocessing

The dataset was organized into folders representing each audio class. Each audio recording was converted into a grayscale image with a size of 128x128 pixels.

## Model Building

The model consists of the following layers:

- **4 2D convolution layers**
- **2 2D MaxPooling layers**
- **2 Dropout layers**
- **1 Flattening layer**
- **1 full link layer with 128 units**
- **1 full connection layer with 10 units**

The model is trained using the Adam optimizer.

## Model Training

The model is trained for 50 epochs. In each epoch, the dataset is sampled in a random order.

## Model Evaluation

The model is evaluated on training and test datasets. The accuracy rate obtained on the training dataset is 99.5%. The accuracy rate obtained on the test dataset is 97%.

## Result

The results show that the model is an effective sound classification model for the UrbanSound8K dataset.

## Future Work

To improve the performance of the model, the following can be done in future studies:

- **The model can be trained further by using more epochs.
- A higher accuracy can be achieved by using a more complex model.
- The performance of the model can be evaluated on other datasets.
