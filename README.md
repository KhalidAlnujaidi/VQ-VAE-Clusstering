# VQ-VAE-Clusstering
Some experimentation with using VQ-VAE embeddings to perform clustering tasks.

This demo uses Vector-Quantized Variational Autoencoders to embedd MNIST into a dicrete latent space then proceed to use K-Means clusstering based on the embedded representations of the digits.

For comparason sake, firt a K-means algorithm is ran on the default dataset (784 features) an image. The results as expected were around 58% accuracy.

Then the MNIST dataset was ran through a VQ-VAE model with a discrete latent space of (3, 3, 1) embedding (9 features). Running K-means based on the embedded features resulted in around 75% accuracy.

Further development is possible by trying to emplement Deep Embedded Clusstering.



### Reference
https://keras.io/examples/generative/vq_vae/#vectorquantized-variational-autoencoders

https://arxiv.org/abs/1511.06335

