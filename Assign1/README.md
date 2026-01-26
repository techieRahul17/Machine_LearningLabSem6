# Assignment 1: Image Dataset Analysis

**Student:** Rahul V S (3122235001104)

## Overview
This assignment focuses on loading and analyzing an image dataset. The goal is to process a CSV file containing image metadata, load the corresponding images from a directory, and perform exploratory data analysis on the image dimensions.

## Files
- `Assignment_1_ML_Rahul_V_S.ipynb`: The main Jupyter notebook containing the code.
- `english.csv`: The dataset file containing image filenames and labels.
- `Img/`: Directory containing the image files.
- `debug_images.py` & `patch_nb.py`: Helper scripts used for debugging paths and patching the notebook (generated during development).

## Key Tasks
1.  **Data Loading**: Reading `english.csv` using Pandas.
    - *Fix Applied*: The CSV loading code was updated to properly handle the header row. Originally, `names=['image_path','label']` was overwriting the actual header, causing a `KeyError`. This has been corrected to let Pandas infer the header.
2.  **Image Processing**: Iterating through image paths listed in the CSV.
    - *Fix Applied*: Updated the image folder path to `Assign1/Img` to correctly locate the images.
    - *Fix Applied*: Corrected the column access from `df['image_path']` to `df['image']` to match the actual CSV column name.
3.  **Visualization**:
    - Loading images using OpenCV/Matplotlib and checking their existence.
    - Calculating and plotting histograms of image heights and widths to understand the data distribution.

## How to Run
1.  Ensure all dependencies are installed (`pandas`, `numpy`, `matplotlib`, `seaborn`, `opencv-python`).
2.  Open `Assignment_1_ML_Rahul_V_S.ipynb` in Jupyter Notebook or VS Code.
3.  Run the cells sequentially.

## Recent Fixes
- Resolved `KeyError: 'image_path'` by using the correct column name `image`.
- Fixed `FileNotFoundError` by pointing to the correct absolute path for the `Img` directory.
