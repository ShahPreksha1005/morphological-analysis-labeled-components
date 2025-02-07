# Morphological Analysis of Labeled Components

## Overview
This project focuses on extracting and analyzing the morphological properties of labeled components in an image. Using Otsu’s thresholding and connected component labeling, it identifies various properties such as:
- **Perimeter & Area**
- **Centroids**
- **Bounding Boxes**
- **Eccentricity**
- **Orientation**

These techniques are widely used in earth sciences for tasks like rock formation analysis, crater detection, and landmass feature identification.

## Key Concepts
1. **Otsu’s Thresholding:** Determines an optimal threshold to separate foreground and background.
2. **Connected Component Labeling:** Assigns unique labels to connected regions.
3. **Region Properties Extraction:** Using `skimage.measure.regionprops`, computes geometric and spatial attributes.
4. **Visualization:** Properties are overlayed on the original image for analysis.

## Dataset
A sample grayscale image (`rocks.jpg`) is used to demonstrate the techniques, representing geological formations or satellite imagery.

## Dependencies
Ensure you have the following Python libraries installed:
```bash
pip install numpy matplotlib scikit-image
```

## Implementation
### 1. Load and Preprocess Image
- Convert image to grayscale.
- Apply Otsu’s thresholding to create a binary image.

### 2. Label Connected Components
- Use `skimage.measure.label` to assign labels.
- Visualize labeled regions with `label2rgb`.

### 3. Extract and Visualize Morphological Properties
- **Perimeter & Area:** Extracted and plotted with red boundary markers.
- **Centroids:** Marked with blue dots.
- **Bounding Boxes:** Highlighted with yellow rectangles.
- **Eccentricity & Orientation:** Computed and displayed.

### 4. Applications in Earth Science
- **Geological Mapping:** Identifies tectonic features.
- **Land Use Analysis:** Classifies forests, urban areas, and water bodies.
- **Disaster Monitoring:** Measures flood or landslide-affected zones.
- **Soil Erosion Studies:** Tracks desertification trends.

## Results
The labeled components and extracted properties are visualized, demonstrating how morphological analysis aids in feature extraction from images.

## Conclusion
This project demonstrates how image morphology analysis helps extract shape, size, and orientation information. These techniques support environmental monitoring, mapping, and geological studies using efficient Python-based image processing.
