# ImageJ Particle Counting Protocol

## Assignment 1 – Yeast Cell Analysis

## Step 0: Image Acquisition

A raw bright-field microscopy image of 
yeast cells (Saccharomyces cerevisiae) 
was downloaded from Wikimedia Commons.
The image was unprocessed and saved in 
the data/raw/ folder.

## Step 1: Opening the Image

File → Open → yeast cell.jpg

## Step 2: Conversion to 8-bit

Image → Type → 8-bit
(Converts image to grayscale)

## Step 3: Subtract Background

Process → Subtract Background
Rolling ball radius = 12 pixels
(Removes uneven background lighting)

## Step 4: Thresholding

Image → Adjust → Threshold
- Dark background = ON
- Sliders adjusted manually until 
  cells appeared black on white 
  background
- Applied threshold

## Step 5: Inversion

Edit → Invert (Ctrl + Shift + I)
Cells appeared black and background 
appeared white after inversion.

## Step 6: Fill Holes

Process → Binary → Fill Holes
(Fills hollow areas inside cells
for accurate counting)

## Step 7: Set Measurements

Analyze → Set Measurements
- Area ✅
- Mean Gray Value ✅

## Step 8: Measure Cell Length

Straight line tool used to draw 
line across individual cells.
Analyze → Measure
(To measure length of yeast cells)

## Step 9: Analyze Particles

Analyze → Analyze Particles
Parameters used:
- Size: 50-500 pixels²
- Circularity: 0.3-1.0
- Show: Outlines
- Display Results: ON ✅
- Summarize: ON ✅

## Step 10: Save Results

Results exported as CSV files:
- yeast_Results.csv
- yeast_Summary.csv
Saved in results/ folder on GitHub.

Processed image saved in 
data/processed/ folder.

## Final Results

- Total yeast cells counted: 78
- Total Area: 21696 pixels
- Average cell size: 278.154 pixels
- %Area: 13.689
- Software: ImageJ/Fiji v2.16.0
