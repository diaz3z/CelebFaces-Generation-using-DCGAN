# DCGAN for Celebrity Face Generation
This project implements a Deep Convolutional Generative Adversarial Network (DCGAN) to generate realistic images of celebrity faces. The model is trained on the CelebA dataset, which contains over 200,000 celebrity images.
## Project Overview
The primary goal of this project is to use DCGAN to learn the distribution of the CelebA dataset and generate new images that resemble celebrity faces. DCGAN leverages convolutional layers to improve the performance of the GAN in generating high-quality images.
## Dependencies
To run this project, you will need the following libraries:

•torch

•torchvision

•matplotlib

•numpy

You can install the required libraries using pip:

```bash
pip install torch torchvision matplotlib numpy

```
## Dataset
The CelebA dataset consists of celebrity images in different poses, lighting conditions, and backgrounds. You can download the dataset from this [link](https://mmlab.ie.cuhk.edu.hk/projects/CelebA.html).
## Data Preprocessing
The images are preprocessed by resizing them to 64x64 pixels and normalizing them. This allows the DCGAN model to handle the data more effectively during training.
## How to Run
1. Clone the Repository:
```bash
git clone https://github.com/diaz3z/CelebFaces-Generation-using-DCGAN.git

cd CelebFaces-Generation-using-DCGAN
```
2. Prepare the Dataset:

• Download the CelebA dataset.

• Extract the dataset into a folder named data within the project directory.

3. Run the Jupyter Notebook:
Open and execute the Jupyter notebook CelebFaces_DCGAN.ipynb to train the DCGAN model and generate new images of celebrity faces.
4. Training:
The DCGAN model is trained on the CelebA dataset using a batch size of 128. The training loop alternates between updating the generator and discriminator. After training, the generator is able to create realistic celebrity face images.
![sphx_glr_dcgan_faces_tutorial_001](https://github.com/user-attachments/assets/63e96af2-0668-450a-aec6-8181ee57d07f)

![Untitled design (1) (2)](https://github.com/user-attachments/assets/f0a5465d-d5dc-4b67-8eb9-684054f825eb)

6. Results:
After training, the notebook will display generated face images. You can also save the generated images for further analysis.



# Model Architecture

## Generator
The generator in DCGAN is a neural network that takes a random noise vector as input and outputs a 64x64 image. It utilizes transposed convolutional layers with batch normalization and ReLU activation.

## Discriminator
The discriminator is a convolutional neural network that takes a 64x64 image as input and outputs a probability that the image is real or fake. It uses convolutional layers with batch normalization and Leaky ReLU activation.

## Example Output
Here are some sample images generated by the DCGAN after training:

![sphx_glr_dcgan_faces_tutorial_004](https://github.com/user-attachments/assets/3b189270-b791-434a-ab46-c5ae2717907e)


##License
This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgements
The CelebA dataset is provided by MMLAB and can be accessed from [here](https://mmlab.ie.cuhk.edu.hk/projects/CelebA.html).

This project is built using PyTorch and Torchvision.


