### Notes For AE 
Z --> Labels i.e (Label Mnist 1 - 9)
xG --> Generated Samples 

**Latent** Space --> hidden Representation of data point.

Autoencoders help us to **Encode** data Automatically. 
- Composed 2 parts : **Encoder** and **Decoder**
- EncodeR --> For learning The Dataset 
- Decoder --> For Reproduce the training Result.
- End to End Training , i.e Only **One** Functions

#### Heres The Architecture of AutoEncoder
- Encoder Network : Input Representation , then reduce the dimension using **learned** encoder 
- Latent Space : Small Representation of smaller dimension of the observation , act as an intermediate step. Its just act like a label, Compressed Representation of the Input ,  . **Organize its thought**
- Decoder Network : Reconstruct the original Object into the original Dimension using Decoder.

Here's How it works
The purpose is just **Minimze** the **Reconstruction** loss ..
- Feed image to Autoencoder
- Get the **Reconstruction** of the image
- Measure the Loss < difference between input and the Reconstructured>

# Vae
- Based on Bayesian Machine learning.
- Latent Space as a distribution with a learned mean and std of the dataset. Typically used **Gausiaan** Distribution.
- Learn From the Distribution, find the right **Parameters** defining the **DIstribution**
- We can generate data from the latent space or the compressed image , which is the distribution.
- At Vae, we learn the **Mean** and the **Variance** of the data to generate new dataset.


the decoder, is also similar to a feed-forward network. However, instead of reducing data to a lower dimension, it reconstructs the data from its lower dimension representation Z to its original dimension X.