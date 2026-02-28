# Bivariate Normal Distribution Analysis - Old Faithful Geyser Dataset

## Project Overview
This project analyzes the relationship between **eruption duration** and **waiting time** for the Old Faithful geyser using bivariate normal distribution. All statistical calculations are implemented from scratch, demonstrating a deep understanding of probability theory and statistical computing.

## Dataset
The dataset (`geyser_data.csv`) contains 272 observations of Old Faithful geyser eruptions with three variables:
- **duration**: Length of eruption (in minutes)
- **waiting**: Time between eruptions (in minutes)
- **kind**: Classification ("long" or "short" eruption)

## Implementation Highlights
- **Pure Python implementation** - No statistical libraries used
- **From-scratch calculations**:
  - Mean, standard deviation, and correlation coefficient
  - Bivariate normal probability density function (PDF)
  - Grid-based PDF evaluation for visualization

## Visualizations
The project generates three complementary visualizations:

1. **Scatter Plot** - Data points colored by their PDF value
2. **Contour Plot** - Topographical view with probability contours
3. **3D Surface Plot** - Three-dimensional view of the PDF surface

## Dependencies
```
Python 3.x
matplotlib
numpy
csv (standard library)
urllib (standard library)
math (standard library)
```

## Key Statistics
- Mean eruption duration: ~3.49 minutes
- Mean waiting time: ~70.90 minutes
- Correlation coefficient: ~0.90 (strong positive correlation)

## Mathematical Foundation
The bivariate normal PDF is implemented as:
```
f(x,y) = 1/(2πσxσy√(1-ρ²)) × 
         exp(-1/(2(1-ρ²)) × [(x-μx)²/σx² + (y-μy)²/σy² - 2ρ(x-μx)(y-μy)/(σxσy)])
```

## Usage
1. Ensure all dependencies are installed
2. Run the Jupyter notebook `Bivariate PDF.ipynb`
3. Execute cells sequentially to load data, calculate statistics, and generate visualizations
