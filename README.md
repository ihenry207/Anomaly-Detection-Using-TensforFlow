# Anomaly-Detection-Using-TensforFlow
This program reads a file and uses a neural network autoencoder and TensorFlow as a framework to detect anomalies in a heartbeat.

# About the Dataset:
We will be using ECG dataset.ECG stands for Electrocardiogram. It checks how your heart is functioning by measuring the electrical activities of your heart.

# Model:
we use Subaclassing we allows us to us the model in different ways.
In the code above, we define a class that serves as an Autoencoder. It includes a constructor where we set up the architecture. The encoder is designed with decreasing layer sizes, and it features bottleneck layers with 8 units. The decoder is responsible for upsampling the data that has been downsampled by the encoder. The final output layer contains 140 units, although the number of units can vary depending on the specific problem we're addressing. The activation function used at the output layer is sigmoid.

The call function in this class acts as the core operation. It takes input data, passes it through the encoder, and then forwards the encoded data to the decoder. When you instantiate and run this Autoencoder class, it returns a model object containing the encoder, bottleneck layer, and decoder components. This model can be further used for various tasks related to data encoding and decoding.

