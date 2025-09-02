<!-- README.md -->

<p align="center">
  <img src="https://raw.githubusercontent.com/yourusername/genai-playground/main/assets/genai-3d-banner.png" alt="Generative AI 3D Banner" width="700"/>
</p>

<h1 align="center">🌀 Generative AI Playground 🌀</h1>
<h3 align="center">Unleash your imagination with Text ✍️ | Images 🎨 | Creativity 🚀</h3>

---

## 🧊 3D Vibe
---

## 🚀 Quick Demo

### 🎭 Text Generation
```python
from transformers import pipeline
gen = pipeline("text-generation", model="google/gemma-2-2b-it")

prompt = "Write a 2-line haiku about street food and neon lights."
print(gen(prompt, max_new_tokens=40)[0]["generated_text"])
from diffusers import StableDiffusionPipeline
import torch

pipe = StableDiffusionPipeline.from_pretrained("runwayml/stable-diffusion-v1-5")
pipe = pipe.to("cuda" if torch.cuda.is_available() else "cpu")

image = pipe("A futuristic 3D holographic cyber market with glowing food stalls").images[0]
image.save("3d_market.png")
