# 🔥 Zenspark – AI-Powered Art Generator

Zenspark is a visually intuitive and powerful platform that blends **text-to-image generation** and **neural style transfer** to let users create stunning AI-generated art in seconds. Whether you're an artist, developer, or enthusiast, Zenspark gives you total control over your creative output — from prompt-driven imagination to artistic styling.

> ✨ "Transform ideas into visuals. Blend creativity with control."

---

## 🌟 Key Highlights

### 🎨 Text-to-Image Generation (Stable Diffusion)
Generate high-quality images from your imagination using **Stable Diffusion v1.5** – a state-of-the-art latent text-to-image model.

- Input: Text Prompt  
- Output: AI-Generated Image  
- High resolution and rich visual coherence.

### 🖌️ Neural Style Transfer (NST)
Give your images an artistic touch using **TensorFlow Hub’s NST model**, which transfers the style of one image onto the content of another.

- Upload a style image
- Stylize the generated or custom-uploaded image
- Control the level of stylization using a dedicated slider

### 🧠 Combine AI and Art
Generate with Stable Diffusion, then apply style transfer for a hybrid masterpiece — all in a **single workflow**.

---

## 🛠️ Enhanced User Features

### 🎯 Style Intensity Control
Set how strongly the artistic style is applied.

- Range: `0.0` (no style) to `1.0` (maximum style)
- Default: `0.8`

### ⚙️ Advanced Settings (for Text-to-Image Generation)

#### ⚡ Generation Steps
- Determines the number of inference steps
- Higher steps = Better image quality
- Range: `10` to `50`

#### 🎛️ Guidance Scale
- Controls how closely the image aligns with the prompt
- Higher values = Better prompt alignment, but less creativity
- Range: `1` to `15`

---

## 💻 Technologies Used

### ✅ Frontend & Interface
- **Gradio** – For building a sleek and interactive web UI
- **HTML/CSS** (in Gradio templates)

### ✅ Backend & Image Processing
- **TensorFlow** – For running the Neural Style Transfer model
- **TensorFlow Hub** – Pretrained NST model
- **Diffusers (Hugging Face)** – Stable Diffusion pipeline
- **Transformers** – Model loading
- **PIL (Pillow)** – Image manipulation and formatting
- **NumPy** – Numerical operations
- **Torch** – (Optional, only used internally by diffusers)
- **OS & shutil** – File management
- **Google Colab** – Optional execution environment

---

## 🖼️ Preview

| Prompt | Stylized Output |
|--------|-----------------|
| "A fantasy castle at sunrise" | ![sample](assets/sample_output.png) |

(Replace with your actual outputs or gifs)


## 🚀 Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/zenspark.git
cd zenspark

pip install -r requirements.txt

pip install gradio diffusers transformers tensorflow tensorflow_hub numpy pillow

from huggingface_hub import login
login(token="your_HF_token")

