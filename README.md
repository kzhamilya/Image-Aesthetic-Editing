# Image-Aesthetic-Editing
WIP RACE model for Image Aesthetic Editing

# RACE: Region-Aware Prompt-Based Image Editing

This project is me trying out different frameworks and models and poking around to try and make some sort of image editor that mainly focuses on aesthetic editing, using user prompts like _"make her smile"_ or _"change hair color to blue"_, etc.. 

It combines [Segment Anything (SAM)](https://github.com/facebookresearch/segment-anything) and [InstructPix2Pix](https://huggingface.co/timbrooks/instruct-pix2pix) to allow **targeted image editing using natural language prompts**.


*************

Features

**Localized Editing** (Only modify regions like the face, eyes, hair, or background)
**SAM-based Masking** (Segment Anything Model used to create soft masks)
**Prompt Editing**: (Stable Diffusion InstructPix2Pix to apply edits)


*************

In order to run, you must install following dependencies:

```bash
pip install torch torchvision diffusers transformers accelerate
pip install git+https://github.com/facebookresearch/segment-anything.git
pip install pillow tkinter
