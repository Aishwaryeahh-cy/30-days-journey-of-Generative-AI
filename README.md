# 🎨 Generative AI Playground

> *"Turning imagination into text, images, and beyond."*  

![Stars](https://img.shields.io/github/stars/yourname/genai-playground?style=social)  
![Issues](https://img.shields.io/github/issues/yourname/genai-playground)  
![Python](https://img.shields.io/badge/Python-3.10+-blue)  
![License](https://img.shields.io/badge/License-MIT-yellow)  

---

## 🚀 What is this?

This repo is a **creative lab** to explore **Generative AI**.  
You can experiment with **Text Generation (LLMs)** and **Image Generation (Diffusion Models)**—all in a beginner-friendly way.  

---

## ⚡ Quick Demo

### Text Generation (Python)

```python
from transformers import pipeline

gen = pipeline("text-generation", model="google/gemma-2-2b-it")

prompt = "Write a short poem about chai and late-night coding."
print(gen(prompt, max_new_tokens=60)[0]["generated_text"])
from diffusers import StableDiffusionPipeline
import torch

pipe = StableDiffusionPipeline.from_pretrained("runwayml/stable-diffusion-v1-5")
pipe = pipe.to("cuda" if torch.cuda.is_available() else "cpu")

image = pipe("A cyberpunk street food market, neon lights, rainy reflections").images[0]
image.save("output.png")
