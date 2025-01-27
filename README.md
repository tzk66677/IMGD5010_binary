# IMGD5010
# 4×4 Mosaic with Binary Color Codes

This Markdown file describes a simple system for creating a **4×4 mosaic** using **4-bit binary** values as color indices.  
Each cell in the 4×4 grid is filled based on its assigned 4-bit value (from 0000 to 1111).

---

## Overview

1. We have a **4×4 grid** (16 cells total).
2. Each cell corresponds to one 4-bit binary value.
3. Each 4-bit value represents a **color index** (0–15).
4. You fill the cells in **row-major order**:
   - The first 4-bit value fills cell 0 (top-left),
   - The second fills cell 1,
   - The sixteenth fills cell 15 (bottom-right).

## Step 1: Color Palette

Below is an example palette mapping **4-bit values** (from `0000` to `1111`) to colors.  
Feel free to change the color definitions (HEX codes) to suit your preferences.

| Binary | Decimal | Color Name     | HEX Code   |
|:------:|:-------:|:--------------:|:----------:|
| 0000   | 0       | White          | `#FFFFFF`  |
| 0001   | 1       | Black          | `#000000`  |
| 0010   | 2       | Red            | `#FF0000`  |
| 0011   | 3       | Green          | `#00FF00`  |
| 0100   | 4       | Blue           | `#0000FF`  |
| 0101   | 5       | Yellow         | `#FFFF00`  |
| 0110   | 6       | Magenta        | `#FF00FF`  |
| 0111   | 7       | Cyan           | `#00FFFF`  |
| 1000   | 8       | Gray           | `#888888`  |
| 1001   | 9       | Pink           | `#FFC0CB`  |
| 1010   | 10      | Orange         | `#FFA500`  |
| 1011   | 11      | Purple         | `#800080`  |
| 1100   | 12      | Brown          | `#A52A2A`  |
| 1101   | 13      | Dark Green     | `#006400`  |
| 1110   | 14      | Light Blue     | `#ADD8E6`  |
| 1111   | 15      | Khaki          | `#F0E68C`  |
![G0-hsl-FFFFFF-000000-FF0000-19E664-0000FF-FFFF00-FF00FF-00FFFF-878787-FFC2CC-FFA600-ADD8E6-A62B2B-006600-F0E78E](https://github.com/user-attachments/assets/fb651d2f-e60e-4b3a-b9ee-e16bdbc6655a)

Step 2: 4*4 Mosaic:

| Binary | Binary | Binary | Binary |
|:------:|:------:|:------:|:------:|
| 0000   | 0001   | 0010   | 0011   |
| 0100   | 0101   | 0110   | 0111   |
| 1000   | 1001   | 1010   | 1011   |
| 1100   | 1101   | 1110   | 1111   |

## How to Create Your 4×4 Mosaic

1. **Choose a 4-bit color code**  
   - Refer to the palette table (e.g., `0000` for white, `0010` for red, etc.) or use your own color definitions.  
   - Each 4-bit value can range from `0000` (0) to `1111` (15).

2. **Select the corresponding cell**  
   - Number the cells from 0 to 15 in row-major order (top-left to bottom-right).  
   - For example, cell 0 is the top-left, cell 3 is the top-right, cell 12 is the bottom-left, and cell 15 is the bottom-right.

3. **Assign the chosen color code to that cell**  
   - Write down the 4-bit code for each of the 16 cell.

4. **Fill or label the 4×4 grid**  
   - Using the color codes assigned to each cell, color or mark each cell accordingly.  
   - You can either draw it by hand on paper or use a digital tool to fill in each cell with the chosen color.

By following these steps, you’ll have a completed 4×4 mosaic defined by 16 binary color codes.

   - 
## Chanllenge
Design your own 4×4 mosaic with those colors


