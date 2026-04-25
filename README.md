# Yeast Cell Particle Counting 
Yeast cell particle counting using ImageJ Fiji for Assignment-1
(Summary)
## Assignment 1 - Yeast Cell Image Analysis

## Study Outline
This assignment involves automated 
counting of yeast cells (Saccharomyces 
cerevisiae) using ImageJ/Fiji software.
Yeast cells are unicellular fungi and 
counting them helps understand cell 
population density and growth patterns.
This is part of Assignment 1 for 
Science Art and Imaging course.

## Image Source
- Image: Yeast cells microscopy image
- Source: Wikimedia Commons
- Type: Bright field microscopy
- Original file: yeast cell.jpg
- Saved in: data/raw/ folder

## Why Yeast Cells?
Yeast cells (Saccharomyces cerevisiae)
are commonly used in research because:
- They are easy to image
- They have clear round/oval shape
- They are good model organisms
- Easy to distinguish from background

## Role of This Analysis
The goal of this analysis was to 
accurately count the number of yeast 
cells present in a microscopy image 
using automated particle counting 
in ImageJ/Fiji software.
This helps in:
- Quantifying cell numbers
- Understanding cell density
- Learning image analysis techniques

## Software Used
- ImageJ/Fiji version 2.16.0
- Platform: Windows 11

## Analysis Summary
1. Image opened in Fiji
2. Converted to 8-bit grayscale
3. Background subtracted (radius=12)
4. Threshold applied manually
5. Image inverted
6. Fill Holes applied
7. Cell length measured
8. Analyze Particles run
9. Results exported as CSV

## Results
- Total yeast cells counted: 78
- Total Area: 21696 pixels
- Average cell size: 278.154 pixels
- %Area covered: 13.689
- Mean intensity: 255

## Repository Structure
data/
  raw/ 
    yeast cell.jpg (original image)
  processed/
    yeast_processed.png (edited image)
analysis/
  ImageJ_Protocol.md (detailed steps)
results/
  yeast_Results.csv
  yeast_Summary.csv
README.md
