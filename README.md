# Autoencoder VS PCA 

This code looks at autoencoders and compare their performance with an autoencoder-based PCA model. For this, we will use the MNIST dataset. The steps and results are well labelled in the jupyther notebook

__PART A__: Three models are built: an autoencoder-based PCA, a 2-layer and a 3-layer autoencoder. The training and testing of these models on the MNIST dataset is provided. This provides comparison of their performances through visual output as well as by ccomputing the test set recontruction error. 
__PART B__: In this part, the code interpolates between two images in the latent space. This is done by first obtaining the encoded images:


<p align=center>
__latent1 = encoder(image1)__ 
</p>

<p align=center>
__latent2 = encoder(image2)__
</p>

and then generating the new interpolated image using the following equation:

<p align=center>
__interpolated_image_lambda = decoder[lambda * latent1 + (1 - $\_lambda$) * latent2]__
</p>
<br>
Using the PCA model and then the autoencoder model and looking at the differences between the two interpolations , the code shows the substantial difference with autoencoders compared to PCA model.
