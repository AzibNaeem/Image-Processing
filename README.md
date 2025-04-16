# 🖼️ Grayscale Image Processor

A C++ application for processing grayscale images in the PGM (Portable GrayMap) P2 format. This tool provides a variety of image manipulation functionalities such as brightness adjustment, filtering, rotation, cropping, and more — all through a simple text-based interface.

---

## 📌 Features

- 🔆 Brightness adjustment  
- 🧪 Contrast stretching  
- ✴️ Sharpening filter  
- 🎚️ Thresholding (binary)  
- ↕️ Resizing (scale up/down)  
- 🔄 Rotation (any angle)  
- ↔️ Horizontal and vertical flipping  
- ✂️ Cropping selected regions  
- ➕ Image combination (horizontal or vertical)  
- 🎛️ Mean and median filtering  
- ⚙️ Custom linear filters (loaded from file)  
- 💾 Load and save images  

---

## 🗂️ Input Format

This application supports **PGM P2** format only (ASCII-encoded grayscale images).  
A valid `.pgm` file should follow this structure:

```
P2
# Optional comment
<width> <height>
<max_gray_value>
<image pixel data (row-wise)>
```

Example:
```
P2
# Example image
4 4
255
0 50 100 150
200 250 255 128
64 32 16 8
0 0 0 0
```

---

## 📄 Menu File Format

The application reads menu options from a plain text file. Format:

```
<number of options>
<menu option 1>
<menu option 2>
...
```

Lines starting with `*` will be treated as comments and not displayed.

Example:
```
4
Change Brightness
Rotate Image
Flip Horizontally
Save Image
```

---

## 📐 Custom Filter File Format

To apply a custom linear filter, provide a text file with the following format:

```
<rows> <columns>
<row 1 values>
<row 2 values>
...
```

Example (3×3 sharpening filter):
```
3 3
0 -1 0
-1 5 -1
0 -1 0
```

---

## ⚙️ Build & Run

Ensure you have a C++ compiler installed (e.g., `g++`).  
To compile and run:

```bash
g++ -o GrayscaleProcessor main.cpp
./GrayscaleProcessor
```

---

## 📎 Notes

- Only **PGM P2** images are supported (not P5 or binary formats).
- File paths must be correctly entered when prompted to avoid runtime errors.
- Outputs will overwrite any existing file with the same name.

---

## 📁 Example Files

Sample files (optional for use):

- `example.pgm` — a sample image file  
- `menu.txt` — a list of processing options  
- `filter.txt` — a custom 3x3 filter  

---

## 🧑‍💻 Author

**M. Azib Naeem**  
C++ Developer | Image Processing Enthusiast

---

## 📃 License

This project is open-source and available under the [MIT License](LICENSE).
