Image Processing Tool in C++

This is a command-line based image processing tool built using C++. It allows users to load, manipulate, and save grayscale images in PGM (P2) format. The tool supports a wide variety of operations such as brightness adjustment, filtering, rotation, flipping, resizing, cropping, and more.

Features
	•	Image I/O
	•	Load and save images in PGM (P2) format
	•	Combine two images (side-by-side or top-to-bottom)
	•	Enhancement & Filtering
	•	Brightness adjustment
	•	Contrast stretching
	•	Binarization (thresholding)
	•	Sharpening
	•	Mean & Median filtering
	•	Custom filter loading from file
	•	Predefined filters:
	•	Linear
	•	Roberts
	•	Laplacian
	•	Geometric Transformations
	•	Resize (scale)
	•	Rotate (clockwise & anti-clockwise)
	•	Flip (horizontal & vertical)
	•	Translate
	•	Crop

Getting Started

Prerequisites
	•	C++ Compiler (supporting C++11 or higher)
	•	Any OS (Tested on Windows)
	•	Image viewer (e.g. IrfanView) to view .pgm files

Input Format

Only PGM (Portable Gray Map) files in P2 (ASCII) format are supported.
You’ll be prompted with a menu loaded from MainMenu.txt. Each option corresponds to a specific image processing function.

Menu Options
	1.	Load Image
	2.	Save Image
	3.	Change Brightness
	4.	Contrast Stretching
	5.	Sharpen Image
	6.	Binarize Image
	7.	Resize Image
	8.	Rotate Image
	9.	Horizontal Flip
	10.	Vertical Flip
	11.	Crop Image
	12.	Combine with Another Image
	13.	Apply Mean/Median Filter
	14.	Apply Linear Filter from File
	15.	Apply Custom Filter (enter manually)
	16.	Apply Roberts Filter
	17.	Apply Laplacian Filter
	18.	Translate Image
	19.	Resize (Uniform Scale)
	20.	Exit

File Structure
	•	image_processing.cpp – Main source file
	•	MainMenu.txt – Menu items configuration (required at runtime)
	•	filters/ – Optional directory to store custom filter matrices

Notes
	•	Images are represented internally using 2D vectors.
	•	All changes must be saved manually before exiting or they will be lost.
	•	Ensure your terminal supports input/output interaction.
	•	Use IrfanView or similar to preview .pgm files.

20
Load Image
Save Image
Change Brightness
Contrast Stretching
Sharpen Image
Binarize Image
Resize Image
Rotate Image
Horizontal Flip
Vertical Flip
Crop Image
Combine Images
Apply Mean/Median Filter
Apply Linear Filter from File
Apply Custom Filter
Apply Roberts Filter
Apply Laplacian Filter
Translate Image
Uniform Resize
Exit
