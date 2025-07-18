# Sudoku Solver with Denoising Diffusion Visualization

This project implements a Sudoku solver inspired by deep learning denoising diffusion models. It simulates the gradual refinement of a noisy Sudoku puzzle to a fully solved solution and visualizes the intermediate steps along with uncertainty maps. The solver also generates tech-style visualizations with neon/glow effects for both noisy inputs and final solutions.

---

## Features

- Simulate multi-step denoising from noisy Sudoku states to solved puzzle.
- Visualize uncertainty using RGB heatmaps (red = uncertain, green = confident).
- Render Sudoku grids with glowing neon effects on a dark theme.
- Generate animated GIFs showing the step-by-step solving process.
- Single-step denoising simulation that maps noisy input directly to final solution.
- Clean, modular Python code using NumPy and Pillow (PIL).

---

## Usage

1. **Load a Sudoku puzzle and its solution** as 9x9 NumPy arrays.
2. **Simulate diffusion steps** with progressive noise reduction.
3. **Render visualizations** for each step:
   - Current sample with partial guesses.
   - Uncertainty heatmap.
   - Final solved grid.
4. **Generate techie-style images** with glowing digits and neon grids.
5. **Create animated GIFs** to visualize the denoising process and single-step jump.

---

## Concepts and Skills Explored

Great question! Here’s a summary of the key concepts and skills you’ve explored while building this **techie-style Sudoku solver visualization with deep learning and denoising concepts**:

---

### 1. **Deep Learning & Generative Modeling Concepts**

* **Denoising / Diffusion Models**:  
  Simulating iterative refinement from noisy inputs \(x_t\) to clean output \(\hat{x}_0\), inspired by diffusion models that progressively reduce noise to generate samples.  
* **Single-step vs. Multi-step Denoising**:  
  The difference between refining predictions step-by-step vs. directly predicting the final output in one step.

---

### 2. **Sequential & Parallel Reasoning**

* **Sequentialization of Variables**:  
  Treating Sudoku cells as random variables with individual noise levels, and controlling their order/amount of denoising (like SRM framework concepts).  
* **Uncertainty Estimation**:  
  Simulating uncertainty maps (\(\sigma_\theta(x_t)\)) that help guide reasoning and sampling, using visual heatmaps.

---

### 3. **Visualization Techniques**

* **Grid Rendering & Image Processing**:  
  Drawing Sudoku grids, digits, and color-coded highlights using PIL (Python Imaging Library).  
* **Color Mapping for Uncertainty**:  
  Mapping uncertainty/confidence levels to colors (RGB heatmaps, glow effects) for intuitive visual communication.  
* **Glow & Neon Effects**:  
  Using layered blurs, alpha transparency, and color overlays to create futuristic “techie” visual styles.  
* **Animated GIF Generation**:  
  Combining multiple images into a GIF to visualize transitions over time.

---

### 4. **Programming & Software Engineering**

* **Python Imaging Library (PIL/Pillow)**:  
  Image creation, drawing shapes/text, layering, filtering, and compositing.  
* **Data Structures for Grids**:  
  Using numpy arrays to represent Sudoku boards and intermediate states.  
* **Modular Code Design**:  
  Writing reusable rendering functions with parameters to customize colors and styles.  
* **Error Handling & Environment Adaptation**:  
  Managing file paths and environment constraints (e.g., saving files, showing images in notebooks).

---

### 5. **Problem Solving & Approximation**

* **Simulating Complex Models**:  
  Approximating diffusion-like sampling without training a full model by heuristic rules (random fills, progressive correction).  
* **Single-step Approximation**:  
  Mapping noisy inputs directly to solution as a stand-in for complex denoising.  
* **Visualization as Explanation**:  
  Using images and animations to explain abstract model behavior visually.

---

### Summary

You’ve combined ideas from **machine learning theory, probabilistic modeling, image processing, and software implementation** to build an educational and visually appealing Sudoku solver that mimics modern denoising diffusion reasoning frameworks!

---

## Requirements

- Python 3.7+
- NumPy
- Pillow (PIL)

Install dependencies via:

```bash
pip install numpy pillow
