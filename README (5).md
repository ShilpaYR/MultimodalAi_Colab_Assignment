# Multimodal AI System (Google Colab)

This repository contains a Google Colab notebook that demonstrates a
complete multimodal AI pipeline using only open-source models (no paid
APIs required).

## Files in this Repo

-   Multimodal_AI_Colab.ipynb --- Main Colab notebook
-   README.md --- Project documentation

## Models Used

1.  Text Generation: google/flan-t5-base (Transformers)
2.  Text-to-Image: runwayml/stable-diffusion-v1-5 (Diffusers)
3.  Image Captioning / Understanding:
    Salesforce/blip-image-captioning-base (BLIP)

## Notebook Sections

### 1) Text-to-Text Generation (FLAN-T5)

Generates creative conversation starters related to multimodal AI topics
using an instruction-tuned model.

### 2) Text-to-Image Generation (Stable Diffusion v1.5)

Generates an image from a text prompt using Stable Diffusion. Output
file: generated_image.png

### 3) Image Understanding (BLIP)

Upload an image inside Colab and generate an insightful caption.

### 4) Animated Output (GIF)

Creates 10 diffusion-generated frames and combines them into a GIF.
Output file: simple_animation.gif

## Requirements

Run in Google Colab with GPU enabled.

The notebook installs: transformers diffusers accelerate torch
torchvision torchaudio pillow imageio

## How to Run

1.  Open the notebook in Google Colab.
2.  Enable GPU (Runtime → Change runtime type → GPU).
3.  Run all cells sequentially.

## Outputs

-   generated_image.png
-   simple_animation.gif

## Notes

This project is for educational purposes and assignment submission. All
models are publicly available via Hugging Face.
