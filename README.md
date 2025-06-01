# Image-Classification-using-Sonification

This project explores a novel approach to evaluating the retention of visual information in sonified images by transforming images into audio using the **inverse Griffin-Lim algorithm**, converting the resulting audio into **spectrograms**, and then classifying these spectrograms using **deep CNN architectures**.

---

## Project Motivation

Understanding how much **visual information** is preserved when an image is converted into sound is an open question with implications in:
- **Cross-modal representation learning**
- **Accessible machine perception** (e.g., assisting visually impaired individuals)
- **Low-bandwidth sensory transmission systems**
- **Creative applications in AI-generated art and music**

---

## Project Pipeline

The full pipeline for this project is structured as follows:

1. **Image Dataset Preparation**  
   Multiple datasets with different class complexities:
   - **2, 4, 10, and 15-class subsets** were created for thorough evaluation.

2. **Sonification via Inverse Griffin-Lim Algorithm**  
   - Each image is transformed into a phase-less spectrogram using image-to-frequency mapping.
   - The **inverse Griffin-Lim algorithm** is used to generate time-domain audio from this spectrogram.

3. **Spectrogram Generation**  
   - The generated audio signals are converted into **2D spectrograms** using standard STFT-based methods.

4. **CNN-Based Classification**  
   Spectrograms are used as input to a set of pre-trained CNN models fine-tuned for classification:
   - `EfficientNet-B0`
   - `EfficientNet-B5`
   - `EfficientNet-B7`
   - `ResNet50`
   - `ResNet150`

---

## Goals & Evaluation

- To evaluate **how well CNN models can classify sonified representations** of visual data.
- To compare model performance across datasets with increasing class complexity.
- To identify which CNN architectures generalize better for spectrogram-based classification of sonified images.
- To finally conclude that **sonified images retain vital information regarding the image after conversion**.

### Metrics Used
- **Accuracy and Loss Curve**
- **F1-score**
- **Confusion Matrices** per dataset/model combination

---

## Technologies Used

| Component         | Library/Tool              |
|------------------|---------------------------|
| Image Processing | OpenCV, PIL                |
| Audio Generation | Librosa, NumPy             |
| Spectrograms     | Librosa, Matplotlib        |
| Deep Learning    | PyTorch                    |
| Models           | EfficientNet, ResNet (pretrained) |


---

## Project Structure
* refer to `/nobooks` folder for code for all 5 model
* refer to `/utilities-notebook` for code for image sonification using Griffin-Lim algo and code for spectrogram representation of generated audio `.wav` files

