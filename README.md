# 🔍 XAI Application Demo – Instrument Classification Example

To illustrate the behavior of our application, we provide a simplified example 
based on an instrument classification task.

While the main application focuses on emotion recognition from audio segments, 
instrument classification offers a clearer and more intuitive scenario to 
visually and perceptually evaluate the relevance of spectrogram regions 
identified by LIME.

In this example:
- The input audio is divided into a 3-second segment.
- The corresponding spectrogram is partitioned into 12 regions.
- the xAI techniques (in this case we made an average of LIME, SHAP and GradCAM, but the same applies if we only use LIME) is applied to highlight the regions that most influenced the model's prediction.
- We extract and sonify the most relevant and least relevant regions 
  to perceptually validate the explanation.

---

## 📊 Relevance Map

![Regions Map](./assets/average_h.png)

---

## 🔊 Audio Comparison

### 🎧 Full 3-Second Segment
[Listen here](./assets/test_audio.wav)

### 🎧 Most Relevant Region (1s)
[Listen here](./assets/most_relevant_region.wav)

### 🎧 Least Relevant Region (1s)
[Listen here](./assets/irrelevant_region.wav)

---

## 🧠 Interpretation

The most relevant region preserves the acoustic characteristics that drive 
the model’s classification decision (e.g., harmonic structure and timbral content), 
whereas the least relevant region contains limited discriminative information.

This perceptual comparison supports the validity of the LIME-based explanation.
