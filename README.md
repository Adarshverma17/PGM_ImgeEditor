# PGM Image Processing Tool

## 📌 Project Overview
This project is a console-based image editor designed specifically to manipulate PGM (Portable Gray Map) files. It provides a comprehensive suite of image processing capabilities, ranging from basic color inversion to complex spatial transformations. The application is built with a focus on modular design, utilizing efficient file handling and mathematical algorithms to process image data directly from memory.

## 🛠️ Tech Stack & Concepts
* **Language:** C++
* **Data Structures:** Utilizes dynamic 2D `std::vector` arrays for robust image data representation and memory management.
* **Core Concepts:** Matrix transformations, basic trigonometry for spatial rotation, and modular programming.

## ✨ Features
The application runs via an interactive command-line interface, offering the following operations:

* **File Management:** Seamlessly load and save `.pgm` (P2 format) files.
* **Image Filters:**
    * **Negative:** Inverts the grayscale pixel intensities.
    * **Mean Filter:** Applies a customizable box-blur effect to smooth the image.
    * **Median Filter:** Reduces "salt and pepper" noise by calculating the median of a pixel neighborhood, utilizing a custom sorting algorithm.
* **Transformations:**
    * **Flip:** Mirror the image horizontally or vertically.
    * **Rotate:** Turn the image clockwise by 90°, counter-clockwise by 90°, or rotate it by any arbitrary angle using trigonometric mapping.
* **Structural Edits:**
    * **Resize:** Adjust the overall height and width of the image.
    * **Crop:** Trim unwanted borders by specifying precise left, top, right, and bottom pixel boundaries.

## 🚀 How to Compile and Run
1. Ensure you have a standard C++ compiler installed (such as `g++`).
2. Open your terminal and navigate to the directory containing the source code.
3. Compile the file by running:
   ```bash
   g++ image_editor.cpp -o image_editor
