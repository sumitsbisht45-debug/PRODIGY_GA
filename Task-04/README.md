# Task-04: Image-to-Image Translation with cGAN

## Internship
Prodigy Infotech - Generative AI Internship

## Task Description

The objective of this task is to implement an Image-to-Image Translation model using a Conditional Generative Adversarial Network (cGAN).

For this project, the Pix2Pix approach is implemented using the Facades paired image dataset. The model learns to translate an input image into its corresponding target image.

## Dataset

The project uses the Facades paired image dataset.

Each image contains two corresponding parts:

- Input image
- Target image

The paired structure allows the Conditional GAN to learn the relationship between the input and desired output.

## Technologies Used

- Python
- PyTorch
- Torchvision
- NumPy
- Matplotlib
- Pillow
- Google Colab
- NVIDIA T4 GPU

## Model Architecture

The Pix2Pix implementation consists of two main networks:

### Generator

A U-Net based Generator is used to generate the translated image from the input image.

### Discriminator

A PatchGAN Discriminator is used to determine whether the generated image is realistic when compared with the input condition.

## Loss Functions

Two losses are used during training:

- Binary Cross Entropy loss for adversarial training
- L1 loss for image reconstruction

The combined objective helps the Generator produce images that are both realistic and close to the target image.

## Training

The model was trained using:

- Optimizer: Adam
- Learning Rate: 0.0002
- Batch Size: 8
- Number of Epochs: 10
- L1 Loss Weight: 100
- Hardware: NVIDIA T4 GPU

## Results

After training, the model was used to generate an output image from an input Facades image.

The notebook compares:

1. Input Image
2. Generated Image
3. Target Image

The generated output demonstrates the image-to-image translation process using a Conditional GAN.

## Files

- `PRODIGY_GA_04_Image_to_Image_Translation_with_cGAN.ipynb` - Complete Google Colab notebook containing the implementation and results.
- `generated_facades_image.png` - Generated output image.
- `requirements.txt` - Required Python libraries.
- `pix2pix_generator.pth` - Saved trained Generator model (if included).

## Conclusion

This task demonstrates the implementation of a Conditional Generative Adversarial Network for paired image-to-image translation using the Pix2Pix approach.

The Generator learns to transform the input image into the desired target domain, while the PatchGAN Discriminator evaluates the realism of the generated output.

The project provides practical experience with GAN architectures, image preprocessing, model training, adversarial loss, reconstruction loss, and image generation using PyTorch.

## Author

Sumit Singh Bisht

Generative AI Internship  
Prodigy Infotech
