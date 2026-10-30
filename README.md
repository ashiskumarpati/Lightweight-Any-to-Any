# Multimodal Any-to-Any AI System

A multimodal AI framework capable of:

- Text → Text
- Text → Image
- Image → Text
- Audio → Text
- Audio + Image → Text
- Text → Audio

Built using:

- Whisper
- Stable Diffusion
- BLIP
- Qwen2.5
- CLIP
- Wav2Vec2

---

# Features

- Shared multimodal latent space
- Transformer-based fusion
- Contrastive learning
- Image generation
- Speech recognition
- Text generation
- Evaluation metrics:
  - BERTScore
  - CLIPScore
  - WER
  - Cosine Similarity

---

# Installation

Run in Google Colab:

```python
!pip install -q transformers diffusers peft accelerate \
open_clip_torch librosa soundfile gtts wikipedia \
openai-whisper gradio datasets torchaudio torchvision \
tqdm bert-score jiwer umap-learn seaborn scikit-learn
```

---

# How to Run

## 1. Open Google Colab

https://colab.research.google.com

---

## 2. Enable GPU

```text
Runtime → Change Runtime Type → GPU
```

---

## 3. Upload the Notebook

Upload your `.ipynb` file.

---

## 4. Run All Cells

```text
Runtime → Run All
```

The framework will:
- Load models
- Train multimodal alignment
- Run evaluations
- Generate outputs and visualizations

---

# Example

```python
response = any_to_any(
    "Explain artificial intelligence",
    output_modality="text"
)

print(response)
```

---

# Output Files

```text
results/
qualitative_results.zip
```
