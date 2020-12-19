# Autoencoder VS PCA 

This code looks at autoencoders and compare their performance with an autoencoder-based PCA model. For this, we will use the MNIST dataset. The steps and results are well labelled in the jupyther notebook

__PART A__: Three models are built: an autoencoder-based PCA, a 2-layer and a 3-layer autoencoder. The training and testing of these models on the MNIST dataset is provided. This provides comparison of their performances through visual output as well as by ccomputing the test set recontruction error. 
__PART B__: In this part, the code interpolates between two images in the latent space. This is done by first obtaining the encoded images:

\ begin{align}
latent\_1 = encoder(image\_1) 
\end{align}

\begin{align}
latent\_2 = encoder(image\_2)
\end{align}

and then generating the new interpolated image using the following equation:

\begin{align}
interpolated\_image\_\lambda = decoder[\lambda* latent\_1 + (1- \lambda) * latent\_2]
\end{align}

Using the PCA model and then the autoencoder model and looking at the differences between the two interpolations , the code shows the substantial difference with autoencoders compared to PCA model.
