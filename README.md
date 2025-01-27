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

Step 2: 4*4 Mosaic:

| Binary | Binary | Binary | Binary |
|:------:|:------:|:------:|:------:|
| 0000   | 0001   | 0010   | 0011   |
| 0100   | 0101   | 0110   | 0111   |
| 1000   | 1001   | 1010   | 1011   |
| 1100   | 1101   | 1110   | 1111   |

## How to Create Your Mosaic

1. **List 16 binary values** (each is 4 bits).  
2. **Assign each binary to a cell** in order:  
   - The 1st binary value → Cell 0  
   - The 2nd binary value → Cell 1  
   - …  
   - The 16th binary value → Cell 15  
3. **Look up each binary** in the color palette table to find its color.  
4. **Fill the grid** accordingly:
   - Row 0: cells 0–3
   - Row 1: cells 4–7
   - Row 2: cells 8–11
   - Row 3: cells 12–15



