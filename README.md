# Image Processing with Matrices (C++ Project)

## 📌 Overview
This project demonstrates basic image processing operations using a custom `Image` class implemented in C++.  
The project uses the **PPM (P3 format)** for simplicity and represents images as a 3D matrix (`height × width × channels`).  

It includes functionality to:
- Load and save images in **PPM format**
- Print image data to the console (for small test images)
- Apply several image transformations and filters  

The code is designed as a **student project** to explore the fundamentals of image manipulation without relying on external libraries like OpenCV.

---

## 🚀 Features
- **Image Class**  
  - Supports color and grayscale images  
  - Handles pixel access via `operator()`  
  - Loads and saves **P3 PPM files**  
  - Prints image matrix to console  

- **Implemented Transformations**  
  - ✅ Convert to Grayscale  
  - ✅ Flip Horizontal  
  - ✅ Flip Vertical  
  - ✅ Adjust Brightness  
  - ✅ Adjust Contrast  
  - ✅ Apply Simple Blur (3×3 average filter)  
  - ✅ Rotate 90° Clockwise  

---

## 🛠️ How It Works
1. A **test image (4×4 pixels)** is generated with a simple color pattern.  
2. The program saves it as `test_image.ppm`.  
3. The test image is loaded back, and all transformations are applied sequentially.  
4. Each result is saved as a new `.ppm` file (e.g., `gray_image.ppm`, `flipped_horizontal.ppm`, `blurred_image.ppm`, etc.).  
5. Console output shows matrix values before and after transformations.  

---

## 📂 Output Files
After running the program, you will get:  
- `test_image.ppm` → Original test pattern  
- `gray_image.ppm` → Grayscale version  
- `flipped_horizontal.ppm` → Horizontally flipped image  
- `flipped_vertical.ppm` → Vertically flipped image  
- `bright_image.ppm` → Brightness adjusted image  
- `contrast_image.ppm` → Contrast adjusted image  
- `blurred_image.ppm` → Blurred image  
- `rotated90_image.ppm` → Rotated 90° clockwise  

---

## 🖼️ Viewing the Results
The generated files are in **PPM (P3)** format.  
You can view them using:
- Linux image viewers (`eog`, `gthumb`, `feh`, etc.)
- Image editors like **GIMP** or **Photoshop**
- Convert to PNG/JPG with:
  ```bash
  convert image.ppm image.png
  ```
  (requires **ImageMagick**)

---

## ⚡ Compilation & Usage
Compile with:
```bash
g++ -o image_processing main.cpp
```

Run:
```bash
./image_processing
```

---

## 📖 Example Console Output
```
Image Processing with Matrices - Student Project
================================================

Created 4x4 test image: test_image.ppm

Image loaded successfully. Dimensions: 4x4

Applying image transformations...
- Grayscale conversion completed
- Horizontal flip completed
- Vertical flip completed
- Brightness adjustment completed
- Contrast adjustment completed
- Blur filter completed
- 90-degree rotation completed

All operations completed successfully!
Check the generated PPM files to see the results.
```

---

## 👨‍💻 Contributors
- Hazem – Brightness & Contrast Adjustments  
- Menna – Grayscale & Vertical Flip  
- Lasheen – Horizontal Flip, Blur, Rotation  
