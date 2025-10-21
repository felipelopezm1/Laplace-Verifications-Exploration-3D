# Laplace Transform — Visual Explorations (Basenji Edition)

### 🎓 A visual journey through the Laplace Transform  
This notebook collection explores the **Laplace Transform** from multiple perspectives — time-domain decay, weighted accumulation, frequency-domain sweep, and 3D geometric intuition — using Python, Matplotlib, and animation.

---

## 🧠 Overview
This project was designed to **visualize the mechanics** of the Laplace Transform in an intuitive way.  
Each “view” breaks down one conceptual layer of what the transform does, showing how signals are weighted, accumulated, and mapped into the complex plane.

| View | Focus | Concept | Visual Summary |
|------|--------|----------|----------------|
| **1. Decay of \( e^{-\sigma t} \)** | Exponential kernel | Time decay | Shows how increasing σ makes the exponential fade faster. |
| **2. Weighting & Accumulation** | Weighted signal integral | Memory & accumulation | Demonstrates how the transform sums a decaying version of \( f(t) \). |
| **3. s-plane Sweep** | Magnitude of \( F(s)=1/(s+1) \) | Complex analysis | Scans through σ + jω to reveal how frequency and decay interact. |
| **4. 3D Surface \( |1/s| \)** | Geometric intuition | Laplace landscape | Plots the “height” of the transform over the σ–ω plane. |

---

## 🎨 Visual & Design
This “**Basenji Edition**” uses a color palette and typography inspired by the **UAL Project: Xylem** visual identity.  
- Deep blue background (`#0e3a8a`)  
- Cyan grid and accents  
- Soft pink and yellow highlights  
- Font: **Basenji Variable** (if available; otherwise falls back to DejaVu Sans)

---

## ⚙️ Environment Setup

```bash
# Create environment
conda create -n laplace python=3.8 -y
conda activate laplace

# Install required packages
conda install numpy scipy matplotlib -y

# Optional (for MP4 animation export)
conda install -c conda-forge ffmpeg -y
