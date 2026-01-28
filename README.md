# Medical-ViT-Explainability
Comparative study of CNNs and Vision Transformers for Medical X-ray Analysis.
This version is written to sound like a **passionate student researcher**. It avoids the generic "AI-style" corporate buzzwords and focuses on your personal journey from NLP to Computer Vision.

***

# Medical Image Analysis: Can Vision Transformers replace CNNs?

### Why I built this
As I transition from my background in **Natural Language Processing (NLP)** toward **Computer Vision**, I wanted to understand one of the biggest debates in the field: **Do Transformers (which changed NLP forever) actually work better than traditional CNNs for medical scans?**

In medical AI, "high accuracy" isn't enough. A doctor needs to know *why* a model thinks a patient has pneumonia. This project is my hands-on study of **Accuracy vs. Explainability** in clinical diagnostics.

---

### [ [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shatabdi-sikta/Medical-ViT-Explainability/blob/main/Medical_vit.ipynb) ]

---

### The Experiment
I compared two different "brains" using a dataset of 5,800+ Chest X-rays:
1.  **ResNet-18 (The CNN Baseline):** The industry standard for images.
2.  **ViT-Tiny (The Vision Transformer):** The modern architecture that treats images like a sequence of "visual words."

### What I found
*   **Performance:** The CNN (ResNet) was slightly more stable and reached **92.4% accuracy** faster. Because medical datasets are often small, the CNN's "baked-in" knowledge of shapes gives it an edge.
   Even though the Transformer was slightly less accurate (**91.1%**), it offered something the CNN couldn't: **Attention Maps.** 

### Visualization of Results
Instead of just a number, the Vision Transformer lets us see a "heatmap" of where the model is looking. 

**Performance Chart:**
![Comparison]<img width="800" height="500" alt="performance_comparison" src="https://github.com/user-attachments/assets/a5bf4521-ada7-4016-8cdc-e15b93a90d08" />



**Explainability Map:**
![Heatmap] <img width="1200" height="600" alt="explainability_output" src="https://github.com/user-attachments/assets/7036ad9f-cfa4-4027-9fcf-05fcec1c8124" />

---

### How to use this
*   **The Code:** Everything is inside `Medical_vit.ipynb`.
*   **The Tech:** I used **PyTorch**, the **timm** library, and **Google Colab** for GPU acceleration.

---
**Shatabdi Majumder**  
[LinkedIn](https://www.linkedin.com/in/shatabdi-majumder-128a301a6) | [GitHub](https://github.com/shatabdi-sikta)

