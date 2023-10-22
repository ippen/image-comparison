# Image Comparison with CNN-based Encoding

## Overview

This code demonstrates a method for comparing images based on their image encodings using a Convolutional Neural Network (CNN) backbone. The process involves extracting image embeddings from a pretrained CNN model and then calculating the cosine similarity between these embeddings to quantify the visual similarity between images. The code then visualizes image pairs along with their computed similarity scores.

## Requirements

- Python
- PyTorch
- Fastai
- Matplotlib
- NumPy

## How to Use

1. Make sure you have the required libraries installed in your Python environment.
2. Place the images you want to compare in a folder and set the `folder_path` variable to the path of that folder.
3. Run the code to perform image comparison.
4. The code will display image pairs along with their similarity scores.

## Output

The output will be a visual representation of how similar the images in the specified folder are to each other. The similarity scores range from 0 (dissimilar) to 1 (identical), where a higher score indicates greater visual similarity.

## Example

The code includes a function called `plot_image_pairs`, which plots image pairs and their similarity scores. An example of the output can be seen in the code above.

## Note

- The code uses a pretrained "convnext_tiny" model for feature extraction, but you can replace it with other pretrained models as needed.
- You can adjust the image size, which is currently set to 192x192 pixels, by modifying the resizing step in the `get_embedding` function.

This code provides a simple yet effective way to compare images based on their visual content, making it useful for various applications such as image retrieval, duplicate detection, and content analysis.
