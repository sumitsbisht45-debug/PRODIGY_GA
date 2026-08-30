# Task-05: Neural Style Transfer

## Internship

Prodigy Infotech - Generative AI Internship

## Task Description

The objective of this task is to implement Neural Style Transfer to apply the artistic style of one image to the content of another image.

In this project, a normal image is used as the content image and a famous painting is used as the style image. A pretrained VGG19 neural network is used to extract content and style features and generate a stylized image.

## Project Overview

Neural Style Transfer combines the content of one image with the artistic characteristics of another image.

The content image provides the main structure and objects, while the style image provides artistic patterns, textures, colors, and visual characteristics.

## Technologies Used

- Python
- PyTorch
- Torchvision
- NumPy
- Matplotlib
- Pillow
- Google Colab
- NVIDIA T4 GPU

## Model

A pretrained VGG19 convolutional neural network is used for feature extraction.

The model is not trained from scratch. Instead, selected VGG19 layers are used to extract:

- Content features
- Style features

A Gram Matrix is used to represent the style information of the reference painting.

## Methodology

The following steps were performed:

1. Loaded the content image.
2. Loaded the famous painting as the style image.
3. Loaded the pretrained VGG19 model.
4. Preprocessed both images.
5. Extracted content and style features.
6. Calculated the Gram Matrix for style representation.
7. Calculated content loss and style loss.
8. Combined the losses into a total loss.
9. Optimized the generated image using Adam optimizer.
10. Generated the final stylized image.
11. Compared the content image, style image, and final result.

## Training / Optimization Parameters

- Image Size: 256 × 256
- Optimizer: Adam
- Learning Rate: 0.02
- Optimization Steps: 300
- Style Weight: 1e6
- Content Weight: 1

## Results

The final output combines the structure of the content image with the artistic characteristics of the selected famous painting.

The project includes a comparison showing:

1. Content Image
2. Style Image
3. Final Stylized Image

## Files

- `PRODIGY_GA_05_Neural_Style_Transfer.ipynb` - Complete implementation notebook.
- `neural_style_transfer_result.png` - Final stylized output.
- `style_transfer_comparison.png` - Comparison of content, style, and generated images.
- `README.md` - Project documentation.
- `requirements.txt` - Required Python libraries.

## Conclusion

This task demonstrates the practical implementation of Neural Style Transfer using a pretrained VGG19 network.

The project successfully combines the content of one image with the artistic style of another image through feature extraction, Gram Matrix based style representation, content loss, style loss, and image optimization.

## Author

Sumit Singh Bisht

Generative AI Internship  
Prodigy Infotech
