# SemanticSegmentation
Project Overview

This project combines semantic segmentation and image colorization to allow targeted colorization of specific regions in an image. Users can select which areas (e.g., foreground, background, people, objects) to colorize while keeping other regions unchanged. The system provides an interactive GUI for selecting regions and previewing results.

Features

Pre-trained DeepLabV3 (ResNet101) for semantic segmentation.

Interactive region selection via dropdown GUI.

Only selected regions are colorized.

Easy to extend with realistic colorization models like DeOldify.

Installation

Clone the repository and install dependencies:
git clone https://github.com/yourusername/semantic-segmentation-colorization.git
cd semantic-segmentation-colorization
pip install torch torchvision opencv-python pillow matplotlib ipywidgets

Usage in Google Colab

Upload your image to Colab.

Run the notebook step by step:
from utils import load_image, segment_image, interactive_colorize

# Load and display image
img = load_image('/content/example.jpg')

# Generate segmentation mask
masks = segment_image(img)

# Interactive colorization
interactive_colorize('/content/example.jpg')


