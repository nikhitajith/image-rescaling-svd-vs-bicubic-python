# image-rescaling-svd-vs-bicubic-python
# Image Rescaling Using SVD and Bicubic Interpolation

## Project Type
Image Processing / Linear Algebra / Scientific Computing

## Description
This project performs image rescaling using two different approaches:  
**Singular Value Decomposition (SVD)** and **Bicubic Interpolation**, and compares their reconstruction behavior.

High-resolution images from the DIV2K dataset are first preprocessed and resized to a fixed resolution to enable efficient computation.  
The SVD-based approach treats a grayscale image as a 2D matrix and reconstructs it using a reduced number of singular values, resulting in a low-rank approximation.  
The bicubic interpolation method rescales images using local pixel neighborhood information and is used as a baseline for comparison.

The project demonstrates how linear algebra–based techniques differ from traditional interpolation methods in image rescaling tasks.

---

## Dataset
- **DIV2K High-Resolution Dataset**
- Images are read in RGB format and converted to grayscale for SVD processing
- Only a subset of images is used for testing due to computational constraints

---

## Methodology
1. Load high-resolution images from the dataset
2. Convert images from BGR to RGB
3. Convert RGB images to grayscale
4. Resize images to **256 × 256** for faster computation
5. Normalize pixel values to the range **[0, 1]**
6. Apply **SVD-based low-rank approximation**
7. Perform **bicubic interpolation**
8. Compare reconstructed images visually and quantitatively

---

## Key Concepts
- Singular Value Decomposition (SVD)
- Low-rank matrix approximation
- Bicubic interpolation
- Image rescaling
- Linear algebra applications in image processing

---

## Technologies Used
- Python
- NumPy
- OpenCV
- Matplotlib

---

## How to Run
1. Clone the repository
2. Install required libraries:
   ```bash
   pip install numpy opencv-python matplotlib

