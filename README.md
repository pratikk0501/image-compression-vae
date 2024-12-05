# image-compression-vae
![generative_ai](https://github.com/pratikk0501/image-compression-vae/blob/main/images/generative_ai.webp)
# Project Description
* This is a course project titled 'Image Compression and Reconstruction Using VAE' done under the guidance of Prof. Asim Tewari with a six-person team in the Statistical Machine Learning and Data Mining Course(ME-781), IIT Bombay.
* This project was focused on data compression using VAE(Variational Autoencoders) to learn compact representations of data while retaining essential information.
## Objectives
* Reduce the size of input data while preserving its essential features.
* Ensure that the compressed data retains a high level of quality.
# Project Features
* A VAE model using TensorFlow and Keras on the MNIST dataset was implemented.
* VAE is a type of generative model that can learn a probabilistic mapping between the input data and a latent space.
* Encoder of VAE was used to compress images and Decoder to decompress images.
## Model Training
* Trained on open sourced MNIST handwritten digits dataset (available in keras.datasets)
1. Data Preprocessing: Normalized pixel values to the range [0, 1] then flattened the 28x28 images into 1D arrays.
2. Model Compilation: Compiled the VAE model using the Adam optimizer.
3. Training Loop: Fitted the VAE model to the training data using a batch size of 64 and trained for 20 epochs. Trained on 6000 images and tested on 1000 images
## Model Testing
1. Compression and Decompression: Used the trained encoder to compress the test data into the latent space.
2. Reconstruction: Used trained decoder to reconstruct the data from the compressed latent space.
3. Visualisation: Visualised the reconstructed images for qualitative assessment.
* Images before passing to the model:
![Before_VAE](https://github.com/pratikk0501/image-compression-vae/blob/main/images/original_mnist_images.png)
* Reconstructed images by decoder:
![After_VAE](https://github.com/pratikk0501/image-compression-vae/blob/main/images/reconstructed_images.png)
