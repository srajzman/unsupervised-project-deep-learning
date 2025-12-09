# unsupervised-project-deep-learning
projet deep learning: Anomaly Detection et GAN + Mode Collapse

This repository contains two independent parts:

1. Anomaly detection on a corrupted EMNIST dataset
2. Exploration of mode collapse in GANs trained on MNIST (without using labels)

---

1. Anomaly Detection on Corrupted EMNIST

Objective

* Work on an altered version of the EMNIST dataset provided by the teacher.
* Identify the types of corruption in the dataset without using labels.
* Apply unsupervised anomaly detection techniques.
* Propose a method to partially or fully reconstruct cleaner images.
* Evaluate the quality of both anomaly detection and reconstruction.

Methods

* Autoencoder or Variational Autoencoder (reconstruction error as anomaly score)
* PCA or Isolation Forest for unsupervised anomaly detection
* Visualization and inspection of anomalies
* Reconstruction or correction methods depending on the corruption type

Evaluation

* Reconstruction error (MSE)
* SSIM or similar metrics
* Visual comparison before and after correction

---

2. Mode Collapse in GANs (MNIST)

Objective

* Train GANs on MNIST without labels.
* Intentionally obtain cases of mode collapse by varying architectures and seeds.
* Implement techniques to mitigate mode collapse.
* Extend experiments to CIFAR or EMNIST when possible.
* Compare GAN results with other generative models such as VAEs or diffusion models.

Methods

* Vanilla GAN, DCGAN
* Training with multiple seeds and hyperparameters
* Techniques to reduce mode collapse: WGAN, WGAN-GP, mini-batch discrimination, feature matching, conditionality using pseudo-labels
* Comparison with VAE or diffusion-based generation

Evaluation

* Diversity metrics and qualitative inspection
* FID or related metrics when applicable
* Grid visualization of generated samples

