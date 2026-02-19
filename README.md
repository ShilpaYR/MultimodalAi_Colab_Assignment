# Multimodal AI System (Google Colab)

This repository contains a Google Colab notebook that demonstrates a **complete multimodal AI pipeline** using only **open-source models** (no paid APIs required).

The notebook covers:
- **Text → Text** generation (LLM)
- **Text → Image** generation (Diffusion)
- **Image → Text** understanding (Vision-Language)
- **Simple animated output** simulation (GIF generation)

---

## Files in this Repo
- `Multimodal_AI_Colab.ipynb` — Main Colab notebook
- `README.md` — Project documentation (this file)

---

## Models Used
1. **Text Generation:** `google/flan-t5-base` (Transformers)
2. **Text-to-Image:** `runwayml/stable-diffusion-v1-5` (Diffusers)
3. **Image Captioning / Understanding:** `Salesforce/blip-image-captioning-base` (BLIP)

---

## What the Notebook Does (Section-by-Section)

### 1) Text-to-Text Generation (FLAN-T5)
- Generates creative conversation starters related to multimodal AI topics using an instruction-tuned model.

### 2) Text-to-Image Generation (Stable Diffusion v1.5)
- Generates an image from a text prompt using Stable Diffusion.
- Saves output to: `generated_image.png`

### 3) Image Understanding (BLIP Image Captioning)
- Prompts you to **upload an image** inside Colab.
- Produces an “interesting insight” by generating a caption for the uploaded image.

### 4) Animated Output Simulation (GIF)
- Generates 10 diffusion-based frames using a consistent prompt and increasing “motion blur level”.
- Combines frames into a GIF.
- Saves output to: `simple_animation.gif`

---

## Requirements
This notebook is designed to run on **Google Colab**.

### Recommended Runtime
- **Runtime → Change runtime type → Hardware accelerator: GPU**

### Python Packages Installed in the Notebook
The notebook installs dependencies via:
```bash
pip install transformers diffusers accelerate torch torchvision torchaudio pillow imageio
